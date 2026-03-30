# AI 营销技能

**面向营销和销售团队的开源 Claude Code 技能。** 由 [Single Brain](https://singlebrain.com/?utm_source=github&utm_medium=skill_repo&utm_campaign=ai_marketing_skills) 团队打造 — 已在真实管道中实战验证，产生数百万美元收入。

这些不是简单的提示词，而是完整的**工作流** — 脚本、评分算法、专家小组和自动化管道，您可以直接插入 Claude Code（或任何 AI 编码代理）并立即运行。

---

## 🗂️ 技能列表

| 类别 | 功能 | 关键技能 |
|------|------|----------|
| [**增长引擎**](./growth-engine/) | 自主运行、测量和优化的营销实验 | 实验引擎、节奏警报、周度记分卡 |
| [**销售管道**](./sales-pipeline/) | 将匿名网站访客转化为合格销售管道 | RB2B 路由器、交易复活器、触发器探测器、ICP 学习器 |
| [**内容运营**](./content-ops/) | 每次发布内容得分均达 90+ | 专家小组、质量关卡、编辑大脑、引言挖掘器 |
| [**外呼引擎**](./outbound-engine/) | 从 ICP 定义到邮件自动进入收件箱 — 全自动化 | 冷启动外呼优化器、线索管道、竞品监控器 |
| [**SEO 运营**](./seo-ops/) | 发现竞争对手忽略的关键词 | 内容攻击简报、GSC 优化器、趋势侦察器 |
| [**财务运营**](./finance-ops/) | 您的 AI CFO，30 分钟内找出隐藏成本 | CFO 简报、成本估算、场景建模器 |

---

## 🚀 快速开始

每个技能类别都有独立的 README 文件，内含设置说明。通用流程如下：

```bash
# 1. 克隆仓库
git clone https://github.com/singlegrain/ai-marketing-skills.git
cd ai-marketing-skills

# 2. 进入对应类别
cd growth-engine   # 或 sales-pipeline、content-ops 等

# 3. 安装依赖
pip install -r requirements.txt

# 4. 配置环境变量
cp .env.example .env
# 在 .env 中填入您的 API Key

# 5. 运行
python experiment-engine.py create \
  --hypothesis "线程帖比单帖获得 2 倍互动" \
  --variable format \
  --variants '["thread", "single"]' \
  --metric impressions
```

---

## 🧠 如何与 Claude Code 配合使用

每个类别都包含一个 `SKILL.md` 文件。将它复制到您的 Claude Code 项目中，AI 代理就会知道如何使用这些工具：

```
# 在您的项目目录中
cp ai-marketing-skills/growth-engine/SKILL.md .claude/skills/growth-engine.md
```

然后对 Claude Code 说：  
*"在 LinkedIn 上运行一个测试：对比轮播帖 vs 静态帖的效果"* — 剩下的全部由它自动处理。

---

## 📊 这些技能的独特之处

**这些不是玩具演示。** 每个技能都为真实业务运营而设计：

- **增长引擎** 使用自举置信区间和 Mann-Whitney U 检验 — 真正的统计学，而非凭感觉
- **交易复活器** 拥有三层智能，包括“跟随冠军”机制 — 追踪已离职联系人跳槽后的新公司
- **ICP 学习器** 根据实际赢单/输单数据自动重写理想客户画像 — 您的定位会持续自我优化
- **专家小组** 使用领域特定专家角色递归评分，直到内容质量达到 90+
- **RB2B 路由器** 在路由到外呼序列前，会进行意图评分、高管层级去重以及代理机构分类

---

## 📁 仓库结构

```
ai-marketing-skills/
├── README.md ← 您正在阅读的文件
├── growth-engine/ ← 自主实验系统
│   ├── SKILL.md
│   ├── experiment-engine.py
│   ├── pacing-alert.py
│   ├── autogrowth-weekly-scorecard.py
│   └── ...
├── sales-pipeline/ ← 访客 → 销售管道自动化
│   ├── SKILL.md
│   ├── rb2b_instantly_router.py
│   ├── deal_resurrector.py
│   ├── trigger_prospector.py
│   ├── icp_learning_analyzer.py
│   └── ...
├── content-ops/ ← 质量评分与内容生产
│   ├── SKILL.md
│   ├── scripts/
│   ├── experts/ ← 9 个专家小组定义
│   ├── scoring-rubrics/ ← 5 个评分标准模板
│   └── ...
├── outbound-engine/ ← 冷启动外呼自动化
│   ├── SKILL.md
│   ├── scripts/
│   ├── references/ ← ICP 模板、文案规则
│   └── ...
├── seo-ops/ ← SEO 智能分析
│   ├── SKILL.md
│   ├── content_attack_brief.py
│   ├── gsc_client.py
│   ├── trend_scout.py
│   └── ...
└── finance-ops/ ← 财务分析
    ├── SKILL.md
    ├── scripts/
    ├── references/ ← 指标、费率、ROI 模型
    └── ...
```

---

## 🤝 贡献

发现 Bug？有改进建议？欢迎提交 PR！

1. Fork 本仓库  
2. 创建特性分支 (`git checkout -b feature/better-scoring`)  
3. 提交更改  
4. 推送分支  
5. 提交 Pull Request

---

## 📄 许可协议

MIT License。您可以随意使用这些技能。

---

*如果您觉得有用，请给仓库点个 Star，帮助更多人发现这些工具。*

---

<div align="center">
**🧠 [想让我们帮您构建并管理这些工具？→](https://singlebrain.com/?utm_source=github&utm_medium=skill_repo&utm_campaign=ai_marketing_skills)**  
*这就是我们在 [Single Brain](https://singlebrain.com/?utm_source=github&utm_medium=skill_repo&utm_campaign=ai_marketing_skills) 为客户构建 AI 代理的方式。*

[Single Grain](https://www.singlegrain.com/?utm_source=github&utm_medium=skill_repo&utm_campaign=ai_marketing_skills) · 我们的营销代理机构  
📬 **[与 14,000+ 营销人员和创始人一起提升营销能力 →](https://levelingup.beehiiv.com/subscribe)** *(免费)*
</div>
