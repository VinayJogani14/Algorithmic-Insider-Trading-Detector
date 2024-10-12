# Algorithmic-Insider-Trading-Detector

This project focuses on detecting potential insider trading activities using advanced data collection, analysis, and machine learning techniques. The core workflow involves retrieving, processing, and analyzing stock price and insider trading data to identify anomalies and potential illegal trading behavior. Key technical components include:

- **Data Collection**: Stock price data is sourced using the `yfinance` Python library, enabling the extraction of historical market data for specific tickers over a defined time period. Insider trading data is obtained from the SEC's EDGAR database, leveraging web scraping with `BeautifulSoup` and HTTP requests to parse Form 4 filings, which document insider trading activities.

- **Feature Engineering**: Raw data is transformed into features that are indicative of insider trading behaviors. Features include transaction volumes, trade timings, price movements post-insider trading reports, and historical price trends, creating a comprehensive dataset for analysis.

- **Anomaly Detection**: Statistical and machine learning models are employed to detect abnormal trading patterns that may indicate insider activity. Techniques include time-series analysis and unsupervised learning models, such as Isolation Forests and clustering algorithms, to flag unusual price and volume shifts in proximity to insider trades.

- **Machine Learning Models**: Supervised learning techniques are also utilized for predictive analysis, attempting to classify trades as suspicious or normal based on historical data. Models like Random Forests and Gradient Boosting are trained on labeled datasets to improve detection accuracy.

- **Visualization and Evaluation**: Key metrics and results are visualized using `matplotlib` and `seaborn` to provide insights into detected anomalies and model performance. Evaluation metrics such as precision, recall, and ROC curves are used to assess the effectiveness of detection models.

This project serves as a foundational framework for algorithmically identifying potential insider trading, with applications in financial compliance, regulatory monitoring, and quantitative finance research.


