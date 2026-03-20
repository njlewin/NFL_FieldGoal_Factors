# What Actually Predicts NFL Field Goal Success?

A few months ago I mentioned to my girlfriend that it's common knowledge kicking field goals in Denver is easier because of the thin air. She had a very reasonable response: *"...Really?"*

Having just covered statistics in my MBA coursework, I decided to find out. This project analyzes 10 years of NFL data using hypothesis testing and linear regression to determine what factors actually drive field goal success.

## Key Findings

* **Denver's altitude advantage is a myth.** No statistically significant impact on field goal success was found.
* **Outdoor kicks are harder.** Field goals attempted outdoors are 5.5% less likely to be converted than indoor kicks, all else being equal.
* **Kickers are getting better.** Success rates have improved roughly 0.3% per season over the last decade.
* **Weather matters at specific stadiums.** Gillette Stadium (New England) and Huntington Bank Field (Cleveland) reduce conversion probability by 4.5% and 5.9% respectively. EverBank Stadium (Jacksonville) and Nissan Stadium (Nashville) increase it by 5.4% and 4.6%.
* **The Ravens, Steelers, and Chiefs are outliers.** Their field goal conversion rates are 10.2%, 8.2%, and 6.2% higher than the league baseline — driven by elite kickers (Tucker, Boswell, Butker) and exceptional coaching stability.

The final model achieved a ROC-AUC score of 0.77.

## View the Analysis

[Full Analysis](https://njlewin.github.io/NFL_FieldGoal_Factors/) — rendered, no code

[Jupyter Notebook](https://github.com/njlewin/NFL_FieldGoal_Factors/blob/main/NFL_FieldGoal_Factors.ipynb) — full code and methodology

## Data

Data sourced from [nfl\_data\_py](https://github.com/nflverse/nfl_data_py).

## Methods

* Exploratory data analysis
* Hypothesis testing
* Linear regression with stadium, team, weather, and environmental controls

