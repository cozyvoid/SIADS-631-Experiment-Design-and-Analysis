# Detailed Overview: Chapter 6 — Statistical Power

**Source:** *Running Randomized Evaluations: A Practical Guide* — Chapter 6, “Statistical Power”

---

## 1. Chapter purpose and scope

This chapter explains **what statistical power is, what determines it, how to calculate it, and how to design studies with enough power to detect meaningful treatment effects**. It treats power as a practical design tool, not just a statistical afterthought: power analysis helps researchers decide sample size, randomization level, number of treatment arms, number of survey rounds, allocation ratios, and outcome measures. fileciteturn5file0

The chapter is organized into five modules:
- **Module 6.1:** The Statistical Background to Power
- **Module 6.2:** The Determinants of Power Explained Graphically
- **Module 6.3:** An Algebraic Exposition of the Determinants of Power
- **Module 6.4:** Performing Power Analysis
- **Module 6.5:** How to Design a High-Powered Study. fileciteturn5file0

---

## 2. Core idea of statistical power

The chapter defines **statistical power** as the probability that, **if a true treatment effect of a given size exists, the study will detect it as statistically significant**. A low-powered study may fail to detect a real effect, producing wide confidence intervals and inconclusive results. The opening example shows a program that appears to raise test scores from 38% to 44%, but the estimate is too imprecise to rule out chance because the plausible impact range is still very wide. fileciteturn5file0

Power is therefore about **sensitivity**: how well an experiment can distinguish a true effect from random noise. The chapter repeatedly emphasizes that “no significant effect” can mean either “there really is no effect” or “the study was too weak to detect it.” fileciteturn5file0

---

## 3. Module 6.1 — The statistical background to power

### 3.1 Sampling variation

The chapter begins with **sampling variation**, the fact that repeated random samples from the same population produce slightly different estimates. Even with unbiased sampling, one sample may overestimate and another may underestimate the true population mean. Power calculations are necessary because researchers nearly always observe only a sample, not the full population. fileciteturn5file0

Two drivers of sampling variation are highlighted:
- **Population dispersion**: more spread in outcomes means more noise.
- **Sample size**: larger samples reduce the gap between sample estimates and the population value. fileciteturn5file0

### 3.2 Standard deviation

The **standard deviation (SD)** is introduced as the measure of dispersion in the underlying population. If the outcome variable is highly dispersed, any sample is more likely to include observations far from the population mean, making estimates noisier. fileciteturn5file0

### 3.3 Standard error

The **standard error (SE)** is the standard deviation of the estimate itself. For a mean, the chapter explains that standard error equals the population SD divided by the square root of sample size. This formalizes two intuitions:
- more variable populations create less precise estimates;
- larger samples create more precise estimates. fileciteturn5file0

### 3.4 Central limit theorem

The chapter uses the **central limit theorem** to justify why sampling distributions are approximately normal in large enough samples, even if the original outcome variable is not normally distributed. This matters because much of hypothesis testing and power analysis relies on normal approximations. fileciteturn5file0

### 3.5 Confidence intervals and confidence levels

A **confidence interval** is a range around a point estimate that reflects uncertainty. A 95% confidence level means that if the same procedure were repeated many times, about 95% of those intervals would contain the true parameter. The confidence interval translates the standard error into an interpretable band of plausible values. fileciteturn5file0

### 3.6 Hypothesis testing

The chapter then shifts to randomized evaluations, where the parameter of interest is usually the **difference in means** between treatment and comparison groups. The difference in means, like the sample mean itself, has a sampling distribution and a standard error. fileciteturn5file0

It defines:
- **Null hypothesis (H0):** treatment effect = 0
- **Research / alternative hypothesis (H1):** treatment effect ≠ 0, or in some cases > 0 or < 0. fileciteturn5file0

A **p-value** is described as the probability of observing results like those in the experiment if the null hypothesis were true. By convention, results are called statistically significant when the p-value is below 0.05. The chapter stresses that failing to reject the null may reflect low power rather than absence of an effect. fileciteturn5file0

