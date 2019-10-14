## Overview

This repository contains the second assignment for the Scientific Programming course MSB1015 in 2019. This assignment is supposed to cover the aspects of R Markdown, Git, SPARQL, PLS, model assessment and reproducibility by building a regression model to predict the boiling point of aliphatic alkanes using Partial Least Squares regression model.

## Installation

The assignment is implemented as interactive notebook R Markdown file integrating plots, code and comments using RStudio. 
The HTML report can run inside any modern web browser. No need to install any special software to run the report.

### Software version
RStudio 1.1.456
R (64bit) 3.5.2

### Steps

1.  Make sure you have RStudio and R installed on your system.
2.  Download the repository from the releases tab.
3.  Unzip the zipped source file.
4.  Open the file "index.rmd" in Rstudio
5.  Explore the file

## Used Packages

| Package                | Description                                                                          |
|-------------------------|--------------------------------------------------------------------------------------|
| WikidataQueryServiceR   | run SPARQL query against Wikidata                                            |
| rJava   | required for rcdk                                           |
| rcdk   | cheminformatics library                                            |
| randomForest   | Random forest machine learning library                                            |
| caret   | Classification And REgression Training library                                           |
| dplyr   | data manipulation library                                            |
| stringr   |     string manipulation library                                        |
| pls   |  Partial Least Squares regression library                            |
| measurements   | library to convert to many units                                            |
| DT   | generate interactive data tables                                          |


## The SPARQL query

We used a SPARQL quert against Wikidata to retreive a list of all alkanes with their corresponding SMILE strings and boiling point with the corresponding unit.

## Data preprocessing
The temprature units were unified by converting Fahrenheit and Celesius units to Kelvin using 'measurements' package, the all rows and columns containing NA values where removed.

## Data Splitting
80% Training set 
20% Training set 

## The regression model
Two models were used to predict the boiling point:
Partial Least Squares model
Random Forest model

## Model performance evaluation
Several measure were used to assess the models:
 - Root Mean Square Error of prediction
 - R square
 - Plot the measured values against the predicted values
 
 
## Results
Random forest model showed better performance that PLS model by both acheiving higher R square value and lower RMSEP.


## References

1.	Wiener, H., Structural determination of paraffin boiling points. Journal of the American Chemical Society, 1947. 69(1): p. 17-20.
2.	Hernández, D., et al. Querying wikidata: Comparing sparql, relational and graph databases. in International Semantic Web Conference. 2016. Springer.
3.	Guha, R. and M.R. Cherto, rcdk: Integrating the CDK with R. 2017.
4.	Wehrens, R. and B.-H. Mevik, The pls package: principal component and partial least squares regression in R. 2007.



## Github pages

You can access the assignment HTML page through Github pages on the following URL:

[https://a-ammar.github.io/MSB1015-Assignment2/](https://a-ammar.github.io/MSB1015-Assignment2/)


## Authors

Ammar Ammar 

Supervised By: Prof. Egon Willighagen
