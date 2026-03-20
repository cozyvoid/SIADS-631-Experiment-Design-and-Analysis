# Detailed Overview: *Social Comparisons and Contributions to Online Communities: A Field Experiment on MovieLens*

**Citation:** Yan Chen, F. Maxwell Harper, Joseph Konstan, and Sherry Xin Li (2010), *American Economic Review*, 100(4): 1358–1398.

---

## 1. Core purpose of the article

This article studies whether **personalized social comparison information** can increase contributions to an online community. The setting is **MovieLens**, a noncommercial online movie recommender system where users rate movies and, in return, receive personalized recommendations. The authors treat many user activities on the platform as forms of **public goods provision** because they benefit not only the acting user but also the broader community. fileciteturn7file0

The central problem is **undercontribution**. Many online communities rely on voluntary time and effort rather than monetary payments, so traditional public-goods mechanisms based on taxes, subsidies, or direct payments are not a natural fit. The paper asks whether a low-cost, scalable alternative—**personalized social information**—can motivate users to contribute more. fileciteturn7file0

---

## 2. Main research question

The article asks:

- Can informing users how they compare with similar others increase online contributions?
- Do different types of social information produce different behavioral responses?
- Do these responses differ for **low contributors**, **average contributors**, and **high contributors**?
- Can online communities use social information not only to increase quantity of activity, but also to increase **high-value, community-benefiting work**? fileciteturn7file0

---

## 3. Main findings in one paragraph

The study finds two headline results. First, when users receive **behavioral information** about how many movies they have rated relative to the **median** user in their cohort, users below the median increase their monthly ratings dramatically, while users above the median decrease theirs. Second, when users receive **outcome information** about their **net benefit score** relative to the **average** user, above-average users shift toward more community-benefiting actions, especially rating rare movies and updating the database. The authors conclude that **effective personalized social information can increase public-goods provision in online communities**, but the effects are heterogeneous and depend on who receives which kind of comparison. fileciteturn7file0L24-L27

---

## 4. Why this problem matters

The article begins by situating the problem in the broader landscape of online communities. Many communities depend heavily on a small minority of contributors, while most users consume content without producing much of it. The paper gives several examples:
- in Gnutella, a small minority shared nearly all content,
- in MovieLens, many movies had too few ratings for good recommendations,
- and in the Xerox Eureka system, only a minority of users contributed repair tips. fileciteturn7file0L28-L46

This matters because recommender systems, discussion forums, wikis, and other communities become more valuable when users contribute useful information. The challenge is not simply getting people to log in, but getting them to do work that benefits others.

---

## 5. The article’s intellectual framing

The paper sits at the intersection of:

- **public goods theory**
- **social comparison theory**
- **conformity theory**
- **inequality aversion / distributional concerns**
- **online community design**
- **field experimentation**

The authors argue that online communities differ from many classic public-goods environments because the platform designer can observe and personalize user behavior at very fine granularity. That creates an opportunity to tailor social information to users and motivate contribution without paying them. fileciteturn7file0L47-L76

### Theoretical roots the paper draws on
The introduction references several relevant traditions:
- **Festinger’s social comparison theory**: people compare themselves to others for guidance and self-evaluation.
- **Conformity models**: people move toward prevalent behavior.
- **Inequality aversion / distributional concern models**: people care about relative outcomes, not just absolute payoff.
- **Interdependent preference models**: utility depends partly on relative position within a distribution. fileciteturn7file0L77-L104

---

## 6. Structure of the article

The paper is organized into five main sections:

1. **MovieLens: An Overview**
2. **Experimental Design**
3. **A Theoretical Framework**
4. **Results**
5. **Conclusion**

There are also appendices with newsletter screenshots, the modified interface, and formal proofs. fileciteturn7file0L125-L129

---

## 7. Section I: MovieLens as the setting