### 3.7 The four possible statistical outcomes

A core conceptual contribution of Module 6.1 is the four-case framework:
1. **False positive (Type I / alpha error):** reject the null when it is true.
2. **True zero:** correctly fail to reject the null when the effect is truly zero.
3. **False zero (Type II error):** fail to reject the null when a true effect exists.
4. **True positive:** correctly reject the null when a true effect exists. fileciteturn5file0

The chapter then defines:
- **α (alpha)** as the false-positive rate, conventionally 5%;
- **κ** as the false-negative rate for a specified true effect size;
- **Power = 1 − κ**, conventionally targeted at 80% or sometimes 90%. fileciteturn5file0

### 3.8 Module 6.1 takeaway

Module 6.1 supplies the basic vocabulary of the whole chapter: sampling variation, SD, SE, confidence intervals, null hypotheses, p-values, Type I and Type II errors, and power. fileciteturn5file0

---

## 4. Module 6.2 — Determinants of power explained graphically

Module 6.2 explains power using overlapping bell curves for estimated effect sizes under the null and under a real-effect hypothesis. The central intuition is that **power depends on how much those two distributions overlap**. Heavy overlap means many observed estimates could plausibly come from either “no effect” or “real effect,” so detection is difficult. fileciteturn5file0

### 4.1 Effect-size distributions

The chapter denotes the true effect by **β**. If β = 0, repeated experiments generate a bell-shaped curve centered on zero. If the true effect is β\*, repeated experiments generate a bell-shaped curve centered on β\*. The farther apart the two curves are, the easier it is to distinguish them and the greater the power. fileciteturn5file0

### 4.2 Critical values and significance thresholds

The **critical value** is the threshold beyond which the null hypothesis is rejected. At the 5% significance level, only estimates in the tail(s) of the null distribution count as significant. Power is the share of the β\* distribution that lies beyond that threshold. fileciteturn5file0

The chapter also distinguishes between:
- **one-sided tests**, which look only for positive or only for negative effects;
- **two-sided tests**, which allow either direction and are more standard. fileciteturn5file0

### 4.3 Minimum detectable effect (MDE)

A central concept introduced here is the **minimum detectable effect (MDE)**: the smallest true effect the study is designed to distinguish from zero at the chosen significance level and power. Power analysis does not discover the true effect in advance. Instead, it answers questions like: “If the true effect were this big, how likely would we be to detect it?” fileciteturn5file0

### 4.4 Residual variance

The width of the effect-size distributions depends on the **variance of the estimator**, which in turn depends on the underlying variability of outcomes and on how much of that variability remains after controlling for observable covariates. That is why baseline measures and strong controls improve power: they reduce residual variance and make the estimate more precise. The chapter notes that baseline test scores in education studies can reduce residual variance dramatically. fileciteturn5file0

### 4.5 Sample size

Larger samples narrow the bell curves, reduce overlap, and increase power. Graphically, increasing sample size makes the distribution of estimated effects tighter around the true value. fileciteturn5file0

### 4.6 Significance level

Using a less stringent significance threshold, such as 10% instead of 5%, increases power because it lowers the bar for rejecting the null. But the chapter warns that this comes at the cost of more false positives. It illustrates the trade-off with a jury-trial analogy: a lower standard for conviction makes it easier to convict the guilty, but also the innocent. fileciteturn5file0

### 4.7 Allocation ratio

For a standard two-arm design, power is maximized when treatment and comparison groups are **equal in size**. Unequal allocation usually wastes precision because it estimates one group mean more precisely than the other. fileciteturn5file0

### 4.8 Clustering and group-level randomization

A major subtopic in Module 6.2 is **cluster randomization**. Randomizing by village, school, or clinic lowers power because outcomes within clusters are correlated. When people inside a cluster resemble each other, adding more people to the same cluster contributes less new information than adding new clusters. fileciteturn5file0

