## Steps run the application and all the resources created

1. clone the repository https://github.com/cchukwu/glover.git
2. go into the directory glover/article-api-app/ to access the application files, Dockerfile, docker-compose and Makefile added

## Running the application using a makefile with docker-compose

1. Command to run / start the application. In the directory glover/article-api-app/ Run `make compose-up`
2. To stop the app using docker-compose. Run `make compose-down`

## Provision the infrasturctures

The `glover/infrastructure/infra/` directory contains the scripts to spin up the following infrastructures.

1. GKE Cluster
2. Cloud Storage
3. Google Container Registry
4. Google Cloud Database

## Provision the cloud-storage

There is a `glover/infrastructure/cloud-storage/` folder which contains the terraform codes for creating the cloud-storage to keep the terraform state files.
