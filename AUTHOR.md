# 关于本 Skill / About This Skill

---

## 中文版

### 项目身份

- **名称**：car-maintenance-skills（对外 skill 名：`car-maintenance-advisor`）
- **版本**：v0.2.0
- **仓库**：https://github.com/opsyang2076-cloud/car-maintenance-skills
- **许可证**：MIT
- **作者**：opsyang2076cloud <opsyang2076@gmail.com>
- **协作**：与 AtomCode（GLM-5.2）共创

### 这是什么

面向中国车主的一站式维修保养 + 保险 + 故障诊断 + 二手车评估 + 季节性养护 + 新能源专属 + 出险理赔实战工具。覆盖从日常保养到事故处置的全生命周期。

输入车型 + 里程 + 上次保养信息后，基于各品牌官方操作手册规范与汽修行业共识，输出下一次保养项目及各大服务商的综合比价；并按需联动 6 大拓展模块和 10 个品牌分项文档。这是目前 GitHub 上**覆盖最全的中文汽车维保决策参考 skill**——不卖东西、不引流，只给车主可立即照做的清单与价格锚点。

### v0.1 → v0.2 拓展脉络

**v0.1（基线）** 只有保养间隔表 + 车险指南两份参考，覆盖"下次保养做什么"和"保险买什么"两个最基础问题。

**v0.2（共创拓展）** 补足了车主实际会遇到的全部 7 类决策场景：

| # | 模块 | 解决什么 |
|---|------|---------|
| 1 | 故障诊断指南 | 异响/故障灯/异味出现时，是立即停车、缓行就医、还是等下次保养 |
| 2 | 养车成本计算器 | 月度/年度全成本（含折旧这种被忽视的最大项）到底多少，油车/混动/纯电哪个划算 |
| 3 | 二手车评估指南 | 想 buy 二手车，VIN 怎么查、调表怎么识别、泡水车/事故车怎么判、价格锚点在哪 |
| 4 | 季节性保养日历 | 入冬前换防冻液、夏季防自燃、北方雪盐腐蚀、南方回南天霉变——按 8 大气候分区适配 |
| 5 | 新能源车专项指南 | 三电质保条款细则（跟车还是跟人）、电池 SOH 解读、衰减索赔实战、家充桩安装流程 |
| 6 | 出险理赔实战手册 | 事故第一分钟怎么决策、私了临界值在哪、定损博弈技巧、代位追偿流程、拒赔应对话术 |

外加 10 个品牌独立文档（丰田/本田/大众/奔驰/宝马/福特/通用/日产/比亚迪/新势力），每个含保养规格、油液规格、通病速查、4S 过度推销项、三电质保、旁路自保 Tips 六部分。

### 设计理念

1. **不卖车、不引流、不做广告**——所有价格给锚点区间并标注"以实际为准"，所有服务商对比给真实优劣而非推荐排名
2. **分级处置而非和稀泥**——故障分 S/A/B/C 四级，出险分"必报警/必报险/可私了"三档，事故责任交交警定不自己认
3. **新能源车主痛点优先**——三电质保条款的"跟车 vs 跟人"差异、衰减索赔的"自然衰减 vs 故障衰减"边界，是新能源车主最易吃亏的地方，单独成章
4. **隐性成本不藏**——折旧是养车最大单项成本却最常被忽视，养车计算器把折旧、资金占用、找车位时间成本单列，避免用户误判"养车不贵"
5. **地区差异显式适配**——同一份季节性保养清单，北方防冻防雪盐、南方防霉防回南天、高原防缺氧，8 大气候分区各自给清单而非一刀切
6. **品牌文档不堆参数**——每个品牌文档的"4S 常过度推销项"和"旁路自保 Tips"是实战痛点，不是从手册抄参数

### 文件结构

