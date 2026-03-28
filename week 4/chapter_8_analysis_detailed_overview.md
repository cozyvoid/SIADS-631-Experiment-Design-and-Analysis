# Detailed Overview of Chapter 8: Analysis

**Source:** *Running Randomized Evaluations: A Practical Guide* — Chapter 8, “Analysis”  
**Authors:** Rachel Glennerster and Kudzai Takavarasha

## Chapter Purpose

Chapter 8 explains how to analyze data from randomized evaluations and draw valid inferences about program impact. It begins with the **basic intention-to-treat framework**, then moves to a **catalog of corrections** needed when the experiment faces complications such as noncompliance, attrition, spillovers, clustered randomization, stratification, and multiple outcomes. It ends with a discussion of **pre-analysis plans (PAPs)** as a safeguard against data mining and selective reporting.

The chapter is organized into three modules:

1. **Module 8.1: Basic Intention-to-Treat Analysis**
2. **Module 8.2: Catalog of Corrections**
3. **Module 8.3: Pre-analysis Plans**

---

## Big Picture

The chapter’s central message is that randomized evaluations are analytically strongest when researchers begin with a simple comparison of randomized groups, but **credible inference often requires adjustments** once real-world complications enter the design. The authors emphasize that good analysis is not just running regressions. It also includes:

- careful data cleaning,
- checking attrition and compliance,
- understanding treatment assignment,
- matching estimation strategy to design,
- correcting standard errors where needed,
- protecting inference when many outcomes or subgroups are examined, and
- specifying analysis decisions in advance when possible.

---

# Module 8.1: Basic Intention-to-Treat Analysis

## Main Idea

The first step in analyzing any randomized evaluation is the **intention-to-treat (ITT)** analysis. ITT compares outcomes by **assigned treatment status**, not by actual take-up. It asks: *What is the effect of being assigned access to the program?*

The chapter stresses that **ITT should always be reported**, even when researchers later estimate effects on compliers or use more complex corrections.

---

## Before Analysis: Data Preparation

Before any formal analysis, the chapter recommends several preparatory steps.

### 1. Correct obvious errors
Researchers should identify impossible or inconsistent values, such as:
- negative farm size,
- biologically impossible heights,
- contradictory responses across survey items,
- broken skip patterns.

The authors stress that corrections should be cautious. Researchers should avoid “overcleaning” by forcing data to fit prior expectations.

### 2. Check for outliers
Outliers should be identified early because later robustness checks may compare results with and without those observations. The default is **not** to drop them automatically.

### 3. Calculate attrition rates
High attrition may require sensitivity analysis or additional fieldwork. Attrition is not only a field problem but also an analytical one.

### 4. Calculate compliance rates
Because take-up may differ from assignment, compliance patterns help determine whether ITT alone is enough or whether further analysis, such as complier estimation, is needed.

### 5. Plot and describe the data
The chapter recommends using summary statistics and visualizations to understand distributions, detect outliers, and sometimes illustrate treatment effects more persuasively than a regression table.

---

## What the ITT Estimate Is

The ITT estimate compares mean outcomes for:
- those **assigned to treatment**, and
- those **assigned to comparison/control**.

The chapter gives a Ghana scholarship example. If average monthly income is:
- **$45** for those assigned scholarships, and
- **$30** for those not assigned scholarships,

then the ITT estimate is **$15 per month**.

This can be estimated either by:
- a **difference in means / t-test**, or
- a **regression with a treatment indicator**.

Conceptually, these are equivalent in a simple randomized design.

---

## What ITT Measures

A critical conceptual point in the chapter is that ITT measures the effect of **offering access**, not necessarily the effect of **receiving treatment**.

For example:
- In a scholarship study, ITT measures the impact of **offering scholarships**, not the pure causal effect of schooling itself.
- In a deworming study, ITT measures the impact of **running a real deworming program**, including imperfect attendance and outside access.

