# Structural Break Analysis in Rolling Kendall Tau and Spearman Correlations in US Sentiment on

Published: 2025-03-12
Medium: [https://medium.com/@kyle-t-jones/structural-break-analysis-in-rolling-kendall-tau-and-spearman-correlations-in-us-sentiment-on-4556f27f1293](https://medium.com/@kyle-t-jones/structural-break-analysis-in-rolling-kendall-tau-and-spearman-correlations-in-us-sentiment-on-4556f27f1293)

## Business context

In digital humanities, computational methods enable the detection of shifts in discourse over time. This study uses structural break analysis on rolling Kendall Tau and Spearman correlations to identify regime changes in US sentiment of economic and political terms. Change point detection on the correlations provides insights into how relationships between economic terms and other discourses evolve, revealing structural shifts in economic narratives.

The primary dataset for this study consists of historical newspapers from *Chronicling America*, a digital archive maintained by the Library of Congress. This collection provides a rich textual record of U.S. journalism from the mid-19th to mid-20th century, capturing major economic and political shifts. We selected newspaper articles mentioning key terms related to Economy, Freedom, Liberty, and Democracy, creating a longitudinal dataset spanning over 100 years.

To quantify sentiment trends, we applied VADER, a lexicon-based sentiment analysis tool optimized for short texts. Each article's sentiment was classified along a polarity spectrum, and aggregated to construct yearly sentiment indices for our four key topics.

## About

Place the code for this article in this repository.
The original article export is saved as `article.md`.

## Files

Add your `.ipynb`, `.py`, `.yaml`, `.js`, `.ts`, or other project files here.

## Disclaimer

Educational/demo code only. Not financial, safety, or engineering advice. Use at your own risk. Verify results independently before any production or operational use.

## License

MIT — see [LICENSE](LICENSE).