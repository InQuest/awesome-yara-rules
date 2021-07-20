<p align="center">
  <img height="128" src="./awesome-yara.png"  alt="Awesome YARA" title="Awesome YARA">
</p>

<h1 align="center">Awesome YARA</h1>

精选的 Yara 规则、工具和相关资源的清单。本清单受到 [awesome-python](https://github.com/vinta/awesome-python) 与 [awesome-php](https://github.com/ziadoz/awesome-php) 的启发创建。

> YARA 是 YARA: Another Recursive Ancronym 或者 Yet Another Ridiculous Acronym 的首字母缩写，怎么解释都可以。
>
> -- *[Victor M. Alvarez (@plusvic)](https://twitter.com/plusvic/status/778983467627479040)*

[YARA](https://virustotal.github.io/yara/) 是为恶意软件研究人员/所有人准备的模式匹配瑞士军刀，由 [@plusvic](https://github.com/plusvic/) 与 [@VirusTotal](https://github.com/VirusTotal) 开发，可在 GitHub 的[仓库](https://github.com/virustotal/yara) 中查看。

### 目录

- [规则](#规则)
- [工具](#工具)
- [服务](#服务)
- [语法高亮](#语法高亮)
- [人员](#人员)
- [相关列表](#相关列表)
- [贡献](#贡献)

### 图例

* :eyes: - 维护积极，值得一看
* :gem: - 创新且富有教育意义
* :sparkles: - 过去半年新兴的好东西
* :trophy: - 绝对不能错过

## 规则

* [AlienVault Labs Rules](https://github.com/AlienVault-Labs/AlienVaultLabs/tree/master/malware_analysis)
    - [AlienVault Labs](https://cybersecurity.att.com/blogs/labs-research) 提供的工具、签名和规则的仓库。可通过 .yar 和 .yara 扩展名找到 Yara 规则，包括 APT 检测到通用的沙盒/虚拟机检测。最后更新时间为 2016 年 1 月。
* [Apple OSX](https://gist.github.com/pedramamini/c586a151a978f971b70412ca4485c491)
    - 近 40 个检测 macOS 上恶意软件的签名。XProtect.yara 文件位于 /System/Library/CoreServices/XProtect.bundle/Contents/Resources/。
* [bamfdetect rules](https://github.com/bwall/bamfdetect/tree/master/BAMF_Detect/modules/yara)
    - Brian Wallace 提供的规则集合。
* [bartblaze YARA rules](https://github.com/bartblaze/Yara-rules) :eyes:
    - 个人 Yara 签名库。
* [BinaryAlert YARA Rules](https://github.com/airbnb/binaryalert/tree/master/rules/public)
    - 为配合 BinaryAlert 工具，AirBnB 提供了数十条规则，在 Linux、Windows 与 OS X 平台上检测恶意软件。
* [Burp YARA Rules](https://github.com/codewatchorg/Burp-Yara-Rules)
    - 通过 Yara-Scanner 扩展与 Burp Proxy 一起使用的 Yara 规则集合。主要针对通过 HTTP 传输的非 EXE 恶意软件，包含 HTML、Java、Flash、Office、PDF 文件等。最新更新于 2016 年 6 月。
* [BinSequencer](https://github.com/karttoon/binsequencer)
    - 在一组样本文件中找到通用的字节模式，据此生成 Yara 签名。
* [CAPE Rules](https://github.com/kevoreilly/CAPEv2/tree/master/data/yara) :eyes:
    - 与 Cuckoo 沙盒的 Config And Payload Extraction（CAPE）扩展绑定的规则集。
* [CDI Rules](https://github.com/CyberDefenses/CDI_yara)
    - [CyberDefenses](https://cyberdefenses.com/blog/) 提供的 Yara 签名库。
* [Citizen Lab Malware Signatures](https://github.com/citizenlab/malware-signatures)
    - Citizen Lab 提供的 Yara 签名库。包含许多恶意软件家族的数十个签名，最后更新时间为 2016 年 11 月。
* [ConventionEngine Rules](https://github.com/stvemillertime/ConventionEngine) :sparkles:
    - 检测看起来很独特、异常或明显带有恶意关键字的 PDB 路径的 Yara 规则。
* [Deadbits Rules](https://github.com/deadbits/yara-rules) :eyes:
    - Splunk 的首席威胁情报分析师 [Adam Swanda](https://www.deadbits.org/) 提供的 Yara 规则库，对外披露对恶意软件的研究进展。
* [Didier Stevens Rules](https://github.com/DidierStevens/DidierStevensSuite) :gem:
    - Didier Stevens 提供的规则集合，用于检查 OLE/RTF/PDF 的工具，这些规则通常是为威胁狩猎而写的，新的规则会在 NVISO 的[博客](https://blog.nviso.eu/)中发布。
* [ESET IOCs](https://github.com/eset/malware-ioc/) :eyes:
    - ESET 提供的 Yara 签名和 Snort 签名库。可以通过文件扩展名搜索 Yara 规则，仓库每月更新。在 [ESET WeLiveSecurity Blog](https://www.welivesecurity.com/) 上也经常披露 IOC 指标。
* [Fidelis Rules](https://github.com/fideliscyber/indicators/tree/master/yararules)
    - Fidelis Cyber 的仓库中有 6 个 Yara 规则，大约每个季度更新一次。
* [FireEye](https://github.com/fireeye/red_team_tool_countermeasures)
    - FireEye 红队工具检测签名库。
* [Florian Roth Rules](https://github.com/Neo23x0/signature-base/tree/master/yara) :eyes: :gem:
    - Florian Roth 不断更新 IOC 与 Yara 规则集合。有数十条积极维护的规则，涵盖了多种威胁类型。
* [Florian Roth's IDDQD Rule](https://gist.github.com/Neo23x0/f1bb645a4f715cb499150c5a14d82b44)
    - 展示检测红队和威胁工具的 POC 规则。
* [f0wl yara_rules](https://github.com/f0wl/yara_rules)
    - https://dissectingmalwa.re/ 博客提供的 Yara 签名库。
* [Franke Boldewin Rules](https://github.com/fboldewin/YARA-rules)
    - [@r3c0nst](https://twitter.com/@r3c0nst) 提供的 Yara 规则集。
* [FSF Rules](https://github.com/EmersonElectricCo/fsf/tree/master/fsf-server/yara)
    - 用于 EmersonElectricCo FSF 的文件类型检测规则。
* [GoDaddy ProcFilter Rules](https://github.com/godaddy/yara-rules)
    - 由 GoDaddy 发布的数十条可与 ProcFilter 一起使用的规则，包括检测壳、mimikatz 和特定的恶意软件。
* [h3x2b Rules](https://github.com/h3x2b/yara-rules) :gem:
    - 由 h3x2b 提供的规则集，可用于辅助逆向工程。例如标识加密代码、高熵值代码（证书发现）、注入\Hook 代码等。
* [Icewater Rules](https://github.com/SupportIntelligence/Icewater)
    - Icewater.io 提供的自动生成的 Yara 规则集合。
* [Intezer Rules](https://github.com/intezer/yara-rules) :sparkles:
    - Intezer 提供的 Yara 规则。
* [InQuest Rules](https://github.com/InQuest/yara-rules) :eyes:
    - InQuest 研究员发布的、针对 VirusTotal 的威胁狩猎规则。规则会不断更新，在 InQuest 的[博客](http://blog.inquest.net)上也会讨论新的发现。
* [jeFF0Falltrades Rules](https://github.com/jeFF0Falltrades/YARA-Signatures) :sparkles:
    - 各类恶意软件家族的 Yara 规则集。
* [kevthehermit Rules](https://github.com/kevthehermit/YaraRules)
    - Kevin Breen 个人的数十条规则，自 2016 年 2 月再未更新。
* [Koodous Community Rules](https://koodous.com/rulesets)
    - 社区驱动的 Android APK 恶意软件检测规则。
* [Loginsoft Rules](https://research.loginsoft.com/yara-rules/)
    - 针对 Microsoft Office 格式文件进行检测的 Yara 规则。
* [Loginsoft Detection Rules](https://github.com/Loginsoft-Research)
    - 用于开源组件的威胁检测与异常检测规则。
* [lw-yara](https://github.com/Hestat/lw-yara)
    - 用于扫描 Linux 服务器中的垃圾邮件、钓鱼网站和其他 Web 恶意程序的规则集。
* [NCC Group Rules](https://github.com/nccgroup/Cyber-Defence/tree/master/Signatures/yara) :eyes:
    - 由 NCC 的网络安全防御团队提供的 Yara 规则集。
* [Malice.IO YARA Plugin Rules](https://github.com/malice-plugins/yara/tree/master/rules) :eyes:
    - 多来源、有关 Malice.IO 框架的 Yara 规则集。
* [Malpedia Auto Generated Rules](https://malpedia.caad.fkie.fraunhofer.de/api/get/yara/auto/zip) :sparkles:
    - 包含由 Malpedia 的 YARA-Signator 自动创建的规则。
* [McAfee Advanced Threat Research IOCs](https://github.com/advanced-threat-research/IOCs)
    - 与 McAfee ATR 的博客和其他公开文章一起发布的 Yara 规则等。
* [McAfee Advanced Threat Research Yara-Rules](https://github.com/advanced-threat-research/Yara-Rules)
    - McAfee ATR Teams 提供的 Yara 规则集。
* [mikesxrs YARA Rules Collection](https://github.com/mikesxrs/Open-Source-YARA-rules) :eyes: :trophy:
    - 各种来源的开源 Yara 规则集合，包含超过 100 个类别、1500 个文件、4000 条规则，如果只能下载一个进行分析，那一定是这个。
* [Patrick Olsen Rules](https://github.com/prolsen/yara-rules) :gem:
    - 针对 RAT、文档、PCAP、可执行文件等恶意软件进行扫描的规则集，不幸的是在 2014 年就停止了更新。
* [QuickSand Lite Rules](https://github.com/tylabs/quicksand_lite)
    - 该仓库包含一个用 C 写的框架和一些用于恶意软件分析的独立工具，以及一些相关的 Yara 规则。
* [Rastrea2r](https://github.com/rastrea2r/rastrea2r)
    - 在几分钟内对数千个端点进行 IOC 扫描狩猎。
* [ReversingLabs YARA Rules](https://github.com/reversinglabs/reversinglabs-yara-rules) :sparkles: :eyes:
    - 由 ReversingLabs 提供的 Yara 规则集，包含 Exploit、窃密软件、勒索软件、木马与病毒等恶意软件类型。
* [Securitymagic's YARA Rules](https://github.com/securitymagic/yara)
    - 应对威胁的 Yara 规则。
* [Sophos AI YaraML Rules](https://github.com/inv-ds-research/yaraml_rules)
    - 自动创建的 Yara 规则库，每个目录下都包含 Yara 规则和相应的元数据（机器学习训练使用的文件哈希值和 ROC 曲线）。
* [SpiderLabs Rules](https://github.com/SpiderLabs/malware-analysis/tree/master/Yara)
    - SpiderLabs 提供的工具与脚本集合。只包含 3 个 Yara 规则，最后一次更新在 2015 年，但仍然值得一看。
* [StrangeRealIntel's Daily IOCs](https://github.com/StrangerealIntel/DailyIOC) :gem: :sparkes: :eyes:
    - 针对新兴威胁定期更新的 Yara 规则集合。
* [t4d's PhishingKit-Yara-Rules](https://github.com/t4d/PhishingKit-Yara-Rules)
    - 用于网络钓鱼工具包的 Yara 规则，基于 zip 压缩文件的原始格式分析发现目录与文件名。
* [Tenable Rules](https://github.com/tenable/yara-rules)
    - Tenable Network Security 提供的小型规则集合。
* [TjadaNel Rules](https://github.com/tjnel/yara_repo)
    - 针对恶意软件的小型规则集合。
* [VectraThreatLab Rules](https://github.com/VectraThreatLab/reyara)
    - 识别反逆向工程技术的 Yara 规则。
* [x64dbg Signatures](https://github.com/x64dbg/yarasigs) :gem:
    - 识别加壳、编译器、加密的签名规则。
* [YAIDS](https://github.com/wrayjustin/yaids) :gem: :sparkles:
    - 使用 Yara 的多线程入侵检测系统，YAIDS 支持所有有效的 Yara 规则、模块与任何 PCAP 兼容数据流（网络、USB、蓝牙等）。
* [YARA-FORENSICS](https://github.com/Xumeiquer/yara-forensics)
    - 文件类型识别规则集合。
* [yara4pentesters](https://github.com/DiabloHorn/yara4pentesters)
    - 识别包含类似用户名、密码等信息文件的规则。
* [YaraRules Project Official Repo](https://github.com/Yara-Rules/rules) :eyes:
    - 社区不断更新维护的规则集。
* [Yara-Unprotect](https://github.com/fr0gger/Yara-Unprotect)
    - 为 Unprotect 创建的规则，用于检测恶意软件逃避技术。

## 工具

* [AirBnB BinaryAlert](https://github.com/airbnb/binaryalert)
    - 开源 AWS 管道，使用配置好的 Yara 签名扫描上传到 S3 中的所有文件。
* [androguard](https://github.com/Koodous/androguard-yara)
    - 集成 APK 分析的 Yara 模块。
* [bamfdetect](https://github.com/bwall/bamfdetect)
    - 从恶意软件中识别并提取信息。
* [base64_substring](https://github.com/DissectMalware/base64_substring)
    - 匹配基于 base64 编码数据的 Yara 规则。
* [CAPE: Config And Payload Extraction](https://github.com/kevoreilly/CAPEv2) :eyes:
    - 用于从恶意软件中提取 Payload 和配置文件的 Cuckoo 的扩展，首次运行检测恶意软件家族，根据不同的家族在二次执行时提取 Payload 和配置文件。
* [CCCS-Yara](https://github.com/CybercentreCanada/CCCS-Yara)
    - Yara 规则元数据规范和验证程序。
* [clara](https://github.com/abhinavbom/clara) :sparkles:
    - 实时 ClamAV + Yara 扫描 S3 存储桶。
* [CrowdStrike Feed Management System](https://github.com/CrowdStrike/CrowdFMS)
    - 自动收集、处理来自 VirusTotal 的样本文件，基于 Yara 规则匹配结果进行处理。
* [CSE-CST AssemblyLine](https://bitbucket.org/cse-assemblyline/alsvc_yara)
    - 由加拿大通信安全机构（CSE）开源的 [AssemblyLine](https://cyber.gc.ca/en/assemblyline)，该工具用于分析恶意文件，也为 Yara 提供了接口。
* [dnYara](https://github.com/airbus-cert/dnYara)
    - 用于本地 Yara 库的多平台 .NET 库。
* [ELAT](https://github.com/reed1713/ELAT)
    - 使用 Yara 规则进行 Windows 事件日志分析。
* [Emerson File Scanning Framework (FSF)](https://github.com/EmersonElectricCo/fsf)
    - 模块化、递归文件扫描工具。
* [findcrypt-yara](https://github.com/polymorf/findcrypt-yara) and [FindYara](https://github.com/OALabs/FindYara)
    - 使用 Yara 规则扫描样本文件文件发现加密常量的 IDA Pro 插件。
* [Fnord](https://github.com/Neo23x0/Fnord)
    - 用于混淆代码的模式提取工具。
* [generic-parser](https://github.com/uppusaikiran/generic-parser)
    - 支持 Yara 的解析器，用于提取文件元信息、执行静态分析并检测文件中的宏代码。
* [GoDaddy ProcFilter](https://github.com/godaddy/procfilter) :gem:
    - ProcFilter 是内置 Yara 的 Windows 进程过滤工具，可以使用自定义的元标记对 Yara 规则进行检测，根据检测结果进行对应的响应处理。工具作为 Windows 服务运行，且与 Windows 的 ETW API 整合在一起，结果在 Windows 事件日志中可见。安装、启动和删除都可以动态完成，无需重新启动计算机。
* [go-yara](https://github.com/hillu/go-yara)
    - Yara 的 Go 接口。
* [halogen](https://github.com/target/halogen)
    - Halogen 是针对嵌入恶意文档中的图片自动创建 Yara 规则的工具。
* [Hyara](https://github.com/hyuunnn/Hyara)
    - 为 IDA Pro、Cutter 以及 BinaryNinja 提供的，为给定起始地址和终止地址之间的 ASCII 和十六进制字符串创建 Yara 规则的插件。
* [IDA_scripts](https://github.com/swackhamer/IDA_scripts)
    - 用于从可执行操作码（包括 .NET 在内）生成 Yara 签名的 IDAPython 脚本。
* [ida_yara](https://github.com/alexander-hanel/ida_yara)
    - 使用 Yara 扫描 IDB 内的数据。
* [ida-yara-processor](https://github.com/bnbdr/ida-yara-processor)
    - 用于编译好的 Yara 规则的 IDA Processor。
* [InQuest ThreatKB](https://github.com/InQuest/ThreatKB)
    - 基于 Yara 规则和 IOC 指标等知识的工作流管理。
* [iocextract](https://github.com/InQuest/python-iocextract)
    - IOC 提取工具，具备 Yara 规则的提取能力。
* [Invoke-Yara](https://github.com/secabstraction/Yara)
    - 在远程设备中运行 Yara 的 PowerShell 脚本。
* [KLara](https://github.com/KasperskyLab/klara)
    - 使用 Python 写的分布式扫描系统，允许研究人员扫描样本库中的样本。
* [Laika BOSS](https://github.com/lmco/laikaboss)
    - 提供可扩展、灵活、详细的对象扫描和入侵检测系统。
    - [Laika BOSS 白皮书](https://github.com/lmco/laikaboss/blob/master/LaikaBOSS_Whitepaper.pdf)
* [MalConfScan](https://github.com/JPCERTCC/MalConfScan)
    - 提取已知恶意软件配置的 Volatility 插件，该工具在内存中搜索恶意软件并提取配置信息。
* [malscan](https://github.com/usualsuspect/malscan)
    - 使用 Yara 进行进程内存扫描，匹配中即执行 Python 脚本。
* [MISP Threat Sharing](https://github.com/MISP/MISP)
    - 包括 IOC、威胁情报、恶意样本在内的威胁情报平台，包括共享、生成和验证 Yara 规则的支持。
* [MITRE MultiScanner](https://github.com/mitre/multiscanner)
    - 通过自动为文件执行分析帮助用户评估一组文件。
* [mkYARA](https://github.com/fox-it/mkYARA)
    - 基于二进制代码创建 Yara 规则。
* [mquery](https://github.com/CERT-Polska/mquery)
    - 用于在大型数据集上快速进行 Yara 扫描的 Web 前端。
* Nextron Systems OSS and Commercial Tools (Florian Roth: @Neo23x0)
    - [Loki](https://github.com/Neo23x0/Loki) Pyton 实现的 IOC 与 Yara 规则扫描工具。（开源、免费）
    - [THOR Lite](https://www.nextron-systems.com/thor-lite/) Go 实现的 IOC 与 Yara 规则扫描工具。（闭源、免费但需要注册）
* [node-yara](https://github.com/nospaceships/node-yara)
    - Yara 的 Node.js 接口。
* [OCYara](https://github.com/bandrel/OCyara)
    - 对图片进行 OCR 再使用 Yara 进行扫描。
* [PasteHunter](https://github.com/kevthehermit/PasteHunter)
    - 使用 Yara 规则扫描 pastebin.com。
* [plast](https://github.com/sk4la/plast)
    - 使用 Yara 构建的检测、处理 IOC 指标的威胁狩猎工具。
* [plyara](https://github.com/plyara/plyara)
    - Python 编写的解析 Yara 规则工具。
* [Polichombr](https://github.com/ANSSI-FR/polichombr)
    - 具有 Yara 规则匹配和其他功能的恶意软件分析框架。
* [PwC Cyber Threat Operations rtfsig](https://github.com/PwCUK-CTO/rtfsig)
    - 简化对 RTF 文档中可能独特的部分进行签名。
* [VirusTotalTools](https://github.com/silascutler/VirusTotalTools)
    - 利用 VirusTotal 分析样本的工具，包括 VT_RuleMGR。
* [QuickSand.io](http://quicksand.io/)
    - 分析恶意文档的 Compact C 框架，包括 Web 界面和在线分析能力。
* [shotgunyara](https://github.com/darienhuss/shotgunyara)
    - 给定一个字符串，基于该字符串创建 255 个异或后的版本的 Yara 规则。
* [spyre](https://github.com/spyre-project/spyre)
    - 基于 Yara 的文件 IOC 扫描工具。
* [static_file_analysis](https://github.com/lprat/static_file_analysis)
    - 使用 clamscan 和 Yara 深度分析文件（doc、pdf、exe 等）
* [stoQ](https://github.com/PUNCH-Cyber/stoq)
    - 模块化和高度定制的框架，用于从多个不同数据源创建数据集。
* [Strelka](https://github.com/target/strelka)
    - 基于 Python3、ZeroMQ 和 Yara 构建的文件分析系统，用于威胁检测和情报收集。
* [SwishDbgExt](https://github.com/comaeio/SwishDbgExt)
    - 使用 Yara 规则在进程内存中进行匹配的 WinDbg 扩展。
* [ThreatIngestor](https://github.com/InQuest/ThreatIngestor/)
    - 多来源信息自动提取 IOC（包括 Yara 在内）。
* [UXProtect](https://digitasecurity.com/uxprotect/)
    - Apple 内置的 XProtect 进行 Yara 扫描。
* [VTCodeSimilarity-YaraGen](https://github.com/arieljt/VTCodeSimilarity-YaraGen) :gem: :sparkles:
    - 由 [@arieljt](https://twitter.com/arieljt) 编写的 VirusTotal 的 `code-similar-to:` 功能的 Yara 规则生成器。
* [Vxsig](https://github.com/google/vxsig) :sparkles:
    - 通过相似样本集自动生成 AV 字节签名。
* [yabin](https://github.com/AlienVault-OTX/yabin)
    - 通过恶意软件的可执行代码创建 Yara 签名。
* [yaml2yara](https://github.com/nccgroup/yaml2yara)
    - 通过 YAML 批量生成 Yarar 规则。
* [YARA-CI](https://yara-ci.cloud.virustotal.com/) :sparkles:
    - YARA-CI 帮助在规则更改时进行自动化测试。
* [yara-endpoint](https://github.com/Yara-Rules/yara-endpoint)
    - 基于 Yara 的事件响应工具。
* [Yara Finder](https://github.com/uppusaikiran/yara-finder)
    - 基于 @tylerha97 的 yara_scan 开发的扫描框架，具有 Web API 与 Docker 化部署。
* [YaraGenerator](https://github.com/Xen0ph0n/YaraGenerator)
    - 快速、简单、有效的 Yara 规则生成工具。
* [YaraGen](https://github.com/mrexodia/YaraGen) and [yara_fn](https://github.com/williballenthin/idawilli/tree/master/scripts/yara_fn)
    - 为 x64dbg 与 IDAPython 编写的、基于函数块生成 Yara 规则的插件。
* [YaraGuardian](https://github.com/PUNCH-Cyber/YaraGuardian)
    - 基于 Django 开发、用于管理 Yara 规则的 Web 界面。
* [yara-java](https://github.com/p8a/yara-java)
    - Yara 的 Java 接口。
* [yaraMail](https://github.com/kevthehermit/yaraMail)
    - 用于 IMAP 订阅与保存流的 Yara 扫描工具。
* [Yara Malware Quick menu scanner](https://github.com/techbliss/Yara_Mailware_Quick_menu_scanner)
    - 将 Yara 扫描添加到 Windows 右键点击菜单中。
* [YaraManager](https://github.com/kevthehermit/YaraManager)
    - 通过 Web 管理 Yara 规则的工具。
* [yaramod](https://github.com/avast/yaramod)
    - 将 Yara 规则解析为 AST 的工具，并且提供了构建 Yara 规则的 C++ 接口。
* [yarAnalyzer](https://github.com/Neo23x0/yarAnalyzer)
    - Yara 规则覆盖度分析工具。
* [yara-parser](https://github.com/Northern-Lights/yara-parser)
    - 使用 Go 编写的解析规则工具。
* [yaraPCAP](https://github.com/kevthehermit/YaraPcap)
    - 用于 IMAP 订阅与保存流的 Yara 扫描工具。
* [yara-procdump-python](https://github.com/google/yara-procdump-python)
    - Yara 进程内存访问 API 的 Python 接口。
* [yara-signator](https://github.com/fxb-cocacoding/yara-signator) :sparkles:
    - 用于 Malpedia 的自动 Yara 规则生成工具。
* [YARA-sort](https://github.com/horsicq/YARA-sort)
    - 根据 Yara 规则扫描文件，详情请查看[博客文章](https://n10info.blogspot.com/2019/10/nfd-sort.html)。
* [Yara Python ICAP Server](https://github.com/RamadhanAmizudin/python-icap-yara)
    - 提供 Yara 扫描的 ICAP 服务器。
* [yarasafe](https://github.com/lucamassarelli/yarasafe)
    - 使用机器学习进行自动化地函数签名生成。
* [Yara-Scanner](https://github.com/PolitoInc/Yara-Scanner)
    - Python 开发的、Burp Suite 的 Yara 扩展。
* [yarascanner](https://github.com/jheise/yarascanner)
    - Golang 开发的、Yara 扫描文件的 Web 服务。
* [yara_tools](https://github.com/matonis/yara_tools)
    - 使用 Python 进行 Yara 规则配置的接口。
* [Yara-Validator](https://github.com/CIRCL/yara-validator)
    - 验证 Yara 规则并尝试修复损坏的规则。
* [yaraVT](https://github.com/deadbits/yaraVT)
    - 使用 Yara 规则扫描文件，将规则匹配结果作为评论发送到 VirusTotal。
* [yara_zip_module](https://github.com/stoerchl/yara_zip_module)
    - 扫描在 zip 压缩文件内的字符串。
* [yarg](https://github.com/immortalp0ny/yarg)
    - 基于 x86/x86-64 代码生成 Yara 规则的 IDAPython 插件。
* [yarGen](https://github.com/Neo23x0/yarGen)
    - 用于发现相关样本进行狩猎的 Yara 规则生成工具。
* [Yara Scanner](https://github.com/ace-ecosystem/yara_scanner)
    - 为 yara-python 项目提供接口，包含多种功能。
* [yaya](https://github.com/EFForg/yaya)
    - 自动管理开源 Yara 规则并运行扫描。
* [YaYaGen](https://github.com/jimmy-sonny/YaYaGen)
    - Android 恶意软件的 Yara 规则生成工具。
* [Yeti](https://github.com/yeti-platform/yeti)
    - 该平台旨在一个库内组织 IOC 指标、TTP 与威胁相关的知识。
* [yextend](https://github.com/BayshoreNetworks/yextend)
    - 使 Yara 可以检测压缩文件的扩展。
* [yaraZeekAlert](https://github.com/SCILabsMX/yaraZeekAlert) :sparkles:
    - 使用 Yara 规则扫描文件，出发告警的可发送电子邮件提醒，如果恶意文件小于 10MB 则将其作为附件发送。

## 服务

* [Hybrid Analysis YARA Search](https://www.hybrid-analysis.com/yara-search)
    - 由 CrowdStrike/Hybrid Analysis 提供的 Yara 检索/狩猎。
* [InQuest Labs](https://labs.inquest.net) :sparkles: :gem:
    - 其中 Yara 规则的部分提供将正则表达式转换为匹配 base64 编码的字符串、将字符串转换为 uint() 可查的序列等示例。
* [Koodous](https://koodous.com/)
    - APK 分析平台，带有社区 Yara 规则库和大型 APK 样本数据集。
* [MalShare](https://malshare.com/)
    - 免费样本库，允许安全研究人员访问恶意样本和 Yara 结果。
* [MalwareConfig](https://malwareconfig.com/)
    - 从 RAT 木马中提取 IOC 指标。
* [YaraEditor (Web)](https://www.adlice.com/download/yaraeditorweb/)
    - 用于创建和管理 Yara 规则的多合一网站。
* [Yara Share](https://yara.adlice.com/)
    - 提供用户上传、共享 Yara 规则的在线社区。

## 语法高亮

* Atom: [language-yara](https://github.com/blacktop/language-yara)
* 基于 GTK 的编辑器，如 gedit 与 xed: [GtkSourceView-YARA](https://github.com/wesinator/GtkSourceView-YARA)
* Sublime Text: [YaraSyntax](https://github.com/nyx0/YaraSyntax/)
* Vim: [vim-yara](https://github.com/yaunj/vim-yara)
* Visual Studio Code: [textmate-yara](https://github.com/infosec-intern/textmate-yara)

## 人员

将本页提到的有关人员的 Twitter 汇总到一个列表（[awesome-yara Twitter list](https://twitter.com/InQuest/lists/awesome-yara)）中，如果未列出可以向我们确认。

## 相关列表

* [Crawler](https://github.com/BruceDone/awesome-crawler)
* [CVE PoC](https://github.com/qazbnm456/awesome-cve-poc)
* [Forensics](https://github.com/Cugu/awesome-forensics)
* [Hacking](https://github.com/carpedm20/awesome-hacking)
* [HackwithGithub](https://github.com/Hack-with-Github/Awesome-Hacking)
* [Honeypots](https://github.com/paralax/awesome-honeypots)
* [Incident-Response](https://github.com/meirwah/awesome-incident-response)
* [Infosec](https://github.com/onlurking/awesome-infosec)
* [IOCs](https://github.com/sroberts/awesome-iocs)
* [Malware Analysis](https://github.com/rshipp/awesome-malware-analysis)
* [ML for Cyber Security](https://github.com/jivoi/awesome-ml-for-cybersecurity)
* [OSINT](https://github.com/jivoi/awesome-osint)
* [PCAP Tools](https://github.com/caesar0301/awesome-pcaptools)
* [Pentesting](https://github.com/enaqx/awesome-pentest)
* [Reversing](https://github.com/tylerha97/awesome-reversing)
* [Security](https://github.com/sbilly/awesome-security)
* [Static Analysis](https://github.com/analysis-tools-dev/static-analysis)
* [Threat Detection](https://github.com/0x4D31/awesome-threat-detection)
* [Threat Intelligence](https://github.com/hslatman/awesome-threat-intelligence)

## 贡献

该列表由 [InQuest](https://inquest.net/) 维护，可以随时补充提交缺少的内容。

提交请查看文档 [CONTRIBUTING.md](CONTRIBUTING.md)。
