# <span style="color: ##0101DF;">OPENCLASSROOMS - Data Scientist course </span> 

#### Student: Kokou AGBOTO

#### Mentor: Chemseddine Nabti

#### Date: 03/23/2022


# Project 7: Implement a scoring model
Credit **Scoring** is a risk analysis tool for granting credit. Based on statistical methods, it takes into account a lot of information relating to the
loan applicant to assess the risk of non-repayment. On a reference basis of known past loans, the tool assigns a score to each client, which makes it possible to
classify it as solvent or non-solvent with respect to a fixed threshold probability.

### Trust
In most cases when a credit application is refused to a client, this one does not always agree; since the refusal criterion is not justified.

### Transparency of information
The new European regulation on the protection of personal data entered into force on May 25, 2018 (https://www.cnil.fr/fr/reglement-europeen-protection-donnees).
Article 12 specifically deals with "Transparency of information and communications and modalities for exercising the rights of the data subject".

### Performance
The quality of the reference data is therefore very important. The aim is to have a database that is as representative as possible of the situations to be dealt with. The techniques and
methods used to build the model obviously have a significant impact on its performance. No model is perfect and we will always meet
cases of misprediction.

The technical challenge is to minimize these cases and to be clearer to customers, in order to have a friendly relationship with them.

## Project
We propose here to create a Credit Scoring tool based on Machine Learning technologies. Machine Learning has a reputation for being intransparent and
closer to a black box. This does not favor its acceptance with regard to the first two points mentioned above.
Nevertheless, enormous progress has been made to date and the field of Machine Learning offers very interesting solutions to improve the understanding of the processes of
decision.

## Modelization
The objective is twofold:

The model must make it possible to define the probability of default of repayment of a credit on the basis of information relating to the customer.
It must also offer a certain level of transparency concerning the data and their processing in order to implement methods for interpreting the variables
(global and local interpretability with the SHAP library). We modeled the tool using supervised learning technologies.

## Application

Beyond the technical aspects, the transparency of the tool is also characterized by the possibilities of interaction with it in order to carry out analyzes
complementary on the basis of the proposed results.

For example, we want to be able to compare 2 similar files whose credit granting predictions are different and visualize the variables that influenced the decisions.
You may also want to perform simulations to estimate the degree to which a file has been refused and identify the discriminating criteria.
We deployed the model through a web application using **FastAPI** for the backend and **streamlit** for the frontend.

# Plan
The project was split into two parts.

### Part 1

The first part of the project consists in carrying out the exploratory analysis of the data and their processing and the simulation of the different models (in two jupyter notebook files).

**Notebook 1: Dataset preparation and feature engineering and exploratory analysis notebook**

**Notebook 2: Simulation notebook and model comparison**


### Part 2
Python files related to application design.

**1. MyApi.py**: Using modern and fast (high performance) web-based **FastAPI** framework for API building (backend part) with Python-3.10.2 version at build time and python file **CreditData .py** a python class of essential features that describe a client.

**2. app.py**: Using the **streamlit** framework for designing the application (frontend part).


The deployment of the script is carried out via the Heroku platform. The application can be loaded with the following link:
https://credit-scoring-streamlit-ak.herokuapp.com/

## <span style="color: ##0101DF;"> Skills assessed in this project </span> 

#### 1. Present your modeling work orally
#### 2. Create a dashboard to present your modeling work
#### 3. Write a methodological note to communicate your modeling approach
#### 4. Use code release software to ensure model integration
#### 5. Deploy a model via an API in the web
