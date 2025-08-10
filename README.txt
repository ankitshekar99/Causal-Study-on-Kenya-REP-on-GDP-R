
Empirical Economic Analysis
	

Project Overview
This project analyzes the impact of Kenya's Rural Electrification Programme (REP) on GDP growth using the Synthetic Control Method. The study covers the period 2003–2017 and includes 13 countries, with Kenya as the treated unit.
Link for data: https://www.kaggle.com/datasets/david780514/world-bank-world-development-indicators-1960-2023
What each file does:
1. Code: Causal Studies.qmd
2. Data: extract-worlddevelopment-indicator.xlsx

Dependencies:
Ensure the following R packages are installed before running the analysis:
library(haven)
library(ggplot2)
library(plm)
library(psych)
library(gplots)
library(car)
library(dplyr)
library(Synth)
library(tidyverse)
library(skimr)
library(readxl)
library(corrplot)
Steps to run code:
1. Load file( Causal Studies.qmd) into R Studio
2. Ensure the file extract-worlddevelopment-indicator.xlsx is in the same directory as the R code.

Based on the papers found in the References section.
Detailed Literature Review:
Economic growth is influenced by multiple interdependent factors, including human capital, macroeconomic stability, institutional quality, and technological progress. Barro (1996) highlights that higher education levels and life expectancy positively impact economic growth, while lower fertility rates contribute to increased per capita income. Strong legal institutions, secure property rights, and efficient government spending create an environment conducive to investment. Macroeconomic stability, characterized by low inflation and favorable terms of trade, further enhances economic performance. Additionally, democracy exhibits a non-linear relationship with growth, where initial increases in political rights stimulate economic expansion, but excessive democratization may hinder economic progress. Long-term growth is also driven by technological advancements and the diffusion of innovation, with human capital playing a crucial role in adopting new technologies. Thus, countries that prioritize education, institutional stability, sound fiscal policies, and technological progress tend to experience sustained economic development (Barro, 1996).
Electricity infrastructure plays a crucial role in facilitating economic growth, particularly in developing economies. Gituura (2024) examined Kenya’s electricity infrastructure from 2000 to 2020, finding a strong positive correlation (54.40%) between transmission line expansion and GDP, reinforcing the Keynesian view that infrastructure investments drive economic development. However, the study also highlights inefficiencies in electricity distribution, such as overcapacity in substations without adequate transmission infrastructure, which can lead to resource misallocation and economic inefficiencies.
Beyond Kenya, Bernard (2010) assessed the impact of rural electrification in Sub-Saharan Africa between the 1980s and 2010, revealing that despite decades of investment, connection rates and productive electricity use remain low. The study identifies three primary drivers for rural electrification: poverty alleviation, market failures due to low private-sector engagement, and political incentives to foster social and economic cohesion. However, Bernard (2010) warns that electrification alone does not guarantee economic growth unless paired with complementary investments in infrastructure and policies that enable productive electricity use.
Further supporting these findings, Khobai, Mugano, and Le Roux (2017) analyzed South African data from 1980 to 2013 and confirmed a long-term relationship between electricity allocation, economic growth, and trade openness. However, the impact of electricity infrastructure on economic performance is highly context-dependent, as illustrated by Lee, Miguel, and Wolfram (2020). Their study on Kenya and Rwanda (2012–2018) found that household electrification alone does not significantly enhance economic outcomes. Instead, the benefits of electricity access depend on broader economic and institutional factors, such as market efficiency, financial inclusion, and the regulatory environment.
Conclusion of Literature Review:
While electricity infrastructure is a key driver of economic growth, its impact is maximized when paired with efficient transmission networks, market-oriented policies, and institutional support. Policymakers should focus on modernizing transmission infrastructure and ensuring equitable access to electricity to unlock its full economic potential. Additionally, long-term growth strategies should integrate human capital development, macroeconomic stability, and institutional improvements to create a sustainable foundation for economic progress.
________________


References
Barro, R. J. (1996). Determinants of economic growth: A cross-country empirical study. NBER Working Paper No. 5698. National Bureau of Economic Research.
Bernard, T. (2010). Impact analysis of rural electrification projects in Sub-Saharan Africa. The World Bank Research Observer, 27(1), 33-51.
Gituura, P. (2024). Relationship between electricity infrastructure development and economic growth in Kenya. Journal of Energy Policy Studies, 18(1), 45-67.
Khobai, H., Mugano, G., & Le Roux, P. (2017). The impact of electricity price on economic growth in South Africa (1980–2013). International Journal of Energy Economics and Policy, 7(1), 108-116.
Lee, K., Miguel, E., & Wolfram, C. (2020). Does household electrification supercharge economic development? Evidence from Kenya and Rwanda (2012–2018). Journal of Economic Perspectives, 34(1), 122-144.