### 7.1 What MovieLens is
MovieLens is an online movie recommender system run by the University of Minnesota. Users rate movies, and the system uses **collaborative filtering** to generate predictions and recommendations based on similarities among users’ past ratings. As of the date reported in the paper, the site had over 13 million ratings from just over 100,000 users. fileciteturn7file0L130-L143

### 7.2 Why ratings matter
A movie rating generates both:
- **private benefit** for the user, because it can improve recommendation quality for that user,
- **public benefit** for others, because it improves the database used by the recommender system. fileciteturn7file0L145-L154

The authors therefore classify rating as an **impure public good**.

### 7.3 Popular vs. rare movies
A crucial distinction in the article is between:
- **popular movies**, which are easier to find and rate and mainly help the rater,
- **rare movies**, which are harder to identify and rate but are more valuable to the community because they improve recommendations where data are scarce. fileciteturn7file0L155-L176

This is one of the paper’s most important design insights. Not all contributions are equal:
- rating a popular movie is relatively low effort and more privately beneficial,
- rating a rare movie is relatively high effort and more publicly beneficial.

### 7.4 Other contribution activities
The platform also allowed other actions:
- **invite a buddy**, which mostly benefits the user’s own experience,
- **update the movie database**, which primarily benefits the community and offers little direct private benefit. fileciteturn7file0L177-L197

This lets the experiment distinguish between:
- activities that mostly help oneself,
- activities that mostly help others,
- and activities that are mixed.

### 7.5 Why MovieLens is a good testbed
MovieLens is a useful experimental setting because:
- it is an online community with visible undercontribution problems,
- users’ actions can be tracked precisely,
- contributions vary in private/public benefit,
- and the platform can easily deliver personalized messages and interface changes. fileciteturn7file0L198-L206

---

## 8. Section II: Experimental design

This section explains the field experiment in detail.

### 8.1 Sample and recruitment
The researchers launched the study in June 2005. They selected users who:
- had logged in during the prior year,
- had rated at least 30 movies,
- and had allowed email contact. fileciteturn7file0L207-L226

From 5,488 eligible users, 1,966 were randomly invited by email, and 398 consented to participate. The paper notes an important **volunteer effect**: participants were more active raters than the overall user population, so the findings are best interpreted as about increasing participation among already engaged users rather than converting total lurkers into contributors. fileciteturn7file0L227-L246

### 8.2 Timeline
The **timeline figure on page 8** shows:
- a newsletter alpha test,
- recruitment and presurvey,
- personalized newsletter delivery,
- treatment implementation,
- and postsurvey,
with behavioral measurement focused on the month before and the month after the newsletter. fileciteturn7file0L207-L246

### 8.3 Presurvey
Participants first completed a 10-question presurvey used for two purposes:
1. estimating perceptions of benefits and costs from using MovieLens,
2. measuring users’ beliefs about how they compared with others in ratings and net benefit. fileciteturn7file0L247-L255

### 8.4 Three experimental groups
The 398 participants were randomly divided into three groups:

- **Rating Info**
- **Net Benefit**
- **Control** fileciteturn7file0L256-L264

#### Rating Info treatment
Users learned how many total movies they had rated relative to the **median** user in their membership cohort. The message explicitly said whether they had rated more, fewer, or about as many movies as the median. fileciteturn7file0L265-L279

#### Net Benefit treatment
Users learned their **net benefit score** relative to the **average** user in their cohort. The newsletter explained net benefit as the value and enjoyment received minus the time and effort contributed. fileciteturn7file0L280-L298

#### Control group
Users received only information about their own profile, such as the share of rated movies that were comedies and their average rating in that genre. They were **not** compared to other users. fileciteturn7file0L318-L327

### 8.5 Membership cohorts
To make comparisons more meaningful, the two treatment groups were split into three **cohorts** based on date of registration:
- **New**
- **Mid**
- **Old** fileciteturn7file0L265-L268

The paper argues this avoids comparing very new users to long-time veterans. **Table 1 on page 11** reports cohort sizes, weeks in MovieLens, and active user counts across treatment arms. fileciteturn7file0L269-L317

