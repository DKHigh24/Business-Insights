##Quality Analytics Copilot CLI Skills Repository
#Purpose
This repository contains reusable Copilot CLI skills for quality-focused business analysis.

The system is designed to help a senior business analyst farm out repeatable analytical assignments to AI-assisted subordinate analysts. Each skill should inspect relevant data, perform a focused analysis, connect findings to business objectives, and produce decision-ready recommendations.

The initial focus is enterprise quality analysis. Future iterations will break insights out by vertical, product type, brand, customer segment, sales channel, region, issue type, and leader-specific areas of responsibility.

Analyst Role
You are a data analyst focused on product and operational quality.

You use the American Society for Quality general model and the Cost of Quality framework, including:

Prevention costs
Appraisal costs
Internal failure costs
External failure costs
Your work is not simply to report metrics. Your job is to connect quality performance to business outcomes.

Overarching Business Objectives
Every metric, KPI, analysis, dashboard, insight, and recommendation must support one or more of the following business objectives.

1. Grow Net Sales
Quality improvement supports net sales growth by improving customer confidence, reducing repeat failures, strengthening customer experience, supporting retention, and potentially increasing market share.

2. Reduce the Cash Conversion Cycle
Quality issues can create delays, credits, disputes, rework, replacement orders, shipment holds, billing delays, and collections friction. Analysis should identify where quality problems slow the conversion of orders into cash.

3. Manage the Balance Sheet
Quality analytics should help reduce or control quality cost, failure cost, warranty exposure, scrap, concessions, freight waste, inventory risk, and other forms of preventable financial leakage.

Core Analytical Belief
Improving quality performance improves customer experience.

Improved customer experience is believed to have a positive relationship with growth in net sales because it increases customer confidence, reduces friction, improves retention, and may support market share growth.

Therefore, all quality analytics should connect:

Quality Performance → Customer Experience → Financial / Business Outcome
First Principle: Prioritize by ROI and Business Breadth
Quality improvement opportunities should be prioritized based on expected return on investment, business impact, and breadth of applicability.

The goal is not to chase every issue. The goal is to identify which issues deserve time, labor, capital, engineering attention, process change, or leadership escalation.

Priority Bias
Prioritize work in this general order:

High volume / high cost / recurring issue
High volume / moderate cost / broad customer impact
Moderate volume / high cost / clear repeatability
Low volume / high cost / strategic or reputational risk
Low volume / low cost / only if broader business justification exists
A high-runner product or process with a costly recurring issue should usually take priority over a low-runner issue with limited cost exposure.

A low-runner issue with low cost should not be prioritized for major improvement effort unless there is an extenuating business reason.

Sales advocacy is a valid reason to review an issue, but it does not automatically justify investment. To justify prioritization, the issue should demonstrate breadth across the business, strategic significance, future exposure, reputational risk, or evidence of a broader systemic failure.

Initial Skills
This repository starts with four core skills.

1. Claims Analysis
Analyzes claims data to identify recurring quality issues, costly failure modes, high-impact products, customer pain points, and improvement opportunities.

Path:

skills/claims-analysis/SKILL.md
2. Constraint Analysis and Alternative Recommendations
Analyzes operational, product, process, supply, data, or organizational constraints and recommends alternatives that reduce business friction, quality risk, customer disruption, or financial impact.

Path:

skills/constraint-analysis-alternative-recommendations/SKILL.md
3. Margin Impact Analysis
Analyzes how quality failures, claims, rework, concessions, scrap, warranty labor, freight, and related costs affect product, customer, channel, or business unit margin.

Path:

skills/margin-impact-analysis/SKILL.md
4. Order Book Analysis
Analyzes open orders, backlog, shipment patterns, customer exposure, and order risk to understand where quality, fulfillment, or operational issues may affect revenue, cash conversion, and customer experience.

Path:

skills/order-book-analysis/SKILL.md
Future Feature Adds
The repo reserves space for future skills.

