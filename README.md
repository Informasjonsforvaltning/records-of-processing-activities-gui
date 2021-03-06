# Records of Processing Activities GUI

## Description

An application for managing records of processing activities.

## Installation and Usage

- Required tools to run this project:
  - Node.js and npm to run locally on a host machine
  - Docker and Docker Compose to run locally in a container

#### Running application locally on a host machine

- Install dependencies by running `npm install`
- Run `npm start` to start local development server

#### Running application in a Docker container

- Build a Docker container using the following command:
  - `docker build -t records-of-processing-activities-gui .`
- Run the container using the following comand:
  - `docker run -d -p 8141:8080 -e OIDC_ISSUER -e RECORDS_OF_PROCESSING_ACTIVITIES_URL -e FDK_REGISTRATION_BASE_URI -e ORGANIZATION_API records-of-processing-activities-gui`

#### Running application using Docker Compose

- Run the application using the following command:
  - `docker-compose up -d`

## Environment Variables

- `OIDC_ISSUER` - OIDC issuer URI
- `RECORDS_OF_PROCESSING_ACTIVITIES_URL` - Base URL of Records of Processing Activities backend
- `FDK_REGISTRATION_BASE_URI` - Base URI for registration clients
- `ORGANIZATION_API` - Base URL of Organization backend
- `SEARCH_HOST` - FDK portal main page URL
- `ADMIN_GUI_HOST` - FDK admin main page URL
