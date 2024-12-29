# STAR Dataset Analysis
This repository contains an analysis of the Student-Teacher Achievement Ratio (STAR) dataset, a large-scale educational experiment conducted in Tennessee. The analysis focuses on evaluating the impact of class size on student performance and investigates the randomization of treatment and control groups.

## Project Overview
The goal of this project is to:

* Assess the effectiveness of small class sizes in improving student test scores.
* Analyze the balance of covariates to evaluate the effectiveness of randomization.
* Quantify the impact of treatment through regression analysis while controlling for confounding variables.
* Explore race and teacher experience as determinants of student performance.

## Dataset Description
The STAR dataset consists of 5,786 observations and 19 variables. Key variables used in the analysis include:

* Test Score: Students' total scores on standardized tests.
* Class Size: Treatment indicator for small classes (small = 1) vs. regular classes (small = 0).
* Gender: Binary indicator (male = 1, female = 0).
* Free Lunch: Binary indicator for eligibility for free/reduced lunch.
* Race: Categorized as White/Asian or Black.
* Teacher Experience: Years of teaching experience.

## Key Insights
### Effectiveness of Small Classes:
* Students in small classes scored on average 13.55 to 14.31 points higher on standardized tests compared to those in regular-sized classes.

### Regression Analysis:
* Regression models confirmed the positive impact of smaller class sizes on test scores, even after adjusting for other variables.
* The significance of certain covariates, such as eligibility for free lunch, highlighted socioeconomic disparities in academic outcomes.

### Covariate Analysis:
* Covariates such as gender, race, free lunch status, and teacher experience were analyzed to assess randomization balance.
* Teacher experience was identified as unbalanced and was incorporated as a control variable in regression models.
* The relationship between teacher experience and test scores was found to be weak and highly dispersed across racial groups.

## Getting Started
1. Clone this repository: git clone https://github.com/username/STAR-Dataset-Analysis.git
2. Open the RMarkdown file STAR_Analysis.Rmd in RStudio.
3. Knit the file to generate a report in HTML, PDF, or Word format.

## Prerequisites
To replicate the analysis, ensure you have:
* R (version 4.0 or higher)
* RStudio
* Required R packages:
  * tidyverse
  * ggplot2
  * dplyr
  * knitr
  * rmarkdown

Install all necessary packages using:
install.packages(c("tidyverse", "ggplot2", "dplyr", "knitr", "rmarkdown"))

## References
Krueger, A. B. (1999). Experimental estimates of education production functions. The Quarterly Journal of Economics, 114(2), 497–532. doi:10.1162/003355399556052.

## Author
Julieta Pappano

Data Analyst and Public Policy Specialist, with a keen interest in leveraging data analysis to address policy and economic challenges.
