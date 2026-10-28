# Huishoubao Valuation Experience Optimization

## AI-Assisted Condition Assessment and Inspection Transparency

An independent product design project exploring how AI assistance and clearer inspection evidence could improve the experience of selling a used smartphone through Huishoubao.

**Status:** Research, requirements, workflows, prototypes, functional rules, and measurement design completed. The proposed service has not been developed or launched. Recognition performance, usability improvements, and conversion impact remain unvalidated.

**Role:** Independent project designer, responsible for user research, competitor analysis, requirements, prioritization, process design, prototyping, metrics, and iteration planning.

## Overview

Online device recycling typically follows four stages: user self-assessment, an estimated quote, professional inspection, and acceptance of a final offer. Users with limited device-inspection experience may struggle to identify cosmetic damage, select the correct condition options, and understand why the final offer differs from the estimate.

This project proposes a connected workflow:

1. Guide users to photograph the phone's screen, back panel, and frame.
2. Use AI to assist with identifying visible cosmetic issues.
3. Let users confirm or edit findings before completing condition fields.
4. Retain photographs and confirmed condition records.
5. Compare those records with professional inspection findings.
6. Explain discrepancies and their monetary impact using inspection evidence and platform pricing rules.

AI is advisory. Users retain control over submitted information, professional inspectors determine final condition, and platform pricing rules determine the offer.

## Problems to Address

| Problem | User difficulty | Product opportunity |
| --- | --- | --- |
| Condition assessment | Distinguishing minor scratches, dents, cracks, and damage severity from reference images | Photo-based assistance with editable results |
| Inspection verification | Checking whether a newly reported issue existed before shipping | Retained pre-order photographs and confirmed records |
| Price interpretation | Understanding how inspection discrepancies affect the final payout | Item-level comparisons and evidence-based explanations |

The objective is to create a continuous, understandable, and verifiable information trail from valuation to the final offer.

## User Research

### Methods and Sample

| Method | Sample | Purpose |
| --- | --- | --- |
| Public feedback analysis | 60 entries: 40 about Huishoubao, 10 about Aihuishou, and 10 about Zhuanzhuan | Identify recurring concerns about valuation, inspection, price adjustments, and trust |
| Semi-structured interviews | 8 participants; 6 had completed online valuations, 3 had experienced professional inspection, and 2 had completed transactions | Explore assessment difficulties, expectations, transaction decisions, and reactions to the AI concept |

Interview experience categories overlap. Public sources included Black Cat Complaints, Zhihu, Baidu Tieba, and public experience articles. Entries were summarized and coded by platform, source, transaction stage, sentiment, topic, and behavior.

### Main Findings

- **Condition assessment requires expertise:** All eight interviewees described some difficulty recognizing subtle issues or grading damage; six drew on actual valuation or transaction experience.
- **Self-assessment can differ from inspection:** All three participants with inspection experience encountered cosmetic issues they had not identified during online self-assessment.
- **Evidence and convenience matter alongside price:** Participants weighed the price gap, available photographs, and return-shipping effort differently.
- **Transparency does not replace price competitiveness:** Users often preferred clearer records when quotes were similar, but some prioritized a substantially higher offer.
- **AI requires user control:** Participants were open to assistance but wanted to review, edit, or bypass recognition results.

### Research Limitations

The sample is small, with only three participants having inspection experience. Complaint-platform sampling may overrepresent negative experiences, and public accounts were not independently verified. Findings support problem discovery and product hypotheses; they do not estimate issue prevalence. Reactions to the AI concept are not evidence of validated prototype usability or realized business impact.

## Target Users

The primary audience is the **Cautious Novice**: a first-time or infrequent platform user with a clear need to sell an old smartphone, limited inspection knowledge, and concerns about unexpected price reductions after shipping.

| Segment | Main need | Priority |
| --- | --- | --- |
| Cautious novice | Assessment support, verifiable evidence, and understandable adjustments | Primary |
| Infrequent convenience seeker | Less repeated assessment, entry, and communication effort | Secondary |
| Price-focused novice | The highest quote, with greater tolerance for uncertainty | Not prioritized in the MVP |
| Experienced price comparer | Competitive quotes across platforms | Not prioritized in the MVP |

## Competitor Research

App walkthroughs conducted in **October 2026**, supplemented by public materials and user feedback, compared Huishoubao, Aihuishou, and Zhuanzhuan.

| Platform | Observed strengths | Opportunity identified in the walkthrough |
| --- | --- | --- |
| Huishoubao | Condition descriptions, reference images, and estimated-price information | Standardized actual-device records and clearer links between findings and price changes |
| Aihuishou | Structured reports with photographs, inspectors, matching items, and discrepancies | Photo-based condition assistance and verified item-level monetary explanations |
| Zhuanzhuan | Photo-based category/model suggestions and detailed inspection reports | Structured cosmetic assessment linked to confirmed records and later inspection findings |

These are observations of the reviewed versions, not claims that an unobserved feature is permanently absent. The differentiation proposed here is the connection between assessment, confirmation, evidence retention, and post-inspection explanations.

## MVP Scope and Prioritization

### Must Have

- Guided photographs of the screen, back panel, and frame.
- AI assistance for visible scratches, dents, cracks, and similar cosmetic issues.
- User confirmation, editing, and automatic condition-field completion.
- Retained photographs and final confirmed condition records.
- Comparison of confirmed records with professional inspection findings.
- Explanations grounded in actual findings and platform pricing rules.
- Retakes for affected areas and an available manual-entry path.

### Later Priorities

| Priority | Feature |
| --- | --- |
| Should have | Multi-turn questions about individual inspection discrepancies |
| Should have | Streamlined handoff to human customer service when AI cannot explain |
| Could have | Anonymous inspection-report sharing |

