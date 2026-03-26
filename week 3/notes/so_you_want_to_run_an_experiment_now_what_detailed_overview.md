# Detailed Overview: *So You Want to Run an Experiment, Now What?*
## Some Simple Rules of Thumb for Optimal Experimental Design

**Citation:** John A. List, Sally Sadoff, and Mathis Wagner (2011), *Experimental Economics*, 14:439–457.

---

## 1. Core purpose of the article

This article is a practical guide to **designing more statistically efficient experiments**. Its central argument is that many experiments use conventional but inefficient design choices—especially **equal sample sizes across treatment cells** and overly simple heuristics such as “30 subjects per cell”—without considering whether those choices maximize power or minimize detectable effect size.

The paper’s goal is to give experimenters a set of **usable design rules of thumb** for:
- choosing a randomization strategy,
- arranging sample sizes across treatment cells,
- handling unequal variances and unequal sampling costs,
- designing cluster-randomized studies,
- and allocating observations when treatment intensity varies.

A recurring theme is that experimenters should not think only about increasing **sample size**. They should also design experiments to:
1. **maximize the variance of the treatment variable**, and  
2. **reduce unexplained variance in outcomes**.  

Those two design levers can materially improve precision without necessarily increasing cost.

---

## 2. Big-picture framing: why experimental design matters

The article begins with the standard causal inference problem: for any unit, we cannot observe both the treated and untreated outcome simultaneously. Experiments solve this by using **random assignment** to construct the counterfactual. The authors emphasize that, relative to observational methods, experiments require fewer identification assumptions, as long as randomization is valid and sample sizes are adequate.

However, once the researcher controls the data-generating process, new obligations emerge:
- deciding how to randomize,
- deciding how many subjects to place in each cell,
- deciding whether equal cell sizes are appropriate,
- and deciding whether design choices are actually efficient.

The paper argues that experimental economics has historically under-discussed these issues compared with other fields. fileciteturn6file0

---

## 3. Main organizing idea of the paper

The article’s central design principle is:

> **Efficient design first maximizes treatment variation, then adjusts allocation to account for variance heterogeneity and cost differences.**

This principle generates several practical rules:
- equal allocation is optimal **only in special cases**,
- unequal variances imply unequal optimal sample sizes,
- unequal treatment costs also imply unequal allocation,
- cluster designs require explicit correction for intracluster correlation,
- and when treatment is continuous, the best design often puts observations at the **extremes** rather than spreading them evenly. fileciteturn6file0

---

## 4. Article structure and subtopics

The article proceeds through six broad sections:
1. Introduction  
2. Randomization techniques  
3. Optimal sample arrangement: basics  
4. Optimal sample arrangement: further considerations  
5. Optimal sample arrangement: varying treatment levels  
6. Concluding remarks  

Each section develops a different part of the practical design toolkit. fileciteturn6file0

---

## 5. Introduction: the problem with default design habits

### 5.1 Experimental identification is easier—but design still matters
The authors contrast:
- **observational methods**, which rely on stronger identifying assumptions, and
- **experiments**, where valid randomization can deliver unbiased estimates of treatment effects.

But they argue that this advantage sometimes causes researchers to overlook design optimization.

### 5.2 Critique of the “equal cells” norm
A major criticism is that many studies:
- divide subjects uniformly across cells,
- often use around 30 subjects per cell,
- and do so whether the treatment is binary or has several intensity levels.

The paper argues this convention is often inefficient because optimal allocation depends on:
- outcome variance,
- treatment heterogeneity,
- desired significance and power,
- detectable effect size,
- and the relative cost of sampling different groups. fileciteturn6file0

### 5.3 Three design scenarios highlighted in the introduction
The authors preview formulas and guidance for:
- **binary treatment with continuous or binomial outcomes**,
- **cluster-randomized designs**, and
- **continuous or multi-level treatments**. fileciteturn6file0

---

## 6. Randomization techniques

This section explains that “randomization” is not one thing. Different randomization structures have different precision implications.

### 6.1 Potential outcomes framework and average treatment effect
The paper presents the outcome under treatment and control as functions of:
- observed covariates,
- subject-specific effects,
- an average treatment effect,
- heterogeneous treatment effects,
- and random error.

The estimation problem is that the treated and untreated outcomes for the same unit cannot both be observed. Random assignment addresses this by making treatment independent of confounding influences. fileciteturn6file0

