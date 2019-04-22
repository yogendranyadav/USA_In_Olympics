# USA in the Olympics - Basic Data Exploration and Preparation

## Introduction:
This project uses the dataset called 120 years of Olympic history from
Kaggle. The objective is to analyze the performance of USA in the Olympics over
the years. Methods like Data Cleaning and Data Preparation were used to get the
data ready for analyzing. Key findings were the standings of USA with respect to
the Medals won, sports dominated by USA in the Olympics and the type of sports
with no medals won.

## Dataset:
The Dataset used here is called 120 years of Olympic history.It contains historical dataset on
the modern Olympic Games, including all the Games from Athens 1896 to Rio 2016.
- Source: Kaggle
- Location: https://www.kaggle.com/heesoo37/120-years-of-olympic-history-athletes-and-results
- Content:
     - The file athlete_events.csv contains 271116 rows and 15 columns. Each row corresponds to an
individual athlete competing in an individual Olympic event (athlete-events). The columns are ID,
Name, Sex, Age , Height, Weight, Team, NOC, Games, Year, Season, City, Sport, Event and
Medal.
     - The file noc_regions.csv contains 230 rows and 3 columns. The columns are NOC (National
Olympic Committee 3 letter code),Country name and Notes.

## Data Preparation and Cleaning:

- By initial analysis, we found that Age, Height, Weight and Medals had lot of missing values. The
column ‘Medal’ had 231333 missing values. This is fine because not all the participants can win a
medal. So replaced these values with ‘No Medal’.
- To get the region of the Team in the athlete events.csv, there was merge done for athlete events and
region dataset based on their NOC values.
- Problems – Some NOC present in the athlete events dataset does not associate to a country from the
regions dataset. But we can easily add them manually based on their TEAM Name. This was
performed to reduce the number of missing values in the dataset.

## Research Question:

The aim here is to get the overall performance of USA in Olympics for Summer and Winter Seasons. Also understand, sports that were dominated by the USA over the years and that needs more attention by the country to improve their performance in the Olympics.

