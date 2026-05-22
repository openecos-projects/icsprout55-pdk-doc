# ICsprout55 PDK Documentation

## Introduction

This repository contains the source files for the ICsprout55 PDK documentation, generated with **MkDocs Material + Tailwindcss** as a bilingual site (`doc/src/zh` and `doc/src/en`) with a lightweight frontend asset pipeline for consistent local preview and production output.

## Usage

Before running commands, make sure your environment has Python 3.10+, Node.js 22+ and Git.

- Setup

  Initialize shared repositories (`res` and `tpl`) and prepare the local project workspace.

  ```bash
  cd doc
  make setup
  ```

- Edit

  Please follow the workflow to add new images or videos:

    - Upload lossless original images (JPG or PNG format) or pre-compressed videos (MP4 format) to the corresponding directory under `doc/res/img`.
    - Run `make gen-webp` command in the `doc` directory, and scripts in `doc/tpl` will automatically convert original images to smaller WEBP images (lossy compression).
    - Reference the generated WEBP images in your Markdown files.

  **Note:** running `make gen-webp` command is optional. If you run `make serve-doc` command in the next **Preview** step, the system will also convert images automatically. **Video compression is not currently supported by script, so please compress videos in advance before uploading them to `doc/res/img`.**

- Preview

  Start a local development server for the Chinese site (default language).

  ```bash
  cd doc
  make serve-doc
  ```

  Start a local development server for the English site.

  ```bash
  cd doc
  make serve-doc MKDOCS_LANG=en
  ```

- Build

  Generate dynamic assets and build the Chinese static site output.

  ```bash
  cd doc
  make gen-doc
  make build-doc
  ```

  Generate dynamic assets and build the English static site output.

  ```bash
  cd doc
  make gen-doc MKDOCS_LANG=en
  make build-doc MKDOCS_LANG=en
  ```

- Deploy

  If you modify files in local `doc/res` or `doc/tpl` (for example, add new images, templates, scripts, or styles), commit and push those changes to their corresponding repositories first.

  Commit and push your changes in `doc/src` to the repository. Then ReadTheDocs (a cloud platform designed to simplify documentation manage) will detect the update of the repository, automatically build and deploy the documentation according to `.readthedocs.yaml` config file.

- Clean

  Remove generated files and local build artifacts for a fresh rebuild.

  ```bash
  cd doc
  make clean
  ```
