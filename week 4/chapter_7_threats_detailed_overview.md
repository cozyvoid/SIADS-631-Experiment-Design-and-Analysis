# Detailed Overview of Chapter 7: Threats to Randomized Evaluations

**Source:** *Running Randomized Evaluations: A Practical Guide* — Chapter 7, “Threats”  
**Authors:** Rachel Glennerster and Kudzai Takavarasha

## Chapter Purpose

Chapter 7 explains that even a well-designed randomized evaluation can be undermined when implementation and data collection do not proceed as planned. The chapter focuses on **four common threats to the integrity of experiments** and shows how each threat can distort causal inference, weaken statistical power, or reduce the credibility of findings.

The four modules in the chapter are:

1. **Module 7.1: Partial Compliance**
2. **Module 7.2: Attrition**
3. **Module 7.3: Spillovers**
4. **Module 7.4: Evaluation-Driven Effects**

---

## Core Theme of the Chapter

A randomized design establishes how a study *should* work in theory. In practice, however, participants, staff, and surrounding conditions often interfere with the original plan. The chapter emphasizes that threats matter because they can:

- reduce the difference in exposure between treatment and comparison groups,
- weaken comparability between groups,
- bias impact estimates,
- reduce statistical power, and
- limit generalizability.

The chapter’s central lesson is that researchers must **anticipate threats at the design stage**, **monitor them during implementation**, and **account for them in analysis whenever possible**.

---

# Module 7.1: Partial Compliance

## Main Idea

**Partial compliance** occurs when participants do not receive the treatment exactly as assigned in the protocol. This includes both failures to deliver treatment to the treatment group and unintended exposure to the treatment in the comparison group.

## What Partial Compliance Looks Like

### 1. Treatment-group members do not receive treatment
Examples include:
- students assigned to training who never attend,
- parents who refuse consent for child deworming,
- logistical barriers such as impassable roads preventing fertilizer delivery.

### 2. Treatment-group members do not complete treatment
Examples include:
- students dropping out of a training program after a few sessions,
- farmers saving or selling fertilizer instead of using it as intended.

### 3. Comparison-group members receive treatment
This can happen when:
- they were already receiving similar services,
- they move into treated locations,
- outside organizations deliver similar services to comparison units.

### 4. Implementation staff depart from protocol
Staff may:
- ignore random assignment,
- selectively provide services based on perceived need,
- alter the treatment itself,
- compensate comparison participants in unplanned ways.

### 5. Defiers react in the opposite direction
A rare but especially serious case occurs when encouragement actually reduces take-up for some people. These participants are called **defiers**.

## Why Partial Compliance Is a Threat

### A. It narrows treatment contrast
If treatment and comparison groups end up with similar exposure rates, the experiment loses the contrast needed to estimate causal effects.

### B. It reduces group comparability
If staff introduce other systematic differences between groups, then the program is no longer the only difference driving outcomes.

### C. Defiers can invalidate interpretation
In encouragement designs, defiers can make it impossible to recover the true treatment effect using standard assumptions. The chapter’s example shows how ignoring defiers can generate a treatment-effect estimate that is almost **double the true effect**.

## How to Limit Partial Compliance

### 1. Make take-up easy
Reduce procedural and logistical barriers so participants can actually access the program.

### 2. Incentivize take-up
Small incentives can meaningfully increase participation without materially changing final outcomes.

### 3. Compartmentalize and routinize field tasks
Assign staff to specific program versions so they do not make treatment decisions ad hoc in the field.

### 4. Randomize at a higher level
Cluster randomization can reduce contamination when people interact closely.

### 5. Give everyone a basic program
Sometimes all participants receive a base intervention and only the treatment group receives an enhanced version. This can ease implementation, though it changes what can be estimated.

## How to Document Compliance

### Track who received what and when
Researchers should combine:
- **monitoring data during implementation**, and
- **endline survey questions** asked consistently of both treatment and comparison groups.

### Identify likely defiers
The chapter recommends using theory of change and baseline data to identify people who may respond perversely to encouragement.

## Key Takeaway from Module 7.1

Partial compliance is not just a nuisance. It can weaken the treatment-control contrast, contaminate the counterfactual, and in some cases fundamentally distort causal interpretation. Prevention, monitoring, and symmetric measurement across groups are essential.

---

# Module 7.2: Attrition

## Main Idea

**Attrition** occurs when researchers cannot measure outcomes for some study participants. This creates a missing-data problem.

## Types of Attrition

### 1. Participants drop out and cannot be measured
Examples:
- death,
- migration,
- withdrawal of cooperation.

### 2. Participants remain in the program but are not measured
Examples:
- not being home during follow-up,
- missing school on testing day,
- refusing interviews.

### 3. Participants refuse some questions
Examples:
- nonresponse on sensitive behaviors,
- refusal to report earnings or illegal activity,
- survey fatigue due to long instruments.

## Why Attrition Is a Threat

### A. It can destroy comparability
If attrition rates differ between treatment and comparison groups, or if different *types* of participants disappear from each group, the remaining samples are no longer comparable.