### 6.2 Randomization bias
The authors briefly discuss **randomization bias**, meaning the possibility that the act of randomizing affects who agrees to participate, so the sample may not represent the target population.

They note:
- this concern is well known in clinical trials,
- it could matter in economics too,
- but available evidence suggests it may not be a major empirical obstacle in many field experiments.

This is an important nuance: even a perfectly randomized experiment can still have external validity concerns if participation itself is selective. fileciteturn6file0

---

## 7. Block and within-subject designs

### 7.1 Completely randomized design
The simplest design assigns treatment probabilistically and independently of subject characteristics.

**Advantage:**
- minimizes correlation between treatment and observed or unobserved subject traits.

**Disadvantages:**
- may leave large residual variance,
- and may produce imbalanced treatment/control sizes by chance,
- both of which reduce inferential precision. fileciteturn6file0

### 7.2 Block designs
A block design groups units by observable characteristics before randomizing within blocks.

**Why block?**
- to reduce unexplained outcome variance,
- to improve precision,
- and to estimate treatment effects separately for subgroups.

The paper explains that blocking is conceptually similar to controlling for covariates in regression, except that blocking builds this structure directly into the design stage. Since estimator variance rises with unexplained error variance and falls with treatment variance, blocking can improve efficiency by reducing the unexplained component. fileciteturn6file0

### 7.3 Within-subject designs
A within-subject design can be interpreted as an extreme block design in which each subject is their own block.

**Advantages:**
- greatly reduces variance due to fixed individual differences,
- requires fewer recruited subjects,
- often increases degrees of freedom and precision.

**Important caution:**
Treating the same person multiple times can create:
- history effects,
- learning effects,
- sensitization to previous treatments,
- and treatment-order interactions.

These effects can change the estimand relative to a between-subject design. The authors mention **crossover designs** as a way to control some order effects, but they still urge caution in interpretation. fileciteturn6file0

### 7.4 Key lesson from this section
The paper does not recommend one design universally. Instead, it emphasizes that gains in precision must be balanced against risks of contamination or treatment interaction.

---

## 8. Factorial designs

### 8.1 What a factorial design does
In a factorial design, the researcher pre-specifies how many observations will go to each treatment combination. This can substantially improve efficiency relative to free-form random allocation.

### 8.2 Why random order still matters
Even with fixed cell counts, assignments should not follow arrival order or another potentially systematic sequence. Random order protects against biases such as early and late participants differing in important ways.

### 8.3 Full versus fractional factorial designs
A full factorial with \(n\) binary treatments requires \(2^n\) combinations.

A **fractional factorial design** reduces the number of combinations if the researcher is willing to assume that some interaction effects are absent.

**Advantage:**
- fewer trials.

**Disadvantage:**
- in simple forms, it becomes impossible to test omitted interaction effects.

The authors also note that even basic factorial designs with equal-sized cells may be inefficient if they ignore outcome variance and the structure of the treatment-response relationship. fileciteturn6file0

---

## 9. Optimal sample arrangement: the basics

This is the heart of the paper. It explains that optimal sample size decisions require thinking jointly about:

- **significance level** (Type I error),
- **power** (1 minus Type II error),
- and **minimum detectable effect size**.

### 9.1 Definitions
- **Significance level (\(\alpha\))**: probability of falsely rejecting the null.
- **Power (1 − \(\beta\))**: probability of correctly rejecting the null when the specified alternative is true.
- **Minimum detectable effect**: the smallest effect the researcher wants the experiment to be able to detect.

The paper notes that many economists think naturally in terms of p-values after estimation, but power analysis asks a different design-stage question: *if the alternative is true, how likely is the experiment to detect it?* fileciteturn6file0

---

## 10. Binary treatment with continuous outcomes

### 10.1 The setup
The paper first considers a two-group comparison:
- treatment vs. control,
- continuous outcomes,
- and a t-test for difference in means.

The experimenter must form prior beliefs about:
- the variance under treatment,
- the variance under control,
- and the minimum effect size worth detecting.

### 10.2 Homogeneous treatment effects case
If treatment and control outcome variances are equal, then the optimal design has:
- **equal sample sizes in treatment and control**.

This is the special case in which the common “split evenly” rule is valid.