### 8.6 The action links embedded in the newsletters
All newsletters contained the same five behavioral links:
- rate popular movies,
- rate rare movies,
- invite a buddy,
- help update the MovieLens database,
- visit the home page. fileciteturn7file0L270-L279

What differed was the **social information** and how the options were framed. This allowed the researchers to observe whether different personalized comparisons shifted behavior toward different kinds of activities.

### 8.7 Modified interface
Users who visited the site saw a slightly modified MovieLens interface with those same shortcuts added to the sidebar. The **screenshot on page 37** shows the added “Rate Popular Movies,” “Rate Rare Movies,” “Invite a Buddy,” and “Maintain the Database” links in the shortcuts pane. fileciteturn7file0L328-L332

### 8.8 Postsurvey
A postsurvey one month later gathered:
- more MovieLens-related responses,
- General Social Survey style items,
- Big Five personality items,
- and demographics. fileciteturn7file0L333-L337

---

## 9. Why the treatment design is clever

The design is strong because it separates two fundamentally different mechanisms:

### 9.1 Behavioral comparison
“Here is how your **behavior** compares to others.”
- This should trigger **conformity** or norm-following.

### 9.2 Outcome comparison
“Here is how your **net outcome** compares to others.”
- This should trigger **distributional concerns**, altruism, or competitive/selfish responses.

The experiment therefore tests not only whether social information matters, but also **which kind of social information** matters for which kind of user.

---

## 10. Section III: Theoretical framework

This section develops the article’s economic model and formal hypotheses.

### 10.1 Static model of MovieLens use
The authors first model user utility as depending on:
- recommendation quality,
- fun from rating,
- nonrating fun (such as browsing or having a buddy),
- benefit from a validated database,
- minus the costs of rating and database updating. fileciteturn7file0L338-L391

The utility function combines private and public-good elements:
- recommendation quality rises with one’s own ratings and others’ ratings,
- rating has enjoyment value,
- database quality is a public good,
- rating and updating take time and effort.

### 10.2 Net benefit score
The **net benefit score** is a calibrated measure based on survey responses and behavioral data. The paper explains that scores shown in the newsletter were normalized to fall roughly in the 60–90 range. fileciteturn7file0L392-L397

This score is important because it converts a messy bundle of benefits and costs into a single outcome measure suitable for social comparison.

---

## 11. Rating Info treatment: conformity model

The paper then extends the static model into a two-period framework for the **Rating Info** treatment.

### 11.1 Behavioral mechanism
Users learn the median total rating count in their cohort and experience disutility from deviating from that norm. The idea comes from conformity theory: people want to move toward the perceived social standard. fileciteturn7file0L398-L429

### 11.2 Observation 1
The model predicts:
- the median user’s behavior stays the same,
- users below the median increase ratings,
- users above the median decrease ratings,
- the control group stays unchanged absent social information. fileciteturn7file0L430-L449

### 11.3 Proposition 1
If conformity pressure is strong enough:
- below-median users should rate at least as much as the median user after treatment,
- above-median users should rate at most as much as the median user,
- and overall the distribution should tighten around the median. fileciteturn7file0L450-L465

This is the article’s formal “conformity toward median behavior” hypothesis.

---

## 12. Net Benefit treatment: outcome comparison model

The paper next develops a model for the **Net Benefit** treatment.

### 12.1 Mechanism
Here the relevant social comparison is not behavior but **outcomes**. Users compare their net benefit score to the average user’s score and experience disutility from inequality. The model allows for heterogeneity in how much users care about others versus themselves. fileciteturn7file0L466-L490

### 12.2 Connection to inequality aversion
In a linear special case, the model resembles **Fehr-Schmidt inequality aversion**:
- below-average users want to improve their own position,
- above-average users may, if sufficiently charitable, be willing to help others rather than further increase their own advantage. fileciteturn7file0L491-L500

