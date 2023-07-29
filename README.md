# yulu_hypothesis-testing
performed hypothesis testing on certain viewpoints on data from yulu

## Table of Contents
- [Introduction](#introduction)
- [Objective](#objective)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Notebooks](#notebooks)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction
The Yulu Hypothesis Testing project focuses on conducting hypothesis tests to validate assumptions and make data-driven decisions. This repository contains Jupyter notebooks and code for performing hypothesis testing on various datasets related to Yulu bike-sharing data.

## Objective
The main objectives of this project are:
- Explain the concept of hypothesis testing and its applications in data analysis.
- Use hypothesis testing to validate claims and draw conclusions from Yulu bike-sharing data.
- Utilize statistical tests to support decision-making and optimize business strategies.

## Features
- Hypothesis testing for means, proportions, and other statistical measures.
- One-sample, two-sample, and paired sample tests to compare different datasets.
- Interpretation and visualization of hypothesis test results.

## Technologies Used
- Python 3
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- SciPy
- Statsmodels

*(Feel free to add or modify the list of technologies based on the tools and libraries used in your project)*

## Installation
To run the Yulu Hypothesis Testing notebooks locally, follow these steps:

1. Clone the repository to your local machine using the following command:
   ```
   git clone https://github.com/raghav1saboo/yulu_hypothesis-testing.git
   ```

2. Navigate to the project directory:
   ```
   cd yulu_hypothesis-testing
   ```

3. Install the required dependencies using the following command:
   ```
   pip install -r requirements.txt
   ```

## Usage
1. Open Jupyter Notebook to access the hypothesis testing notebooks:
   ```
   jupyter notebook
   ```

2. In the Jupyter Notebook interface, navigate to the "notebooks" directory and open the desired notebook.

3. Run the code cells in the notebook to perform hypothesis testing on Yulu bike-sharing data.

*(If there are specific usage instructions or guidelines for your project, provide them here)*

## Dataset
Describe the Yulu bike-sharing dataset(s) used in this project. Mention their sources, formats, and any data preprocessing steps performed. You can also provide links to the original datasets or mention how to obtain them.

## Notebooks
List the available Jupyter notebooks and their purposes. For example:
- `one_sample_test.ipynb`: Demonstrates one-sample hypothesis testing on Yulu bike-sharing data.
- `two_sample_test.ipynb`: Illustrates two-sample hypothesis testing for comparison between datasets.

*(Add any additional notebooks relevant to your project)*

## Contributing
Contributions to this project are welcome. If you find any issues or have improvements to suggest, please feel free to open an issue or create a pull request.

## License
This project is licensed under the [MIT License](LICENSE).

## Contact
If you have any questions or need further assistance, you can reach me via email at [your_email@example.com](mailto:your_email@example.com).

*(Replace 'your_email@example.com' with your actual email address)*

---

You can copy and paste this template into a new file named "README.md" in the root of your "yulu_hypothesis-testing" repository. Customize the content to match the specifics of your project, such as the objective, features, technologies used, dataset, notebooks, and contact details. Additionally, consider providing examples of hypothesis tests performed on Yulu bike-sharing data in the notebooks to showcase the significance of the analysis in making data-driven decisions.

About Yulu

Yulu is India’s leading micro-mobility service provider, which offers unique vehicles for the daily commute. Starting off as a mission to eliminate traffic congestion in India, Yulu provides the safest commute solution through a user-friendly mobile app to enable shared, solo and sustainable commuting.

Yulu zones are located at all the appropriate locations (including metro stations, bus stands, office spaces, residential areas, corporate offices, etc) to make those first and last miles smooth, affordable, and convenient!

Yulu has recently suffered considerable dips in its revenues. They have contracted a consulting company to understand the factors on which the demand for these shared electric cycles depends. Specifically, they want to understand the factors affecting the demand for these shared electric cycles in the Indian market.

How you can help here?

The company wants to know:

Which variables are significant in predicting the demand for shared electric cycles in the Indian market?
How well those variables describe the electric cycle demands
Dataset:

Dataset Link: yulu_data.csv

Column Profiling:

datetime: datetime
season: season (1: spring, 2: summer, 3: fall, 4: winter)
holiday: whether day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
workingday: if day is neither weekend nor holiday is 1, otherwise is 0.
weather:
1: Clear, Few clouds, partly cloudy, partly cloudy
2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
temp: temperature in Celsius
atemp: feeling temperature in Celsius
humidity: humidity
windspeed: wind speed
casual: count of casual users
registered: count of registered users
count: count of total rental bikes including both casual and registered
Concept Used:

Bi-Variate Analysis
2-sample t-test: testing for difference across populations
ANNOVA
Chi-square
How to begin:

Import the dataset and do usual exploratory data analysis steps like checking the structure & characteristics of the dataset
Try establishing a relation between the dependent and independent variable (Dependent “Count” & Independent: Workingday, Weather, Season etc)
Select an appropriate test to check whether:
Working Day has effect on number of electric cycles rented
No. of cycles rented similar or different in different seasons
No. of cycles rented similar or different in different weather
Weather is dependent on season (check between 2 predictor variable)
Set up Null Hypothesis (H0)
State the alternate hypothesis (H1)
Check assumptions of the test (Normality, Equal Variance). You can check it using Histogram, Q-Q plot or statistical methods like levene’s test, Shapiro-wilk test (optional)
Please continue doing the analysis even If some assumptions fail (levene’s test or Shapiro-wilk test) but double check using visual analysis and report wherever necessary
Set a significance level (alpha)
Calculate test Statistics.
Decision to accept or reject null hypothesis.
Inference from the analysis
