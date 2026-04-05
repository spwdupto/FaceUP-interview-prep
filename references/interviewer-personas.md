# Interviewer Personas Reference

Three universal interviewer types appear across most structured interview processes. Each has a distinct focus and probing style. Generate questions from each perspective independently — they should not overlap.

---

## 一、业务/技术面试官 (Business / Technical Interviewer)

**Typical profile**: Direct manager, senior IC, or domain expert. Has deep knowledge of the role's craft. Will probe the rigor behind any claim.

**Core focus**: Is this candidate's judgment sound? Do they know what they don't know?

### What they probe

**Numbers**
- Are quantitative claims actually meaningful, or are they inflated vanity metrics?
- Is the measurement methodology defensible (sample size, evaluation design, ground truth)?
- Are performance numbers acceptable given the use case, or glossed over?

**Decisions**
- What alternatives were considered before this choice was made?
- What was given up by choosing this approach?
- Were the tradeoffs consciously made or accidentally discovered?

**Methodology**
- Is the process designed with rigor, or assembled ad hoc?
- How are edge cases handled?
- What would cause this approach to fail, and does the candidate know it?

### Role-specific variants

| Role | What this interviewer cares most about |
|------|----------------------------------------|
| AI PM | Evaluation system design, pipeline decisions, preventing metric gaming |
| QA | Test strategy completeness, automation decision criteria, shift-left practices |
| Sales | Customer qualification methodology, competitive handling, deal strategy depth |
| Engineering | Architecture tradeoffs, failure mode awareness, system design rigor |
| Research | Experimental design, baseline selection, generalization claims |

### Probing style
Asks follow-up "why" questions. Will challenge numbers with: "Is that statistically meaningful?", "What's the confidence interval?", "Could you have just done X instead?"

---

## 二、HR 面试官 (HR / Recruiter Interviewer)

**Typical profile**: HR BP, talent partner, or recruiter. Less domain expertise, more focused on culture fit, growth potential, and soft skills.

**Core focus**: Will this person thrive here? Can they collaborate and grow?

### What they probe

**Motivation and authenticity**
- Why this role, this company, this timing?
- Is the candidate's interest genuine or generic?
- Do their personal experiences connect meaningfully to the work?

**Resilience and problem-solving under constraint**
- What was the hardest challenge, and how was it overcome?
- How did they prioritize when everything felt urgent?
- What did they give up to succeed on the key thing?

**Collaboration and influence**
- How do they work with people who disagree?
- How do they bring along non-technical stakeholders?
- Can they influence without authority?

**Career direction clarity**
- Where are they going? Does this role fit the trajectory?
- What distinguishes them from other candidates with similar backgrounds?
- What does "growth" mean to them in the next 2-3 years?

### Role-specific variants

| Role | Specific HR angle |
|------|-------------------|
| AI PM | Why PM not engineering/research? How do you handle ambiguity without code? |
| QA | How do you maintain quality advocacy when under release pressure? |
| Sales | How do you handle rejection? What's your longest losing streak and recovery? |
| Engineering | How do you balance shipping fast vs. doing it right? |
| Research | How do you stay motivated when experiments fail for months? |

### Probing style
Asks open-ended behavioral questions. Listens for specificity — vague answers get follow-up: "Can you give me a concrete example?", "What specifically did you do?"

---

## 三、公司高层 (Senior Leadership / Hiring Executive)

**Typical profile**: VP, Director, or C-suite. Evaluates strategic fit, ambition, and whether the candidate can grow into broader scope.

**Core focus**: Can this person create real business value and scale with the company?

### What they probe

**Commercial judgment**
- Does the candidate understand how their work connects to revenue, retention, or competitive advantage?
- Can they quantify the value they've created, not just describe the work?
- Do they understand who the customer is and what makes them pay / stay?

**Strategic thinking**
- Can the candidate identify what's truly differentiated vs. what's table stakes?
- Do they understand the competitive landscape and where threats come from?
- How do they think about making bets under uncertainty?

**Scaling instinct**
- What breaks if this grows 10x? Does the candidate see it?
- What technical, organizational, or market risks exist that haven't been addressed?
- How would they allocate limited resources to maximize impact?

**Execution credibility**
- Is this person a force multiplier or a solo contributor?
- How do they think about building vs. buying vs. partnering?
- What's their roadmap philosophy — incremental or moonshot?

### Role-specific variants

| Role | Specific leadership angle |
|------|--------------------------|
| AI PM | PMF hypothesis, defensible moat vs. API wrapper risk, build vs. integrate decision |
| QA | How does quality function scale without linear headcount growth? |
| Sales | What's the market expansion theory? What's the ceiling on current approach? |
| Engineering | Platform thinking vs. feature factory, technical debt as business risk |
| Research | Path from research to product impact, publication vs. application tradeoff |

### Probing style
Asks big, open questions: "If you had 3 engineers and 6 months, what would you build?", "What would it take for this to be a $10M product?" Listens for clarity of mental model, not just domain knowledge.
