# Detailed Overview — Chapter 4: **Randomizing**
**Source:** Rachel Glennerster and Kudzai Takavarasha, *Running Randomized Evaluations* (2013), Chapter 4, “Randomizing”

## Chapter purpose
This chapter explains how to introduce randomization into a program or policy evaluation in a way that is technically valid, operationally feasible, and ethically defensible. It moves from the broad question of **where opportunities to randomize come from** to the concrete question of **how to carry out random assignment in practice**, and ends with a catalog of field examples that illustrate different designs.

The chapter is organized into six modules:
1. Opportunities to Randomize
2. Choosing the Level of Randomization
3. Deciding Which Aspects of the Program to Randomize
4. The Mechanics of Simple Randomization
5. Stratified and Pairwise Randomization
6. A Catalog of Designs

---

## Module 4.1 — Opportunities to Randomize

### Core idea
A randomized evaluation requires the treatment group to have **greater exposure to the program** than the comparison group. The chapter identifies **three aspects of a program** that can be randomized:

- **Access**: who is offered the program
- **Timing of access**: when eligible units receive the program
- **Encouragement**: who gets extra inducement or help to participate

These can be randomized at the **individual** level or at a **group** level such as schools, villages, clinics, or communities.

### 1. Randomizing access
This is the most common approach. Some eligible units are randomly offered the program, while others serve as comparisons.

**Example used in the chapter:** If only 100 of 200 eligible schools can receive textbooks, randomly select 100 schools for the evaluation period, and use the other 100 as the comparison group.

### 2. Randomizing timing of access
When everyone will eventually receive the program but resources or logistics prevent simultaneous rollout, evaluators can randomize **who gets it first and who gets it later**.

**Example:** A deworming program in Kenya phases 75 schools into the intervention over three years. In year 1, one group is treated while the others remain comparisons; later groups are phased in over time.

### 3. Randomizing encouragement
When access itself cannot be restricted because the program is open to all, evaluators can randomize additional **information, nudges, incentives, or application support** designed to increase take-up.

**Example:** Eligible farming households can all open a savings account, but only a randomly selected subset receives outreach letters and assistance completing the paperwork.

### Common situations that create opportunities to randomize
The chapter identifies ten recurring settings where randomized evaluation is often feasible:

1. **New program design**
2. **New programs**
3. **New services**
4. **New people**
5. **New locations**
6. **Oversubscription**
7. **Undersubscription**
8. **Rotation**
9. **Admission cutoffs**
10. **Admission in phases**

### Key details on each opportunity

#### New program design
When implementers know there is a problem but have not yet settled on a solution, evaluators can help design and test alternatives from the outset.

#### New programs
Pilot programs are especially amenable to randomization because impacts are uncertain and random assignment is often viewed as a fair allocation mechanism.

#### New services
Existing programs may add components such as savings, insurance, financial literacy, or health modules. These additions can be randomly introduced.

#### New people / new locations
Program expansion often cannot cover all new people or places at once, making random allocation a fair way to determine who is served first.

#### Oversubscription
When demand exceeds supply, a lottery is often both practical and publicly defensible.

#### Undersubscription
If a program is open to all but take-up is low, randomized encouragement can identify the impact of increasing participation.

#### Rotation
When benefits or burdens must be shared over time because resources are fixed, groups can take turns under a randomized order.

#### Admission cutoffs
If eligibility depends on a score or threshold that is somewhat arbitrary at the margin, evaluators can randomize among applicants near the cutoff.

#### Admission in phases
When capacity grows over time, units can be randomly phased into the program.

### Module 4.1 takeaways
- The key design requirement is to create **differential exposure** between treatment and comparison groups.
- Not all programs can randomize access directly, but many can randomize **timing** or **encouragement**.
- Randomization often works best when resources are limited, rollout is gradual, or participation is incomplete.

---

## Module 4.2 — Choosing the Level of Randomization

### Core idea
Once evaluators know *what* can be randomized, they must choose the **unit of randomization**:
- individuals
- households
- schools
- clinics
- villages
- districts
- other clusters

The chapter emphasizes that the choice of level is not purely technical. It affects **measurement, spillovers, attrition, compliance, power, ethics, politics, logistics, and cost**.