The chapter gives two especially important scenarios:

- **Differential attrition rates:** low-achieving students remain in the treatment group but drop out in the comparison group, making the treatment group look worse than it really is.
- **Different types of attrition with equal rates:** even when the number lost is equal in both groups, the estimate is biased if different kinds of people are lost from each group.

### B. It reduces statistical power
Because attrition shrinks the observed sample size, it makes it harder to detect true effects.

## Visual Examples in the Chapter

The figures on **pages 6–7** illustrate how attrition can reverse the apparent program effect:

- **Figure 7.1** shows how **different attrition rates** can make a helpful remedial education program appear harmful.
- **Figure 7.2** shows that even when attrition rates are the same, **losing different kinds of participants** in each group can still bias the estimate.

These diagrams reinforce the chapter’s main point: missing data are dangerous not merely because there is less data, but because the missingness can alter the composition of the groups being compared.

## How to Limit Attrition

### 1. Use a design that promises future access
Phase-in designs can reduce refusal by making participants expect future treatment, though they may introduce anticipation effects.

### 2. Change the level of randomization
Assigning treatment at a higher social level can reduce resentment from being untreated while neighbors are treated.

### 3. Improve data collection systems

#### Pilot instruments and procedures
Poor survey design, confusing skip patterns, inappropriate interviewer-respondent pairings, and overly long instruments can all increase attrition.

#### Follow everyone originally randomized
Track participants wherever they go rather than only measuring those who remain in place.

#### Do not wait too long to follow up
Longer gaps between survey rounds increase the chance of migration, death, and lost contact information.

#### Collect tracking information at baseline
Useful tracking variables include:
- expected migration,
- destination information,
- cell phone numbers,
- contact details for relatives or friends.

#### Use participatory tracking when needed
Peers and classmates can help locate participants who moved.

#### Time surveys strategically
Survey timing during the day or year can matter substantially. Avoid predictable absence periods, or use holiday return windows when trying to locate migrants.

#### Intensively track a subsample of attriters
If full tracking is too expensive, carefully follow a random sample of attriters and use that information to assess sensitivity to missing data.

#### Provide incentives
Small compensation can help encourage completion of long or difficult follow-up surveys.

## Key Takeaway from Module 7.2

Attrition threatens both **internal validity** and **precision**. It is especially dangerous when loss to follow-up is systematic or differs by group. Good tracking, careful instrument design, and proactive follow-up are central to credible evaluation.

---

# Module 7.3: Spillovers

## Main Idea

**Spillovers** are indirect effects of the program on people who were not directly treated. These are also called externalities.

## Types of Spillovers

The chapter identifies several channels:

### 1. Physical spillovers
Example: immunized children reduce disease transmission in the wider community.

### 2. Behavioral spillovers
Example: untreated farmers imitate fertilizer techniques learned by treated neighbors.

### 3. Informational spillovers
Example: people learn from others about bed nets or preventive health products.

### 4. Marketwide or general equilibrium effects
Example: subsidies for hiring one group reduce employment for another group.

## Why Spillovers Matter

Spillovers are common and often important for real-world policy. The chapter stresses that researchers should not treat them as rare anomalies.

## Why Spillovers Are a Threat

### A. They weaken the counterfactual
If comparison-group members benefit from or are harmed by nearby treatment, then their outcomes do not represent what would have happened in the complete absence of the program.

### B. They bias estimated impacts when unaccounted for
- **Positive spillovers** to the comparison group lead to **underestimation** of the program’s effect.
- **Negative spillovers** to the comparison group lead to **overestimation**.

The deworming example makes this concrete: if untreated children in the same school benefit from reduced transmission, then within-school individual randomization understates the effect of treatment.

## How to Manage Spillovers

### 1. Identify possible spillovers early
The chapter recommends asking:
- **What** is spilling over?
- **From whom to whom**?
- **How** does it spread?
- Is it **positive or negative**?

### 2. Reduce spillovers through design
Choose a level of randomization that matches likely pathways of interaction:
- classroom vs. school,
- business vs. market,
- individual vs. village.

### 3. Measure spillovers explicitly
Collect outcome data for untreated people who are likely to be indirectly affected, such as:
- neighbors,
- spouses,
- non-targeted community members.

## Key Takeaway from Module 7.3

Spillovers are not only a threat to clean estimation; they are also substantively important policy effects. Good design should either minimize them or deliberately measure them.

---

# Module 7.4: Evaluation-Driven Effects

## Main Idea

The process of being in an evaluation can itself change behavior, independently of the treatment. These are **evaluation-driven effects**.

## Six Forms of Evaluation-Driven Effects

### 1. Hawthorne effects
The treatment group works harder simply because it is being observed or feels specially chosen.

### 2. John Henry effects
The comparison group competes harder because it knows it is being compared to the treatment group.

### 3. Resentment and demoralization effects
The comparison group becomes discouraged or resentful for not receiving treatment.

### 4. Demand effects
Participants try to behave in ways they think align with what researchers want to see.

### 5. Anticipation effects
The comparison group changes behavior because it expects to receive the treatment later.

