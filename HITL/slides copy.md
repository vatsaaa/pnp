---
marp: true
theme: default
class: lead
paginate: true
---

# Human‑in‑the‑Loop is Not Enough
### The Persistent and Evolving Limits of Human Oversight in High‑Stakes AI

---

## About me

[**Ankur Vatsa**](mailto:ankur.vatsa@gmail.com)
**Experience, Expertise and Education:**
- Built SaaS-based regulatory reporting systems with ML-powered validation
- Led AI/ML adoption across 180+ applications at global investment banks  
- Specialist in AI-powered regulatory reporting, risk analytics, and compliance automation
- Expert in Human-AI collaboration patterns in high-stakes financial environments
- AWS Solutions Architect – Professional, with 17+ years in global investment banking technology
- M.Tech. in Artificial Intelligence and Machine Learning – BITS Pilani

<!--
Speaker notes:
- Establish strong credibility: 17+ years at top-tier investment banks (Wells Fargo, Nomura, RBS)
- Technical credentials: M.Tech in AI/ML, AWS Solutions Architect Professional
- Practical experience: Built actual AI systems for regulatory compliance and risk management
- Real-world HITL experience: Led teams implementing AI oversight in financial services
- This positions the speaker as uniquely qualified to discuss HITL limitations and solutions
-->

---

## What Attendees Will Walk Away With

- **Recognize** HITL failure modes across financial, healthcare, transportation, and scientific domains
- **Evaluate** whether current HITL implementations provide adequate safety margins
- **Design** layered defense systems using discriminator agents and automated safeguards
- **Implement** concrete monitoring metrics and audit trail requirements
- **Establish** governance structures that support reliable human-AI collaboration
- **Prioritize** remediation steps using risk-based frameworks for their specific domain

<!--
Speaker notes:
- These expanded learning outcomes reflect the full scope of both technical and organizational solutions
- Emphasize the cross-domain applicability—patterns are universal but manifestations differ
- Focus on actionable outcomes attendees can implement immediately in their organizations
- Governance is just as important as technical solutions—culture and incentives matter
-->

---

## Human‑in‑the‑Loop (HITL)

- **Common remedy** where intelligent systems hand over control to humans in several key scenarios:

| **Key scenario** | **Description** |
|---|---|
| **Errors and anomalies observed** | AI detects anomalies or unexpected outputs |
| | System confidence drops below threshold |
| | Error conditions trigger human intervention |
| **Low risk appetite** | High‑stakes decisions require human approval |
| | Regulatory compliance mandates human oversight |
| | Business‑critical processes need human validation |

- not just "humans reviewing AI outputs" — it's a structured handover mechanism designed to catch AI limitations before they cause harm.

<!--
Speaker notes:
- Define HITL clearly as a handover mechanism, not just "humans reviewing AI"
- Focus on the first two trigger categories: error detection and risk management
- Emphasize structured handover — this isn't ad hoc human involvement
- Set up expectation that HITL should provide comprehensive safety net
- Next slide completes the picture with domain expertise and legal requirements
-->

---

## Human‑in‑the‑Loop (Continued)

| **Key scenario** | **Description** |
|---|---|
| **Need for domain expertise** | Complex edge cases beyond AI training scope |
| | Nuanced judgment calls requiring contextual understanding |
| | Ethical considerations and value‑based decisions |
| **Legal/regulatory mandates** | Healthcare diagnostics requiring physician approval |
| | Financial lending decisions with fair lending requirements |
| | Criminal justice applications with due process rights |

- HITL offers defence to AI limitations; but faces issues — _speed, scale, bias, skillsgap_

<!--
Speaker notes:
- Human expertise 
- Complete the four trigger categories: domain expertise and legal/regulatory mandates
- Domain expertise: AI may lack context for complex edge cases or ethical nuance
- Legal/regulatory: Some domains explicitly require human decision‑makers
- "The Promise" sets up expectation that HITL should work as comprehensive safety net
- "Reality Check" transitions to next section showing why this promise fails in practice
- This sets up the five failure modes that follow
- Failure trigger category: speed, scale, bias, and skill gaps
-->

---

## The Case for Enhanced AI Oversight

- **$460M in 45 minutes**: Knight Capital flash crash (2012)
- **10,000 families wrongfully penalized**: Dutch childcare scandal
- **30% error miss rate**: Hospital audits of AI diagnostic reviews
- **95% false positive rate**: AML alert systems overwhelming investigators

HITL alone is insufficient for high‑stakes AI deployment.