### 10.3 Heterogeneous treatment effects case
If outcome variances differ across treatment and control, the optimal sample arrangement is **not** equal.

The key rule is:

> **The ratio of sample sizes should equal the ratio of standard deviations.**

So the group with the larger outcome variance should receive a larger share of the sample. This improves precision because noisier groups need more observations. fileciteturn6file0

### 10.4 Why the “30 per cell” rule is misleading
The authors show that a generic fixed-cell-size rule only makes sense under narrow assumptions about:
- the standard deviation of outcomes,
- the effect size the researcher wants to detect,
- and the desired power.

Using standard benchmark values (\(\alpha = 0.05\), power = 0.80), they show that:
- to detect a **1 standard deviation** effect, about **16 per cell** suffices,
- to detect a **0.5 standard deviation** effect, about **64 per cell** is needed.

So “30 per cell” is not a universal design principle; it simply corresponds to a particular, implicit effect-size assumption. fileciteturn6file0

---

## 11. Empirical illustration: List (2001) field auction experiment

The paper uses an experiment on sportscard auctions to illustrate inefficient equal allocation.

### 11.1 Context
The experiment compared:
- hypothetical bidding,
- versus actual bidding,
among non-dealers.

### 11.2 Design issue
The variance of bids in the hypothetical condition was roughly **twice** that of the actual condition, but the experiment used nearly equal sample sizes.

### 11.3 Consequence
With a 2:1 standard deviation ratio, equal allocation required a larger total sample than the optimal design to achieve the same power. The authors calculate that:
- the optimal design would allocate more subjects to the higher-variance hypothetical condition,
- and equal allocation slightly reduced power.

They also show that as variance differences grow, the efficiency loss from equal allocation becomes much larger. This example concretizes the paper’s main message: **equal cell sizes can be statistically costly**. fileciteturn6file0

---

## 12. Treatments with unequal costs

The article next relaxes the assumption that treatment and control observations cost the same.

### 12.1 Why this matters
In many real experiments:
- treatment is more expensive to administer than control,
- or costs vary across different interventions.

### 12.2 Key rule
When both variances and costs matter, optimal allocation depends on:
- standard deviations of outcomes, and
- relative cost per observation.

The main result is:

> **Sample sizes should be inversely proportional to the square root of relative costs, and directly proportional to relative standard deviations.**

This means:
- expensive groups should generally be smaller,
- noisy groups should generally be larger,
- and both considerations enter symmetrically through square-root scaling. fileciteturn6file0

### 12.3 Intuition
If treatment is costly, it may be inefficient to devote too many observations to treatment unless the variance structure justifies it. This extends the earlier “variance matching” rule by adding budget realism.

---

## 13. Parameter uncertainty and adaptive design concerns

### 13.1 The practical problem
All power calculations require prior assumptions about:
- variance,
- effect size,
- and sometimes treatment heterogeneity.

But those assumptions are often uncertain before the experiment starts.

### 13.2 Pilot studies and historical data
The authors recommend using:
- prior studies,
- historical data,
- or pilot experiments,
to estimate plausible design parameters.

### 13.3 Equivalence testing
The paper also notes that sometimes the goal is not to reject a null of zero effect, but to show that any effect is **small enough to be negligible**.

In that case, **equivalence testing** is more appropriate than standard null-hypothesis testing. This is an important methodological reminder because failure to reject a null does not, by itself, prove no meaningful effect. fileciteturn6file0

### 13.4 Adaptive designs
The authors mention the possibility of adjusting design choices as new information arrives during the experiment, including Bayesian and sequential approaches. These are more complex to implement, but can be attractive when sampling is expensive.

---

## 14. Further considerations: binomial outcomes

The paper then adapts the design logic to **binary outcomes**.

### 14.1 Why binary outcomes are special
For binary data, variance is tied directly to the mean through \(p(1-p)\). That changes the design implications.

### 14.2 Main rule under a null of equal means
If the null hypothesis is that treatment and control have the same binary outcome mean, then the variances are also equal under the null.

Therefore:

> **Equal sample sizes are optimal under the null of equal means for binomial outcomes.**

### 14.3 When allocation becomes unequal
If the null or alternative implies different success probabilities across groups, then variances differ and the same logic from the continuous case reappears:
- the group closer to \(p=0.5\) has higher variance,
- and should generally receive more observations.