The authors argue that this is often the most policy-relevant quantity because real-world programs also have imperfect take-up.

---

## Including Covariates

### Why include them?
Covariates are pre-treatment characteristics such as:
- gender,
- ethnicity,
- baseline test scores,
- parental education.

Because treatment is randomized, covariates are **not required for unbiasedness** in a simple individual-level randomized design. However, they can improve **precision** by reducing unexplained variance.

### How they are used
Researchers can add covariates to the estimating regression. The treatment coefficient remains the main quantity of interest.

### Which covariates to include
The chapter warns against including too many controls. The best controls are those that strongly predict the outcome. Often the single most useful control is the **baseline value of the outcome variable**.

### Reporting practice
It is common to show results:
- **without covariates**, and
- **with covariates**,

so readers can assess sensitivity and precision gains.

---

## Heterogeneous Effects: If Subgroups Are Relevant

Program effects may differ across subgroups. These are **heterogeneous treatment effects**.

### Examples
- Textbooks may help only students already reading at a high level.
- Remedial education may mainly help initially low-performing students.

### How subgroup analysis works
Researchers estimate the program effect within a subgroup defined by a **pre-treatment characteristic**, such as:
- girls only,
- children under age 5,
- low baseline performers.

This is valid because the subgroup definition is not affected by treatment.

### Main caution: low power
Subgroup analysis has less power because the sample is smaller. The chapter gives an important warning:
- finding a statistically significant effect in one subgroup and a non-significant effect in another does **not** automatically mean the effects differ from each other.

To compare subgroups properly, researchers need a direct statistical test for equality of treatment effects.

---

## Interaction Terms

Interaction terms are useful when heterogeneity relates to a **continuous variable**, such as:
- age,
- income,
- baseline test score.

Instead of dividing people into categories, the analysis can estimate whether treatment effects increase or decrease along that continuous dimension.

### Key interpretation
The interaction coefficient tells whether the treatment effect:
- rises,
- falls, or
- stays constant

as the continuous characteristic changes.

### Important rule
Whenever an interaction term is included, the model must also include:
- the treatment term itself, and
- the underlying continuous variable.

---

## Multiple Observations Over Time

Many studies have:
- baseline and endline data, or
- multiple waves before and after treatment.

The chapter explains that repeated observations open up richer analysis strategies.

### Uses of repeated observations
- control for the baseline outcome,
- analyze changes over time,
- examine pre-treatment trends,
- study whether effects persist, decay, or grow.

### Example from the chapter
The authors discuss a study of the Vietnam draft lottery that plotted earnings over multiple years. The figure on **page 14** shows how taxable earnings of draft-eligible and draft-ineligible men evolved over time, allowing readers to see:
- similar pre-treatment trajectories,
- divergence after treatment,
- differences across white and nonwhite males.

This visual use of longitudinal data strengthens causal interpretation because it shows when the groups begin to diverge.

---

## Multiple Treatments

Many evaluations include more than one treatment arm.

### Bangladesh example
The chapter discusses a girls’ empowerment study with multiple treatment arms, including:
- girls’ clubs,
- marriage-delay incentives,
- a combined package.

### Analytical structure
The regression includes a separate indicator for each treatment arm. This yields:
- treatment effect of arm 1 vs. control,
- treatment effect of arm 2 vs. control,
- treatment effect of arm 3 vs. control.

### Important caution
Researchers must not conclude that one treatment is better than another merely because:
- one coefficient is statistically significant and another is not, or
- one point estimate is larger than another.

A proper test must be run to determine whether the treatment effects are statistically different from each other.

---

## Beyond Average Effects

The chapter notes that average treatment effects do not always capture what matters.

### Why mean effects may be insufficient
A program may:
- raise mean yields but increase risk,
- reduce average health expenditures but mainly matter by reducing catastrophic expenses,
- affect the lower or upper tail of a distribution rather than the mean.

