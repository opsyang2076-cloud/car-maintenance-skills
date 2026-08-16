# 汽车维保顾问 Skill

## 📋 项目信息

- **Skill 名称**: car-maintenance-advisor
- **版本**: 0.1.0
- **作者**: Hermes Agent
- **许可证**: MIT
- **语言**: 中文

## 🎯 功能

面向中国车主的一站式维修保养 + 保险推荐工具。输入行驶里程、车辆品牌型号、上次保养日期/里程后，基于各品牌官方操作手册规范与汽修行业共识，输出下一次保养项目及各大服务商的综合比价。

### 支持功能

1. **保养计划生成**
   - 根据里程和日期预测下次保养时间
   - 提供详细的保养项目清单
   - 基于车型手册的个性化建议

2. **价格比价**
   - 4S 店报价
   - 连锁修理厂价格
   - 路边店价格对比

3. **保险推荐**
   - 车险方案优化
   - 三者额度建议
   - 附加险选择指导

4. **用车建议**
   - 不同用车场景建议
   - 恶劣环境保养提醒
   - 里程规划

## 📁 项目结构

```
car-maintenance-advisor/
├── SKILL.md              # Skill 主文档
├── README.md             # 项目介绍
├── PUSH_GUIDE.md         # GitHub 推送指南
├── PUSH_STATUS.md        # 推送状态
└── references/
    ├── car-insurance-guide.md   # 保险指南
    └── maintenance-intervals.md # 保养周期表
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
