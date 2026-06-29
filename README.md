# Twitter Sentiment Analysis

I worked on this project to understand how tweets can be classified as positive or negative using different machine learning models. The dataset used here is Sentiment140, and the main goal was to compare traditional ML models with a BERT-based approach.

Along with the notebook work, I also prepared visual outputs and a Power BI reporting workflow so the project is easier to explain and present.

## What I Did

- Loaded and cleaned the Sentiment140 tweet dataset.
- Converted the raw CSV data into Parquet format while working locally, mainly to make repeated analysis faster.
- Preprocessed tweet text for NLP tasks.
- Trained and compared Logistic Regression, Random Forest, XGBoost, and DistilBERT.
- Checked model performance using accuracy, precision, recall, F1 score, and confusion matrices.
- Created charts for final model comparison.
- Prepared a Power BI dashboard workflow and a simple pipeline architecture diagram.

## Model Results

DistilBERT gave the best F1 score in my final comparison.

| Model | F1 Score |
|---|---:|
| DistilBERT | 0.8029 |
| Logistic Regression | 0.7708 |
| XGBoost | 0.7573 |
| Random Forest | 0.7066 |

## Visuals

### BERT Confusion Matrix

![BERT Confusion Matrix](_bert_confusion.png)

### Final F1 Score Comparison

![Final Model Comparison](_bert_f1_ranking.png)

### Data Pipeline Architecture

![Twitter Sentiment Analysis Data Pipeline Architecture](Twitter%20Sentiment%20Analysis%20Data%20Pipeline%20Architecture.drawio.png)

## Files in This Repository

- `twitter_sentiment_project.ipynb` - main notebook for cleaning, preprocessing, modeling, and evaluation
- `Final Documentation.pdf` - final project documentation
- `_bert_confusion.png` - confusion matrix for the BERT model
- `_bert_f1_ranking.png` - model comparison chart
- `Twitter Sentiment Analysis Data Pipeline Architecture.drawio.png` - pipeline architecture diagram
- `training.1600000.processed.noemoticon.csv.zip` - compressed Sentiment140 dataset file

## Note About Large Files

Some local files are not included in this repository because they are larger than GitHub's normal upload limit:

- `Twitter_Sentiment_Analysis.pbix`
- `training.1600000.processed.noemoticon.parquet`
- `training_1600000.parquet`

The Parquet files can be recreated from the dataset during preprocessing. The Power BI file is kept separately because of its file size.

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- XGBoost
- DistilBERT
- Power BI

## Dataset

This project uses the Sentiment140 dataset. In this dataset, negative tweets are labeled as `0` and positive tweets are labeled as `4`.

## Author

Renu Bala
