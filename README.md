# Estimating State Populations Using the 2022 ACS Data

## Overview

This repo leverages data from the 2022 American Community Survey (ACS), obtained through IPUMS USA, to estimate the total number of respondents in each state. The focus is on respondents whose highest educational attainment is a doctoral degree. Using the ratio estimator approach, California is taken as the reference state to calculate proportional estimates for other states.

## Key Components

### Data:
- The dataset includes educational attainment levels for respondents, with a specific focus on those holding doctoral degrees (using the EDUCD variable, where EDUCD = 116 indicates a doctoral degree).
- State-level data is extracted using the STATEICP variable, representing state codes.

### Method(Ratio Estimator Approach):
- California serves as the reference state, where both the total number of respondents and the number of respondents with doctoral degrees are known.
- The ratio of doctoral degree holders to total respondents in California is used to estimate the total population for other states based on their number of doctoral degree holders.

### Comparison:
- The estimated total number of respondents is compared to the actual respondent counts for each state.
- The comparison reveals discrepancies, which are analyzed to understand the influence of regional differences in education and demographics.


## Statement on LLM usage

LLMs such as ChatGPT were not used for this paper. 