The NERICA example from Sierra Leone shows the practical consequence: under individual randomization, the sample size needed to detect a 20% yield increase would be modest, but under village-level randomization with an intracluster correlation of 0.19 and 10 farmers per village, the design would require **80 villages and 800 farmers**. fileciteturn5file0

### 4.9 Module 6.2 takeaway

Graphically and intuitively, power rises with larger effects, larger samples, lower residual variance, balanced allocation, and lower intracluster correlation. It falls sharply when randomization moves from individuals to groups. fileciteturn5file0

---

## 5. Module 6.3 — Algebraic exposition of the determinants of power

Module 6.3 formalizes the graphical intuitions using regression notation and variance formulas.

### 5.1 Individual-level randomization

For individual-level randomization, the chapter models the outcome as a function of:
- a constant,
- a treatment indicator,
- control variables,
- and an error term. fileciteturn5file0

The variance of the treatment effect estimate depends on:
- **N** = total sample size,
- **σ²** = residual variance,
- **P** = treatment allocation fraction. fileciteturn5file0

The algebra confirms the earlier intuition: power rises when sample size increases, variance falls, MDE increases, or treatment allocation approaches 0.5. fileciteturn5file0

### 5.2 Formal MDE relationship

The MDE is presented as a function of:
- critical values implied by alpha and desired power,
- residual variance,
- allocation fraction,
- sample size. fileciteturn5file0

Even if the reader does not work through the equations, the practical meaning is clear: **effects are easier to detect when they are large relative to noise and sample size is large relative to uncertainty**. fileciteturn5file0

### 5.3 Group-level randomization

For clustered designs, the model adds:
- a **cluster-level shock**,
- an **individual-level shock within cluster**. fileciteturn5file0

This produces the concept of **intracluster correlation (ρ)**, the proportion of total variance attributable to cluster-level similarity. High ρ means the design loses more precision when randomization is done at the cluster level. fileciteturn5file0

### 5.4 Design effect

The chapter introduces the **design effect**, which captures how much less precise a clustered design is than an individually randomized design with the same total sample size. It rises with:
- larger cluster size,
- higher intracluster correlation. fileciteturn5file0

This formalizes one of the chapter’s most practically important messages: in clustered designs, power is often much more sensitive to the **number of clusters** than to the **number of respondents within each cluster**. fileciteturn5file0

### 5.5 Module 6.3 takeaway

The algebraic module turns the chapter’s intuition into formulas that software can implement, while reinforcing the same applied message: bigger samples, lower variance, balanced allocation, lower clustering, and larger detectable effects all improve power. fileciteturn5file0

---

## 6. Module 6.4 — Performing power analysis

This module explains what inputs are needed for a power calculation, where to get them, and how to use statistical software. fileciteturn5file0

### 6.1 Desired power

The chapter notes that the most common target is **80% power**, though 90% is also used. With 80% power, the study will detect a true effect of the chosen MDE size in 80% of comparable repeated experiments. fileciteturn5file0

### 6.2 Choosing the MDE

The chapter argues that choosing the MDE is the **hardest and most important** part of power analysis. It strongly warns against treating MDE as a guess of the true effect or as a desired program target. Instead, it should represent the **smallest effect that would matter for practical decisionmaking**. fileciteturn5file0

It proposes three main ways to think about MDE:

#### (a) Standard effect-size conventions
In some fields, rules of thumb exist, such as 0.2 SD as “small but respectable” and 0.4 SD as “large” in education. But the chapter warns that such conventions are context dependent and weak as stand-alone guides. fileciteturn5file0

#### (b) Comparisons with similar interventions
Researchers can compare their program with other rigorously evaluated programs with similar goals and similar costs. This gives a practical benchmark for what counts as meaningful. fileciteturn5file0

#### (c) Cost-effectiveness threshold
The chapter presents this as the strongest framework: determine what effect size would make the program cost-effective relative to alternatives. Cheap programs may be worthwhile even with small impacts, which means they require smaller MDEs and therefore larger evaluation samples. fileciteturn5file0

