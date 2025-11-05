# Deep Iterative Thinking

> **Author**: wanpeng.xie@gmail.com

When users request "deep iterative thinking", "exploratory iteration", or "non-linear iterative thinking", you must strictly follow the process below.

---

## Step Zero: Understand the Problem (MANDATORY)

Before starting any thinking, you must:

### 1. Understand the Problem Itself
- What exactly is the user asking?
- What is the real intent behind the question?
- What implicit assumptions exist?

### 2. Understand the Problem's Context
- In what context does this problem exist?
- What existing designs and decisions are involved?
- What other parts are related?
- Interactions with other objects/problems

### 3. Understand the Higher Dimensions
- What is the essential problem behind this problem?
- Is there a more abstract perspective?
- Is there a simpler problem statement?


**If the problem understanding is unclear, you MUST use the AskUserQuestion tool to clarify before proceeding.**

> Note: Truly profound insights don't solve problems—they change how we think about them.
---

## Step One: Establish Exploratory TODOs (MANDATORY)

Use the `TodoWrite` tool to establish a TODO list, which must include:

### Minimum Requirement: At least 5 TODO items

### TODO Type Distribution:
1. **Confusion Type** (at least 1): Record current confusion points
   - Example: "Confusion: What exactly does XX mean?"

2. **Exploration Type** (at least 2): Explore from different angles
   - Example: "Exploration A: Understanding from YY perspective"
   - Example: "Exploration B: Comparing from ZZ angle"

3. **Validation Type** (at least 1): Validate with counterexamples or cases
   - Example: "Counterexample validation: What if we don't do XX?"
   - Example: "Case validation: Test with specific scenarios"

4. **Dynamic Type** (optional): Add dynamically based on discoveries

### Prohibited TODO Patterns:
- ❌ Linear steps: "Step 1... Step 2... Step 3..."
- ❌ Preset answers: "Validate feasibility of XX solution" (already assuming XX)
- ❌ Pure technical execution: "Implement XX feature"

### Correct TODO Examples:
```
- Confusion: What exactly is the balance point between "interruption" and "value"?
- Exploration A: Understanding notification necessity from user scenarios
- Exploration B: Understanding classification logic from product goals
- Counterexample validation: What happens if we don't classify? How would users react?
- Deep inquiry: Why does the notification system need to be designed this way?
```

---

## Step Two: Execute Real Iteration (MANDATORY)

### Core Principle: Real thinking, not performance thinking

### Execution Rules:

#### 1. Execute TODOs One by One
- When starting a TODO, immediately mark it as `in_progress` with `TodoWrite`
- When completing a TODO, immediately mark it as `completed` with `TodoWrite`
- **Prohibited** to complete multiple TODOs before batch updating

#### 2. Show Real Thinking Process
```markdown
## Exploration A: From XX Perspective

Attempt 1: ...
Discovered problem: ...
Attempt 2: ...
New confusion: ...

Wait, this understanding is wrong!
Because...
Need to rethink...
```

#### 3. Allow and Encourage Overthrowing
- When discovering misunderstanding, immediately admit and overthrow
- Don't defend wrong directions
- Add new TODOs to record directions that need re-exploration

#### 4. Continuously Ask for Essence (Integrating Discussion Principles)
- Don't stay on the surface
- Ask "why" for each discovery
- Seek more abstract, more essential understanding
- Validate abstract understanding with concrete cases

#### 5. Multi-angle Validation
- **Typical cases**: Validate with normal situations
- **Counterexamples**: Validate with extreme situations
- **Abnormal examples**: Validate with boundary situations
- Verify thinking completeness

#### 6. Dynamically Adjust TODOs
- Discover new problems → Immediately add new TODOs
- Discover TODO is meaningless → Delete and explain reason
- Discover need to step back → Modify TODO status

### Minimum Iteration Rounds: 3 rounds

Even if the problem seems simple, at least 3 rounds of exploration are required:
1. Round 1: Initial understanding
2. Round 2: Deepen/challenge the first round's understanding
3. Round 3: Comprehensive validation

---

## Step Three: Case Validation (MANDATORY)

After reaching preliminary conclusions, you must validate with complete case scenarios:

### Validation Requirements:
1. **Construct complete scenarios**: Not simple examples, but complete usage scenarios
2. **Simulate actual usage**: Assume how real users would use it in practice
3. **Check effectiveness**: Can it support actual needs?
4. **Find loopholes**: Try to find problems in the solution

### If Validation Fails:
- Don't patch, step back and rethink
- Add new TODOs to record problems
- May need to overthrow the entire direction

---

## Step Four: Summarize and Record (MANDATORY)

### Summary Must Include:

1. **Final Conclusion**
   - Clearly state the conclusion
   - Mark completeness (if not 100% complete)

2. **Key Insights**
   - What is the most important discovery?
   - Which understandings are crucial?

