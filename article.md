---
author: "Kyle Jones"
date_published: "March 12, 2025"
date_exported_from_medium: "November 10, 2025"
canonical_link: "https://medium.com/@kyle-t-jones/structural-break-analysis-in-rolling-kendall-tau-and-spearman-correlations-in-us-sentiment-on-4556f27f1293"
---

# Structural Break Analysis in Rolling Kendall Tau and Spearman Correlations in US Sentiment on... In digital humanities, computational methods enable the detection of
shifts in discourse over time. This study uses structural break...

### Structural Break Analysis in Rolling Kendall Tau and Spearman Correlations in US Sentiment on Economic and Political Terms from 1850--1963
In digital humanities, computational methods enable the detection of shifts in discourse over time. This study uses structural break analysis on rolling Kendall Tau and Spearman correlations to identify regime changes in US sentiment of economic and political terms. Change point detection on the correlations provides insights into how relationships between economic terms and other discourses evolve, revealing structural shifts in economic narratives.

### Methodology
The primary dataset for this study consists of historical newspapers from *Chronicling America*, a digital archive maintained by the Library of Congress. This collection provides a rich textual record of U.S. journalism from the mid-19th to mid-20th century, capturing major economic and political shifts. We selected newspaper articles mentioning key terms related to Economy, Freedom, Liberty, and Democracy, creating a longitudinal dataset spanning over 100 years.

To quantify sentiment trends, we applied VADER, a lexicon-based sentiment analysis tool optimized for short texts. Each article's sentiment was classified along a polarity spectrum, and aggregated to construct yearly sentiment indices for our four key topics.

#### Rolling Kendall Tau and Spearman Correlations
We computed rolling Kendall Tau and Spearman correlations over a ten-year window to capture temporal trends in the association between "Economy" versus \[Freedom, Liberty, and Democracy\]. Kendall Tau is a rank-based correlation measure robust to non-linearity and outliers, while Spearman's correlation assesses monotonic relationships, making it useful for capturing broader trends.

The rolling correlations were computed over a 10 year rolling window for Kendall Tau and Spearman correlation coefficients relative to Economy.

#### Structural Break Detection
Change point detection was performed using the Binary Segmentation algorithm from the ruptures package. This method effectively identifies multiple breakpoints by iteratively segmenting the data by using the binary segmentation algorithm with an L2 cost model, which detects points where the mean structure of the data shifts significantly.

#### Visualization and Interpretation
The results were visualized by plotting the rolling Kendall Tau and Spearman correlations over time.


### Results
The structural break analysis revealed significant shifts in the correlation patterns between "Economy" and related topics. The detected breakpoints correspond to known historical and economic events, suggesting shifts in discourse alignment:

- Some breakpoints coincided with major economic recessions, indicating changes in how economic discussions were framed relative to other topics.
- Other breaks aligned with technological advancements, policy changes, or sociopolitical movements, suggesting shifts in the influence of economic discourse.

Comparing Kendall Tau and Spearman correlations:

- Kendall Tau correlation shifts often aligned with structural changes in discourse ranking, indicating shifts in relative importance.
- Spearman correlations provided a broader view of changing monotonic relationships, capturing trends in discourse emphasis over time.

### Discussion and Implications
This study applied time series and correlation techniques to sentiment analysis to identify structural shifts in discourse. The rolling Kendall Tau and Spearman correlation methods combined with change point detection offer a scalable framework for analyzing historical trends in text data. By identifying points of discourse transformation, scholars can contextualize linguistic and thematic shifts within broader historical narratives.

Future research could extend this approach by:

- Incorporating additional linguistic features beyond term frequencies, such as sentiment analysis or topic modeling.
- Expanding the time window to test for stability across different scales.
- Applying the method to other domains, such as political discourse or scientific communication.

This analysis underscores the evolving nature of economic narratives and the methodological potential of digital humanities in uncovering these transformations.
