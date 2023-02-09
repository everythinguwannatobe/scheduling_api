# SCHEDULING API (Rails)

## _USER REQUIREMENTS_
There are mainly two types of requirements - Individual & Group requirements.

1. Individual requirements
* Manage their own scheduling.
* Create, Remove a group.
* Add a new member to a particular group if he is a creator of it.
* Transfer the scheduled event to Group content
2. Group requirements
* Prevent duplication for time interval of every event
* Send request, get permission for the duplicated time interval
3. Common requirements
* Schedule & reschedule an event
* Search & analyze the data according to specific items
* Reminder functionality


## _TECHNOLOGIES REQUIRED IN THE API_
* Docker
* Microservices architecture
* OpenAPI
* OpenSSL
* OTP
* .env validation
* Unit testing
* E2E testing
* CI/CD
* Amazon Web Services(ECS)

## _DATABASE STRUCTURE_
Three main models are used in this api.
* User
* Group
* Event

Associations between models
* User --- Event: One-to-Many
* User --- Group: Many-to-Many
* Grop --- Event: Many-to-Many

## _MICROSERVICES ARCHITECTURE_
This api is decomposed into three Microservices.

* User Management Service
* Group Management Service
* Event Management Service


## _ROADMAP_
1. Set up environment using Docker.
2. Design the project architecture based on Microservices architecture.
3. Compose OpenAPI specification documentation.
4. Implement CRUD using OpenAPI.
5. Implement Auth functionality.
    * Implement Sign In/Up using OpenSSL
    * Implement OTP
6. Validate .env file.
7. Implement Unit Testing functionality.
8. Implement E2E Testing functionality.
9. Implement CI/CD with Github Actions.
10 Deploy to Amazon ECS.