Quality Calculator
Reusable calculations for claim rate, failure rate, Cost of Quality, external failure cost, internal failure cost, ROI, exposure, quality-adjusted margin, and improvement payback.

Predictive Failure Analysis
Predictive analytics skill to identify products, orders, customers, or failure modes with elevated future quality risk.

Value Analysis
Business value skill for comparing improvement opportunities by customer value, company value, strategic relevance, financial impact, and customer experience impact.

Iterative Operating Model
The system is designed to mature over time.

Phase 1: Enterprise Quality View
The first version should evaluate quality across the company to identify the largest quality cost drivers, failure patterns, business risks, and improvement opportunities.

Phase 2: Breakout by Business Dimension
Future iterations should segment analysis by:

Vertical
Product type
Brand
Customer segment
Sales channel
Region
Business unit
Failure type
Claim type
Process stage
Strategic growth area
Phase 3: Leader-Tailored Insights
As the system matures, each leader should receive analysis specific to their area of responsibility:

What quality issues matter most to my business area?
Which products, brands, or customers carry the most quality risk?
Where are we losing margin, cash, or customer confidence?
Which improvement opportunities should my team prioritize?
What action should be taken next?
The progression should be:

Enterprise View → Segment View → Leader-Specific View → Actionable Improvement Plan
Skill Output Standard
Every skill should move from data to decision.

Use this standard structure:

Observation → Business Impact → Prioritization → Recommendation → Expected Outcome
Each skill output should include:

Executive summary
Key findings
Business impact
KPI interpretation
Priority ranking
Recommended actions
Risks, assumptions, and data gaps
Suggested next analysis
Metric Standard
No KPI should exist only because it is measurable.

Every KPI should answer at least one of these questions:

Does this help us grow net sales?
Does this help us reduce the cash conversion cycle?
Does this help us reduce failure costs or protect the balance sheet?
Does this improve customer confidence or reduce customer friction?
Does this identify where quality failures are creating financial or operational drag?
Does this help prioritize improvement work based on ROI?
Definition of Done for Any Skill
A skill is complete when it has produced:

A clear answer to the business question
A quantified view of impact where data allows
A connection to one or more business objectives
A prioritization rationale
A recommended action
A list of assumptions and data gaps
A reusable output format that can be used by a business leader
Recommended Repository Structure
quality-analytics-copilot-cli/
  README.md

  governance/
    GOVERNING_PREMISE.md
    PRIORITIZATION_PRINCIPLES.md
    ITERATIVE_OPERATING_MODEL.md

  skills/
    README.md

    _skill-template/
      SKILL.md

    claims-analysis/
      SKILL.md

    constraint-analysis-alternative-recommendations/
      SKILL.md

    margin-impact-analysis/
      SKILL.md

    order-book-analysis/
      SKILL.md

  future-skills/
    README.md

    quality-calculator/
      README.md

    predictive-failure-analysis/
      README.md

    value-analysis/
      README.md

  docs/
    DATA_INPUTS.md
    OUTPUT_STANDARDS.md
    KPI_DICTIONARY.md

  examples/
    prompts/
      claims-analysis-prompts.md
      constraint-analysis-prompts.md
      margin-impact-analysis-prompts.md
      order-book-analysis-prompts.md

    outputs/
      README.md

  data/
    input/
      .gitkeep

    reference/
      .gitkeep

  reports/
    .gitkeep
How to Use This Repo with Copilot CLI
Use the skill files as operating instructions.

Example:

Use the Claims Analysis skill in skills/claims-analysis/SKILL.md.
Review the claims extract in data/input.
Identify the top quality cost drivers and recommend which issues deserve improvement investment.
Tie every recommendation to net sales, cash conversion cycle, balance sheet management, or customer experience.
Guiding Reminder
These skills are not passive reporting tools.

They are structured quality intelligence agents designed to help identify where quality issues are creating the greatest business drag and where improvement work is most likely to generate meaningful return.# Business-Insights
