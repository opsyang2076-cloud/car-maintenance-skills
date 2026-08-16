# 汽车维保顾问 Skill

## 📋 项目信息

- **Skill 名称**: car-maintenance-advisor
- **版本**: 0.2.0
- **作者**: Hermes Agent
- **许可证**: MIT
- **语言**: 中文

## 🎯 功能

面向中国车主的一站式维修保养 + 保险 + 故障诊断 + 二手车评估 + 季节性养护 + 新能源专属 + 出险理赔实战工具。覆盖从日常保养到事故处置的全生命周期，按场景加载对应参考文档。

### 支持功能

1. **保养计划生成**
   - 根据里程和日期预测下次保养时间
   - 提供详细的保养项目清单
   - 基于车型手册的个性化建议（含 10+ 品牌分项文档）

2. **价格比价**
   - 4S 店报价
   - 连锁修理厂价格
   - 路边店价格对比

3. **保险推荐**
   - 车险方案优化
   - 三者额度建议
   - 附加险选择指导

4. **故障诊断（v0.2 新增）**
   - 仪表盘警示灯分级速查
   - 异响/渗油/异味/抖动分类诊断流程
   - 缓行就医决策树与品牌通病速查

5. **养车成本估算（v0.2 新增）**
   - 月度/年度全成本（固定+变动+隐性）
   - 油车/混动/纯电能源成本对比
   - 节流策略与同档位对比

6. **二手车评估（v0.2 新增）**
   - VIN 查询与车源筛选四步法
   - 调表识别五大法与重大事故痕迹判断
   - 关键部件剩余寿命估算与价格锚点

7. **季节性保养（v0.2 新增）**
   - 春夏秋冬预防性清单与节前必检
   - 8 大地区气候分区适配
   - 新能源车季节特别提示

8. **新能源专属（v0.2 新增）**
   - BEV/PHEV/EREV/HEV 分类保养矩阵
   - 三电质保条款细则与衰减索赔实战
   - 家用桩安装与公共桩使用技巧

9. **出险理赔实战（v0.2 新增）**
   - 事故第一分钟决策树与现场六步法
   - 私了 vs 走保险临界值速查
   - 定损博弈、代位追偿与拒赔应对

10. **用车建议**
    - 不同用车场景建议
    - 恶劣环境保养提醒
    - 里程规划

## 📁 项目结构

```
car-maintenance-skills/
├── SKILL.md                          # Skill 主文档（主流程 + 参考资料路由）
├── README.md                         # 项目介绍
├── LICENSE                           # MIT 许可证
├── PUSH_GUIDE.md                     # GitHub 推送指南
├── PUSH_STATUS.md                    # 推送状态
└── references/
    ├── car-insurance-guide.md        # 车险购买与推荐指南
    ├── maintenance-intervals.md      # 各品牌保养周期速查表
    ├── fault-diagnosis.md            # 故障初步诊断指南（v0.2）
    ├── ownership-cost.md             # 养车成本计算器（v0.2）
    ├── used-car-evaluation.md        # 二手车评估与选购指南（v0.2）
    ├── seasonal-maintenance.md       # 季节性保养日历（v0.2）
    ├── ev-specific-guide.md          # 新能源车专项指南（v0.2）
    ├── claims-practical-guide.md     # 出险理赔实战手册（v0.2）
    └保养规格/油液规格/通病/4S推推销/三电质保
        ├── toyota.md
        ├── honda.md
        ├── volkswagen.md
        ├── mercedes-benz.md
        ├── bmw.md
        ├── ford.md
        ├── gm.md
        ├── nissan.md
        ├── byd.md
        └档理想/蔚来/小鹏/零跑等新势力
```

## 🚀 使用方法

### 输入信息

需要用户提供：
- 车辆品牌 & 型号
- 当前总里程
- 上次保养日期
- 上次保养里程
- 用车性质（可选）
- 所在城市（可选）

### 输出内容

1. 下次保养建议
2. 各项目价格对比
3. 保险方案推荐
4. 用车注意事项

## 🔧 GitHub 推送

### 推送命令

```bash
cd "D:/软件/Hermes/skills/car-maintenance-skills"

# 拉取并合并
git pull origin main --allow-unrelated-histories --no-rebase

# 推送
git push -u origin main
```

### 认证信息

- **Username**: `opsyang2076-cloud`
- **Password**: GitHub 个人访问令牌

## 📄 许可证

MIT License

## 🤝 贡献

欢迎贡献！请提交 PR。