The chapter also notes that if the policy question is not only “is the effect nonzero?” but “which program is better?”, then precision matters beyond simple statistical significance. fileciteturn5file0

### 6.3 Choosing the number of clusters

For clustered designs, there is a trade-off between:
- sampling more clusters, which improves power,
- and sampling more people within a cluster, which may be cheaper because fixed travel and setup costs are already paid. fileciteturn5file0

The chapter emphasizes that the marginal power benefit of more within-cluster observations diminishes, but so may the marginal survey cost. The optimal balance depends on both the intracluster correlation and the cost structure of fieldwork. fileciteturn5file0

### 6.4 Allocation fractions and exceptions to 50/50

Although equal allocation is usually optimal in a simple two-arm design, the chapter explains several exceptions:

#### (a) One budget funds both program and evaluation
If treated units are much more expensive than control units, maximizing power under a fixed budget may require putting **more observations in the comparison group**. fileciteturn5file0

#### (b) Different MDEs across multiple treatment arms
If some treatments are cheaper or more policy important, they may justify smaller MDEs and different sample shares. fileciteturn5file0

#### (c) Comparison group used in many pairwise comparisons
When one control group serves several treatment comparisons, adding sample to the control group can improve multiple analyses at once. fileciteturn5file0

#### (d) Unequal variances across groups
In principle, unequal group variances could justify unequal allocation, though the chapter says this is rarely the main reason in practice. fileciteturn5file0

### 6.5 Estimating residual variance

Residual variance can be estimated using:
- prior data from similar populations,
- pilot surveys,
- previous experiments,
- or regressions on historical data using likely controls. fileciteturn5file0

The chapter warns that using total variance instead of residual variance will generally overstate the required sample size, because final analysis often includes covariates that reduce noise. fileciteturn5file0

### 6.6 Repeat observations and temporal correlation

Baseline and endline data can improve power because repeated measurements allow the analyst to control for persistent individual differences. But the benefit depends on **intertemporal correlation**: if outcomes are highly persistent, repeat measures are very valuable; if not, their benefit is more limited. The chapter also reminds the reader that observing 100 people five times still gives a sample size of 100, not 500. fileciteturn5file0

### 6.7 Intracluster correlation

For cluster-randomized studies, getting a good estimate of **ρ** is crucial. The chapter recommends using pilot data or prior surveys from similar settings, because power calculations can be highly sensitive to this parameter. fileciteturn5file0

### 6.8 Software tools

The chapter discusses two main software tools:

#### Stata
It highlights `sampsi` for individual-level calculations and `sampclus` for clustered designs, showing how users enter means, SDs, desired power, cluster size, and rho. fileciteturn5file0

#### Optimal Design
It presents Optimal Design as a useful dedicated package because it graphically displays trade-offs and handles more complex multilevel or repeated-measures structures. It also notes that users need to translate the reported sample size correctly when there are more than two treatment cells. fileciteturn5file0

### 6.9 Case study: remedial education in Mumbai

This is one of the chapter’s most applied sections. Using pilot data from six schools, the researchers estimate:
- average test score = 26%,
- SD = 20,
- intracluster correlation = 0.17. fileciteturn5file0

They decide the program is worthwhile only if it raises scores by at least 10%, which corresponds to:
- 2.6 percentage points,
- or a standardized MDE of **0.13 SD**. fileciteturn5file0

The chapter then walks through alternative designs:
- **40 children per school** → about **356 schools** needed for 80% power.
- **80 children per school** → about **336 schools**.
- **80 children per school plus baseline controls explaining about half of endline variance** → about **180 schools**. fileciteturn5file0

This case study illustrates three powerful lessons:
- adding more respondents per cluster may help only modestly;
- using strong baseline controls can greatly reduce the required number of clusters;
- adding more treatment variants can make the design unaffordable. fileciteturn5file0