### Example: quantile regression
The authors describe a Colombian school voucher study in which attrition and selection into taking an exam complicated mean comparisons. The researchers instead used **quantile regression** to examine treatment effects at different points in the outcome distribution.

### Lesson
Analysis can go beyond means to study:
- variance,
- tail risks,
- distributional effects,
- percentiles.

---

# Module 8.2: Catalog of Corrections

## Main Idea

Simple ITT analysis is valid for a clean individual randomization, but many evaluations face complications that require adjustments. Module 8.2 provides a catalog of those corrections, focusing on:

- partial compliance,
- attrition,
- spillovers,
- group-level randomization,
- stratified or matched randomization,
- unequal assignment fractions by strata,
- multiple outcomes,
- multiple subgroup tests.

---

## If There Is Partial Compliance

### Problem
Partial compliance arises when:
- some assigned to treatment do not take it up,
- some assigned to comparison access treatment anyway.

In that setting, ITT still answers the policy question of offering access, but researchers may also want the **effect on compliers**.

### Average effect on compliers
This estimates the effect on those who take up treatment **because of** the random assignment.

### Wald estimator
The chapter explains the simplest complier calculation:

- divide the ITT estimate by the difference in treatment take-up rates between treatment and comparison groups.

This rescales the ITT effect to reflect the fact that only part of the sample changed treatment status because of assignment.

### Instrumental variables (IV)
The chapter also explains the IV version:
- random assignment serves as an instrument for actual take-up.

This is especially useful because it allows control variables in the first-stage and second-stage estimation.

### When complier estimates are useful
They are especially useful in:
- encouragement designs,
- settings where take-up is incomplete,
- situations where researchers want to distinguish low take-up from small treatment effects.

### Strong warnings
The chapter is emphatic on two points:

#### Never drop noncompliers
Doing so reintroduces selection bias.

#### Never reassign treatment status based on actual treatment
Changing randomized assignment to reflect actual take-up also destroys the causal design.

### When complier estimation is inappropriate
Complier estimation relies on the assumption that assignment affects outcomes only through actual take-up. The chapter says this fails when:
- merely being **offered** treatment changes behavior,
- there are positive or negative spillovers within treatment groups.

In those cases, Wald and IV-based complier estimates can be biased.

---

## If There Is Attrition

### Problem
Attrition means some participants’ outcomes are missing. Random attrition mainly reduces power; **differential attrition** threatens internal validity by reintroducing selection bias.

### Three analytical steps recommended by the chapter

#### 1. Determine the overall attrition rate
How much data are missing overall?

#### 2. Check for differential attrition
Do attrition rates differ by treatment status?  
Are different types of participants attriting in the two groups?

#### 3. Determine the range of possible impacts given attrition
How sensitive are conclusions to what might have happened among those missing?

### Model-based approach
One approach predicts missing outcomes from observables, such as baseline covariates. The chapter notes that this is useful but rests on an untestable assumption:
- that missing participants are like observed participants with similar characteristics.

### Using a tracked subsample of attriters
If a random subset of attriters is followed intensively and successfully found, those data can strengthen model-based recovery of missing outcomes.

### Bounding approaches
The chapter discusses two major bounding methods:

#### Manski-Horowitz bounds
Assign best-case outcomes to missing treatment observations and worst-case outcomes to missing control observations, then reverse the assumption for the lower bound.

#### Lee bounds / Lee trimming
Trim observations from the group with lower attrition to construct bounds under a monotonicity assumption.

### Takeaway on attrition
These methods do not “solve” attrition. They show how much results depend on assumptions. The real priority remains preventing attrition during design and fieldwork.

---

## If Spillovers Occur

### Problem
If treatment affects non-treated units, the comparison group is contaminated and is no longer a true counterfactual.

- Positive spillovers lead to underestimation.
- Negative spillovers lead to overestimation.

