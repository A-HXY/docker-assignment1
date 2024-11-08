## Docker Assignment - Agile Software Practice.

__Name:__ Xinyue Huang 

__Demo:__ https://youtu.be/8F-lhav82Q4

This repository contains the containerization of the mukti-container application illustrated below.

![](./images/arch.png)

### Database Seeding.

[Briefly explain how you automated the seeding of the application's database.]
To automate the seeding of the application's database, I created a seeder.js script that connects to the database and populates it with initial data.     This script imports predefined data (like movies.js) and uses the appropriate database client to insert records.
In a Dockerized environment, I included seeder.js in the Docker setup.     When the container starts, seeder.js runs automatically to seed the database.     This automation is handled by adding a command in the Dockerfile or docker-compose.    yml file to execute seeder.js after the database service is ready, ensuring the data is seeded consistently across all environments.

### M.ulti-Stack.

[Briefly explain how you support building development and production stack options.]
