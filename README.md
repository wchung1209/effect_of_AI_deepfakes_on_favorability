# Measuring the Causal Effect of AI Deepfake Videos on Favorabilities of Public Figures
This is a project repo for DATASCI241: Experiments and Causal Inference project.

## Abstract 

This project designs and executes a causal experiment in which the effect of deepfake videos created by AI is measured as difference in favorability of the figures deepfaked between treatment and control groups. Using a randomized expreiment, survey analysis, and regression modeling, we delve into the causal inference and the implications of AI  deepfakes on the Internet. 

## Motivation

- As AI-generated content becomes more prevalent, its potential to shift opinions and polarize society grows, especially in politics.
- Prior academic work rarely uses rigorous experimental design to quantify these effects. Findings highlight risk and mitigation strategies for safe AI use.

**Objective**: Do deepfake videos of public figures saying controversial things reduce their favorability? Does labeling content as AI-generated (in a disclaimer) alleviate the negative effects (if any)?

## Experimental Design

Survey Panel: US general population, colelcted through PureSpectrum
Public Figures Tested: Joe Biden, Donald Trump, Mark Zuckerberg, Elon Musk
Groups:
- Control: Rates favorability with no video exposure
- Treatment 1: Rates favorability after seeing a deepfake video
- Treatment 2: Rates favorability after seeing a deepfake video with explicit disclaimer
Scale: 11-point Likert scale for each figure
Sample Size: 289 participants, demographics stratified to match US Gen Pop

## Analysis & Modeling

- Regression: Linear models compare favorability across experimental groups
- Covariates tested: Age group, gender, political party, industry of work

Key Model: $averagefavorability = treatment + agegroup + gender + politicalparty + industry$
We delve into variations with the key model in the regression experimentation.

## Results 

Overall, no statistically significant effect of deepfake videos or disclaimers for the full participant pool. By subgroup, we observe that those aged 65+ are significantly affected; disclaimers help alleviate this effect. Age and political party are more predictive of favorability than other covariates tested. While these stats are significant, sample size remains low overall and results may vary with prolonged or repeated exposure. 

<img width="914" height="360" alt="image" src="https://github.com/user-attachments/assets/5ac5d665-4a25-4201-9ee2-43a4894501b5" />
<img width="848" height="518" alt="image" src="https://github.com/user-attachments/assets/8373dbe3-7b85-4221-a11b-d4ac393e15ca" />
<img width="735" height="850" alt="image" src="https://github.com/user-attachments/assets/c67ea7e6-27d8-46df-96c5-586b3155dec1" />
<img width="564" height="726" alt="image" src="https://github.com/user-attachments/assets/c7a1f44f-f7ba-448a-98d9-f3c3699ecc9e" />