### 6. Survey effects
Being frequently surveyed changes later behavior.

## Detailed Logic of Each Effect

### Hawthorne effects
Participants may increase effort because they feel lucky, selected, or watched.

### John Henry effects
Comparison participants may temporarily overperform to defend their status or jobs, which can make the treatment appear less effective than it really is.

### Resentment/demoralization
Untreated participants may do worse because they are discouraged, making the treatment appear more effective than it really is.

### Demand effects
Participants infer the study’s purpose and consciously or unconsciously adjust behavior.

### Anticipation effects
Participants expecting later treatment may alter current decisions, such as borrowing or delaying investment.

### Survey effects
Repeated questioning can itself act as a reminder or intervention. The chapter cites a Kenya water-treatment study in which frequent surveys increased use of purification products.

## Why Evaluation-Driven Effects Are a Threat

### A. They can reduce power and generalizability
If both groups change behavior due to survey frequency or observation, treatment effects may become harder to detect or may no longer generalize to real implementation settings.

### B. They can reduce comparability
If the induced behavior affects only one group, the estimated impact becomes biased because the comparison is no longer fair.

### C. They can bias estimates in different directions
- Hawthorne and demoralization effects can **inflate** estimated impacts.
- John Henry effects can **deflate** them.
- Anticipation effects can go either way.

## How to Limit Evaluation-Driven Effects

### 1. Identify interactions that exist only because of the evaluation
Researchers should map how the evaluation changes incentives, observation, and contact patterns.

### 2. Change the level of randomization
Reducing direct interaction between treatment and comparison participants can reduce demoralization, anticipation, and competition.

### 3. Do not announce phase-in plans when appropriate
This can reduce anticipation effects, though it introduces ethical and practical trade-offs.

### 4. Keep implementation staff impartial
Staff should not feel their employment or program survival depends on a positive result.

### 5. Ensure equivalent evaluator interaction across groups
Treatment and comparison groups should experience the same survey procedures, enumerators, timing, and intensity of contact, apart from actual treatment access.

### 6. Measure evaluation effects experimentally
Researchers can randomize evaluation procedures themselves, such as survey frequency, to estimate how much the evaluation changes behavior.

## Key Takeaway from Module 7.4

Evaluations are not passive measurement devices. They can shape behavior directly. A strong evaluation design therefore accounts not only for treatment effects, but also for the effects of observation, comparison, expectation, and repeated measurement.

---

# Cross-Cutting Lessons Across the Chapter

## 1. Threats often begin in implementation, not only in analysis
A randomized design does not guarantee valid estimates if treatment delivery, participant behavior, or measurement procedures drift from plan.

## 2. Symmetry matters
Whenever possible, treatment and comparison groups should be monitored and measured in equivalent ways.

## 3. Design choices are trade-offs
Many solutions introduce new risks:
- phase-in designs can reduce attrition but create anticipation effects,
- higher-level randomization can reduce contamination but may reduce power,
- incentives can improve compliance and retention but must be small enough not to become treatments themselves.

## 4. Monitoring is as important as randomization
Researchers need routine process data, strong tracking systems, and endline measures that capture actual exposure and missingness.

## 5. Some “threats” are also substantively meaningful effects
Spillovers and survey effects may be threats to clean estimation, but they may also reveal how programs function in real social settings.

---

# Concise Study Guide Summary

## Module 7.1: Partial Compliance
- Assigned treatment is not delivered or comparison participants receive treatment.
- Main risks: weaker treatment contrast, reduced comparability, problems with defiers.
- Main responses: simplify take-up, incentivize participation, structure staff roles, randomize at higher levels, track compliance carefully.

## Module 7.2: Attrition
- Outcomes are missing for some participants.
- Main risks: biased comparisons and lower statistical power.
- Main responses: strong tracking, shorter follow-up gaps, better survey design, incentives, and careful timing.

## Module 7.3: Spillovers
- Untreated people are indirectly affected by treatment.
- Main risks: contaminated counterfactual and biased impact estimates.
- Main responses: anticipate spillover pathways, randomize at appropriate levels, and measure indirect effects directly.

## Module 7.4: Evaluation-Driven Effects
- People change behavior because they are being evaluated.
- Main risks: reduced generalizability, undermined comparability, biased estimates.
- Main responses: equalize evaluator contact, manage expectations, adjust randomization level, and experimentally test evaluation procedures when needed.

---

# Why This Chapter Matters

Chapter 7 is practically important because it shifts attention from **ideal experimental logic** to **real-world experimental fragility**. It teaches that valid causal inference depends not only on random assignment, but also on maintaining treatment integrity, measuring outcomes consistently, anticipating social interactions, and recognizing that evaluation itself can shape behavior.

In that sense, the chapter functions as a bridge between:
- **designing randomized evaluations**, and
- **implementing them credibly in field settings**.

---

# Citation

Glennerster, Rachel, and Kudzai Takavarasha. *Running Randomized Evaluations: A Practical Guide*. Princeton University Press, 2013. Chapter 7: “Threats.”