This section shows that the equal-allocation rule for binary outcomes is conditional, not universal. fileciteturn6file0

---

## 15. Cluster-randomized designs

This is one of the most practically important sections.

### 15.1 Why cluster designs are different
In many field experiments, treatment is assigned at the **group level** (village, school, clinic, firm), while outcomes are measured at the **individual level**.

That creates **within-cluster correlation**, meaning observations inside the same cluster are not independent.

### 15.2 Intracluster correlation and variance inflation
The paper shows that the required sample size in a cluster design is inflated by a **variance inflation factor**:
- larger clusters increase redundancy,
- higher intracluster correlation increases redundancy further.

The main implication is that clustering can sharply reduce effective information content relative to the same nominal sample size with independent observations. fileciteturn6file0

### 15.3 Design recommendation
The authors emphasize:

> **When intracluster correlation is present, it is generally better to randomize over many small clusters rather than a few large clusters.**

This is a critical practical lesson for field work.

### 15.4 Optimal cluster size
The optimal number of subjects per cluster depends on:
- the ratio of within-cluster to between-cluster variation,
- the per-subject sampling cost,
- and the fixed cost of opening a new cluster.

The paper’s key rule is:

> **Optimal cluster size increases when within-cluster variation is large relative to between-cluster variation, and decreases when opening new clusters is cheap relative to sampling additional people within a cluster.**

Strikingly, the optimal cluster size is independent of the total budget; the researcher should first decide cluster size, then sample as many clusters as the budget allows. fileciteturn6file0

---

## 16. Varying treatment levels and continuous outcomes

This section shifts from binary treatment to a **continuous or multi-level treatment variable**.

### 16.1 Core logic
When treatment can vary in intensity, precision depends on the variance of the treatment variable itself. Therefore, the researcher should design the experiment to **maximize treatment variation** subject to the assumed functional form.

### 16.2 If the treatment effect is linear
If the researcher has strong prior reason to believe the treatment effect is linear, then the optimal design places observations at:
- the **minimum** treatment level,
- and the **maximum** treatment level,

with **equal allocation to the two extremes**.

The paper strongly challenges the instinct to spread observations evenly across intermediate levels. Under linearity, intermediate treatment values waste information because they reduce treatment variance. fileciteturn6file0

### 16.3 If the treatment effect is quadratic
If the researcher expects a quadratic relationship, then at least **three treatment levels** are needed:
- lower endpoint,
- midpoint,
- upper endpoint.

The optimal allocation is:
- one-quarter at the low end,
- one-half at the midpoint,
- one-quarter at the high end.

### 16.4 General polynomial rule
For higher-order polynomial relationships, the article states:

> **The number of treatment cells should equal the highest polynomial order plus one.**

So:
- linear → 2 cells,
- quadratic → 3 cells,
- cubic → 4 cells,
and so on. fileciteturn6file0

### 16.5 Ordinal/categorical treatment levels
If treatment levels are categories rather than a continuous dosage scale, allocation depends on **which contrasts are substantively important**.

Example:
- if one baseline condition is compared separately to two alternatives, the baseline may deserve a larger share because it enters two contrasts;
- if the key contrast is only between two non-baseline groups, the baseline may receive no observations in the optimal design for that specific comparison.

This section emphasizes that “optimal” depends on the question being asked, not just on the number of cells.

---

## 17. Empirical illustration: Karlan and List (2007) charitable giving

### 17.1 Study context
The paper discusses a field experiment on charitable fundraising where households were assigned to different matching ratios:
- 1:1,
- 2:1,
- 3:1.

### 17.2 Design interpretation
The authors argue that:
- if the researcher’s true interest were only in a **linear price effect**, the 1:1 and 3:1 endpoints would have been sufficient,
- and including the middle cell reduced efficiency.

### 17.3 Implication
A three-cell design can require substantially more observations than a two-endpoint design if the true goal is estimation of a linear effect. This example reinforces the broader design lesson:
- do not add treatment levels reflexively,
- add them only when needed to estimate the functional form of real interest. fileciteturn6file0

---

## 18. Final rules of thumb from the conclusion

The paper closes with a concise list of practical design rules. These are the central takeaways and are worth memorizing.

### Rule 1
With **continuous outcomes**, equal treatment/control allocation is optimal **only when variances are expected to be equal**, which corresponds to homogeneous treatment effects. fileciteturn6file0