<!--
Speaker notes:
- Lead with the dramatic statistics to grab attention
- Knight Capital: $460M lost in 45 minutes because humans couldn't react fast enough
- Dutch scandal: Automation bias led to wrongful penalties for 10,000 families
- Hospital study: Clinicians missed 30% of AI diagnostic errors due to overtrust
- Set up the problem: HITL isn't the silver bullet many assume it to be
-->

---

## Case Study: Dutch Childcare Scandal

**The System:**
- AI flagged 26,000 families for alleged childcare benefit fraud, human reviewers had to process hundreds of cases without thorough checks. 10,000 families wrongfully penalized, forced to repay thousands of euros

**All Five HITL Failure Modes in One System:**
- **Scale mismatch:** Reviewers couldn't properly assess the volume of cases
- **Overtrust:** Trusted AI fraud flags without sufficient scrutiny  
- **Coordination gaps:** Unclear escalation procedures and role definitions
- **Systematic bias:** AI unfairly targeted immigrant families and dual nationals
- **Skill erosion:** Caseworkers lost ability to properly evaluate complex cases

**Devastating Impact:** Families pushed into bankruptcy, relationships destroyed, government resignation

<!--
Speaker notes:
- This became a massive political scandal that brought down the Dutch government
- Perfect example of all five failure modes occurring simultaneously in one system
- Shows the importance of algorithmic accountability in public services
- Led to new AI governance requirements in European Union
- Complete remediation: system shutdown, manual case review, family compensation
- - This case study demonstrates why HITL alone is insufficient—need systematic safeguards
-->

---

## Five Failure Modes of HITL

1. **Speed Mismatch**: Microsecond AI vs. second‑scale humans _(Knight Capital: 45 minutes, $460M)_
2. **Scale Mismatch**: 10,000+ daily alerts vs. limited reviewers _(AML: 95% false positives)_
3. **Overtrust**: Automation bias hides critical errors _(Hospital study: 30% miss rate)_
4. **Skill Erosion**: "Out‑of‑the‑loop" degraded expertise _(Tesla Autopilot incidents)_
5. **Coordination Gaps**: Unclear handovers and protocols _(Dutch childcare: role confusion)_

<!--
Speaker notes:
- Each failure mode is paired with a real‑world example for impact
- Speed: Knight Capital lost $460M in 45 minutes—no human could intervene
- Scale: Banks process 10,000+ AML alerts daily with 95% false positive rates
- Overtrust: Hospital study showed clinicians missed 30% of AI diagnostic errors
- Skill erosion: Tesla Autopilot incidents where drivers weren't ready to take control
- Coordination: Dutch childcare scandal—unclear roles led to mass wrongful penalties
-->

---

## Systematic Patterns Across Domains

**Pattern 1: Cognitive Load Management**
- Information overload leads to satisficing behavior ("good enough" decisions)
- Structured output creates false sense of validation and trustworthiness

**Pattern 2: Trust Miscalibration**  
- Over-reliance on confident AI outputs despite known limitations
- Under-appreciation of edge case risks and failure modes

**Pattern 3: Organizational Pressures**
- Cost reduction prioritized over safety margins and thorough review
- Inadequate training and support for human reviewers
- Alert fatigue from >90% false positive rates in AML systems

<!--
Speaker notes:
- These patterns appear across all domains discussed in this presentation
- Cognitive load: humans default to "good enough" when overwhelmed
- Trust miscalibration: neither blind trust nor complete skepticism is optimal
- Organizational pressures often undermine HITL effectiveness
- Understanding these patterns helps design better interventions
- Alert fatigue is particularly problematic—when 90%+ alerts are false, humans stop paying attention
-->

---

## Comprehensive Risk Assessment

| **Risk Category** | **Financial** | **Healthcare** | **Transportation** | **Scientific** |
|---|---|---|---|---|
| **Speed Mismatch** | Flash crashes | Emergency decisions | Split-second reactions | Submission deadlines |
| **Scale Mismatch** | Thousands of alerts | Patient overload | Fleet monitoring | Volume of papers |
| **Overtrust** | Structured reports | Confident diagnoses | Automation reliance | AI-generated content |
| **Skill Erosion** | Analyst capabilities | Clinical judgment | Driver readiness | Research skills |
| **Coordination** | Role confusion | Handoff protocols | Mode transitions | Review processes |

**Cross-cutting impacts:** Regulatory non-compliance, safety incidents, financial losses, reputation damage

