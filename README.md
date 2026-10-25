API Foundry

A simple REST API for managing software engineers, built with Java and Spring Boot.

The API lets you add software engineers, store their tech stacks, and fetch their information from a PostgreSQL database.

Tech Stack

Java 21, Spring Boot, Spring Data JPA, PostgreSQL, and Maven.

What It Does

GET /api/v1/software-engineers

Fetch all software engineers.

POST /api/v1/software-engineers

Add a new software engineer.

Example request:

{
  "name": "Alex",
  "techStack": "Java, Spring Boot"
}

The data gets saved to PostgreSQL and can be retrieved through the API.

Project Structure

Controller: Handles incoming HTTP requests.

Service: Connects the controller to the repository.

Repository: Handles database operations through JPA.

Entity: Represents a software engineer in the database.

Running Locally

You'll need Java 21 and Docker installed.

git clone https://github.com/aL3xyy/api-foundry.git
cd api-foundry
docker compose up -d

Open the project in IntelliJ IDEA and run Application.java.

The API runs at http://localhost:8080.
