---
name: "tech-planning"
description: "Helps create tech planning documents using management planning framework (function/goal/team/path). Invoke when user asks for tech planning, roadmap, technical strategy, or wants to plan team technical direction."
---

# Technical Planning Skill

A systematic skill for creating technical planning documents based on the management planning framework from "知行：技术人的管理之路" (The Way of Technology Management).

## When to Invoke

Invoke this skill when:
- User asks to create a technical planning document
- User mentions "技术规划" (tech planning), "技术路线图" (tech roadmap), "技术战略" (tech strategy)
- User wants to plan team's technical direction
- User needs to make technical decisions or selections
- User asks about team positioning and goal setting

## Core Framework: Management Planning Four Elements

The skill is based on four core questions that every technical planning must answer:

```
Management Planning Four Elements:
┌─────────────────────────────────────────┐
│  FUNCTION: Why does this team exist?     │
│  GOAL: What output is expected?          │
│  TEAM: What team development expected?   │
│  PATH: What resources needed?            │
└─────────────────────────────────────────┘
```

**Relationship:**
- **Function** = Team positioning, determines value foundation
- **Goal** = Value manifestation, clarifies expected results
- **Team** = Resource base, determines capability to achieve goals
- **Path** = Achievement means, connects resources to goals

## Skill Workflow

### Step 1: Clarify Function (Team Positioning)

**Three Core Questions:**
1. Why was this team established?
2. What's the unique value if this team continues to exist?
3. What dimensions to measure team value?

**Two Levels of Team Function:**
```
Responsibility (Lower Bound): Team survival
    ↓ At least complete the work
Mission (Upper Bound): Team development
    ↓ Manager's own planning and expectations
```

**Three-Step Method:**
```
Step 1: Collect Information
├── Listen to superior's expectations and requirements
├── Ask team members about future expectations
├── Clarify boundaries with sibling teams
└── Combine with own understanding of the domain

Step 2: Refine and Elevate
├── Use easy-to-understand text to simplify and refine function
└── Combine with industry trends, set expectations

Step 3: Confirm and Advocate
├── Get superior's support and recognition
└── Promote team responsibilities and mission in appropriate occasions
```

**Output Template:**
```
## Function Positioning

**Responsibility (Lower Bound):** [What must be done]
**Mission (Upper Bound):** [What the team aims to become]

**Team Value Statement:**
[Clear statement of team's unique value and positioning]
```

### Step 2: Define Goals (Expected Output)

**Three Types of Goals:**

| Goal Type | Description | Priority | Example |
|-----------|-------------|----------|---------|
| **Business Goal** | Goals from business perspective | Required | Launch new features, customer volume, revenue |
| **Professional Goal** | Goals from technical capability perspective | Optional | Stability, service capacity, processing capability |
| **Team Goal** | Team size and gradient growth | Optional | Personnel growth,梯队培养 |

**SMART Principle:**
```
SMART Principle:
├── Specific: Clear and specific goals
├── Measurable: Quantifiable standards
├── Achievable: Realistic goals
├── Relevant: Related to team function
└── Time-bound: Clear timeframes
```

**Key Principle: Goals should be as few as possible.**

**Decision Priority:** Business Value > Controllable Scope > Technical Depth

**Output Template:**
```
## Goal Setting (SMART)

### Business Goal (Required)
[Clear business objectives with metrics and timeline]

### Professional Goal (Optional)
[Technical capability objectives]

### Team Goal (Optional)
[Team development objectives]
```

### Step 3: Plan Team (Resource Base)

**Three Dimensions:**

```
Team Planning Three Dimensions:
┌─────────────────────────────────────┐
│  Size: Current headcount, future additions │
│  Division: Business areas, personnel config│
│  Gradient: Capability distribution, maturity│
└─────────────────────────────────────┘
```

**Ideal Gradient Structure:**
```
Ideal Team Gradient:
┌──────────────────┐
│ Core骨干 (20%)    │ ← Key decisions, technical攻坚
├──────────────────┤
│ 中坚力量 (60%)    │ ← Daily work, stable output
├──────────────────┤
│ Growth潜力 (20%)  │ ← Learning, backup培养
└──────────────────┘
```

