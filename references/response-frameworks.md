# Response Frameworks Reference

This file contains the canonical answer frameworks for different question types encountered in interviews. Select the appropriate framework based on question type, then adapt to the candidate's actual content.

---

## General Narrative Frameworks

### STAR (Behavioral / Experience Questions)
Best for: "Tell me about a time when...", "Describe a challenge you faced..."

```
S — Situation: Set the context briefly (company, team, constraint)
T — Task: What was your specific responsibility or goal?
A — Action: What steps did YOU take? (focus on individual contribution)
R — Result: What was the measurable outcome? What did you learn?
```

**Pitfall to avoid**: Spending too long on S and T, leaving no time for A and R. The interviewer cares most about A.

---

### FAR (Decision / Judgment Questions)
Best for: "Why did you choose X over Y?", "How did you decide to...?"

```
F — Frame: What was the decision context and the constraints?
A — Analyze: What options did you consider, and what criteria did you use?
R — Reflect: What happened, and what would you do differently with hindsight?
```

---

### Three-Layer Depth (Strategic / Reflective Questions)
Best for: "What did you learn from this project?", "How do you evaluate success?"

```
Layer 1 — 表象 (What): What happened at the surface level?
Layer 2 — 判断 (Why): What reasoning or principle drove the outcome?
Layer 3 — 反思 (Learned): What would you revise or carry forward?
```

---

## Numeric Question Frameworks (5 Categories)

**Core principle**: Open with the action logic or definition that produced the number. Never open with "admitting limitations" — that is a defensive posture that signals weakness before being challenged.

The sequence is always:
> **Establish credibility first → Show self-awareness second**

---

### ① Sample Size Questions
*Triggered by*: "Why only N users/cases/examples?"

**Framework**:
1. **Selection logic**: How were these N chosen to maximize coverage? (segmentation, diversity criteria, saturation point)
2. **MVP constraint**: What time/resource limit made this the right tradeoff at this stage?
3. **Next step**: How would you expand if given more resources?

**Role-specific credibility anchors**:
- PM: Theoretical saturation (patterns stopped emerging after ~N interviews) + deliberate segment selection
- QA: Equivalence class coverage (N cases cover M distinct behaviors) + risk-based prioritization
- Sales: Territory scope definition (these N accounts represent the addressable segment for this period)

---

### ② Accuracy / Hit-Rate Questions
*Triggered by*: "How did you measure that? Is that rigorous enough?"

**Framework**:
1. **Definition**: State exactly what "success" means — the operational judgment criteria (who evaluated, by what standard)
2. **Benchmark design**: Why is the evaluation set representative? How was it constructed to avoid bias?
3. **Limitation awareness**: Which scenarios may not be covered? What would cause the metric to fail?
4. **Improvement direction**: What would make the measurement more rigorous next?

**Role-specific credibility anchors**:
- PM: Anti-overfitting measures (held-out test set, blind evaluation, diverse difficulty levels)
- QA: False positive / false negative tradeoff rationale (missing a bug vs. blocking unnecessarily)
- Sales: External factor acknowledgment (win rate adjusted for market conditions, deal size, competitive context)

---

### ③ Performance / Speed Questions
*Triggered by*: "Can users/the business actually accept this?"

**Framework**:
1. **Usage context**: In what scenario does this number occur? (async task vs. real-time interaction changes the acceptability threshold)
2. **Product/process layer**: What UX or workflow design mitigates the impact on perceived experience?
3. **Optimization roadmap**: Which step is the bottleneck? What is the known improvement path?

**Role-specific credibility anchors**:
- PM: Streaming / progress feedback design + comparison to user mental model of task duration
- QA: Parallelization strategy + selective test execution (smoke vs. full regression)
- Sales: Pipeline acceleration tactics + where in the cycle the delay occurs and why it's acceptable there

---

### ④ Business Metric Questions
*Triggered by*: "What's the denominator? How is this defined?"

**Framework**:
1. **Precise definition**: State the exact numerator and denominator with no ambiguity
2. **Collection method**: How was the data captured? What is the time window?
3. **Interpretation**: What does this number mean in context? What would a "good" benchmark look like?

**Role-specific credibility anchors**:
- PM: Cohort definition + action definition for adoption events (copy vs. export vs. citation confirmed)
- QA: Escaped defect classification (severity threshold for what counts as "escaped")
- Sales: Quota definition (total bookings vs. new ARR vs. expansion), territory normalization

---

### ⑤ Timeline Questions
*Triggered by*: "That's fast — what got sacrificed? What's the quality like?"

**Framework**:
1. **Scope boundary**: State explicitly what was in scope and what was deliberately deferred
2. **Current quality state**: Be honest about known gaps, debt, or risks
3. **Payoff plan**: How will the deferred items be addressed?

**Role-specific credibility anchors**:
- PM: Features cut from MVP scope + current technical debt inventory + post-launch roadmap
- QA: Test coverage gaps known at launch + monitoring/hotfix plan to catch what was missed
- Sales: Relationship depth vs. breadth tradeoff in compressed timeline + follow-up plan

---

## Decision Question Framework

*Triggered by*: "Why did you choose X?", "What alternatives did you consider?"

```
1. Decision context    — What constraints shaped the option space? (time, cost, team skill, existing infra)
2. Alternatives considered — What were the 2-3 realistic options? (be specific, not strawmen)
3. Selection rationale — What criteria drove the choice? (weight the factors explicitly)
4. Acknowledged tradeoff — What did you give up by choosing this? (shows intellectual honesty)
5. Retrospective evaluation — With hindsight, was it the right call? Would you change it?
```

**Key**: Step 5 is where strong candidates differentiate themselves. Being willing to say "I'd do X differently now because..." signals growth mindset and depth of reflection.

---

## Methodology Question Framework

*Triggered by*: "How did you design your evaluation system?", "Walk me through your process for..."

```
1. Goal definition   — What were you trying to measure or achieve?
2. Design choices    — What specific design decisions did you make and why?
3. Safeguards        — What did you do to ensure reliability / avoid bias?
4. Limitations       — Where does this methodology fall short?
5. Evolution         — How has or would this methodology improve with more resources?
```