### 12.3 Proposition 2
The model predicts:
- **average and below-average** users should choose activities that improve their own net benefit, especially **rating popular movies**;
- **above-average** users may choose either self-benefiting or other-benefiting actions depending on their degree of charity/altruism;
- sufficiently charitable above-average users should be more likely to **rate rare movies** and **update the database**. fileciteturn7file0L501-L517

This proposition is the formal basis for the article’s main interpretation of the Net Benefit results.

---

## 13. Section IV: Results

This is the empirical core of the paper.

---

## 14. Result 1: Rating Info vs. Control

The first analysis compares how ratings changed in the Rating Info treatment relative to control.

### Main result
Compared to control, the change in movie ratings in the Rating Info group is:
- **significantly larger** for the below-median group,
- **significantly larger** for the median group,
- and not significantly different for the above-median group in that specific comparison. fileciteturn7file0L549-L567

### Big descriptive effect
The paper reports a striking descriptive pattern:
- below-median users show a **530% increase** in monthly ratings,
- above-median users show a **62% decrease**,
- and behavior converges toward the median. fileciteturn7file0L536-L544

The **bar charts on page 19** visually display this dramatic convergence for both all users and active users. fileciteturn7file0L536-L544

---

## 15. Result 2: Conformity in ratings

The next analysis tests whether the Rating Info treatment produced within-treatment conformity.

### Findings
Among active users:
- below-median users rated significantly more movies than the median group after treatment,
- the average distance from each active user to the cohort median shrank after the newsletter. fileciteturn7file0L568-L589

The evidence is therefore broadly consistent with conformity, though not perfectly. The article notes that the prediction for above-median users is weaker than expected because some above-median users still rated more than the median after treatment. This suggests the mechanism is not “pure conformity” alone.

### Role of conforming personality
Using postsurvey measures of conformity, the paper shows that the conformity result is stronger for users classified as **conforming types**. **Table 4 on page 22** reports that conforming users show statistically significant tightening toward the median, whereas nonconforming users do not. fileciteturn7file0L590-L614

---

## 16. Competition interacts with conformity

One of the paper’s most interesting refinements is that **competitive preferences** seem to interact with conformity.

### Interpretation
The site already encouraged users to rate more movies. So:
- for below-median users, conformity and competition point in the same direction,
- for above-median users, conformity suggests reducing ratings, but competition may encourage continued high activity. fileciteturn7file0L615-L623

### Evidence
The **graphs on page 23** show:
- below-median users increase ratings more when they are more competitive,
- above-median users reduce ratings less, or even slightly increase them, when they are more competitive. fileciteturn7file0L624-L635

This is a key theoretical contribution of the paper: social comparison effects may depend on an interaction between **conformity** and **competition**, rather than conformity alone.

---

## 17. Rating Info did not increase database updating

The paper notes that conformity theory predicts movement in ratings, but not necessarily any systematic difference in database updating. Consistent with that, users in the Rating Info treatment were not significantly differentiated by database-entry behavior, and control users even weakly exceeded treatment users in database entries. The authors suggest the novelty of the database feature may have drawn more attention in control. fileciteturn7file0L636-L641

---

## 18. Result 3: Net Benefit vs. Control

For the Net Benefit treatment, the first comparison is again against control.

### Main result
The increases in **popular movie ratings** are significantly greater than control for:
- **below-average** users,
- **average** users. fileciteturn7file0L642-L653

However, corresponding treatment-control differences for **rare movie ratings** are not significant. So the net benefit information clearly stimulates self-benefiting activity more than rare-movie public-good activity for those lower in the net-benefit distribution. fileciteturn7file0L654-L658

The **panel charts on pages 25–27** summarize popular ratings, rare ratings, and database entries before and after the newsletter. fileciteturn7file0L659-L678

---

## 19. Result 4: Inequality aversion / distributional concern

Within the Net Benefit treatment, users behaved differently depending on whether they were below average, average, or above average.

### Findings
The article reports:

