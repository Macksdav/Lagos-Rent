# Lagos Rent Prediction

A data science and machine learning project focused on understanding and predicting residential rental prices across Lagos, Nigeria. The project combines web scraping, data cleaning, feature engineering, and predictive modeling to estimate rent based on property characteristics such as location, number of bedrooms, bathrooms, furnishing status, and property type.

## Project overview

The real estate market in Lagos is highly dynamic, and rent varies widely based on location, property size, and amenities. This project aims to build a practical price prediction model using real listing data from PropertyPro.NG, helping to uncover the main drivers of rental prices and create a scalable framework for similar markets.

The workflow includes:

- Scraping property listings from a real estate website
- Cleaning and structuring the raw data
- Transforming housing attributes into usable features
- Building and comparing predictive models
- Identifying the most important features influencing rent

## Problem statement

Rental prices in Lagos can differ significantly between neighborhoods and property categories. A buyer, renter, or investor often wants a quick estimate based on the type of property and its characteristics. This project addresses that need by building a model that predicts rent from available listing attributes.

## Dataset

The project uses scraped property listings stored in:

- `data/lagos-rent.csv`
- `data/nigeria-rent.csv`

Key fields include:

- `Title`
- `Price`
- `City`
- `Neighborhood`
- `Bedrooms`
- `Bathrooms`
- `Toilets`
- `Serviced`
- `Newly Built`
- `Furnished`

The raw data is cleaned and transformed into a modeling-ready dataset before training the prediction model.

## Project structure

```text
Lagos-Rent/
├── 1 Web Scraper.ipynb
├── 2 Lagos Extracting and Cleaning.ipynb
├── 3 Data Preprocessing.ipynb
├── 4 Model Building.ipynb
├── Feature Importance.ipynb
├── data/
│   ├── lagos-rent.csv
│   ├── nigeria-rent.csv
│   └── name of city.csv
├── requirements.txt
├── tools/
└── README.md
```

## Workflow

1. Web scraping: collect rental listings from PropertyPro.NG
2. Data extraction: pull relevant housing attributes from each listing
3. Cleaning: standardize formats, convert strings to numeric values, handle missing values
4. Preprocessing: prepare features for modeling
5. Modeling: train and compare regression models
6. Evaluation: assess prediction quality with validation metrics
7. Feature importance: analyze which variables most affect rent prices

## Models used

The project evaluates and compares several machine learning algorithms, including:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost
- LightGBM
- Other scikit-learn based regressors as needed

The final model is selected based on performance using appropriate regression metrics.

## Tech stack

- Python
- pandas
- NumPy
- scikit-learn
- XGBoost
- LightGBM
- BeautifulSoup
- Matplotlib
- Seaborn
- Jupyter Notebook

## Setup

Clone the repository and install dependencies:

```bash
git clone <repository-url>
cd Lagos-Rent
pip install -r requirements.txt
```

## Running the project

Open the notebooks in order:

1. `1 Web Scraper.ipynb` – scrape listing data
2. `2 Lagos Extracting and Cleaning.ipynb` – process and clean collected listings
3. `3 Data Preprocessing.ipynb` – prepare training data
4. `4 Model Building.ipynb` – train and evaluate the rent prediction model
5. `Feature Importance.ipynb` – inspect the most important predictors

## Key insights

This project is designed to uncover the living conditions and property characteristics that most strongly influence rent in Lagos, including:

- location and neighborhood
- number of bedrooms and bathrooms
- furnishing and servicing status
- whether the property is newly built
- overall property size and category

## Use cases

This kind of model can be used for:

- estimating fair rent prices
- supporting real-estate decision-making
- comparing neighborhood values
- analyzing housing affordability trends
- building automated property valuation tools

## Future improvements

Potential next steps include:

- collecting more recent listings across multiple Nigerian cities
- adding geospatial features and map-based analysis
- deploying the model as a small web app
- improving prediction accuracy with more advanced ensemble methods
- adding a user-friendly dashboard for rent estimation

## License

This project is intended for educational and portfolio use. If you plan to reuse or redistribute it, please verify the relevant licensing or source restrictions tied to the data source and scraped content.

## Author

Built as a practical data science project to explore real estate pricing patterns in Lagos and apply machine learning techniques to housing market analysis.
