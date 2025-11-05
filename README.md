🧮 Reliability of Odds Ratios Confidence Intervals

Authors: Bryce Anderson, Miles Standish, Lormel Bationo, and Jordon Silcox
Date: March 2025

🔍 Overview

This project evaluates the reliability of three widely used odds ratio (OR) confidence intervals — Woolf, Gart, and Agresti — under both normal and extreme sampling conditions. We also assess how Welch’s t-test adjustment (typically used for unequal variances) can stabilize coverage rates for these intervals in small-sample or unbalanced scenarios.

To test performance, we ran 10,000 Monte Carlo simulations across 2,352 unique parameter combinations, varying sample sizes, probabilities, and odds ratios.

📊 Key Insights

🧩 Gart’s OR confidence interval performed the most reliably overall, especially for small sample sizes or low odds ratios.

⚖️ Welch’s adjustment improved stability and reduced bias, particularly when the standard Z-based confidence intervals failed under unequal variance conditions.

💡 Agresti’s interval showed strong performance in small samples but became less consistent as sample sizes increased.

🧠 Woolf’s interval, while historically foundational, proved less reliable unless the true OR was near 1.

💊 Real-World Application

We validated our findings on a clinical trial dataset investigating a treatment for rheumatoid arthritis.
Across six different confidence interval methods, all intervals excluded 1.0, indicating statistically significant treatment effectiveness.
Welch-adjusted intervals were slightly wider, reflecting their robustness under potential heteroscedasticity.

Techniques: Monte Carlo simulation, odds ratio analysis, Welch’s t-test, coverage rate evaluation

Languages: R (tidyverse, ggplot2, plotly)

Simulation scale: 10,000 × 2,352 = 23.5M total iterations

Focus: Improving inference reliability for categorical data and small-sample designs
 This paper seeks to determine the reliability of three different odds ratios:
 Woolfe’s OR confidence interval, Gart’s OR confidence interval, and the Agresti
 OR confidence interval, using a variety of normal and extreme parameters.
 Along with finding reliable confidence intervals, this paper also seeks to de
termine the performance of the two-sample t-test Welch’s adjustment when
 applied to the three different OR confidence intervals. Through our study, we
 found that the Gart’s OR confidence interval performed the best when dealing
 with small sample sizes and odds ratios. We also found that Welch’s adjust
ment helped provide more consistent confidence intervals when working with
 small odds ratios. To achieve these results we performed 10,000 Monte Carlo
 simulations on 2352 different combinations of our chosen parameter values.

## View the full paper  
[Download/view the PDF](FinalDraft.pdf)