### Analytical adjustment
Correction is possible only if researchers can identify:
- treatment units,
- spillover-exposed control units,
- uncontaminated control units.

The analysis can then estimate effects on:
- directly treated units,
- indirectly affected spillover units,
- unaffected controls.

### Example: school-based deworming
The chapter explains an approach in which researchers:
- drew geographic radii around schools,
- counted nearby students,
- counted nearby treated students.

Because the **share of nearby treated students** is randomized, the regression can estimate spillover effects.

### Key condition
Researchers must understand the mechanism of spillovers well enough to define who is exposed and who is not.

---

## If Randomization Is at the Group Level

### Problem
Sometimes randomization is by:
- school,
- village,
- clinic,
- household,
- district,

while outcomes are measured at the individual level.

### Why this matters
Individuals within the same group tend to have correlated outcomes because of:
- shared environments,
- common shocks,
- social sorting.

If researchers ignore that dependence and analyze individuals as if treatment were individually randomized, standard errors will be too small and significance overstated.

### Two analytical approaches

#### 1. Analyze at the group level
Aggregate outcomes to the randomization unit and estimate effects there. This is the simplest and most conservative approach.

#### 2. Analyze at the individual level with clustered standard errors
This is common when there are many clusters and individual-level data are available.

### Core rule
Standard errors must be clustered at the **level of randomization**.

If randomization is by school, cluster by school.  
Do not cluster at unrelated or lower levels just because outcomes are correlated there too.

### Small number of clusters
When the number of clusters is small, standard cluster adjustments become unreliable. The chapter recommends **randomization inference** as an alternative.

### Randomization inference
This method compares the observed treatment effect to the distribution of all treatment effects that could have arisen under the randomization scheme. It is especially useful when conventional asymptotics are weak.

---

## If There Is Stratified or Pairwise Randomization

### Problem
Standard tests assume independent random assignment. Stratification and matching impose constraints on the assignment process, so inference should account for them.

### When there is stratification
The usual adjustment is to include indicator variables for the strata.

### When there is matching
Matching is treated as an extreme form of stratification. Researchers include fixed effects or dummies for matched pairs.

### If there is baseline imbalance
The chapter notes that random imbalance is possible. Researchers do not have to adjust for every imbalanced variable, but it is often good practice to control for variables strongly correlated with the outcome as a robustness check.

---

## If Allocation Fractions Differ by Strata

### Problem
Sometimes treatment probabilities differ by subgroup. For example:
- more scholarships may be allocated to girls than boys.

If treatment effects also differ by subgroup, naïvely pooling the full sample can produce a biased estimate of the average effect.

### Solution
Estimate treatment effects within each stratum, then construct a **weighted average**.

Possible weighting schemes include:
- weights matching how the program was actually implemented,
- hypothetical weights for a different policy allocation.

This is conceptually important because the “overall” effect depends on what population or allocation rule the researcher wants to represent.

---

## If There Are Multiple Outcomes

### Problem
If researchers test many outcomes separately, the probability of finding at least one false positive rises sharply.

### Four main solutions described in the chapter

#### 1. Pre-specify one primary outcome
This is the simplest solution and is common in medical trials.

#### 2. Collapse related indicators into an index
Combine multiple measures of the same underlying concept into a single summary measure.

#### 3. Use mean standardized treatment effects
Standardize outcomes within a family and average treatment effects across them.

This allows multiple indicators to contribute to one overall hypothesis test.

#### 4. Adjust confidence intervals / p-values
The chapter mentions:
- **Bonferroni adjustment**, and
- **free step-down resampling** for family-wise error rate control.

### Sierra Leone example
The chapter describes a community-driven development study with more than 300 indicators. The researchers:
- grouped indicators into hypothesis families,
- estimated family-level mean effects,
- adjusted p-values for the number of tested hypotheses.

The table on **page 50** illustrates this strategy. It shows a strong average effect for “hardware” outcomes such as development infrastructure, but not for many “software” outcomes involving institutional and social change.