**Key Insight: Mature gradient teams won't collapse due to core member leaving.**

**Output Template:**
```
## Team Planning

### Team Size
- Current: [N] people
- Planned addition: [N] people
- Total target: [N] people

### Team Division
[Clear division of responsibilities and personnel allocation]

### Team Gradient
[Capability distribution and development plan]
```

### Step 4: Define Path (Achievement Means)

**Two Core Questions:**
1. What paths are available? What key work to achieve goals?
2. What preparation needed? How much resources for each?

**Available Means:**

```
Path Selection Matrix:
┌─────────────┬──────────────┬──────────────┐
│   Means     │ Scenario      │ Characteristics│
├─────────────┼──────────────┼──────────────┤
│ Self-develop│ Core capability│ Strong control, long cycle│
│ Hire experts│ Missing key skills│ Fast fill, high cost│
│ Borrow engineers│ Temporary needs│ Flexible, requires coordination│
│ Partnership│ Capability complement│ Resource sharing, boundary mgmt│
│ Outsourcing │ Non-core work│ Efficient, quality control needed│
└─────────────┴──────────────┴──────────────┘
```

**Resource Types:**
```
Resource Types:
├── Human resources: Personnel count, capability structure
├── Financial resources: Budget, cost control
├── Material resources: Equipment, facilities, infrastructure
├── Time resources: Deadlines, milestone nodes
├── Information resources: Internal and external information mastered
└── Authority resources: Permission scope available
```

**Key Insight: Time, information, and authority are also very important resources.**

**Dependency Analysis:**

```
Dependency Analysis Matrix:
┌─────────────┬────────────┬─────────────┐
│  Dependency │ Importance │ Control Power│
├─────────────┼────────────┼─────────────┤
│ Dependency1 │ High/Med/Low│ Strong/Med/Weak│
│ Dependency2 │ High/Med/Low│ Strong/Med/Weak│
│ Dependency3 │ High/Med/Low│ Strong/Med/Weak│
└─────────────┴────────────┴─────────────┘
```

**Decision Logic:**
- High importance + Strong control → Can depend, include in plan
- High importance + Medium control → Need backup plan or leader support
- High importance + Weak control → Must get leader support, or remove dependency
- Low importance + Weak control → Acceptable risk, have alternatives

**Output Template:**
```
## Path Planning

### Available Paths
[List of available means and key work items]

### Resource Requirements
- Personnel: [Specific requirements]
- Budget: [Financial requirements]
- Time: [Timeline and milestones]
- Information: [Information needs]
- Authority: [Permission requirements]

### Dependency Analysis
[Key dependencies and control analysis]
```

## Technical Selection Framework

When technical selection is part of planning, use **AHP (Analytic Hierarchy Process)**.

**Evaluation Dimensions:**

| Dimension | Description | Evaluation Points |
|-----------|-------------|-------------------|
| Business Fit | Meets business needs | Function coverage, scalability, scenario fit |
| Technical Maturity | Stability and reliability | Community activity, version stability, production cases |
| Team Capability | Learning and mastery cost | Learning curve, skill match, training cost |
| Ecosystem Support | Third-party support | Documentation quality, third-party libs, toolchain |
| Long-term Maintenance | Sustainability | Commercial support, tech roadmap, upgrade cost |
| Cost-Benefit | ROI | Development cost, operation cost, time cost |

**AHP Steps:**
1. Build decision hierarchy (goal → criteria → alternatives)
2. Build judgment matrix (pairwise comparison with 1-9 scale)
3. Calculate weight vector (normalize, average)
4. Consistency check (CR < 0.1)
5. Calculate final ranking
6. Select optimal alternative

## Implementation Guidelines

### Small Steps Iteration

**Key Principle: Control scope, small step iteration.**