1. **Popular movie ratings**: average users rate significantly more popular movies than below- or above-average users.
2. **Rare movie ratings**: above-average users rate significantly more rare movies than below-average users.
3. **Database entries**: above-average users provide **94% of the new database updates** in the Net Benefit treatment. fileciteturn7file0L679-L695

This is one of the clearest and most important empirical findings in the paper. It supports the idea that users who learn they are already above average in net benefit may shift toward **other-regarding contributions**, while average and below-average users respond by doing activities that help themselves more directly.

---

## 20. Altruism matters among above-average users

The authors then use postsurvey measures of altruism to split above-average users by altruism score.

### Table 6 findings
Among above-average users:
- popular movie ratings tend to **decrease** with altruism,
- rare movie ratings tend to **increase** with altruism,
- database entries also rise with altruism, though less strongly statistically. fileciteturn7file0L696-L717

The strongest significant difference is in rare movie ratings: highly altruistic above-average users contribute substantially more rare ratings than low-altruism above-average users.

### Interpretation
This supports Proposition 2: above-average users are not all the same. Some are selfish or competitive, while others are sufficiently charitable to shift effort toward community-benefiting activities.

---

## 21. Regression analysis

The paper reports pooled Tobit regressions to compare treatment effects and to assess covariates.

### Table 7
Compared to control:
- the **Rating Info** treatment significantly increases total ratings,
- the **Net Benefit** treatment does not significantly increase total ratings overall, which is sensible because it reallocates behavior across types of activity rather than simply increasing total ratings. fileciteturn7file0L718-L733

### Table 8
Regression results show:
- below-median users in Rating Info rate significantly more,
- competitive preferences strengthen this effect for below-median users,
- above-average users in Net Benefit rate fewer popular movies and contribute more database updates,
- high-altruism active users contribute more rare movie ratings. fileciteturn7file0L734-L760

The regressions also reveal some demographic patterns:
- active students rate fewer movies,
- male users contribute fewer rare movie ratings,
- older users contribute more rare movie ratings,
- more educated users contribute fewer database entries. fileciteturn7file0L761-L769

---

## 22. Anchoring as an alternative explanation

The authors explicitly test whether the results could simply be **anchoring**—that is, whether mentioning any number in a newsletter would change behavior.

They use the control condition for this check and find that the personal statistics shown in the control newsletters are not significantly correlated with later behavior. They therefore conclude that simple anchoring is unlikely to be the main mechanism. fileciteturn7file0L770-L774

This strengthens the interpretation that the effects are due to **social comparison**, not mere numeric suggestion.

---

## 23. Ranking stability

The article also checks whether users changed their relative ranking positions after treatment. Despite meaningful changes in absolute activity, rank correlations before and after remain high. That means the interventions altered contribution levels, but they did not radically reorder the hierarchy of contributors. fileciteturn7file0L775-L779

---

## 24. Section V: Conclusion and implications

The conclusion draws together both the practical and theoretical significance of the results.

### 24.1 Practical conclusion
Social comparison can serve as an **effective nonpecuniary incentive** in online communities. Designers can:
- classify users into meaningful segments,
- personalize messages,
- and use different social information for different groups. fileciteturn7file0L780-L804

### 24.2 Design recommendation
The authors suggest:
- use **median behavior information** for low contributors to increase ratings,
- use **net benefit comparison** for high-benefit users to channel them toward more community-benefiting tasks. fileciteturn7file0L790-L804

### 24.3 Theoretical contribution
The paper also argues that the literature on conformity may need to pay more attention to **competition**. When the social norm itself points toward the common good, competition can amplify conformity effects for low contributors but attenuate them for high contributors. fileciteturn7file0L805-L813

### 24.4 Limitation
A major limitation acknowledged by the authors is that MovieLens is a **leisure community**. The results may not automatically generalize to more work-oriented communities like Wikipedia or SourceForge. fileciteturn7file0L814-L819

