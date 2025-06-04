# Employee Sentiment and Engagement Analysis

This project analyzes employee sentiment using textual data from emails/messages and derives insights on engagement and flight risk, along with basic predictive modeling.

## Project Structure

- `sp_test.csv`: Raw dataset containing employee communication data.
- `labeled_dataset.csv`: Cleaned and sentiment-labeled dataset.
- `Employee_Sentiment_and_Engagement_Analysis_Final_Report.docx`: Final report containing methodology, analysis, visualizations, and insights.
- `countplot.png`: Bar chart showing distribution of sentiment labels.
- `lineplot.png`: Line chart showing monthly sentiment trends.

## Steps Performed

1. **Data Wrangling**
   - Loaded and inspected the dataset.
   - Combined `Subject` and `body` into `full_text`.

2. **Sentiment Labeling**
   - Used NLTK’s VADER for sentiment classification (`Positive`, `Negative`, or `Neutral`).

3. **Exploratory Data Analysis (EDA)**
   - Visualized sentiment distribution and monthly sentiment trends.

4. **Employee Score Calculation**
   - Mapped sentiment to numerical values and calculated monthly sentiment scores per employee.

5. **Employee Ranking**
   - Identified top 3 positive and negative employees per month.

6. **Flight Risk Identification**
   - Flagged employees with at least 4 negative messages in a 30-day window.

7. **Predictive Modeling**
   - Built a Linear Regression model to predict sentiment score using message count and average length.
   - R² Score: 0.713 | RMSE: 1.84

## Requirements

- Python 3.x
- pandas, numpy, seaborn, matplotlib, nltk, scikit-learn

## How to Run

1. Clone this repo or use the notebook environment.
2. Ensure required libraries are installed.
3. Run each cell in sequence to reproduce the results.
