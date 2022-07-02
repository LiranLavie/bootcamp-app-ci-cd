Weight Tracker App CI-CD

![Demo](docs/build-weight-tracker-app-demo.gif)

This project consists of using Azure Pipelines to configure a complete CI/CD pipeline for the WeightTracker application.


## Configuration
1. Source code is stored in [**Github**](https://github.com/LiranLavie/bootcamp-app-ci-cd)
2. Adding two yaml pipelines:  **weight-tracker-ci** and **weight-tracker-cd**
3. CI pipeline will trigger automatically on every commit.
4. The CI pipeline archive the source directory and store the build in Azure Artifacts.
5. The CD pipeline deploy to Staging using Continuous Deployment and to Production using Continuous Delivery.
6. To enable manual approval i created two environments in the azure devops portal and added the **Approvals** option for the Production environment.
7. The CD pipeline will deploy the app to the environment using ansible playbook file named **app_deploy_playbook.yml**