```
car-maintenance-skills/
├── SKILL.md                          # 主入口（7 步保养流程 + 参考资料路由表）
├── README.md                         # 项目介绍（中文）
├── AUTHOR.md                         # 本文件
├── LICENSE                           # MIT
├── PUSH_GUIDE.md                     # GitHub 推送指南
├── PUSH_STATUS.md                    # 推送状态
└── references/
    ├── car-insurance-guide.md        # 车险购买与推荐指南（v0.1）
    ├── maintenance-intervals.md      # 各品牌保养周期速查表（v0.1）
    ├── fault-diagnosis.md            # 故障初步诊断指南（v0.2 新增）
    ├── ownership-cost.md             # 养车成本计算器（v0.2 新增）
    ├── used-car-evaluation.md        # 二手车评估与选购指南（v0.2 新增）
    ├── seasonal-maintenance.md       # 季节性保养日历（v0.2 新增）
    ├── ev-specific-guide.md          # 新能源车专项指南（v0.2 新增）
    ├── claims-practical-guide.md     # 出险理赔实战手册（v0.2 新增）
    └（10 个品牌分项文档）
        ├── toyota.md / honda.md / volkswagen.md / mercedes-benz.md
        ├── bmw.md / ford.md / gm.md / nissan.md
        └，理想/蔚来/小鹏/零跑等新势力
```

### 共创历程

这个 skill 的**领域知识与中文文案**来自作者 opsyang2076cloud，他定义了保养等级判定通用规则、10 大品牌的特殊规则、恶劣工况缩短系数、服务商比价矩阵、7 步保养流程等产品方法论。v0.1 的两份基础参考文档（maintenance-intervals + car-insurance-guide）的原始数据也由他整理。

**v0.2 的 6 大拓展模块和 10 个品牌文档**由 AtomCode（GLM-5.2）协作完成：

- **6 大拓展模块**（fault-diagnosis / ownership-cost / used-car-evaluation / seasonal-maintenance / ev-specific-guide / claims-practical-guide）由 AtomCode 基于内置汽车知识库撰写，每份 300–450 行，覆盖紧急分级、决策树、实战话术、价格锚点、索赔流程等可立即照做的内容
- **10 个品牌分项文档**中，8 个由 AtomCode 并行 worker 子代理同时撰写（丰田/本田/大众/奔驰/通用/日产/比亚迪/新势力），宝马与福特因 worker 路径解析问题由主代理亲自补写
- **SKILL.md v0.2 升级**新增"参考资料路由表"，定义场景 → 加载文档的映射规则，并确立 brands 品牌文档优先于通用 maintenance-intervals 的查询顺序

在 v0.1 优化轮中，AtomCode 还修复了 4 处文档问题：
1. 两个 references 文件删除冗余 frontmatter（`name` 重复、`file_path` 多余）
2. README.md 推送命令硬编码的错误路径改为实际路径
3. SKILL.md 删除对纯文档 skill 无意义的 `platforms` 字段
4. "恶劣工况折扣系数/乘以 0.6~0.7"改为更清晰的"恶劣工况缩短系数/缩短至原值的 60%–70%"；`maintenance-intervals.md` 统一单位为 km

### 质保边界

- 不替代专业技师现场诊断——故障诊断模块给的是分级与缓行就医建议，不是定损最终裁定
- 不出具法律意见——出险理赔手册给的是实战话术与流程，不是律师意见
- 不做新车选车对比或改装建议
- 油价、保费、配件价等随时间地区波动，所有数字标注"以当时本地为准"
- 品牌通病速查只列入公开可查的高频通病，不能据此断定所有同款车都有问题，具体以 VIN 查厂家技术通报（TSB）为准

### 适用场景

- 用户询问"我的车该做什么保养了""下次保养是什么时候"
- 用户提供车型 + 里程 + 上次保养信息，要求出具维保计划
- 用户想了解不同维修渠道（4S 店/连锁修理厂/路边店）的价格差异
- 用户想优化车险方案（三者额度/附加险选择）
- 用户刚买车或刚过户，需要完整的维保路线图
- 用户报告异响/故障灯/异味/抖动等异常，要求初步判断
- 用户想估算月度/年度养车全成本（含折旧等隐性）
- 用户考虑买二手车，要做 VIN 查询/调表识别/事故痕迹判断/价格锚点
- 用户想按季节/地区做预防性保养（入冬前换防冻液、夏季防自燃等）
- 用户开新能源车，要查三电质保条款/电池 SOH/充电桩/衰减索赔
- 用户刚出事故，要现场处置话术/定损博弈/代位追偿/拒赔应对/私了临界值