<!--
Speaker notes:
- This table shows how the five failure modes manifest differently across domains
- But the underlying patterns are remarkably consistent
- This analysis can help attendees identify risks in their own domains
- Cross-cutting impacts affect all sectors—no one is immune
- Financial: $460M losses, healthcare: patient safety, transportation: fatalities, scientific: knowledge integrity
-->

---

## Financial Services: When Structure Deceives

**The Problem:**
- AI extracts regulatory requirements from EMIR, MiFID, CFTC rules
- **Hallucination risk**: LLMs invent non‑existent field requirements
- **False confidence**: Well‑formatted JSON output appears trustworthy
- **Scale challenge**: Hundreds of fields vs. limited compliance staff

**Real Impact:**
- Potential fines: >$50M for insufficient swap reporting
- Deutsche Bank: $150M AML penalty for ongoing failures

<!--
Speaker notes:
- Focus on the deception: structured output (JSON/tables) looks authoritative but can be wrong
- Regulatory extraction is a perfect storm: complex rules + high stakes + volume
- Real penalties: Deutsche Bank $150M, potential CFTC fines >$50M
- The formatted output creates false confidence—humans trust neat tables
- Mention the Dutch childcare example briefly as an anecdote about overtrust and scale
- Emphasize audit trails and explainability for regulatory inspections
-->

---

## Healthcare: Life‑or‑Death Automation Bias

**The Evidence:**
- Hospital audits: Clinicians miss **30% of AI diagnostic errors**
- Emergency departments: Time pressure prevents thorough AI output validation
- Training gaps: Physicians lack awareness of AI system limitations

**Why HITL Fails:**
- **Automation bias**: Trusting confident AI assessments of "normal" results
- **Mode confusion**: Unclear guidance on when to override AI recommendations
- **Workload pressure**: No time for careful review during patient surges

<!--
Speaker notes:
- 30% error miss rate is catastrophic in healthcare—that's life‑or‑death territory
- Automation bias: when AI says "normal," clinicians often don't look closer
- Emergency departments are pressure cookers—no time for careful validation
- Mode confusion: doctors don't know when to trust vs. question AI
- Stress patient-safety focus. Cite need for prospective trials, not just retrospective validation.
- Note privacy constraints and medico-legal implications.
-->

---

## Transportation: Split‑Second Decisions

**NHTSA Findings (2023):**
- Multiple fatal Tesla Autopilot incidents
- Drivers had **seconds** to react, weren't ready to take control
- "Out‑of‑the‑loop" problem: Skill erosion from over‑reliance

**The Core Issue:**
- AI operates in **milliseconds**
- Human reaction time: **1‑3 seconds**  
- Handover complexity: Mode awareness, situational context, skill maintenance

<!--
Speaker notes:
- NHTSA investigations documented multiple fatal incidents
- The timing mismatch is fundamental: AI acts in milliseconds, humans need seconds
- "Out‑of‑the‑loop" problem: when drivers rely on automation, they lose situational awareness
- Quick scenario example: unexpected road debris — who intervenes and when?
- Mention simulation-to-real validation as cost-effective before fleet testing
- This isn't just about autonomous vehicles—it applies to any human‑AI handover scenario
-->

---

## Scientific Publishing: When AI Writes Science

**The Growing Risk:**
- AI-generated research content without proper disclosure
- **Citation hallucinations**: Non-existent references making it through peer review
- **Nonsensical terminology**: "Vegetative electron microscopy" and other fabricated terms

**Why HITL Fails:**
- **Peer review limitations**: Reviewers can't verify every citation or detect subtle AI generation
- **Volume challenge**: Editorial teams overwhelmed by AI-assisted submissions  
- **Academic integrity crisis**: Fake citations undermine scientific credibility

