# Blog_age_fairness
Jupyter notebook simulating fairness metric results by race/ethnicity group for a process that depends on age only.

2019 US Census population by age and race/ethnicity is downloaded, and used to simulate a process that depends on age but not on race/ethnicity.  A logistic regression model is constructed for the simulated process, and fairness metrics for race/ethnicity groups are calculated.  This example shows large metric discrepancies for the racial/ethnic groups due to age effects only.  These metric discrepancies arise from differences in base rates and model probability distributions.  

In a [Towards Data Science post](https://medium.com/towards-data-science/measuring-fairness-when-ages-differ-177d9597dd3b), I use this example to illustrate the importance of considering age effects when evaluating fairness metrics.  Differences that appear to be associated with race/ethnicity (or gender, etc.) may have age as a cause.  Deciding whether a model is fair or unfair requires understanding reasons for differences, and attempts to correct or adjust a model to optimize fairness metrics could have unintended consequences if age effects are not considered.
