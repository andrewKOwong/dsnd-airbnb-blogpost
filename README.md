# Analysis and modelling of Airbnb listings in Vancouver, BC, Canada from April 2021

## Table of Contents

1. Project Motivation
2. File Description
3. Libraries Required
4. Summary of Results
5. Acknowledgements

## Project Motivation

This project is part of the Udacity Data Scientist Nanodegree. The goal is to find a dataset and formulate a business question associated with it, prepare and analyze the data, and communicate the results in a blog post and a Github repo.

I chose a dataset of Airbnb listings from Vancouver, Canada spanning the month of April 2021. If a potential Airbnb host wanted to set a price for their listing, they might want to know what everyone else is setting their prices at, and what features of their listing might justify the price. The following three main questions guided the rest of the research questions in the analysis:

- Where are the Airbnb listings in Vancouver, and how are they priced?
- What features affect the price of an Airbnb listing?
- Can we fit a model to predict a listing’s price based on its features?

An associated Medium post is [here](https://medium.com/@aKOwong/its-really-mostly-about-the-bedrooms-a-brief-saunter-into-a-month-of-airbnbs-in-vancouver-9106617cb9e9).

## File Description

`README.md` - This file describing the repo.  
`project_notebook.ipynb` - Analysis and modelling Jupyter notebook.
`project_notebook.html` - HTML export of the notebook.
`data` - folder containing the data set, in which contains:

- `listings_summary.csv` and `listings.csv` - source of the features used in the analysis
- `reviews_summary.csv`, `reviews.csv`, `calendar.csv` - additional data provided not used in the analysis.
- `neighbourhoods.csv` and `neighbourhoods.geojson` - data describing the location of the neighbourhoods of Vancouver.

`blogpics` - folder containing exported data for the blog post on Medium.

## Libraries Required

`numpy` and `pandas` for data manipulation.  
`matplotlib` and `seaborn` for visualization.  
`geopandas` and `contextily` for map drawing.  
`scipy` and `statsmodels` for stats.  
`scikit-learn` for linear modelling.

## Summary of Results

- Most Vancouver AirBnb listings were located in Downtown.
- The median nightly price of a listing is 115 CAD, although the distribution of prices was right skewed.
- Of the quantitative variables, the price of a listing was most correlated with how many bedrooms/the size of an listing.
- Some listings appear to be mispriced, where the listed nightly price likely is intended as a monthly price for a longer term rental.
- A linear model was fit to predict price with R^2 score of 0.41.

## Acknowledgements

Data is from [Inside AirBnb](http://insideairbnb.com/).
