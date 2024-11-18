# Analysis of Forecasted Population Growth in Emerging Markets

### Overview

In developing nations, large and young populations are strong indicators of future economic growth. As the labor force expands, the economy must similarly grow to support the increasing population. The purpose of this analysis is to examine recent trends in population growth and forecast future trends, aiming to uncover key indicators that highlight specific regions or countries that present promising opportunities for investment in emerging markets.

---

## Table of Contents
1. [Data](#Data)
2. [Requirements](#Requirements) 
3. [Executive Summary](#Executive-summary)

---

## Data
The data for this ananlysis was sourced primarily from [Gapminder](https://www.gapminder.org/)

- [GNI per Capita](../my_data/gni_clean.csv)
- [Population](../my_data/pop_clean.csv)
- [Internal Investment](../my_data/internal_clean.csv)
- [Foreign Investment](../my_data/foreign_clean.csv)

### Data Dictionary


|Feature|Type|Dataset|Description|
|---|---|---|---|
|growth_rate_last_20|float|pop_clean| The growth rate of the population over the last 20 years.
|growth_rate_2050|float|pop_clean| The forecasted growth rate of the population by 2050.
|growth_rate_last_20|float|gni_clean| The growth rate of GNI per capita over the last 20 years.
|growth_rate_2050|float|gni_clean| The forecasted growth rate of GNI per capita by 2050.
|avg_investment|float|internal_clean| The average internal percentage of GDP invested in fixed assets.
|total_investment|float|internal_clean| The total internal percentage of GDP invested in fixed assets.
|avg_investment|float|foreign_clean| The average foreign investment as a percentage of GDP.
|total_investment|float|foreign_clean| The total foreign investment as a percentage of GDP.

---

## Requirements

- A programming environment such as Jupyter Lab
- pandas
- numpy
- matplotlib.pyplot
- An internet connection to access the data sets on [Gapminder](https://www.gapminder.org/)

---

## Executive Summary
In developing nations, several factors can play a role in shaping economic prospects. Large and young populations serve as strong indicators of potential economic growth, as they signify a growing labor force that can drive productivity and consumption. However, for economies to harness this potential, they must expand concurrently to accommodate the increasing population.

This analysis focuses on recent trends in population growth across developing regions and offers forecasts for the coming decades. By also examining factors such as internal investment in fixed assets, I aim to identify specific regions or countries that present promising opportunities for investment in emerging markets.

Our study involves a comprehensive review of historical population data, socioeconomic indicators, and existing investment landscapes. I will utilize statistical modeling techniques to project future population trends, enabling us to pinpoint areas where economic growth is likely to occur.

#### Purpose
I set out to find countries or regions likely to see economic growth. Specifcally I attempted to find patterns that would indicate where economic growth might concentrate. Factors such as a growing population are one part of the formula, however regions that are also investing in their own fixed assets are more likely to grow their economies.
  
#### Methods
I sampled population data from 195 countries dating back to 2004. Once I had these values I subtracted them from current populations and divided the result by the 2004 populations. This gave a rate of population growth over the last 20 years. I next did the same for future population levels, subracting the population today from the forecasted population in 2050. I sorted by both these rates to show which countries had grown the most over the last two decades and which were forecasted to grow the most through 2050. 

Next I analyzed data on internal and foreign investment on nearly 200 countries. By summing the total rates of investment per country and dividing by the number of years in the table I was able to calcualte an average investment rate as a percentage of GDP for internal and external investment. Sorting by these values I could see which countries were investing the most on their fixed assets and which were receiving the most foreign investment.

#### Findings
I found that over the last twenty years of the top ten countries which saw the largest rates of population growth, six were in Africa. When I looked at the forecasted rates of population growth, I found that of the top ten countries all ten were in Africa. This indicated Africa, across the continent, is forecasted to see the largest increase in young labor supply of any region in the world over the next 25 years.

I also found that of the top ten countries when sorted by internal investment in fixed assets, three of them were in Africa. This is a good indication that the region of Africa should expect to see increases in economic growth in the coming decades.

#### Next Steps
While the increases in population and the indications of internal investment are good signs for coming economic expansion in Africa, more analysis is needed on other economic factors. Africa, while resource rich, is still a poor region with political and economic instability. A good place to start would be to analyze trends in education, employment, as well as more robust analyses than GNI per capita to determine the strength of the middle class.