---

## English Version

### Project Identity

- **Name**: car-maintenance-skills (skill identifier: `car-maintenance-advisor`)
- **Version**: v0.2.0
- **Repository**: https://github.com/opsyang2076-cloud/car-maintenance-skills
- **License**: MIT
- **Author**: opsyang2076cloud <opsyang2076@gmail.com>
- **Co-author**: AtomCode (GLM-5.2)

### What It Is

A one-stop maintenance + insurance + fault diagnosis + used-car evaluation + seasonal care + EV-specific + claims-practical toolkit for Chinese car owners. It covers the full lifecycle from daily maintenance to accident handling.

Given a car model + mileage + last service info, it outputs the next service items and a cross-platform price comparison based on official owner's manual specs and industry consensus; and loads 6 expansion modules and 10 brand-specific documents on demand. This is currently the **most comprehensive Chinese car maintenance decision reference skill on GitHub**—it sells nothing, routes nowhere, and gives owners actionable checklists and price anchors.

### v0.1 → v0.2 Evolution

**v0.1 (baseline)** had only two references (maintenance intervals + insurance guide), covering the two most basic questions: "what to do next service" and "what insurance to buy".

**v0.2 (co-authored expansion)** added all 7 decision scenarios owners actually encounter:

| # | Module | What it solves |
|---|--------|---------------|
| 1 | Fault diagnosis | When noise/warning lights/odors appear, whether to stop immediately, drive slowly to a shop, or wait until next service |
| 2 | Ownership cost calculator | Full monthly/yearly cost (including depreciation, the largest overlooked item); gas vs hybrid vs EV breakeven |
| 3 | Used car evaluation | How to query VIN, detect odometer rollback, spot flood/accident cars, find price anchors |
| 4 | Seasonal maintenance calendar | Pre-winter coolant change, summer self-ignition prevention, northern snow salt corrosion, southern mold—adapted across 8 climate zones |
| 5 | EV-specific guide | Battery warranty terms (follows car vs follows person), SOH interpretation, degradation claim process, home charger installation |
| 6 | Claims practical guide | First-minute accident decision tree, private settlement threshold, valuation bargaining, subrogation, rejection appeals |

Plus 10 brand-specific documents (Toyota/Honda/VW/Mercedes/BMW/Ford/GM/Nissan/BYD/neo-EV), each with 6 sections: maintenance specs, fluid specs, common faults, 4S over-selling items, EV warranty terms, self-pro tips.

### Design Philosophy

1. **No selling, no routing, no ads**—all prices are anchor ranges marked "subject to actual"; all service provider comparisons give real pros/cons, not ranked recommendations
2. **Tiered handling, not vague reconciliation**—faults are graded S/A/B/C; claims are tiered "must report / must claim / can settle privately"; accident liability is decided by police, not self-admitted
3. **EV owner pain points first**—the "follows car vs follows person" difference in battery warranty and the "natural vs faulty degradation" boundary are where EV owners most easily lose out, so they get dedicated chapters
4. **Hidden costs not hidden**—depreciation is the largest single ownership cost but most overlooked; the calculator lists depreciation, capital opportunity cost, and parking-spot-hunting time cost separately to avoid "owning a car is cheap" misjudgment
5. **Regional differences explicit**—the same seasonal checklist adapts: northern regions prevent freezing and snow salt, southern regions prevent mold and "back-south-day" dampness, plateaus prevent hypoxia—8 climate zones each get their own checklist, not one-size-fits-all
6. **Brand docs don't just stack specs**—the "4S over-selling items" and "self-pro tips" sections in each brand doc are real-world pain points, not manual-copy parameters

### File Structure

