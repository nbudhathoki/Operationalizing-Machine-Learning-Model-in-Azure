
# Operationalizing Machine Learning in Azure- Bank Marketing Campaigns

This dataset contains marketing campaigns of a bank in which we can analyze the data , and build some predictive models to find new strategic ways to improve the future marketing campaigns, and target the right customers. The data is related with direct marketing campaigns of a banking institution. The classification goal is to predict if the client will subscribe to a term deposit (variable y).

The goal of this project is to use the Azure ML tools to configure a cloud-based machine learning production model, deploy it, and consume it. We will also create, publish, and consume a ML pipeline in Azure.

## Architectural Diagram

Below is the architectural diagram followed for this project, starting from setting up proper authentication, training model by automl, deploying the best model, creating pipeline, consuming the model, enable logging in app insights, and swagger documentation. <br/>

<kbd><img src= "./images/architecture.png"> </kbd>

## Key Steps
### Step 1: Authentication:
I am using my Azure account for this project. The azureML workspace is created, and I am the owner of it with all the required access verified by Identity and Access Management (IAM) through AAD (Azure Active Directory). For security reason, my account id is greyed out. However, authentication is set up properly as the first key step: <br/>

<kbd><img src= "./images/access.png"> </kbd> <br/>

### Step 2: AutoML Experiment:
Before we set up autoML experiment, we need to make sure we have uploaded the dataset. The data set is uploaded from [this URL](https://automlsamplenotebookdata.blob.core.windows.net/automl-sample-notebook-data/bankmarketing_train.csv). We can preview the uploaded dataset: <br/>

<kbd><img src= "./images/dataset_uploaded.png"> </kbd> <br/>

After the dataset is uploaded, autoML experiment is set up. The completed experiment can be verified as: <br/>

<kbd><img src= "./images/exp_complete.png"> </kbd> <br/>

Best Model: VotingEnsemble is the best model with accuracy **0.92049** <br/>

<kbd><img src= "./images/votingEnsemble.png"> </kbd> <br/>

### Step 3: Deploy the Best Model:





## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
