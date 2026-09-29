**week 1 - intro**

*what is machine learning?*
- the essence of machine learning: we take characteristics from a dataset (*features*) and the output we want to predict (*target*), put it int a ML algorithm and the model learns the pattern itself (*training*/*fitting a model*) --> extract patterns from data

- once we have a model, we can use it to predict targets which we don't know the output

-----------------------
*ML vs Rule-Based Systems*
- in the second one we extract rules ourselves and write them in code (hard-coded)
- in ML the rules are learned automatically from data and the outcome is the input -> the predictions are probabilities, to make a decision is necessary to define a threshold

-----------------------
**supervised ML**
- feature matrix (X) --> 2 dim array --> rows are observations, columns are the features
- target variable (y) --> vector --> each row of X it contains the answer
- *the model is denoted as g*
- *The goal of supervised machine learning is to come up with this function g such that when we apply it to X, the output is as close as possible to the target variable*
            g(x)~= y


**types of supervised training**

- regression
    - g returns a number

- classification
    - the output is a category 
        - binary: exactly two categories (0, 1)
        - multiclass: more than 2

- ranking
    - score/probabilities

-----------------------
**CRISP-DM**: *Cross_Industry Standard Process for Data Mining*

- methodology that describes how ML projects should be organized

    1. Business Understanding: identify the problem and also: do we actually need ml? if yes, some number needs to be attached to the KPI
    2. Data Understanding: does this source really work? is the data reliable? is it large enough?
    3. Data preparation: extracting features, cleaning and removing noise, building pipelines, apply transformations, convert to tabular format
    4. Modeling: try and train different models and select the best one
    5. Evaluaiton: measure how well the model performs
    6. Deployment: roll out the model to production

    - iteration:
        - start simple
        - learn from the feedback
        - improve

-----------------------------