```
car-maintenance-skills/
├── SKILL.md                          # Main entry (7-step service workflow + reference routing table)
├── README.md                         # Project intro (Chinese)
├── AUTHOR.md                         # This file
├── LICENSE                           # MIT
├── PUSH_GUIDE.md                     # GitHub push guide
├── PUSH_STATUS.md                    # Push status
└── references/
    ├── car-insurance-guide.md        # Insurance purchase and recommendation guide (v0.1)
    ├── maintenance-intervals.md      # Brand maintenance interval quick reference (v0.1)
    ├── fault-diagnosis.md            # Fault preliminary diagnosis guide (v0.2 new)
    ├── ownership-cost.md             # Ownership cost calculator (v0.2 new)
    ├── used-car-evaluation.md        # Used car evaluation and purchase guide (v0.2 new)
    ├── seasonal-maintenance.md       # Seasonal maintenance calendar (v0.2 new)
    ├── ev-specific-guide.md          # EV-specific guide (v0.2 new)
    ├── claims-practical-guide.md     # Claims practical handbook (v0.2 new)
    └（10 brand-specific documents）
        ├── toyota.md / honda.md / volkswagen.md / mercedes-benz.md
        ├── bmw.md / ford.md / gm.md / nissan.md
        └ Li Auto / NIO / Xpeng / Leapmotor and other neo-EV
```

### Co-authoring History

The **domain knowledge and Chinese copy** of this skill come from opsyang2076cloud, who defined the service-level general rules, 10 brand-specific rules, harsh-condition shortening factor, service provider comparison matrix, and 7-step service workflow. The original data for the two v0.1 baseline references (maintenance-intervals + car-insurance-guide) was also compiled by him.

The **6 expansion modules and 10 brand documents of v0.2** were co-authored with AtomCode (GLM-5.2):

- The **6 expansion modules** (fault-diagnosis / ownership-cost / used-car-evaluation / seasonal-maintenance / ev-specific-guide / claims-practical-guide) were written by AtomCode based on its built-in automotive knowledge, each 300–450 lines, covering emergency grading, decision trees, practical scripts, price anchors, and claim processes
- Of the **10 brand documents**, 8 were written simultaneously by AtomCode's parallel worker subagents (Toyota/Honda/VW/Mercedes/GM/Nissan/BYD/neo-EV); BMW and Ford were written by the main agent after a worker path-resolution issue
- The **SKILL.md v0.2 upgrade** added a "reference routing table" defining scene-to-document mapping, and established that brand documents take precedence over the generic maintenance-intervals for queries

In the v0.1 optimization round, AtomCode also fixed 4 documentation issues:
1. Removed redundant frontmatter from two reference files (duplicate `name`, unnecessary `file_path`)
2. Fixed hardcoded wrong push-command path in README.md to the actual path
3. Removed the meaningless `platforms` field for a pure-document skill in SKILL.md
4. Changed "harsh-condition discount factor / multiply by 0.6–0.7" to the clearer "harsh-condition shortening factor / shorten to 60%–70% of original"; unified units to km in maintenance-intervals.md

### Quality Boundaries

- Does not replace professional on-site technician diagnosis—the fault diagnosis module gives grading and slow-drive-to-shop advice, not final claims adjudication
- Does not provide legal opinions—the claims handbook gives practical scripts and processes, not lawyer advice
- Does not do new-car comparison or modification recommendations
- Fuel prices, insurance premiums, and parts prices fluctuate by time and region; all numbers are marked "subject to current local rates"
- The brand common-fault quick reference only includes publicly available high-frequency faults; it cannot be used to assert all cars of the same model have the issue—verify with VIN-based TSB queries

### Applicable Scenarios

- User asks "what service does my car need now" or "when is the next service"
- User provides car model + mileage + last service info, requesting a maintenance plan
- User wants to compare prices across service channels (4S/chain/independent shops)
- User wants to optimize insurance (third-party limits/add-on coverage)
- User just bought a car or transferred ownership, needs a full maintenance roadmap
- User reports noise/warning lights/odor/vibration, wants preliminary judgment
- User wants to estimate monthly/yearly full ownership cost (including hidden depreciation)
- User is considering a used car, needs VIN query/odometer rollback detection/accident sign judgment/price anchors
- User wants seasonal preventive maintenance (pre-winter coolant, summer self-ign prevention)
- User drives an EV, needs battery warranty terms/SOH/charger/degradation claim info
- User just had an accident, needs scene handling scripts/valuation bargaining/subrogation/rejection appeal/private settlement threshold