### Core lesson
Multiple-outcome adjustment is both a statistical and conceptual exercise. Researchers need to think carefully about:
- which outcomes represent the same construct,
- which are primary versus secondary,
- how many hypotheses they are truly testing.

---

## Multiple Subgroup Testing

The chapter notes that subgroup testing creates the same inferential problem as multiple outcome testing. If many subgroup analyses are run, at least one may appear significant by chance.

The recommended safeguards are:
- test only a small number of theory-driven subgroups,
- define them in advance,
- adjust inference when necessary.

---

# Module 8.3: Pre-analysis Plans

## Main Idea

Pre-analysis plans (PAPs) are written in advance to specify how the data will be analyzed before researchers see the treatment effects. Their main purpose is to reduce the risk or appearance of **data mining**, also called cherry-picking.

---

## Why PAPs Are Needed

### The data mining problem
If researchers examine:
- many outcomes,
- many subgroups,
- many model specifications,

they can often find a statistically significant effect somewhere purely by chance.

PAPs help prevent this by requiring researchers to specify in advance:
- what they will test,
- how they will measure it,
- which analyses are primary,
- which models they will run.

### Distinction from trial registration
The chapter distinguishes two related practices:

#### Registering the existence of a trial
This helps reduce publication bias.

#### Registering a PAP
This addresses within-study data mining by recording the planned analysis in detail.

---

## When PAPs Are Especially Useful

### 1. When there are many outcome measures
This is particularly important when programs aim to affect broad concepts such as:
- social capital,
- trust,
- empowerment,
- conflict.

### 2. When subgroup analysis is central
If the theory predicts different impacts across groups, a PAP helps show those groups were chosen for substantive reasons rather than after seeing the data.

### 3. When there are multiple reasonable specifications
For example:
- levels vs. logs,
- OLS vs. logit,
- with controls vs. without controls,
- randomization inference vs. asymptotic inference.

---

## Drawbacks of PAPs

The chapter gives a balanced discussion and does not treat PAPs as a universal solution.

### Main drawbacks

#### 1. They reduce flexibility
A rigid plan may omit results that later turn out to be theoretically important.

#### 2. They may be incomplete
Researchers may fail to anticipate important mechanisms, side effects, or subgroup patterns.

#### 3. Good analysis often depends on what the data reveal
For example:
- if the program helps, researchers may next examine mechanisms;
- if it harms, they may next examine why.

A PAP cannot easily anticipate every branch of that decision tree.

### Practical stance of the chapter
The authors suggest that exploratory analysis is still valuable, but it should be clearly distinguished from pre-specified analysis.

---

## When Should a PAP Be Written?

The chapter discusses several timing options.

### Earliest option: before the study begins
This offers the strongest protection against accusations of data mining, but it ignores useful information learned during implementation.

### Common option: after endline data are collected but before analysis
This allows the design and field experience to inform the plan while still preventing cherry-picking based on treatment effects.

### Alternative: inspect control-group endline data before finalizing the plan
Because treatment effects are still hidden, researchers can refine measures based on distributions and data quality without biasing inference.

### Hybrid approach
Researchers can register:
- broad hypotheses early,
- then finalize the full PAP later before analysis.

This balances credibility and flexibility.

---

## What a PAP Should Include

The chapter identifies several core components:

1. **Main outcome measures**
2. **Primary vs. secondary outcomes**
3. **Exact composition of families for mean-effects analysis**
4. **Subgroups to be analyzed**
5. **Expected direction of impact if using one-sided tests**
6. **Primary estimating specification**

The chapter stresses that outcome definitions must be precise.  
For example, instead of saying “immunization rates,” the PAP should specify exactly:
- the age range,
- the vaccines counted,
- the source of measurement,
- the time window.

It should also clearly distinguish:
- primary outcomes tied to the main theory of change,
- secondary outcomes measuring intermediate mechanisms.