### Individual-level vs group-level randomization
The chapter contrasts:
- **Individual-level randomization**: eligible individuals within a site are assigned to treatment or comparison
- **Group-level randomization**: whole villages, schools, or clinics are assigned as units

### Six main considerations

#### 1. Unit of measurement
The randomization level must be the same as, or higher than, the level at which outcomes are measured.

**Example:** If the outcome is firm profits, randomizing individual workers is not sufficient because profits are measured at the firm level.

#### 2. Spillovers
Programs can generate indirect effects beyond the directly treated units. Spillovers may be:
- **Physical** (e.g., reduced disease transmission)
- **Behavioral** (e.g., imitation)
- **Informational** (e.g., social learning)
- **Market-wide / general equilibrium** (e.g., displacement in labor markets)

The core validity issue is that outcomes for one unit should not depend on how surrounding units were assigned. Spillovers violate that condition.

##### Two design responses to spillovers
- **Limit spillovers to the comparison group** by randomizing at a higher level, such as school instead of classroom
- **Measure spillovers explicitly** by creating variation in exposure to treated neighbors or treated density

Examples discussed include:
- untreated students in treated schools
- untreated schools near treated schools
- designs with two levels of randomization to isolate spillover channels

#### 3. Attrition
Randomizing within a group can create resentment among untreated units who see neighbors benefiting. That can reduce cooperation with follow-up data collection. Group-level randomization may reduce visible unfairness and lower attrition risk.

#### 4. Compliance
Choosing the right level can improve adherence by:
- **program staff**, who may find some assignment schemes too confusing or unfair to implement properly
- **participants**, who may share treatment or otherwise undermine assignment

**Example:** In an iron supplementation study, treatment was assigned at the household level because household members might share pills and participants might struggle to track who should take what.

#### 5. Statistical power
All else equal, more randomized units mean more power. Randomizing clusters instead of individuals often sharply reduces effective sample size because outcomes within a cluster are correlated.

The rough rule highlighted in the chapter: **the number of randomized units matters more than the number of individuals interviewed**.

#### 6. Feasibility
Four feasibility dimensions matter:
- **Ethics**
- **Politics**
- **Logistics**
- **Cost**

### Ethics and consent
The chapter warns that individual-level randomization may create social tension if some nearby individuals receive large benefits while others do not. Group-level designs raise their own challenges around **informed consent**, especially when not every beneficiary is directly surveyed. Community meetings and community-level consent may be appropriate, but the correct approach depends on the IRB and study context.

### Politics and fairness
Allocation can appear arbitrary when equally needy people in close contact are assigned differently. Sometimes a technically ideal design is not politically acceptable, so evaluators must move to a higher-level randomization or modify the design.

### Reality check on units
Administrative units are not always socially meaningful. “Village,” “class,” or “community” boundaries may be fuzzy in practice. The chapter recommends using local knowledge, participatory methods, or alternative cluster definitions when needed.

### Module 4.2 takeaways
- The level of randomization is a design choice with major consequences.
- Higher-level randomization can help with spillovers, compliance, and fairness, but often reduces power and increases cost.
- Evaluators should match the randomization level to the program’s delivery mechanism, outcome measurement, and real social structure.

---

## Module 4.3 — Deciding Which Aspects of the Program to Randomize

### Core idea
This module maps the three randomizable aspects of programs—access, timing, and encouragement—onto concrete research designs. It focuses on five major strategies:

1. **Treatment lottery**
2. **Lottery around a cutoff**
3. **Phase-in design**
4. **Rotation design**
5. **Encouragement design**

It also introduces **hybrid multistage strategies**.

### 1. Treatment lottery

#### Design
Eligible units are randomly assigned to treatment or comparison, and that status remains fixed through the evaluation.

#### Best suited for
- oversubscribed programs
- pilots or limited-scale programs
- evaluations interested in **long-run impacts**

#### Advantages
- familiar and easy to explain
- often perceived as fair
- straightforward to implement
- preserves a comparison group over time

#### Disadvantages
- untreated units may attrit more because they know they will never receive the program
- politically harder when everyone expects eventual access

#### Ethical discussion
The chapter distinguishes two cases:

- **No change in the number of beneficiaries**: if limited resources mean some units would not have received the program anyway, a lottery may be ethically acceptable because it changes allocation, not total coverage.
- **Evaluation reduces short-run coverage**: then the ethical case depends on uncertainty about program benefits, possible harm, and the social value of learning.