3. **Overthrown Assumptions**
   - Which ideas were proven wrong?
   - Why were they wrong?
   - What does this imply for the future?

4. **Key Turning Points in Iteration**
   - At which moments did important changes occur?
   - Why did they change?

5. **Unsolved Problems**
   - What problems remain unsolved?
   - What should be done next?

---

## Integrated Discussion Principles

### From Core Principles in CLAUDE.md:

#### 1. Dimensions of Thinking
- ✅ Always think about context and higher dimensions
- ✅ Deep thinking, not superficial
- ✅ Probe from both abstract essence and concrete cases
- ✅ Find common counterexamples to validate completeness
- ✅ Focus on essential problems, not technical details

#### 2. Avoid Premature Convergence
- ✅ Don't rush to give solutions
- ✅ Think, understand, and discuss thoroughly
- ✅ Don't become a slave to the first solution

#### 3. Design Philosophy
- ✅ Let LLM do what it's good at
- ✅ Don't over-structure
- ✅ Simple structure, complex processing

---

## Required Tools

### TodoWrite (Required)
- Establish TODO list
- Update status in real-time
- Dynamically add/delete TODOs

### AskUserQuestion (When Needed)
- When problem understanding is unclear
- When multiple viable directions are discovered and choice is needed
- When key decision points need confirmation

---

## Checklist

At the end of each stage, ask yourself:

### Problem Understanding Stage:
- [ ] Do I really understand what the user is asking?
- [ ] Do I understand the problem's environment and context?
- [ ] Have I found a more essential problem statement?

### Iteration Execution Stage:
- [ ] Am I really thinking or just performing?
- [ ] Do I allow myself to be confused?
- [ ] Do I dare to overthrow my own ideas?
- [ ] Have I done at least 3 rounds of iteration?
- [ ] Have I validated with typical cases, counterexamples, and abnormal examples?

### Validation Stage:
- [ ] Did I validate with complete scenarios?
- [ ] Is the validation really effective or just self-consolation?
- [ ] Did I try to find loopholes?

### Summary Stage:
- [ ] Did I record overthrown assumptions?
- [ ] Did I admit incomplete parts?
- [ ] Did I clarify the next steps?

---

## Common Error Warnings

### Error 1: Fake Iteration
**Manifestation**: Write "Round 1... Round 2... Round 3..." but actually wrote it all at once
**Identification**: All rounds progress linearly, no real stepping back or overthrowing
**Consequence**: Low thinking quality, unreliable conclusions

### Error 2: Premature Convergence
**Manifestation**: Quickly give "perfect" framework, looks very professional
**Identification**: No confusion, no contradictions, too "reasonable"
**Consequence**: May miss the real essence, design a monitoring system instead of life

### Error 3: Ignoring Context
**Manifestation**: Think about the problem in isolation, not considering context
**Identification**: No mention of related existing designs, no comparison with other modules
**Consequence**: Incoherent design, violates overall architecture

### Error 4: Staying on Surface
**Manifestation**: Only answer "what is", don't ask "why"
**Identification**: No deep essence, lack of abstract understanding
**Consequence**: Shallow understanding, cannot guide design

---

## Successful Case Reference

### Case: Notification System Classification Design

**Problem**: Our product needs to design a notification system. How should we classify and prioritize?

**Execution Process**:
1. ✅ Understand the problem: First figure out what the essence of "notification" is
2. ✅ Establish TODOs: Confusion, multi-angle exploration, counterexample validation
3. ✅ Real iteration:
   - Explore classification by content → Discovered too many categories, users find it hard to understand
   - Try classification by importance → Discovered too subjective, unable to unify standards
   - Reflect on "user scenario" principle → Found the idea of classifying by "urgency of user behavioral response"
4. ✅ Multiple overthrowing: At least 3 major direction adjustments
5. ✅ Case validation: Complete validation with scenarios like "friend request", "system maintenance", "content recommendation"
6. ✅ Honest summary: Admit that boundary scenarios (like event notifications) still need further discussion

**Result**: Got a three-level classification scheme (immediate/same-day/deferrable), clarified boundary problems to be resolved

---

## When to Use This Pattern

### Should Use:
- Complex design problems (no clear answer)
- Problems requiring deep understanding of essence
- Decisions involving multiple dimensions and trade-offs
- System architecture design

### Should Not Use:
- Simple implementation problems (clear solution exists)
- Pure information queries (no design decision needed)
- Urgent problem fixes (need quick resolution)

---

## Trigger Keywords

Automatically enable this pattern when users say:
- "deep iterative thinking"
- "exploratory iteration"
- "non-linear iteration"
- "think deeply about this problem"
- "don't rush to conclusions"
- "multi-angle iteration"

---

**Core Concept**: Understand Problem → Real Exploration → Deep Essence → Honest Summary

**Highest Principle**: Real thinking, not performative iteration.