---

## How Many Outcomes Should a PAP Include?

The chapter argues there is no single correct number. Too many outcomes weaken power and raise multiple-testing problems. Too few may ignore the theory of change.

The recommended approach is to use:
- a clear theory of change,
- priority ordering of outcomes,
- grouping into meaningful families,
- justification for chosen subgroups.

---

## PAPs in Multi-Arm Studies

Multi-arm trials naturally generate many hypotheses because each arm can be compared to:
- control,
- other treatment arms,
- pooled versions of other arms.

The chapter advises using theory to narrow comparisons to the ones that actually answer substantive questions.

### Bangladesh example
In the girls’ empowerment study, many pairwise comparisons were possible, but not all were meaningful. The chapter argues that researchers should focus on comparisons tied to the study’s actual conceptual objectives, such as:
- effect of empowerment components,
- effect of delayed-marriage incentives,
- complementarity across components.

---

# Cross-Cutting Lessons from Chapter 8

## 1. ITT is the analytic anchor
No matter how complicated the design becomes, analysis should begin with the effect of assignment to treatment.

## 2. Analysis must match design
Corrections are not optional technical add-ons. They are required when assignment or implementation departs from the simplest design.

## 3. Real-world complications are central, not peripheral
Noncompliance, attrition, spillovers, clustering, and multiple outcomes are common features of field experiments.

## 4. Precision and validity are different
Adding covariates may improve precision, but some corrections—especially for attrition and spillovers—are about protecting validity.

## 5. Transparency matters
Pre-analysis plans, explicit primary outcomes, and clearly specified subgroup tests all improve the credibility of findings.

## 6. Good analysis is both statistical and substantive
The chapter repeatedly ties econometric choices back to:
- theory of change,
- program implementation,
- policy relevance,
- practical interpretation.

---

# Concise Study Guide Summary

## Module 8.1: Basic ITT Analysis
- Start with treatment assignment, not take-up.
- Clean and inspect the data first.
- ITT estimates the effect of being offered the program.
- Covariates improve precision, not validity.
- Subgroup and interaction analysis help study heterogeneity.
- Repeated observations allow trend and persistence analysis.
- Multiple treatment arms require formal comparisons, not casual coefficient comparisons.

## Module 8.2: Catalog of Corrections
- Use Wald or IV approaches for effects on compliers, but only under strong assumptions.
- Never drop noncompliers or reassign treatment status.
- Attrition requires rate checks, differential attrition diagnostics, and sensitivity analysis.
- Spillovers require identifying contaminated and uncontaminated controls.
- Group-level randomization requires clustered standard errors or group-level analysis.
- Small numbers of clusters may require randomization inference.
- Stratification and matching should be incorporated into the analysis.
- Unequal assignment fractions require weighted averaging across strata.
- Multiple outcomes and subgroup tests require careful control of false positives.

## Module 8.3: Pre-analysis Plans
- PAPs reduce data mining and selective reporting concerns.
- They are most useful when there are many outcomes, subgroups, or plausible specifications.
- PAPs should specify outcomes, subgroup tests, model choices, and hypothesis families.
- They improve credibility but can reduce flexibility.
- Exploratory analysis is still valuable if clearly labeled as such.

---

# Why This Chapter Matters

Chapter 8 is the book’s bridge from **experimental design** to **causal inference in practice**. It shows that randomization gives researchers a strong foundation, but not a complete one. Sound analysis requires matching the estimator to the design, correcting for deviations from ideal conditions, and being transparent about analytic choices. In that sense, the chapter is both a practical handbook and a warning: even randomized evaluations can mislead if their analysis ignores how the study was actually implemented.

---

# Citation

Glennerster, Rachel, and Kudzai Takavarasha. *Running Randomized Evaluations: A Practical Guide*. Princeton University Press, 2013. Chapter 8: “Analysis.”
