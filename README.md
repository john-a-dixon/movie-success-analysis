# Movie Success Analysis

## Overview

### Goal
Given data about movies, discern various trends for the stakeholder that'll help them understand what makes a movie successful. Then, using statistical analysis, test various hypotheses proposed by the stakeholder to verify (with certainty) what makes a movie successful, specifically with regard to MPAA Rating, Budget, and Revenue.

> _**Note**: The analysis uses data from 2000-2010 only._

### File Summary

- **_1-process.ipynb:_** Takes data from IMDb's publicly available dataset and processes it according to stakeholder specifications.
- **_2a-efficient-API.ipynb:_** Queries the TMDb API and stores the results in the `/Data` directory.
- **_2b-EDA.ipynb:_** Explores the TMDb API data to discern trends the stakeholder may find pertinent to their goals.
- **_3-SQL.ipynb:_** Processes all the gathered data into a MySQL database for the final hypothesis testing.
- **_4-hypothesis-testing.ipynb:_** Tests various stakeholder hypotheses to give them information about what makes a movie successful.

### Data Attribution
The data comes from two sources:
1. TMDb API
    <pre>
    <img src="https://www.themoviedb.org/assets/2/v4/logos/v2/blue_square_2-d537fb228cf3ded904ef09b136fe3fec72548ebc1fea3fbbd1ad9e36364db38b.svg" width="200" />
    </pre>
2. IMDb's publicly available dataset:
    <pre>
    Information courtesy of
    IMDb
    (https://www.imdb.com).
    Used with permission.
    Source: https://datasets.imdbws.com/
    </pre>

## Results

### Exploratory Data Analysis

At a high level, a few trends were apparent:
- Most of the data had no valid budget or revenue info. Those that didn't were filtered out in the end.
- There was a severe class imbalance within the data, where rated R was most represented while rated G was least represented.
- Though rated G movies were least represented, on average their revenue almost tripled their budget. In contrast, on average the revenue for rated R movies slightly doubled their budget.

### Hypotheses Testing

1. _Does the MPAA rating of a movie (G/PG/PG-13/R) affect how much revenue the movie generates?_
    - The MPAA rating affects the generated revenue. Rated G and PG movies generate the most revenue while rated R movies generate the least.
2. _Does a movie being over 2.5 hours long significantly affect its revenue?_
    - 
3. _Does a high rating (rated >= 7.0) affect whether a movie's revenue will exceed its budget?_
    - 

### Recommendations