The chapter shows that comparing two treatment versions directly would have required **1,068 schools**, so the researchers simplified to one treatment arm with 180 schools and 80 children per school. fileciteturn5file0

### 6.10 Module 6.4 takeaway

The module ends with a practical checklist of ingredients for power analysis:
- significance level,
- comparison-group mean,
- residual variance,
- MDE,
- allocation fractions,
- intracluster correlation,
- desired power,
- repeat observations and intertemporal correlation. fileciteturn5file0

---

## 7. Module 6.5 — How to design a high-powered study

The final module turns the chapter into a set of design principles. It argues that power must be built into the study from the start and protected through design, data collection, implementation, and analysis. fileciteturn5file0

### 7.1 During evaluation design

#### Choose a decent sample size
A sufficiently large sample is essential for precision, though increasing sample size can be expensive. fileciteturn5file0

#### Use fewer treatment groups
Every additional treatment arm divides the available sample. If total sample is fixed, each pairwise comparison becomes less precise. The chapter advises ensuring that at least one central question can be answered with good precision. fileciteturn5file0

#### Randomize at the lowest feasible level
Randomizing individuals is usually more powerful than randomizing groups because it avoids the precision loss caused by cluster-level correlation. fileciteturn5file0

#### Use a design that increases compliance
Partial compliance shrinks the actual treatment-control contrast and therefore shrinks the effective effect size. The chapter shows that if compliance falls, required sample sizes can increase dramatically because sample size scales with the square of the dilution factor. fileciteturn5file0

#### Use a design that limits attrition
Attrition reduces effective sample size and therefore weakens power, in addition to threatening internal validity. fileciteturn5file0

#### Use stratification
Stratification balances treatment and comparison groups on key predictors, especially in small samples. This reduces residual variance and improves precision. fileciteturn5file0

#### Choose allocation fraction thoughtfully
Equal allocation is often best, but budget constraints and multiple treatment comparisons can justify deviations. fileciteturn5file0

### 7.2 During data collection planning

#### Choose proximate outcomes
More proximate outcomes in the causal chain are often less noisy and easier to detect than very distal outcomes. The chapter uses immunization as an example: take-up is much easier to measure with power than downstream child mortality. But it also warns against choosing outcomes so proximate that they no longer capture meaningful impact. fileciteturn5file0

#### Collect strong control variables
Especially baseline values of the main outcome, because these often explain a large share of endline variation. fileciteturn5file0

#### Collect multiple observations when justified
Repeated measures can increase power when outcomes are stable enough over time. fileciteturn5file0

#### Plan data collection to limit attrition
The chapter suggests practical tracking strategies such as collecting phone numbers, alternate contacts, and periodic check-ins. fileciteturn5file0

#### Limit procedural variation
Consistent implementation and measurement reduce variance and therefore increase power. fileciteturn5file0

### 7.3 During implementation

#### Increase compliance
Researchers should try to keep the difference in actual treatment receipt between groups as large as possible. fileciteturn5file0

#### Limit attrition continuously
Tracking participants throughout rollout helps preserve sample size and power. fileciteturn5file0

### 7.4 During impact analysis

#### Use control variables
Including pre-treatment covariates in the final regression reduces unexplained variance and improves power. fileciteturn5file0

#### Use conventional significance thresholds
The chapter explicitly discourages designing a study around relaxed significance levels merely to claim more power. The conventional 5% threshold remains the recommended planning standard. fileciteturn5file0

---

## 8. Important figures and visuals in the chapter

Several visuals reinforce the chapter’s major ideas:

- **Figure 6.1** shows repeated estimates of a population mean and directly visualizes sampling variation. fileciteturn5file0
- **Figure 6.2** presents the four-case matrix of true effect / no effect crossed with significant / not significant outcomes, visually defining alpha, Type II error, and power. fileciteturn5file0
- **Figures 6.4–6.9** use overlapping bell curves to show how effect size, sample size, and significance thresholds affect power. fileciteturn5file0
- **Figure 6.8** contrasts small and large sample sizes by showing how larger samples narrow the distribution of estimated effects. fileciteturn5file0
- **Figure 6.11** in the Mumbai case study shows how required numbers of clusters change under different assumptions. The key lesson from that figure is that **good baseline controls can matter more than simply increasing the number of respondents within clusters**. fileciteturn5file0