**Real Impact:**
- [Delft University study](https://www.nature.com/articles/d41586-024-00762-8): Widespread "junk science" with hallucinated citations
- Trust erosion in scientific literature and research findings

<!--
Speaker notes:
- This is an emerging but critical domain as AI becomes widespread in research
- Citation hallucination is particularly dangerous—creates false knowledge
- Publishers like Nature and Science are struggling with disclosure policies
- Reviewers need new tools and training to detect AI assistance
- Unlike other domains, the impact here is on the integrity of human knowledge itself
-->

---

## Solutions: Beyond Traditional HITL

**The Strategy: Layered Defense Systems**
- **Prevention**: Stop problems before they occur (circuit breakers, input validation)
- **Detection**: Catch problems quickly (discriminator agents, monitoring)
- **Response**: Handle problems effectively (escalation, audit trails)

**Core Principles:**
- No single point of failure
- Automated safeguards scale better than human reviewers
- Measurable outcomes enable continuous improvement
- Governance structures ensure accountability

**Implementation Categories:**
- Technical safeguards (next slides)
- Organizational changes (governance)
- Systematic monitoring and measurement

<!--
Speaker notes:
- This bridges from problem analysis to solution implementation
- Layered defense: multiple independent safeguards, not just HITL
- Prevention is better than detection, detection better than response
- Automation scales where human review cannot
- This sets up the detailed implementation patterns that follow
-->

---

## Technical Safeguards: Prevention Layer

**Automated Circuit Breakers:**
- Financial: Trading halts when anomalies detected (<1 second response)
- Healthcare: Confidence‑based escalation to senior clinicians
- Regulatory: Stop processing when hallucination rate exceeds threshold

**Input Validation:**
- Schema validation for structured data
- Content filtering for obvious hallucinations
- Source verification for regulatory documents

**Ensemble Model Validation:**
- Multiple independent models must agree on high-stakes decisions
- Disagreement triggers human review
- Reduces single-model bias and hallucination risk

<!--
Speaker notes:
- Prevention layer stops problems before they impact decisions
- Circuit breakers act faster than humans can react
- Input validation catches obvious problems early
- Ensemble validation provides redundancy - if models disagree, escalate
- Focus on automation because humans can't match the speed and scale needed
-->

---

## Technical Safeguards: Detection Layer

**Discriminator Agents: Automated Validation**
- Specialized AI systems that detect errors, hallucinations, or inconsistencies
- Architecture: `Source → Primary AI → Discriminator AI → Flagged Items → Human Review`
- Types: Binary classifiers, consistency checkers, adversarial critics, provenance verifiers

**Continuous Monitoring Metrics:**
- **Model drift**: Alert if accuracy drops >5% from baseline
- **Human interception**: Warn if <80% error catch rate  
- **Confidence escalation**: Review if AI confidence <70% on critical outputs
- **Anomaly rate**: Flag if >10% of outputs marked unusual in 24h

<!--
Speaker notes:
- Detection layer catches problems that slip through prevention
- Discriminator agents provide "automated peer review" - scales human attention
- Architecture shows the flow: primary AI generates, discriminator validates, humans focus on flagged items
- Monitoring metrics provide early warning of degrading performance
- These are concrete, measurable thresholds organizations can implement today
-->

---

## Technical Safeguards: Response Layer

**UI Design for Trust Calibration:**
- Show confidence scores and uncertainty ranges
- Highlight source material for AI conclusions
- Force deliberation on high‑risk overrides
- Provide "second opinion" views from ensemble models

**Escalation Procedures:**
- Clear handoff protocols when AI confidence drops
- Defined roles: who reviews what types of flagged outputs
- Time-bound response requirements for different risk levels

**Audit Trail Capture:**
- Complete decision lineage from input to final outcome
- AI confidence scores and reasoning paths
- Human reviewer actions and rationale
- Discriminator agent findings and flags

<!--
Speaker notes:
- Response layer handles problems when they occur
- UI design is critical for trust calibration—enables humans to make better decisions
- Show confidence, don't hide uncertainty, make overrides deliberate not accidental
- Escalation procedures prevent coordination gaps - clear roles and timing
- Audit trails enable learning from failures and regulatory compliance
-->

---

## Beyond Technical Solutions: Governance Changes

**Organizational Structure:**
- Define clear roles: Model Owner, Data Steward, Risk Committee
- Establish Red Team functions for ongoing adversarial testing
- Create escalation paths and incident response procedures

**Process Controls:**
- Mandatory model cards and data sheets for transparency
- Staged rollout procedures with defined success criteria  
- Regular third-party audits and compliance reporting

**Training and Culture:**
- Education programs on automation bias and AI limitations
- Simulation exercises for crisis scenarios
- Incentive alignment: reward finding errors, not just efficiency

<!--
Speaker notes:
- Technical solutions alone are insufficient—need organizational change
- Model owners must be accountable for ongoing performance monitoring
- Red teams actively try to break systems to find vulnerabilities before bad actors do
- Training is crucial—humans need to understand AI limitations and their own biases
- Incentives matter—reward people for finding problems, not just being efficient
- Many failures stem from organizational pressures that undermine technical safeguards
-->

---

## An Implementation Roadmap

**Phase 1: Foundation (0‑3 months)**
✓ Establish baselines with benchmark datasets  
✓ Implement structured logging and audit trails  
✓ Define concrete alerting thresholds  

**Phase 2: Detection (3‑6 months)**  
✓ Deploy continuous drift monitoring  
✓ Add discriminator agents for high‑risk outputs  
✓ Start measuring human interception rates  

**Phase 3: Prevention (6‑12 months)**
✓ Implement automated circuit breakers  
✓ Add ensemble validation for critical decisions  
✓ Establish incident response playbooks

<!--
Speaker notes:
- This is a practical 12‑month implementation timeline
- Phase 1: Cannot monitor what isn't measured—start with baselines
- Phase 2: Add the safety nets—monitoring and discriminators catch problems
- Phase 3: Prevention—circuit breakers and ensembles stop problems before they happen
- Attendees should identify current organizational position and plan next 30‑day sprint
-->

---

## The Foundation of Accountability

**Audit Trails Are Critical:**
- **Regulatory compliance**: Prove decisions were made properly during audits
- **Incident investigation**: Trace back through decision chain when things go wrong
- **Continuous improvement**: Identify patterns in human-AI collaboration failures

**Capture:**
- Complete decision lineage from input to final outcome
- AI confidence scores and reasoning
- Human reviewer actions and rationale
- Discriminator agent findings and flags

**The Business Case:**
- Avoid regulatory fines through demonstrated compliance
- Reduce investigation time from weeks to hours
- Enable systematic learning from failures

<!--
Speaker notes:
- Position audit trails as business necessity, not just technical requirement
- Regulatory compliance is often the primary driver for implementation
- Investigation speed matters: from weeks of manual reconstruction to hours of log analysis
- Learning from failures is how organizations improve their HITL processes over time
- This sets up the technical schema that follows
-->

---

## Audit Trail Technical Schema

**Complete Decision Record:**
```json
{
  "event_id": "uuid",
  "timestamp": "2025-09-02T10:00:00Z",
  "input": {"source": "doc123", "content_hash": "abc789"},
  "ai_output": {"model": "v1.2", "prediction": "...", "confidence": 0.85},
  "discriminator": {"model": "discA", "flag": true, "reason": "inconsistency"},
  "human_review": {"reviewer": "user456", "action": "approve", "notes": "..."},
  "outcome": {"final": "approved", "error_detected": false}
}
```

**Implementation Requirements:**
- **Immutable storage**: Cannot be deleted or modified after creation
- **Retention policies**: 7+ years for financial, 10+ years for healthcare
- **Audit access**: Readable by regulators with proper permissions
- **Performance**: Sub-second query for incident investigation

<!--
Speaker notes:
- Each field and its importance for compliance and debugging should be explained
- Immutable storage: critical for regulatory credibility—no tampering possible
- Retention policies: vary by regulation—financial services typically 7 years, healthcare longer
- This schema captures the full decision flow: input → AI → discriminator → human → outcome
- Performance matters: during incidents, need fast access to decision history
- Content hash ensures input document integrity—proves what the AI actually processed
-->

**Key Requirements:**
- Immutable storage for regulatory compliance
- Accessible to auditors with proper retention policies  
- Captures full decision lineage for post‑incident analysis

<!--
Speaker notes:
- Each field and its importance for compliance and debugging should be explained
- Immutable storage: can't delete or modify logs after creation
- Retention policies: how long to keep logs varies by regulation and use case
- This schema captures the full decision flow: input → AI → discriminator → human → outcome
-->

---

## Summary and Conclusions

**HITL is necessary but not sufficient**

**The evidence across domains:**
- Knight Capital: $460M in 45 minutes (speed mismatch)
- Dutch childcare: 10,000 families wrongfully penalized (all five failure modes)
- Hospital study: 30% diagnostic error miss rate (overtrust)
- Scientific publishing: Citation hallucination undermining research integrity

**The solution:**
Layered defenses combining technical safeguards, governance changes, and systematic monitoring

**Next steps:**
Start with benchmarks and baseline measurements—systems cannot be improved without measurement

<!--
Speaker notes:
- Close with the core message: HITL is necessary but not sufficient  
- Repeat the key evidence from multiple domains—these aren't hypothetical risks
- Dutch childcare scandal shows all five failure modes can occur simultaneously
- Scientific publishing represents emerging risk to knowledge integrity
- End with a concrete next step: measurement comes before improvement
- Offer to share resources and templates for implementation
-->