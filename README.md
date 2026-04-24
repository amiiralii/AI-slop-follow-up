## Overview

This README summarizes a set of **short, publishable research directions** that build directly on the recent study on AI-generated software artifacts ("AI slop"). The goal is to support **fast-turnaround research (≈6–12 weeks)** with clear empirical contributions suitable for strong software engineering and human-centered computing venues.

Each idea operationalizes a claim from prior qualitative findings into a **measurable experiment**, enabling meaningful contributions without requiring a long-term project.

---

# Research Ideas Summary Table

| Proposed Title                                             | Core Research Question                                                                 | Experiment / Study Idea (Minimal Viable Design)                                                                                          | Primary Contribution                                      | Estimated Timeline | Best-Fit Venues      |
| ---------------------------------------------------------- | -------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- | ------------------ | -------------------- |
| **Do AI-Assisted Pull Requests Increase Review Effort?**   | Do AI-generated or AI-assisted PRs require more review effort than human-written ones? | Mine GitHub PR data. Compare AI vs non-AI PRs on metrics like review time, number of comments, and revision cycles.                      | Quantifies reviewer burden as a measurable metric.        | 6–8 weeks          | MSR, ESEM, ICSE SEIP |
| **The Comprehension Gap in AI-Assisted Programming**       | Do developers understand AI-generated code less than human-written code?               | Controlled experiment. Participants review code snippets (AI vs human). Measure explanation accuracy, debugging success, and confidence. | Empirical evidence of differences in code understanding.  | 8–12 weeks         | ICSE, CHI, ASE       |
| **Detecting Risky Patterns in AI-Generated Code**          | Can automated heuristics identify low-quality or risky AI-generated code patterns?     | Build rule-based or ML classifier using static analysis signals. Evaluate detection performance on labeled dataset.                      | Practical detection method or lightweight tool.           | 10–14 weeks        | ASE, FSE Tool Track  |
| **Do Productivity Incentives Increase AI Code Defects?**   | Do speed-based incentives lead to lower-quality AI-generated code?                     | Controlled experiment with two groups rewarded differently (speed vs quality). Compare defect rates and maintainability.                 | Evidence linking incentives to software quality outcomes. | 6–10 weeks         | ICSE, CSCW           |
| **Technical Debt Acceleration in AI-Assisted Development** | Does AI-assisted coding increase technical debt accumulation over time?                | Analyze version history before and after AI adoption. Track code complexity, churn, and defect density longitudinally.                   | Quantifies long-term maintainability effects.             | 10–12 weeks        | ICSE, FSE            |
| **Trust Calibration in AI Code Review**                    | How accurately do developers judge the reliability of AI-generated code?               | Participants review mixed-quality code labeled as AI or human. Measure trust decisions vs actual correctness.                            | Model of trust miscalibration in AI workflows.            | 8–10 weeks         | CHI, ICSE            |

---

# Short Descriptions of Each Experiment

## 1) Review Effort Study

**Title:** Do AI-Assisted Pull Requests Increase Review Effort?

This experiment investigates whether AI-generated code shifts effort from development to code review. The study uses repository mining to compare review behavior across AI-assisted and traditional pull requests.

### Key Metrics

* Review time
* Number of review comments
* Number of revisions
* Pull request lifespan

### Why It Matters

This is the **fastest and most reliable path to publication**, because it transforms a widely discussed claim into measurable evidence.

---

## 2) Comprehension Gap Experiment

**Title:** The Comprehension Gap in AI-Assisted Programming

This study evaluates whether developers understand AI-generated code differently from human-written code. It focuses on cognition rather than code quality alone.

### Study Design

Participants review code and answer questions such as:

* What does this code do?
* Where is the bug?
* How confident are you?

### Why It Matters

Understanding—not code generation—is becoming the bottleneck in software engineering.

---

## 3) Risky Pattern Detection Tool

**Title:** Detecting Risky Patterns in AI-Generated Code

This project develops a lightweight detection mechanism for identifying risky AI-generated code patterns using static analysis or machine learning.

### Example Signals

* Dead code
* Duplicate logic
* Test manipulation
* Excessive complexity
* Unsafe shortcuts

### Why It Matters

This is an engineering-oriented contribution with clear practical value.

---

## 4) Incentive Impact Experiment

**Title:** Do Productivity Incentives Increase AI Code Defects?

This experiment tests whether performance incentives influence software quality when AI tools are used.

### Study Setup

Group A:
Rewarded for speed

Group B:
Rewarded for quality

Participants complete the same programming task using AI tools.

### Why It Matters

This isolates **organizational behavior** as a root cause of quality problems.

---

## 5) Technical Debt Acceleration Study

**Title:** Technical Debt Acceleration in AI-Assisted Development

This study examines whether AI-assisted coding increases long-term maintenance costs by analyzing repository history over time.

### Metrics

* Code churn
* Complexity
* Defect density
* Refactoring frequency

### Why It Matters

This addresses sustainability and maintainability rather than short-term productivity.

---

## 6) Trust Calibration Study

**Title:** Trust Calibration in AI Code Review

This experiment investigates whether developers trust AI-generated code appropriately relative to its actual correctness.

### Core Measurement

Trust Accuracy:

```
Trust Decision vs Actual Code Quality
```

### Why It Matters

Misplaced trust in automation is a major risk in AI-assisted development systems.

---

# Recommended Starting Points

If you want:

Fastest publication:

* Start with **Review Effort Study**

Strongest theoretical contribution:

* Choose **Comprehension Gap**

Tool-oriented contribution:

* Choose **Risky Pattern Detection**

Behavioral or organizational research:

* Choose **Incentive Impact**

---

# Suggested Project Scope

Typical minimal publishable unit:

* Dataset: 30–50 repositories or participants
* Duration: 6–12 weeks
* Paper length: 6–8 pages
* Contribution: One measurable metric or validated hypothesis