---

## 9. Key formulas and concepts to know

The chapter repeatedly returns to a manageable set of concepts:
- **Standard error** decreases as sample size rises.
- **Power = 1 − Type II error**.
- **Alpha** is the false-positive rate.
- **MDE** is the smallest effect the study is designed to detect.
- **Residual variance** matters more than raw variance when controls are used.
- **Intracluster correlation** drives the power loss from clustering.
- **Design effect** summarizes the precision penalty from cluster randomization.
- **Baseline controls and repeated measures** can materially improve power.
- **Compliance and attrition** can substantially change effective sample size needs. fileciteturn5file0

---

## 10. Big-picture lessons from the chapter

### 10.1 Power is a design problem
The chapter’s strongest theme is that power must be considered at design stage, not after the fact. It affects feasibility, budget, and whether the study can answer the questions it sets out to answer. fileciteturn5file0

### 10.2 MDE should be policy relevant
The right MDE is not an arbitrary benchmark. It should reflect the smallest effect that would matter for action, often judged through cost-effectiveness or comparison with realistic alternatives. fileciteturn5file0

### 10.3 Cluster randomization is statistically costly
Cluster randomization may be necessary for spillovers or logistics, but the power penalty can be large. In many studies, the number of clusters matters far more than the number of observations per cluster. fileciteturn5file0

### 10.4 Baseline data are highly valuable
One of the clearest practical lessons is that baseline outcomes and strong covariates can dramatically reduce residual variance and therefore cut required sample sizes. fileciteturn5file0

### 10.5 More questions can weaken the study
Every extra treatment arm consumes precision. Simpler experiments may answer fewer questions overall but answer the most important ones more credibly. fileciteturn5file0

### 10.6 Operations affect statistical performance
Compliance, attrition, and implementation quality are not just field-management details. They directly affect the study’s ability to detect effects. fileciteturn5file0

---

## 11. Condensed study guide

### What power means
Power is the probability that the study detects a real treatment effect of a specified size as statistically significant. fileciteturn5file0

### What increases power
- Larger sample size
- Larger MDE / true effect
- Lower residual variance
- Strong baseline controls
- Balanced treatment-control allocation
- Lower intracluster correlation
- More clusters in clustered designs
- Better compliance
- Lower attrition
- More proximate outcomes when substantively appropriate. fileciteturn5file0

### What decreases power
- Small samples
- High variance
- Cluster randomization with few clusters
- High intracluster correlation
- Many treatment arms
- Weak controls
- Poor compliance
- High attrition
- Noisy distal outcomes. fileciteturn5file0

### Most testable concepts from the chapter
- Type I vs Type II error
- Alpha, confidence level, power
- MDE
- Residual variance
- Intracluster correlation
- Design effect
- Why cluster randomization lowers power
- Why baseline covariates can sharply reduce sample requirements
- Why MDE should be tied to policy relevance and cost-effectiveness. fileciteturn5file0

---

## 12. Bottom line

Chapter 6 presents statistical power as the link between statistical theory and evaluation design. Its practical message is that a randomized evaluation must be not only unbiased, but also precise enough to detect the kinds of effects that matter for policy. Power analysis helps researchers decide whether a design is feasible, whether the MDE is appropriate, whether clustering is affordable, and whether additional treatment arms are worth the loss of precision. The chapter’s overall lesson is that **high-powered studies come from disciplined choices: policy-relevant MDEs, adequate samples, low clustering where possible, strong baseline data, good covariates, low attrition, high compliance, and a design simple enough to answer the most important questions well**. fileciteturn5file0
