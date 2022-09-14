[![Python application test with Github Actions](https://github.com/IrisStream/project-2-azure/actions/workflows/main.yml/badge.svg)](https://github.com/IrisStream/project-2-azure/actions/workflows/main.yml)
# Overview

Python-based machine learning application using the Flask web framework. The model will predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on.

## Project Plan

* [Trello dashboard](https://trello.com/b/8Tt1zmdW/udacity-azuredevops)
* [spreadsheet](https://docs.google.com/spreadsheets/d/1XFMMsncwQbGezandp_MkGfrga6Fc4ainkcWSCCbG25A/edit?usp=sharing)

## Instructions

![diagram](./images/diagram.png)

* Project running on Azure App Service
``` bash
az webapp up --sku F1 -n <web_app_name>
```

![az webapp](./images/az_webapp.png)

* A screenshot of Azure Azure App Service

![azure web app](./images/project-2-iris.png)

* Project cloned into Azure Cloud Shell

![git clone](./images/git_clone_cloudshell.png)

* Passing tests that are displayed after running the `make all` command from the `Makefile`

![make all](./images/make_all.png)

* Output of a test run

![predict](./images/github_action_build.png)

* Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).

![home page](./images/home_page.png)

* Running Azure App Service from Azure Pipelines automatic deployment

![azure devops deploy](./images/azure_devops.png)

* Locust testing

![locust](./images/locust.png)

* Successful prediction from deployed flask app in Azure Cloud Shell.  [Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:

![test cloudshell](./images/test_cloudshell.png)

* Output of streamed log files from deployed application

![stream log](./images/stream_log.png) 

## Enhancements

* Add more test to CI pipeline
* Build infrastructure using IaC
* Apply Blue-green deployment

## Demo 

[Youtube link](https://www.youtube.com/watch?v=0EVQ4y_59GU