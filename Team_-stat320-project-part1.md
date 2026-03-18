# Impulsive Reaction Time between Casual and Top 150 Esports Players
Kiwi & Isabella

revealjs

<!-- Please note that this is not the final format for the presentation, just for the submission of Part 1 of the Project.  See the Project Presentation Template for a more complete version of the presentation slide requirements (but still read through the OVERVIEW) -->

<!--- Note: you will want to replace my instructions with your actual responses on each slide --->

## Research Question(s)

Write your research question(s) on this slide

> Is there a significant difference in population means of mean GO
> reaction time (ms) for super smash bros ultimate players that have
> competed in the Monterey and San Jose Counties for casual super smash
> bro gamers and for top 150(elite) super smash bro gamers?

## Description of Data

- Identify Population, Individuals, Sample

> Population: All super smash bros ultimate players that have competed
> in the Monterey and San Jose Counties  
> Case: smash bros ultimate player that has competed in the Monterey or
> San Jose Counties  
> Sample : 43 super smash bros ultimate players that have competed in
> the Monterey and San Jose Counties

- Identify Variables and Types, including new variables you will create
  \<\<\<\<\<\<\< HEAD

> Health and Lifestyle:  
> Sex - Male or Female (Qualitative)  
> Age_years (Quantitative)  
> Gaming_hr_week_ratio - Hours per week gaming (Quantitative)  
> Caffeine_Intake_mg_d - Reported caffeine intake (mg) per day
> (Quantitative)  
> Sleep_hrs - Typical hours of sleep per night (Quantitative)  
> Exercise_hours_week - Hours per week exercising (Quantitative)  
> Difference (Actual mean - Practice mean) of Cognitive measure test in
> milliseconds (ms):  
> SR_ROC_Mean_RT - Simple Reaction test (Quantitative)  
> ROC_Mean_Go_RT - Go/No Go test (Quantitative)  
> ROC_Mean_Valid_Cue_RT_ms - Posner Cueing test (valid cue)
> (Quantitative)  
> PP_ROC_Building_Test - Purdue Pegboard test (Quantitative)  
> Level of Gaming/Type:  
> Gaming (measured as Non-Gamer, Casual-SB, Elite-SB, FPS, MOBA)
> (Qualitative)  
> ======= Health and Lifestyle: Sex - Male or Female (Qualitative)
> Age_years (Quantitative) Gaming_hr_week_ratio - Hours per week gaming
> (Quantitative) Caffeine_Intake_mg_d - Reported caffeine intake (mg)
> per day (Quantitative) Sleep_hrs - Typical hours of sleep per night
> (Quantitative) Exercise_hours_week - Hours per week exercising
> (Quantitative) Difference (Actual mean - Practice mean) of Cognitive
> measure test in milliseconds (ms): SR_ROC_Mean_RT - Simple Reaction
> test (Quantitative) ROC_Mean_Go_RT - Go/No Go test (Quantitative)
> ROC_Mean_Valid_Cue_RT_ms - Posner Cueing test (valid cue)
> (Quantitative) PP_ROC_Building_Test - Purdue Pegboard test
> (Quantitative) Level of Gaming/Type: Gaming (measured as Non-Gamer,
> Casual-SB, Elite-SB, FPS, MOBA) (Qualitative) \>\>\>\>\>\>
> dee06a76a177a40dfbd0295d0fc6b101dbbe56d1 Abbreviations: SB (Super
> Smash Bros Ultimate), FPS (First Person Shooter), MOBA (multiplayer
> online battle arena)

- Describe how data was collected

> The participant collection included visiting local Monterey, San Jose,
> and CSUMB tournaments for esports, visiting the CSUMB library to ask
> people to join, and other non-random methods of obtaining
> participants.

## Summary Statistics and Graphics

Provide descriptions and inset values from R output.

![](Team_-stat320-project-part1_files/figure-commonmark/unnamed-chunk-2-1.png)

![](Team_-stat320-project-part1_files/figure-commonmark/unnamed-chunk-2-2.png)

                  response      Game    min       Q1  median      Q3     max
    1 Actual_Mean_Go_RT_ms Casual-SB 262.55 286.4125 315.275 339.200 494.950
    2 Actual_Mean_Go_RT_ms  Elite-SB 260.20 296.8000 322.750 379.225 612.421
          mean       sd  n missing
    1 323.8971 54.56114 24       0
    2 350.6801 84.25903 19       0

## Analysis

Provide analysis using parametric methods (will not be in your final
presentation)


        Welch Two Sample t-test

    data:  Actual_Mean_Go_RT_ms by Game
    t = -1.2005, df = 29.399, p-value = 0.1198
    alternative hypothesis: true difference in means between group Casual-SB and group Elite-SB is less than 0
    95 percent confidence interval:
         -Inf 11.10626
    sample estimates:
    mean in group Casual-SB  mean in group Elite-SB 
                   323.8971                350.6801 

## Failure of Parametric Methods

Describe why or provide evidence for why parametric methods are not
reasonable

> Parmetric methods are not reasonable for assessment becuase it
> violates the conditions for a t test, normality of sufficient sample
> size. Due to the right skew that we see in the histograms for both
> casual gamers and elite gamers. The small sample size of 24 for casual
> gamers, and 19 for elite gamers, which are both less than 30, we do
> not have sufficient sample sizes given our data with a heavy right
> skew. Therefore, we cannot use the t distribution as a model of the
> sampling distribution make parametric methods innappropriate to use
> for analysis.
