# nd082-ent-project-2
Proyecto 2 para DevOps Engineer for Microsoft Azure Nanodegree Program

[![Python application test with Github Actions](https://github.com/adelriob/nd082-ent-project-2/actions/workflows/pythonapp.yml/badge.svg)](https://github.com/adelriob/nd082-ent-project-2/actions/workflows/pythonapp.yml)

[![Build Status](https://dev.azure.com/adelriob0110/Project-2/_apis/build/status/adelriob.nd082-ent-project-2?branchName=main)](https://dev.azure.com/adelriob0110/Project-2/_build/latest?definitionId=4&branchName=main)

# Overview

This is the second project of the course "DevOps Engineer for Microsoft Azure Nanodegree Program". With this project, the CI / CD process will be carried out through Azure Pipelines pipes.

## Project Plan

* A link to a Trello board for the project
    * https://trello.com/b/v1p899YD/projectflask
* A link to a spreadsheet that includes the original and final project plan
    * https://github.com/adelriob/nd082-ent-project-2/blob/main/project-management-template.xlsx

## Instructions

* Architectural Diagram (Shows how key parts of the system work)

![System architecture](screenshot/Diagram_Udacity_Project_2.png)

* Project cloned into Azure Cloud Shell

    * Open Azure Cloud Shell, create a SSH key pair by: ssh-keygen -t rsa;
    
    ![Create SSH](screenshot/ssh.JPG)

    * Copy and paste the public SSH key to github.com -> Settings -> SSH and GPG Keys -> New SSH Key
    
    ![Add SSH](screenshot/add_ssh.JPG)
    
    * Clone repository

    ![Clone repo](screenshot/git_clone.JPG)

* Project running on Azure App Service

    * Go to directory: cd nd082-ent-project-2/flask-sklearn 

    ![Directory](screenshot/directory.JPG)

    * Create virtual environment

    ![Environment](screenshot/environment.JPG)

    * Go to virtual environment

    ![Virtual Environment](screenshot/virt_env.JPG)

    * Run make all

    ![make all](screenshot/make_all.JPG)

    * Run app to verify

    ![Run App](screenshot/run_app.JPG)

    ![Run App](screenshot/run_app_2.JPG)

    * Create Webapp on Azure: az webapp up --sku FREE --name adelriob-flask --location "East US" 

    ![Create webapp](screenshot/create_webapp.JPG)

    ![Create webapp](screenshot/create_webapp_t.JPG)

    * Modify make_predict_azure_app.sh with the webapp name adelriob-flask in the POST target line

    ![adelriob-flask](screenshot/adelriob-flask.JPG)

    ![adelriob-flask](screenshot/adelriob-flask-2.JPG)

    * Performance TEST
    We use LOCUST to performance test of the apply.

        * Install Locust: pip install locust

        ![Install Locus](screenshot/install_locust.JPG)

        * Run Locust

        ![Run Locus](screenshot/run_locust.JPG)

        * Go to link: http://localhost:8089/ and simulate users

        ![Simulate](screenshot/simulate.JPG)

        ![Simulate](screenshot/simulate_2.JPG)

    * Github Actions and Azure Pipelines status

    ![Github Actions](screenshot/github_actions_pylint_pytest_ok.JPG)

    ![Github Actions](screenshot/azure_pipelines.JPG)


## Enhancements

In the future, the application will be moved to Azure Repos to keep all the flow from Azure Cloud.

## Demo 

Look at this demo of the application from youtube, below the link [HERE](https://youtu.be/0jcIIQIIKQI).


