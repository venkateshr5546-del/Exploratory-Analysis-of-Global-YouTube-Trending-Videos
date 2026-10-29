# Exploratory Analysis of Global YouTube Trending Videos

A data analysis project exploring trends in YouTube videos across countries. The project focuses on understanding video popularity and engagement using views, likes, comments, categories, and country-level comparisons.

> **Data note:** Any small CSV files or graph images previously created for demonstration are illustrative/synthetic, not official YouTube observations. Replace them with a verified dataset before reporting findings or drawing conclusions.

## Project Objectives

- Explore the structure and quality of a YouTube trending-video dataset.
- Clean records and prepare fields for analysis.
- Identify popular videos and categories.
- Examine relationships between views, likes, and comments.
- Compare trending-video records across countries, when country data is available.
- Visualize key patterns with charts.

## Example Visualizations

The project can include these plots:

1. Top 10 videos by views
2. Most popular video categories
3. Distribution of video views
4. Views versus likes
5. Views versus comments
6. Correlation heatmap for engagement metrics
7. Trending videos by country
8. Average views, likes, and comments

The charts should be regenerated from the dataset used in the final analysis. Some plots require fields such as `country`, `category_id`, `views`, `likes`, and `comment_count`.

## Dataset

Use an authentic dataset and cite its source in your report. One possible source is the [YouTube Trending Video Dataset on Kaggle](https://www.kaggle.com/datasets/rsrishav/YouTube-Trending-Video-Dataset).

Dataset schemas can vary. Check the column names and country coverage before running the analysis. Do not upload private data, credentials, or API keys to this repository.

## Tools and Libraries

- Python
- Jupyter Notebook or Google Colab
- pandas
- NumPy
- Matplotlib
- Seaborn

## Getting Started

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Add the dataset

Download the dataset from its source and place the CSV file in your project data folder, for example:

```text
data/
└── youtube_trending.csv
```

Do not commit a large dataset unless its license and repository limits allow it. If necessary, include instructions for downloading it instead.

### 4. Run the analysis

Open your notebook in Jupyter or Google Colab, load the CSV, inspect its columns, perform cleaning, and run the visualization cells.

Example data-loading code:

```python
import pandas as pd

df = pd.read_csv("data/youtube_trending.csv")

print("Dataset shape:", df.shape)
print(df.head())
print(df.info())
print(df.isna().sum())
```

Adjust the file path and column names to match the dataset you downloaded.

## Suggested Project Structure

```text
youtube-trending-analysis/
├── README.md
├── notebooks/
│   └── youtube_trending_analysis.ipynb
├── data/
│   └── README.md
├── images/
│   ├── top_10_videos_by_views.png
│   ├── popular_video_categories.png
│   ├── views_distribution.png
│   ├── views_vs_likes.png
│   ├── views_vs_comments.png
│   ├── engagement_correlation_heatmap.png
│   ├── trending_videos_by_country.png
│   └── average_video_engagement.png
└── requirements.txt
```

This is a suggested structure; change it to match the files actually present in your repository.

## Data Cleaning Checklist

- Review column names and data types.
- Check for duplicate records.
- Inspect missing values.
- Convert engagement columns to numeric values where appropriate.
- Parse date/time fields when available.
- Check for impossible or invalid values.
- Document any rows or columns removed and why.

Keep a copy of the original source data separate from the cleaned data, and make the cleaning process reproducible.

## Analysis Questions

- Which videos have the highest view counts in the selected dataset?
- Which categories appear most often among trending records?
- How are video views distributed?
- Do videos with more views generally receive more likes or comments?
- Which engagement metrics are correlated?
- How does the number of trending records differ by country, if country information is available?

Answers should be based on calculations from the authentic dataset, not on illustrative charts.

## Reproducibility

Record the dataset source, download date, relevant license, filtering rules, cleaning decisions, and software requirements. Dataset coverage and values can change between releases.

## Contributors

- **Sanjai R** — `814725243154`
- **Venkatesh R** — `814725243182`

## License

Add a license appropriate for your code and confirm the dataset's license separately. A repository license does not automatically grant permission to redistribute third-party data.