The chapter also notes a medical-ethics analogy: if one treatment is clearly superior mid-trial, there may be an obligation to stop early. Social programs differ because resource scarcity often persists even after effectiveness is known.

### 2. Lottery around a cutoff

#### Design
Applicants are ranked by eligibility score, then randomization occurs around the margin rather than across all applicants.

#### Variants
1. **Lottery among the marginally ineligible**
2. **Lottery among the marginally eligible and marginally ineligible**
3. **Lottery among the qualified**

#### Key analytic implication
This design estimates effects for a **specific policy-relevant margin**, not always for the average participant.

#### Main design issues
- Does the design answer the policy question of interest?
- How wide should the score range around the cutoff be?
- How should fairness be balanced against statistical power?

A narrower band may look fairer, but it reduces sample size and power.

#### Ethical discussion
The central issue is whether it is acceptable to reallocate access away from people who score somewhat higher. The chapter argues that this depends heavily on uncertainty about the quality of the scoring system itself. If the cutoff is imperfect or poorly validated, learning about the margin can be highly valuable.

The chapter also explains **varying allocation fractions**: people closer to being clearly qualified can receive a higher probability of selection than those farther below the cutoff.

### 3. Phase-in design

#### Design
Everyone eventually receives the program, but the order of entry is randomized.

#### Best suited for
- programs that must reach everyone eventually
- settings with genuine logistical or budgetary rollout constraints
- situations where anticipation effects are unlikely or weak

#### Advantages
- politically and ethically appealing because nobody is permanently excluded
- can reduce attrition because later groups know they will be treated
- often matches real implementation constraints

#### Disadvantages
- the comparison group disappears once all groups are treated
- hard to estimate long-run effects
- anticipation of future treatment can bias behavior before receipt

#### Critical design condition
The time until the last phase-in must be long enough for treatment effects to emerge. If the program’s effects take longer to appear than the phase-in window, the evaluation may miss real impact.

### 4. Rotation design

#### Design
Groups take turns receiving the program. The treated group in one period becomes the comparison group later, and vice versa.

#### Best suited for
- settings where fixed resources must be shared over time
- programs whose effects are short-lived and do not persist after treatment ends
- questions about what happens **during exposure**, or about timing and seasonality

#### Advantages
- intuitive because rotation is common in real life
- can be useful for studying timing of exposure relative to natural seasons or institutional cycles

#### Disadvantages
- long-run pure comparisons usually do not exist
- anticipation effects can distort behavior
- lingering effects invalidate later comparisons

### 5. Encouragement design

#### Design
The program remains open to everyone, but a treatment group is randomly given extra encouragement to participate.

#### Best suited for
- undersubscribed programs
- situations where take-up is low because applications are costly, confusing, or effortful
- cases where a valid encouragement exists that shifts participation without directly changing outcomes

#### Key identification condition
The encouragement must satisfy the **exclusion restriction**:
it should affect the outcome **only by changing take-up of the program**, not through any independent channel.

#### Additional requirement
The encouragement should satisfy **monotonicity**:
it should not encourage some people and discourage others.

#### What this design estimates
The effect is identified for the group of people whose participation changes because of the encouragement—the **compliers** or marginal takers—not necessarily for everyone already in the program.

### Hybrid and multistage strategies
The chapter shows how combining designs can address more complex research questions.

#### Hybrids for spillovers
Use treatment lotteries and encouragement designs at multiple levels to generate variation in treatment density and identify social effects.

#### Hybrids for behavioral channels
A South African credit study combines random rate offers and later randomized loan terms to distinguish:
- **moral hazard**
- **adverse selection**

### Module 4.3 takeaways
- Different randomization strategies answer different causal questions.
- No single design is universally best; the right choice depends on access constraints, expected spillovers, time horizons, compliance, and ethics.
- The identification logic must match the policy question.

---

## Module 4.4 — The Mechanics of Simple Randomization

### Core idea
This module shifts from design logic to operational procedure. It explains what is required to perform random assignment and how to do it transparently.

### Five ingredients of random assignment
1. **A list of eligible units**
2. **The number of randomization cells**
3. **Allocation fractions**
4. **A randomization device**
5. **Initial data on eligible units** for stratification or balance checks

### Building the list of eligible units
The chapter discusses several ways to construct the eligible pool:

