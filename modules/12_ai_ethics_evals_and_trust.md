# Module 12: AI Ethics, Evals, And Trust

## Why This Matters

Weak AI work often fails for reasons that are not visible in a demo.

Examples:

- unsupported answers
- biased outputs
- brittle behavior on edge cases
- privacy violations
- poor fit for the user workflow

If you want to be taken seriously in AI, you need more than output generation.

You need trustworthiness.

## Professional Standard

For most applied AI work, you should be able to answer:

1. What can this system do well?
2. Where does it fail?
3. How do we know?
4. What is the risk if it is wrong?
5. What safeguards exist?

## The Trust Stack

Think about AI quality in layers.

| Layer | Key Question |
|-------|--------------|
| **Use Case Fit** | Should AI be used for this task at all? |
| **Data And Context** | Is the model working from good, relevant, allowed inputs? |
| **Output Quality** | Are responses correct, grounded, and useful? |
| **Safety And Risk** | What happens if the model is wrong or harmful? |
| **Operations** | Can we monitor, audit, and improve it over time? |

## Ethics In Practical Terms

Ethics is not only philosophy language.

In practice, it usually means making good decisions around:

1. fairness
2. privacy
3. transparency
4. accountability
5. appropriate human oversight

## Common Failure Patterns

### Pattern 1: Demo Success, Workflow Failure

The model looks good in a notebook, but fails in real use because the task is messy and context is incomplete.

### Pattern 2: Hidden Bias

The system performs well on common cases but behaves poorly for minority groups, edge inputs, or underrepresented data conditions.

### Pattern 3: No Evaluation Discipline

The builder uses anecdotal testing instead of a repeatable eval set.

### Pattern 4: Unclear Escalation Path

The system makes confident mistakes but there is no fallback to a human or another workflow.

## Minimum Evaluation Discipline

Even for a small project, you should try to include:

1. a set of representative test cases
2. a set of edge cases
3. a failure log
4. a simple scoring rubric
5. notes on known limitations

For LLM projects, evaluate things such as:

1. groundedness
2. instruction following
3. format correctness
4. refusal behavior when data is missing
5. stability across prompt variation

## Bias And Fairness Questions

Ask these before shipping anything important.

1. Who might be misrepresented by the data?
2. Which user groups might experience systematically worse outcomes?
3. Is this task sensitive enough that human review should remain mandatory?
4. Are we accidentally automating an unfair process?

## Trust-Building Design Choices

Good builders often make their system more trustworthy by doing things like:

1. grounding answers in known documents
2. showing sources or evidence
3. making confidence limitations explicit
4. using structured outputs where possible
5. adding human review for high-risk steps
6. logging failures and user feedback

## How This Helps Your Career

Trust and evaluation skill are strong differentiators.

They help you stand out because many candidates can build a prototype, but fewer can:

1. define quality
2. detect failure modes
3. reduce risk
4. explain why a system is safe enough for real use

## Practical Rule

Do not ask only, "Can I make the model answer?"

Also ask, "Can I make the system dependable enough that a serious user would trust it?"