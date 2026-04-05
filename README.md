# FaceUP-interview-prep

**A role-adaptive Claude Code skill for comprehensive interview preparation.**

中文 | [English](#english)

---

## 中文说明

### 这是什么

`FaceUP-interview-prep` 是一个 [Claude Code](https://claude.ai/code) Skill，帮助求职者系统准备面试。

输入你的简历/项目经历和目标岗位，自动生成：

- **简历高风险细节清单** — 识别面试官最可能深挖的数字、决策、方法论
- **三类面试官视角问题** — 业务/技术面试官、HR 面试官、公司高层
- **每题回答框架** — 可复用的逻辑骨架模板
- **结构化参考回答** — 基于你真实经历的具体回答

### 支持岗位类型

| 岗位族群 | 示例 |
|---------|------|
| AI PM / 产品经理 | AI 产品、B/C 端 PM、增长 PM |
| QA / 测试工程师 | 功能测试、自动化测试、性能测试 |
| 销售 / 商务拓展 | To B 销售、BD、客户成功 |
| 研究 / 算法工程师 | NLP、CV、推荐系统 |
| 工程 / 后端开发 | 后端、全栈、基础设施 |

### 安装方法

1. 克隆本仓库或下载 zip
2. 将 `FaceUP-interview-prep/` 文件夹放入你的 Claude Code skills 目录：
   ```
   # macOS / Linux
   ~/.claude/skills/FaceUP-interview-prep/

   # Windows
   C:\Users\<用户名>\.claude\skills\FaceUP-interview-prep\
   ```
3. 重启 Claude Code

### 使用方法

在 Claude Code 中直接输入，例如：

```
帮我准备字节跳动 AI PM 岗位的面试，我的项目经历是：[粘贴简历片段]
```

```
我要面试路觅教育的 AI 师资产品经理（实习生），公司品牌手册已上传，请帮我准备面试问题和回答
```

```
帮我为 QA 工程师岗位面试准备问题，简历如下：[简历内容]
```

### 文件结构

```
FaceUP-interview-prep/
├── SKILL.md                        # Skill 核心文件（触发条件 + 工作流）
└── references/
    ├── response-frameworks.md      # 5类数字问题框架 + 决策/叙事框架
    ├── interviewer-personas.md     # 三类面试官关注点详解
    └── role-patterns.md            # 5个岗位族群 × 3类问题的高频题库
```

### 设计理念

**数字类问题回答不从"承认局限"开场** — 先建立数字背后的决策可信度，再展示自我反思意识。

五类数字问题各有专属框架：样本量类、精度/命中率类、性能/速度类、业务指标类、时间线类。

---

<a name="english"></a>
## English

### What is this

`FaceUP-interview-prep` is a [Claude Code](https://claude.ai/code) Skill for systematic interview preparation.

Provide your resume / project experience and target role, and it generates:

- **High-risk resume detail checklist** — surfaces the specific numbers, decisions, and methodology claims interviewers will probe
- **Questions from three interviewer perspectives** — business/technical, HR, and senior leadership
- **Response framework for each question** — a reusable logical scaffold
- **Structured model answer** — concrete answers grounded in your actual experience

### Supported Role Types

PM · QA/Testing · Sales/BD · Research/ML · Backend Engineering

### Installation

1. Clone this repo or download the zip
2. Place the `FaceUP-interview-prep/` folder in your Claude Code skills directory:
   ```
   # macOS / Linux
   ~/.claude/skills/FaceUP-interview-prep/

   # Windows
   C:\Users\<username>\.claude\skills\FaceUP-interview-prep\
   ```
3. Restart Claude Code

### Usage

Just describe your interview prep need in Claude Code:

```
Help me prepare for a PM interview at [company]. My project experience: [resume snippet]
```

### Key Design Principle

Numeric question answers open with **action logic and definitions**, never with "admitting limitations." Five numeric sub-types each have a dedicated framework: sample size, accuracy/hit-rate, performance/speed, business metrics, and timeline.

---

## License

MIT © 2026 [spwdupto](https://github.com/spwdupto)