### Out of Scope

- Inferring internal faults, functional problems, or repair history from photographs.
- AI submission of condition information without user confirmation.
- AI determination of the final condition or price.
- Cross-platform quote comparison.
- Tablets, laptops, and other device categories in the initial MVP.

## Core User Journey

### Before Ordering

Users upload photographs of the three required areas. The system checks image suitability and attempts visible-condition assessment. Users can retake affected areas or choose manual entry without a minimum number of attempts.

After reviewing or editing the findings, users report functional issues and repair history. The platform retains photographs and confirmed information, displays an estimate, and allows users to place a recycling order.

### After Inspection

Professional inspectors submit actual findings. The platform compares those findings with the user's confirmed pre-order records and applies pricing rules to calculate the final offer and item-level impacts.

Users can view the inspection report, expand discrepancy explanations, optionally mark explanations helpful or unhelpful, and request manual review of a specific finding.

## Prototype Screens

| Screen | Main interactions |
| --- | --- |
| Guided photo capture | Upload screen, back-panel, and frame photographs; preview or replace images; start assessment |
| Recognition confirmation | Review marked issue locations, edit condition fields, add missed issues, and confirm |
| Inspection and price explanation | Compare pre-order and inspection evidence, review price impacts, open the full report, submit feedback, or request review |

The project document contains the prototypes, persona, competitor evidence, and workflow diagrams. Original Chinese interface screenshots and prototype visuals are retained in the English report with explanatory English text.

## Functional Rules

- Retain completed uploads and form fields when a user retakes an image or corrects missing information.
- Keep manual entry available without requiring a fixed number of failed attempts.
- Use the user's final confirmed condition as the comparison baseline.
- Calculate monetary amounts through platform pricing rules; AI explains rather than inventing prices.
- Reconcile item-level monetary impacts with the total change in the offer.
- Link review requests to the relevant photographs and records.

**Specification point to resolve before development:** The source document contains different descriptions of AI-result retention. Some sections retain recognition results alongside confirmation records; the detailed rules retain only photographs and final confirmed condition, without separately storing the original AI assessment. The implementation specification should settle this data-retention choice.

## Metrics

The **North Star metric** is valuation-to-transaction conversion, measured by linking completed valuation sessions to subsequent completed orders.

| Metric | Definition |
| --- | --- |
| Valuation-to-transaction conversion | Completed valuation sessions leading to a completed transaction / Completed valuation sessions |
| Valuation completion | Sessions displaying an estimated quote / Sessions starting valuation |
| Valuation-to-order conversion | Completed valuation sessions leading to an order / Completed valuation sessions |
| Post-inspection transaction conversion | Completed orders / Orders displaying a final quote |
| Discrepancy explanation click rate | Orders with explanation clicks / Orders with report views and discrepancies |
| Explanation helpfulness rate | Orders with helpful feedback / Orders submitting helpful or unhelpful feedback |

Multiply each ratio by 100% for percentage presentation. Deduplicate by session or order as appropriate and use a consistent conversion observation window. Valuation completion includes AI-assisted and manual-entry paths. Helpfulness excludes nonresponses and reflects voluntary respondents rather than all report viewers.

## Event Tracking

| Event | Trigger | Key properties |
| --- | --- | --- |
| Valuation started | User enters the valuation flow | Session ID, event time |
| Valuation completed | Estimated quote successfully displayed | Session ID, event time |
| Order created | Recycling order successfully created | Session ID, order ID, event time |
| Final quote displayed | Post-inspection offer successfully displayed | Order ID, event time |
| Transaction completed | Order status becomes completed | Order ID, event time |
| Inspection report viewed | User opens the report | Order ID, discrepancy indicator, event time |
| Discrepancy explanation clicked | User opens an explanation | Order ID, event time |
| Explanation feedback submitted | User voluntarily submits a response | Order ID, helpful/unhelpful response, event time |

Bind the order ID to the valuation session at order creation to connect the pre-order journey with inspection and transaction outcomes.

## Feasibility and Risks

| Area | Consideration | Proposed response |
| --- | --- | --- |
| Recognition accuracy | Lighting, image quality, and angle can cause errors or omissions | User review, editing, retakes, and manual entry |
| Explanation credibility | AI may generate unsupported explanations | Ground explanations in inspection evidence and pricing outputs; allow manual review |
| AI integration | Adaptation and inference costs | Validate recognition performance and reduced user effort before expansion |
| Interface and storage | Capture, confirmation, comparison, and record-storage costs | Define the evidence and retention requirements before development |
| Inspection and pricing integration | Linking orders, findings, and monetary adjustments | Define consistent item mappings and reconcile price impacts |

Expected benefits remain hypotheses. No deployed system, production recognition accuracy, measured conversion uplift, or realized financial return is claimed.

## Deliverables

- Problem definition and product objectives.
- Public feedback analysis and interview findings.
- User segmentation and core persona.
- Competitor feature comparison.
- User stories and MoSCoW prioritization.
- MVP boundaries and business workflow.
- Three core screen prototypes.
- Functional rules and exception handling.
- Metric definitions and event-tracking plan.
- Feasibility assessment and future iteration plan.
- Research appendices with sample feedback, recruitment questions, and interview guide.

## Future Iterations

Potential extensions include item-specific AI follow-up, human-service handoff, and anonymous report sharing. Later category expansion could cover tablets and laptops, with adapted photography guidance, cosmetic standards, inspection items, and pricing rules.

AI would remain advisory for visible-condition assessment and explanations. Functional issues would continue to be reported by users and confirmed through professional inspection.