### 24.5 Future research
The paper suggests studying:
- other online communities,
- other forms of social comparison such as leaderboards or status levels,
- and long-term effects on user growth and community production. fileciteturn7file0L819-L823

---

## 25. Key subtopics to remember

### Conceptual subtopics
- social comparison theory
- conformity
- inequality aversion / social preferences
- public goods in online communities
- personalized incentive design

### Design subtopics
- natural field experiment
- email-based intervention
- cohort-based comparison groups
- behavioral versus outcome information
- control group design

### Platform subtopics
- collaborative filtering
- private vs. public benefits of ratings
- popular vs. rare movies
- database updating as altruistic service

### Empirical subtopics
- treatment heterogeneity
- volunteer effects
- Tobit regression
- postexperiment survey measures of conformity, competitiveness, and altruism

---

## 26. Main strengths of the article

1. **Real-world field setting** rather than a purely artificial lab setting.
2. **Clear treatment contrast** between behavioral comparison and outcome comparison.
3. **Behavioral granularity**, distinguishing among multiple types of contribution.
4. **Personalization**, which makes the design directly relevant for online platform management.
5. **Theory-to-data integration**, using formal models to generate predictions and then testing them. fileciteturn7file0

---

## 27. Main limitations and caveats

The article is careful about several limitations:

- participants are volunteers and more active than the overall user base,
- the control and treatment newsletters differ somewhat in wording and framing, not only in social information,
- “invite a buddy” generated too little data for meaningful inference,
- the net benefit concept is more opaque than raw rating counts,
- results may not generalize to all online communities. fileciteturn7file0L227-L246 fileciteturn7file0L318-L327

---

## 28. Best concise interpretation

The article shows that **social information works, but it works differently for different people**.

- Tell low contributors how they compare to the median, and they work harder.
- Tell high-benefit users how they compare on outcomes, and some shift effort toward helping the community.
- The right message depends on whether you want more **quantity** of contribution or more **high-value** contribution.

That is the paper’s most important contribution for both platform design and behavioral economics.

---

## 29. Study guide summary

This paper studies whether personalized social comparisons can increase contribution in the MovieLens online community. The authors run a randomized field experiment with three groups: a Rating Info treatment, a Net Benefit treatment, and a control. The Rating Info treatment tells users how their total ratings compare with the median user in their cohort, while the Net Benefit treatment tells them how their overall net benefit compares with the average user. The authors model the first as a conformity problem and the second as an inequality-aversion or social-preference problem. Empirically, they find that below-median users respond strongly to median-rating information, increasing their movie ratings dramatically, while above-median users reduce ratings. In the Net Benefit condition, below- and average users mainly increase popular-movie ratings, while above-average users shift toward more community-benefiting tasks, especially rare-movie ratings and database updates. The paper concludes that personalized social information can be an effective nonpecuniary incentive in online communities, especially when tailored to different types of users. fileciteturn7file0L24-L27

---

## 30. Good review questions

1. Why do the authors describe many MovieLens activities as public goods?
2. Why is rating a rare movie more socially valuable than rating a popular one?
3. What is the difference between the Rating Info and Net Benefit treatments?
4. Why did the authors compare users within membership cohorts?
5. What does the conformity model predict for below- and above-median raters?
6. What does the outcome comparison model predict for above-average users with high altruism?
7. Why is the control group important for ruling out regression-to-the-mean and anchoring explanations?
8. What explains the stronger response of below-median users in the Rating Info treatment?
9. Why does the Net Benefit treatment not simply increase all ratings equally?
10. What design lesson does the paper offer to managers of online communities?

---

## 31. Bottom line

This article is a strong example of how behavioral economics and platform design can work together. Its key lesson is that **social comparison is not a one-size-fits-all intervention**. Behavioral comparison can pull low contributors toward the norm, while outcome comparison can redirect high-benefit users toward costly, prosocial tasks. For online communities that depend on voluntary labor, this is a powerful design insight.