### Rule 2
When variances are unequal, the **ratio of sample sizes should equal the ratio of standard deviations**. fileciteturn6file0

### Rule 3
When sampling costs differ across cells, the **ratio of sample sizes is inversely proportional to the square root of the relative costs**. fileciteturn6file0

### Rule 4
In cluster-randomized settings, optimal cluster size rises with the ratio of within-cluster to between-cluster standard deviation and falls with the square root of the ratio of per-subject cost to fixed cluster-startup cost. fileciteturn6file0

### Rule 5
When treatment is continuous and the researcher assumes a linear response, the sample should be split across the **endpoints** of the feasible treatment range, with no intermediate levels sampled. fileciteturn6file0

---

## 19. Major themes and conceptual insights

### 19.1 Precision is a design problem, not just a sample-size problem
The paper repeatedly argues that researchers focus too much on “how many observations” and not enough on:
- how the observations are allocated,
- how much treatment variation exists,
- and how much residual variance can be reduced.

### 19.2 Equal allocation is often a convenience, not an optimum
A major myth the article confronts is that balanced designs are always best. They are not.

### 19.3 Functional form assumptions matter
Optimal treatment-level allocation depends on whether the researcher assumes:
- linear,
- quadratic,
- or higher-order response patterns.

### 19.4 Costs and logistics belong in design formulas
Good design is not purely statistical. The paper explicitly integrates:
- differential treatment costs,
- cluster setup costs,
- and the feasibility of recruiting across cells.

### 19.5 The estimand should drive the design
This is perhaps the deepest message: experimental design must be tailored to the **specific contrast or parameter** the researcher wants to estimate.

---

## 20. Limitations and caveats acknowledged by the authors

The authors are clear that their rules are not universal. Important caveats include:
- effect sizes and variances are often unknown ex ante,
- multiple-hypothesis settings complicate allocation,
- reviewers may be uncomfortable with sparse intermediate treatment levels even when statistically optimal,
- and many design questions remain beyond the scope of the paper, including generalizability, strategy methods, repeated observations, heterogeneous treatment effects, and Bayesian/frequentist differences in design logic. fileciteturn6file0

---

## 21. Why this article matters

This article is valuable because it translates formal design theory into practical guidance for researchers running real experiments. It bridges:
- causal inference logic,
- statistical power analysis,
- and field/lab implementation decisions.

For students and researchers, the paper is especially useful because it teaches how to think about design **before data collection**, rather than treating power analysis as a mechanical afterthought.

---

## 22. Concise study guide summary

This article argues that many experiments are designed inefficiently because researchers default to equal cell sizes and conventional heuristics rather than optimizing allocation. The authors show that the optimal design depends on the outcome variance, treatment heterogeneity, sampling costs, clustering, and the structure of the treatment-response relationship. For continuous outcomes with unequal variances, sample sizes should be proportional to the standard deviations. For unequal costs, they should additionally be inversely related to the square root of relative cost. In cluster designs, intracluster correlation inflates variance, making many small clusters preferable to a few large ones. For continuous treatment levels, the best design usually maximizes treatment variance, which means assigning observations to the extremes when the expected relationship is linear. The paper’s overarching lesson is that experimental precision depends as much on smart allocation and treatment variation as on total sample size. fileciteturn6file0

---

## 23. Review questions

1. Why is equal allocation across treatment cells not always optimal?
2. Under what condition is equal treatment/control allocation optimal for continuous outcomes?
3. How should sample sizes be allocated when treatment and control variances differ?
4. How do unequal treatment costs change the optimal allocation rule?
5. What is the main efficiency problem in cluster-randomized designs?
6. Why are many small clusters often better than a few large ones?
7. How should treatment levels be allocated if the treatment-response relationship is assumed linear?
8. Why can intermediate treatment levels reduce efficiency under linearity?
9. How does the paper distinguish between power analysis and post-estimation significance testing?
10. What does the article suggest about the limitations of generic rules like “30 subjects per cell”?

---

## 24. Bottom line

The article is a methodological guide to building **more powerful, more efficient, and more purposeful experiments**. Its core lesson is simple but important: do not default to balanced cells and conventional habits. Design the experiment around the variance structure, the estimand, the costs, and the treatment-response form you actually care about.