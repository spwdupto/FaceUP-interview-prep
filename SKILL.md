---
name: FaceUP-interview-prep
description: Helps job candidates prepare for interviews by generating likely interview questions from three interviewer perspectives (business/technical, HR, and senior management), creating structured response frameworks, and drafting model answers tailored to the candidate's actual experience and role type. Use this skill whenever the user wants to prepare for a job interview, practice answering questions, generate a Q&A preparation sheet, simulate a mock interview, or tailor experience to a specific company and role. Effective across PM, QA/testing, sales, engineering, research, and other technology roles.
---

# FaceUP Interview Prep

A role-adaptive skill for generating comprehensive interview preparation materials: high-risk resume detail analysis, role-matched interview questions, response frameworks, and tailored model answers.

## When to Trigger

Use this skill when the user provides any of:
- A resume, project description, or summary of experience
- A target job title and/or company
- A request to "prepare for an interview" or "generate interview questions"

---

## Workflow

### Step 1: Collect Context

Ask the user to provide:
1. **Candidate background**: Resume, key projects, or a brief summary. Extract:
   - All quantitative claims (numbers, percentages, timelines, rates)
   - Key decisions made and the options considered
   - Methods, frameworks, and evaluation systems used
   - Outcomes and business impact
2. **Target role**: Job title, company name, and job description if available
3. **Role type**: Classify into one of: `PM` / `QA` / `Sales` / `Engineering` / `Research` / `Other`
4. **Company materials** (optional): Brand manuals, JD, website content for company-specific tailoring

### Step 2: Identify High-Risk Resume Details

Before generating questions, surface the specific resume claims most likely to be probed. Organize into three categories:

**数字类 (Quantitative claims)** — numbers are always challenged:
- Sample sizes, dataset sizes, user counts → representativeness and selection method
- Accuracy/hit-rate metrics → measurement methodology, evaluation set design
- Performance metrics (latency, throughput, SLA) → user/business acceptability
- Business metrics (conversion, retention, quota attainment) → denominator definition, window
- Timeline claims ("shipped in N days") → scope, quality state, tech debt

**决策类 (Decision points)** — PM/professional judgment under scrutiny:
- Architecture, tool, or method choices → what alternatives were considered and why rejected
- Scope decisions → what was cut and why, what was kept and why
- Evaluation method choices → why this metric/framework over alternatives

**方法论类 (Methodology)** — process rigor:
- How research/testing/analysis was conducted
- How results were measured and validated
- How iterations were tracked and improvements attributed

### Step 3: Load Role-Specific Patterns

Read `references/role-patterns.md` and load the section matching the candidate's role type from Step 1.

Use the role-specific high-frequency questions as the foundation for Step 4 — adapt them to the candidate's actual resume details rather than using them verbatim.

### Step 4: Generate Questions from Three Interviewer Perspectives

Read `references/interviewer-personas.md` for each type's focus areas. Generate questions organized by sub-theme within each section.

For each question, note the **interviewer's intent** — what underlying judgment or capability they are testing.

**三类面试官视角**:
- **业务/技术面试官**: Deepest scrutiny of quantitative claims, product/technical decisions, methodology rigor
- **HR 面试官**: Motivation, growth mindset, collaboration under constraint, career direction
- **公司高层**: Commercial viability, competitive differentiation, scaling risks, resource allocation

### Step 5: Generate Response Framework + Model Answer for Each Question

Read `references/response-frameworks.md` and select the appropriate framework based on question type:
- Quantitative claim questions → use the relevant 5-category numeric framework
- Decision questions → use the Decision template
- Experience/behavioral questions → use STAR or Three-Layer Depth
- Commercial/strategic questions → use FAR

For each question, produce two outputs:

**回答框架 (Response Framework)**:
A role-neutral bullet scaffold showing the logical structure. Should be usable as a template by any candidate regardless of specific project.

**结构化回答 (Structured Model Answer)**:
A concrete answer drawing on the candidate's actual data and details. Must:
- Reference specific numbers and details from the resume exactly as stated
- Show honest self-awareness about limitations (do NOT oversell)
- Demonstrate professional judgment (tradeoffs, iterations, lessons learned)
- Be defensible under follow-up questioning

### Step 6: Company-Specific Customization (if company materials provided)

1. Extract key company metrics, products, values, and strategic challenges from the materials
2. Identify where the candidate's experience maps directly to company needs
3. Generate additional questions testing fit with the company's specific context
4. Tailor model answers to reference company-specific data points

---

## Output Format

```
## 简历高风险细节清单

### 数字类
- [Claim] → [Why it will be probed]

### 决策类
- [Decision] → [Likely challenge]

### 方法论类
- [Method] → [Likely challenge]

---

## 一、业务面试官 / [Role] at [Company if known]

### [Sub-theme (e.g., 用户研究, Pipeline设计, 评测体系)]

**Q1.** [Question text]
> 考察意图：[What the interviewer is really testing]

**回答框架**
- [Bullet 1]
- [Bullet 2]
- ...

**结构化回答**
[Concrete answer with specific data from candidate's resume]

[Repeat for all questions in this section]

---

## 二、HR 面试官

[Same format]

---

## 三、公司高层

[Same format]

---

## 附：主动提问建议

1. [Question candidate can ask interviewer]
2. ...
```

---

## Quality Checks

Before finalizing output, verify:
- All numbers in model answers exactly match what the candidate provided (no rounding, no inflation)
- Model answers acknowledge limitations honestly — interviewers respect self-awareness, not perfection
- Each question has a distinct focus — no two questions should test the same underlying judgment
- Company-specific questions reference actual data from provided materials, not generic assumptions
- Numeric question answers open with action logic or definition, NOT with "承认局限/admitting limitations"