#### Existing administrative data
- local government records
- school registers
- other provider lists

#### Resource appraisals
- census-based needs assessments
- community participatory targeting
- “revealed need,” where timing is used to identify those who could not access services without support

#### Random sampling
Sometimes evaluators first draw a random sample from a wider population to create a representative study pool and improve external validity.

### Number of randomization cells
A basic impact evaluation usually has:
- **1 treatment cell**
- **1 comparison cell**

More complex studies may include:
- multiple treatment arms
- several phase-in cohorts
- designs intended to isolate mechanisms or compare versions of the intervention

### Allocation fractions
The simplest allocation is **50/50**, which often maximizes statistical power. But unequal allocations may be useful when:
- there are multiple treatment arms
- implementers need larger treatment groups
- designs around cutoffs use different probabilities

### Randomization devices

#### Mechanical devices
Examples:
- coin flips
- cards
- dice
- balls in containers
- drawing names from hats

**Advantages**
- familiar
- public
- transparent
- often perceived as fair

**Disadvantages**
- impractical for large samples
- vulnerable to physical failures or manipulation
- can generate imbalance if not mixed properly

#### Random number tables
Historically used, but largely replaced by computerized tools.

#### Computerized random number generators
Available in spreadsheets and statistical packages. The chapter specifically mentions Excel, Google Docs spreadsheets, and statistical software such as Stata.

### Steps in simple random assignment

#### Step 1: Order the eligible list randomly
Assign each unit a random number and sort by that number.

#### Step 2: Allocate units to groups
Once sorted, assign units to treatment/comparison groups based on blocks, intervals, or predetermined allocation rules.

#### Step 3: Randomly determine which group is treatment
This may be done at the end, especially when treatment arms are equal in size.

### Balance checks
After randomization, evaluators usually compare treatment and comparison groups on baseline variables to assess whether observable characteristics are balanced.

#### Why balance checks are reported
- to reassure readers that the randomization was credible
- to detect implementation problems
- to document that any imbalance is within what chance could produce

### Rerandomization
The chapter discusses, and largely discourages, rerandomizing repeatedly until acceptable balance is achieved.

#### Why it is discouraged
Because once evaluators reject “bad draws,” not every allocation remains equally likely. That complicates inference and can covertly impose constraints that are hard to reproduce analytically.

#### Recommended alternative
Use **stratified randomization** on a few key variables from the start.

### Module 4.4 takeaways
- Randomization is operationally simple, but only if procedures are documented clearly and executed consistently.
- Transparency, replicability, and predefined rules matter.
- Balance checking is useful, but rerandomizing to force balance is not ideal.

---

## Module 4.5 — Stratified and Pairwise Randomization

### Core idea
Simple randomization can produce imbalance by chance, especially with smaller samples. Stratified and pairwise randomization are ways to “help chance” create treatment and comparison groups that are balanced on important characteristics.

### Stratified random assignment

#### Procedure
1. Divide eligible units into **strata** based on chosen variables
2. Randomize within each stratum
3. Randomly assign cells to treatment or comparison status

#### Why stratify
- to achieve balance on key covariates
- to improve statistical power
- to support subgroup analysis
- to satisfy political or logistical constraints

### Which variables to stratify on

#### Discrete variables
These work naturally because units can be grouped into categories.

#### Continuous variables
They must first be converted into ranges or bins, such as:
- high vs low test scores
- deciles of income
- score bands

#### Strong predictors of the outcome
The chapter emphasizes prioritizing variables highly correlated with the final outcome. Baseline values of the main outcome are especially valuable.

#### Variables used for subgroup analysis
If the evaluation will report separate effects by gender, ethnicity, or region, stratifying on those variables helps ensure representation and power.

### How many variables to stratify on
The chapter stresses trade-offs:
- **stratum size**
- **practicability**
- **statistical power**

The practical guidance is to stratify on a **small number of high-value variables**, especially:
- baseline outcomes
- geography
- key subgroup indicators

### Pairwise randomization

#### Design
Units are matched into pairs based on important characteristics, then one is assigned to treatment and the other to comparison.

#### Advantages
- very strong balance
- especially useful with small samples
- particularly helpful in cluster-randomized studies with few clusters

#### Main drawback
Attrition becomes more problematic. If one unit in a pair is lost and analysis uses pair fixed effects, the pair can become analytically compromised.

