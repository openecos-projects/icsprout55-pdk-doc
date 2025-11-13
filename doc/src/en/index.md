# Project Home
## Introduction
The **ICsprout 55nm Open Source PDK** (hereinafter referred to as this PDK) is an open source [Process Design Kit](https://en.wikipedia.org/wiki/Process_design_kit) independently developed by ICsprout Integrated Circuit Co., Ltd. (hereinafter referred to as ICsprout) and released in October 2025 with the assistance of **ECOS Team, Institute of Computing Technology, Chinese Academy of Sciences (hereinafter referred to as ECOS Team).** A significant breakthrough in the global open source chip ecosystem, **this PDK represents the industry's most advanced open source process node at the time of its release**. Built on mature 55nm CMOS process technology, it provides a complete and production-proven design rule files, device models, standard cell libraries, and parameterized cells. It fully supports the backend physical design flow of digital integrated circuits, including key steps such as logic synthesis, place and route, and physical verification, etc. Ultimately, it can be taped out on ICsprout's own production lines.

The open-source release of this PDK revolutionizes the traditional challenges of **high barriers and high costs** in chip design. By providing universities, research institutions, and the open-source community with a complete path from chip design to tapeout, it empowers researchers and developers to transform their wildest ideas into physical silicon. Furthermore, thanks to the advanced nature of the 55nm process node within the open-source chip field, the complexity and flexibility of future open-source chip designs will be significantly enhanced, providing a powerful boost to the development of an open-source chip ecosystem and the cultivation of chip talent.

<p style="text-align: center;">
    <img alt="" src="./res/img/pdk/icsprout.png" style="width: 75%;">
</p>

## Background
ICsprout's development of this PDK stems primarily from its desire to overcome the limitations of the closed-source model in the existing semiconductor design ecosystem. Traditional closed-source PDKs are constrained by commercial licensing models, resulting in issues such as **the inability to obtain the PDK (due to certain special reasons)** and high tapeout costs. This significantly restricts the innovative vitality of universities, research institutions, and open-source communities in the chip field. Although several open-source PDK projects worldwide have already undergone tapeout verification, ICsprout chose to independently develop its own open-source PDK. The core reasons are: **1. This PDK can provide local users with a complete industry chain capability covering chip physical design and tapeout manufacturing, avoiding the influence of overseas open-source tapeout policies.** 2. An open-source PDK based on local production lines can significantly reduce tapeout costs and accelerate the conversion efficiency of chips from code to prototype products.

Finally, as of the time of this PDK release, most mainstream open-source PDKs in the industry focus on mature process nodes such as 180nm or 130nm. **However, this PDK introduces the 55nm process node, which gives open-source chips designed based on this node a strong competitive advantage in fields such as IoT, edge computing, and artificial intelligence that prioritize energy efficiency.** By releasing this PDK, ICsprout not only fills the gap in 55nm-level process nodes but also provides chip developers in China and globally with a manufacturing platform that is closer to industry needs. This will powerfully promote the development of the open-source chip ecosystem towards a **more efficient and practical** direction.

## Goal
As a key maintainer of this PDK and a major provider of open-source chip design services, the ECOS Team will collaborate closely with ICsprout. The ultimate goal is to **complete the tapeout of an open-source SoC chip based on open-source IP + open-source SoC + open-source EDA + open-source PDK (this PDK),** and on this basis, continuously optimize the EDA toolchain and integrated platform, actively develop or introduce more high-performance open-source IP components, **promoting the rebirth of the open-source chip and truly making it usable by users**. To achieve these goals, concrete actions are needed in the following areas:

- **Data Provision**: Led by ICsprout, continuously resolving and optimizing potential issues in this PDK. In addition to the initial content provided, such as STD Cell and IO, we will actively collaborate with third-party manufacturers or open-source communities to promote the adaptation of core components such as SRAM (Memory Compiler) and PLL to this PDK.
- **Integration and Chaining**: Led by the ECOS Team, this involves integrating the PDK with an open-source EDA toolchain into a comprehensive solution supporting agile design and verification of open-source chips. This process requires addressing a series of issues, including EDA tool adaptation and chaining based on the PDK, business process construction, and user experience optimization, to automate the chip design process.

Finally, the ECOS Team believes that while most people perceive chip development as very costly, including tool expenses (EDA tools and IP licensing), personnel costs, and manufacturing costs (tapeout and packaging), often reaching hundreds of millions of dollars, the increasing maturity of open-source chip design solutions (open-source IP + open-source SoC + open-source EDA + open-source PDK) has significantly reduced the barriers and costs of designing and verifying a chip. **This is an inevitable trend of the technological age and a natural progression of history.**

## Status
!!! warning "Warning"
    ICsprout currently offers the PDK contents as a preview release only!

This PDK is currently still in the development verification and iterative optimization phase and has not yet passed full silicon testing and reliability certification. **Therefore, it is strictly prohibited for use in any form of commercial mass production tapeout projects!** According to internal decisions by ICsprout and ECOS Team, the first engineering batch tapeout shuttle of this PDK is tentatively scheduled for December 2025. The data obtained from this tapeout will provide critical data for evaluating the PDK's process performance and reliability. Furthermore, it is important to note that **​​even after multiple successful tapeouts in the future, there is still no guarantee that the PDK has reached commercial mass production.** For the foreseeable future, this PDK will only support small-batch test tapeouts for talent development and academic research. Currently, the ECOS Team is closely collaborating with ICsprout to continuously fix and optimize potential issues in this PDK, and is committed to improving its compatibility and stability with mainstream open source EDA tool chains. We sincerely thanks global open source communities for their continued attention and support, and will promptly share the latest progress of this PDK with communities after the first round of tapeout.

## About
### ICsprout
ICsprout is a semiconductor foundry co-founded in 2021 by the Zhejiang Provincial Government and Zhejiang University. Leveraging an advanced 12-inch wafer pilot line, the company has built a process portfolio covering multiple nodes and categories. **​It not only offers mature 180nm and 55nm CMOS processes but also possesses specialized process capabilities such as 55nm embedded Flash (eFlash) and 180nm BCD (Bipolar-CMOS-DMOS)​,** these can extensively meet diverse manufacturing needs for analog, mixed-signal, power devices, IoT chips, etc. As a rising star and key player in China's domestic semiconductor ecosystem, ICsprout is actively promoting in-depth communication and collaboration among universities, research institutions, and open source communities in the fields of open source PDK and chip foundry services. Guided by the principles of ​​**open-source sharing**​​ and **​​independent innovation​**​, the company is committed to building a comprehensive technology platform centered on talent development and scientific research , contributing significantly to addressing the shortage of semiconductor talent and leading the development of the open source chip ecosystem.

### ECOS Team
ECOS Team's name, derived from the initials of EDA, Chip, OneStudentOneChip, and System, also represents the first four letters of Ecosystem, signifying "ecosystem". The ECOS Team was formed by the merger of the original "One Student One Chip" Team and the original "iEDA" Team. Its members primarily come from the [Frontier System Laboratory, Center for Advanced Computer Systems, Institute of Computing Technology, Chinese Academy of Sciences](https://acs.ict.ac.cn/english) and [Beijing Institute of Open Source Chip](https://www.bosc.ac.cn), etc. ECOS Team are committed to building open-source chip design solutions and its supporting technology ecosystem, using the concept of **"open source"** to innovate chip design methods, and realizing the ultimate vision of **"lowering the threshold of chip design with open source and empowering thousands of industries".**

## Contribution
The ICsprout and ECOS Team sincerely invite open source teams, experts, scholars, and enthusiasts from fields such as open source PDKs, open source EDA tools, digital IP and SoC design, backend design flows, and chip design cloud platforms to participate in the subsequent iterations and optimizations of this PDK. **We firmly believe that the successful experience of cross-domain, multi-party collaboration worldwide is applicable not only to open-source software but also to hardcore projects like open-source PDKs.​** ​Therefore, if you are passionate about this or have any questions or valuable ideas, please do not hesitate to contact us at any time. Thank you! Finally, **the ​ICsprout and ECOS Team express their highest respect to the pioneers of open-source PDKs (such as SkyWater/Google, GlobalFoundries/Google, IHP, etc.) for their outstanding contributions to the development of open-source chips!** We will do our best to apply the valuable experiences we have learned from them to the maintenance of this PDK, so that more people can freely and cost-effectively complete chip design using the 55nm process.

This PDK is licensed under the Apache 2.0 Open Source License, which primarily **allows users to modify the code and use it as either closed-source or open-source products (i.e., commercially friendly). However, it requires that copyright, patent, trademark, and attribution notices in the original code be retained when distributing the software, and that the modifications be noted in the header comments of the modified files.** The release, use, and distribution of this PDK are governed by the terms of the [Apache 2.0 Open Source License](https://github.com/openecos-projects/icsprout55-pdk/blob/main/LICENSE). To strictly comply with the license requirements and ensure legal enforceability extends to every component file, each source file in this PDK contains an Apache 2.0 license header information. **This measure is intended to provide clear licensing guidance to all users, ensuring that they can freely use, modify, and distribute the relevant design files in compliance with the terms of the license.**

```
Copyright 2025 ICsprout Integrated Circuit Co., Ltd.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

## Contact Us
| Name | Company | E-mail | Roles |
| - | - | - | - |
| ECOS Team | Institute of Computing Technology, Chinese Academy of Sciences | [ecos-all@ict.ac.cn](mailto:ecos-all@ict.ac.cn) | Project management, Document maintenance |

> Authors：Yuyang Miao (myyerrol)