**Implementation Points:**
- First phase: Integrate with existing system, gradually transition to new approach
- Select one core system for pilot, not all at once
- Each phase has clear delivery goals and validation criteria

### OKR Integration

**OKR Chain:**
```
Product Strategy → OKR Setting → KPI Selection → Strategy Landing Feedback
```

**Technical OKR Principles:**
- Objective: Clear business value orientation
- Key Results: Quantifiable technical metrics

**Example:**
```
O: Improve platform stability, ensure core business continuity
KR1: Core service availability from 99.5% to 99.9%
KR2: Average recovery time from 30min to 10min
KR3: Complete 80% core service monitoring and alerting system
```

## Complete Output Template

```markdown
# [Team Name] Technical Planning Document

> Based on management planning framework

## 1. Function Positioning

**Responsibility (Lower Bound):** [What must be done - survival]
**Mission (Upper Bound):** [What the team aims to become - development]

**Team Value Statement:** [Unique value and positioning]

## 2. Goal Setting (SMART Principle)

### Business Goal (Required)
[Clear business objectives with metrics and timeline]

### Professional Goal (Optional)
[Technical capability objectives]

### Team Goal (Optional)
[Team development objectives]

## 3. Team Planning

### Team Size
- Current: [N] people
- Planned addition: [N] people
- Total target: [N] people

### Team Division
[Clear division of responsibilities and personnel allocation]

### Team Gradient
[Capability distribution and development plan]

## 4. Path Planning

### Available Paths
[List of available means and key work items]

### Resource Requirements
- Personnel: [Specific requirements]
- Budget: [Financial requirements]
- Time: [Timeline and milestones]
- Information: [Information needs]
- Authority: [Permission requirements]

### Dependency Analysis
[Key dependencies and control analysis]

## 5. Technical Roadmap

### Quarterly View
[Q1-Q4 milestone planning]

### Technical Evolution
[Technology stack evolution path]

## 6. OKR Alignment

### Objectives
[Key objectives aligned with planning]

### Key Results
[Quantifiable results for each objective]

## 7. Risk Management

### Key Risks
[Risk identification]

### Mitigation Plans
[Risk mitigation strategies]

---

Created: [Date]
Manager: [Name]
```

## Usage Examples

### Example 1: New Team Planning

User: "我需要为新成立的数据团队做技术规划"

**Response Approach:**
1. First clarify function positioning: Why does the data team exist? What's the unique value?
2. Define goals: What business outcomes expected? What technical capabilities needed?
3. Plan team: How many people? What roles? What gradient?
4. Define path: Self-develop or hire? What resources needed?

### Example 2: Technology Upgrade Planning

User: "我们团队要做技术栈升级，怎么规划?"

**Response Approach:**
1. Function positioning remains unchanged, but mission elevates
2. Goals focus on: stability improvement, capability enhancement
3. Team planning: Training needs, skill upgrade plan
4. Path: Phased upgrade, pilot first, then full rollout

### Example 3: Technical Selection

User: "我们需要选择一个新的数据库，应该怎么决策?"

**Response Approach:**
1. Use AHP framework
2. Define evaluation dimensions and weights
3. Compare alternatives systematically
4. Make decision with clear rationale

## Key Principles Summary

1. **Function positioning is the foundation** - Clear responsibility (lower bound) and mission (upper bound)
2. **Goals should be differentiated** - Business, professional, team goals each with focus
3. **Team gradient ensures resilience** - Mature teams won't collapse due to key person leaving
4. **Multiple path options available** - Self-develop, hire, borrow, partner, outsource各有适用场景
5. **Business value > Controllable scope > Technical depth** - Decision priority
6. **Small steps iteration for landing** - Control scope, pilot first, validate then expand
7. **Dependency management is critical** - High importance + Weak control = Must get leader support

## Related Resources

- Source document: team-management/process/如何做好技术规划.md
- Reference: 《知行：技术人的管理之路》刘建国著
- Template: team-management/process/README.md

---

*This skill provides systematic guidance for technical planning based on proven management framework.*