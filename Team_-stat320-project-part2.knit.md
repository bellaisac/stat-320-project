---
title: "Impulsive Reaction Time between Casual and Top 150 Esports Players"
subtitle: "Kiwi, Isabella"
author: "Kinesiology Department at CSUMB, Marine Science Department at CSUMB,"
format: 
  revealjs:
    theme: blood
embed-resources: true
html-math-method: mathml
execute: 
  warning: false
  echo: false
  error: true
---

## Motivation

<style>
#title-slide h1 {
  font-size: 2em;
}
</style>

- Esports as a field requires accuracy where one thousandth of a second can determine whether a team or person wins. Skills like quick reaction times increase the chances of succeeding in faster paced video games which require these skills (Ersin at al. 2022).  
- A recent study (Ziv et. al., 2022) found evidence that asking participants about their gaming status (gamer or non-gamer) positively affected performance for gamers and had an adverse effect on non-gamers in cognitive motor task performance. 


## Outline

- 

## Background  

- In the growing Esports industry, competitive Super Smash Bros Ultimate (SSBU) players require quick reactions and timely responses to stimuli.
- Professional Esports athletes practice 5-10 hours per day, nearly consistent with traditional sports and more than their casual counterpart (Emara et al. 2020).

![GX3 February 2026, Winners Semi-finals](images/2U4A2485.jpg){#id .class width=40% height=40%}


# Methods  
<!-- A single hashtag # will create a title type slide to create a clear distinction between sections of the presentation. -->

## Methods - Data Collection 

- Participant collection included visiting local Monterey, San Jose, and CSUMB SSBU tournaments to ask people to join, and other non-random methods of obtaining participants.  
- Conducted computerized practice assessment to get them accustomed to the software and then the actual congitive test to collect data on impulsivity via the GO/NoGO test  
- Casual SSBU players (play at least 4 hours per week of the game), Elite SSBU players (ranked top 150 in the world)  


## Methods - Variable Creation

- Measure of reaction time to an
- Mean GO reaction time: Difference between the actual mean GO reaction time (ms) and the practice mean GO reaction time (ms).  
![GO Prompt](images/go.png){#id .class width=40% height=40%}
![NoGO Prompt](images/nogo.png){#id .class width=40% height=40%}

## Methods - Analytic Methods

- We are planning on running a permutation test to obtain our statistics  
- Followed by a bootstrap interval to obtain our CI

## Methods - Analytic Methods

*Why did you use nonparametric methods?*  
  
- A skew across groups.   
- The small sample size within groups. ($n_{casual}$ = 24, $n_{elite}$ = 19)  
- T-Distribution would not be appropriate as a model of the null distribution with these conditions.  

# Results

## Summary Statistics and Graphics

- Boxplots of mean GO reaction time (ms) for smash bros ultimate players in the Monterey and San Jose Counties for casual SSBU players and for Elite SSBU players


::: {.cell}
::: {.cell-output-display}
![](Team_-stat320-project-part2_files/figure-revealjs/unnamed-chunk-1-1.png){width=960}
:::
:::


# Non-parametric Analysis

## Permutatation null distribution


::: {.cell}

:::



::: {.cell}
::: {.cell-output-display}
![](Team_-stat320-project-part2_files/figure-revealjs/null-dist-1.png){width=960}
:::
:::


- P-value = 0.1221

## Bootstrapping Confidence Interval


::: {.cell}
::: {.cell-output-display}
![](Team_-stat320-project-part2_files/figure-revealjs/bs-ci-1.png){width=960}
:::
:::


- Confidence Interval : (-73.2477177, 13.1057177)  
- Include negative, zero and positive numbers.  
- Casual can have mean GO reaction time faster, slower, or equal to that of Elite. 


# Summary  


## Conclusions  

- There no significant difference in population means of mean GO reaction time (ms) for SSBU players that have competed in the Monterey and San Jose Counties for Casual SSBU and for Elite SSBU players. 
- Weak evidence against the null hypothesis (p-value = 0.1221, $\alpha = 0.05$, $\bar{x}_{casual} - \bar{x}_{elite} =$ 26.7829693).    
- 100% of Casual mean GO reaction time is contained within 100% of Elite mean GO reaction time.   
- Convenient sample contains bias, cannot generalize to all super smash bros ultimate players.

## Future Work

Include a random sample to generalize to the larger populations  

Delve into the other variables not included such as:  
  - Other game types  
  - Other measures of reaction time  
  - Controller specific reaction speed  

## References {.smaller}
-  Emara, Ahmed K., et al. “Gamer’s Health Guide: Optimizing Performance, Recognizing Hazards, and Promoting Wellness in Esports.” Current Sports Medicine Reports, vol. 19, no. 12, Dec. 2020, pp. 537–45. DOI.org (Crossref), https://doi.org/10.1249/JSR.0000000000000787.  
- Ersin, A., Tezeren, H., Pekyavas, N., Asal, B., Atabey, A., Diri, A., & Gonen, I. (2022). The relationship between reaction time and gaming time in E-sports players. Kinesiology, 54(1), 36-42.  
- Ziv, G., Lidor, R. & Levin, O. Reaction time and working memory in gamers and non-gamers. Sci Rep 12, 6798 (2022). https://doi.org/10.1038/s41598-022-10986-3  