The chapter therefore suggests:
- use **pairs** when randomization is at a stable group level with low attrition risk
- use **larger strata** when attrition risk exists at the unit of randomization

### Best practices summarized by the chapter
- report the randomization method clearly
- report variables used for stratification or balance
- explain how randomization was carried out in practice
- avoid rerandomization as a way to force balance
- stratify on baseline outcomes, geography, and subgroup variables
- consider power when deciding how many strata to create
- save seeds or code so the process is replicable
- ensure strata are large enough if attrition is possible

### Module 4.5 takeaways
- Stratification is usually preferable to post hoc rerandomization.
- Pairwise randomization is a powerful but sometimes fragile special case.
- Good randomization design anticipates both analysis and implementation realities.

---

## Module 4.6 — A Catalog of Designs

### Core idea
The final module illustrates the chapter’s design principles through real field studies. Each example identifies:
- the context
- the opportunity to randomize
- the level of randomization
- the randomization strategy used
- the causal questions enabled by the design

### Example 1: Treatment lottery among the eligible — Extra Teacher Program in Kenya
After Kenya abolished primary school fees, first-grade enrollment surged and class sizes exploded. Because only a limited number of extra teachers could be funded, schools were randomized at multiple stages into extra-teacher, tracking, and school-based-management conditions. This design isolated several causal channels at once.

### Example 2: Lottery among the marginally ineligible — Credit in the Philippines
A rural bank used credit scores to classify applicants. Those clearly below and above the threshold were rejected or accepted automatically, while those near the margin were randomized with score-dependent approval probabilities. This estimated the impact of expanding credit access near the cutoff.

### Example 3: Randomized phase-in — Primary School Deworming Project in Kenya
A school-based deworming intervention could not be rolled out everywhere at once. Schools were divided into three phase-in groups and treated over time. The design matched logistical constraints and also helped analyze spillovers.

### Example 4: Rotation — Remedial education in India
Pratham’s tutoring program expanded to new schools, but authorities wanted all eligible schools to benefit. Tutors were assigned to different grades in different years, then rotated. This allowed estimation of both one-year and two-year exposure effects.

### Example 5: Encouragement — Retirement savings at a large American university
Employees were eligible for retirement accounts, but take-up was low. Departments and individuals were randomized so some employees received a $20 inducement to attend a benefits fair. The design identified both direct and peer effects.

### Example 6: Instrument-like encouragement — Delayed marriage incentive in Bangladesh
Researchers could not randomize marriage age directly, so they randomized a modest family incentive intended to delay marriage. This illustrates how randomized encouragement can play the role of an instrumental variable.

### Example 7: Treatment density variation to measure spillovers — Job counseling in France
Employment agencies were randomized to different treatment densities, from 0% to 100%. This created variation in exposure to treated competitors and allowed the study of negative spillover or displacement effects.

---

## Cross-cutting themes across the chapter

### 1. Randomization is broader than lotteries for access
The chapter’s main conceptual move is to show that randomization is not limited to simple treatment/control lotteries. It can also be embedded in:
- rollout timing
- threshold rules
- incentives
- rotating access
- multistage designs
- treatment density

### 2. Design must fit implementation
The best design is the one that:
- matches how the program is delivered
- respects operational constraints
- preserves causal identification
- remains ethically and politically feasible

### 3. Spillovers are central, not peripheral
Indirect effects can either:
- invalidate a simple comparison, or
- become an object of study in their own right

### 4. Ethics are inseparable from design
Design choices must be evaluated in terms of:
- risk-benefit tradeoffs
- fairness
- consent
- community perceptions
- whether evaluation changes who benefits and when

### 5. Documentation and transparency matter
Randomization should be:
- prespecified
- replicable
- clearly reported
- understandable to both technical and nontechnical audiences

---

## Concise chapter summary
Chapter 4 is the operational heart of the book’s framework for randomized impact evaluation. It explains that evaluators do not merely “randomize treatment”; they design credible variation in exposure while working within real constraints. The chapter provides a toolkit for identifying opportunities to randomize, choosing the right unit, selecting the right design, implementing assignment transparently, improving balance through stratification, and adapting designs to field realities. Its examples show that randomized evaluations can answer not just whether a program works, but also **for whom**, **through what channel**, **under what conditions**, and **with what spillover effects**.
