# \# Snowflake ID Generator

# 

# A microservice for generating unique distributed identifiers based on the Twitter Snowflake algorithm.

# 

# \[!\[Kotlin](https://img.shields.io/badge/Kotlin-1.9+-purple.svg)](https://kotlinlang.org)

# \[!\[Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen.svg)](https://spring.io/projects/spring-boot)

# \[!\[Gradle](https://img.shields.io/badge/Gradle-8.x-blue.svg)](https://gradle.org)

# \[!\[Docker](https://img.shields.io/badge/Docker-ready-blue.svg)](https://www.docker.com/)

# 

# \## Description

# 

# Snowflake ID Generator is a high-performance microservice for generating unique 64-bit identifiers in distributed systems. Based on the Twitter Snowflake algorithm, it guarantees:

# 

# \- \*\*Uniqueness\*\* — each ID is unique across the entire system

# \- \*\*Sortability\*\* — IDs are ordered by creation time

# \- \*\*Performance\*\* — generation of up to 4096 IDs per millisecond per node

# \- \*\*Distribution\*\* — support for multiple nodes without coordination

# 

# \##  Quick Start

# 

# \### Requirements

# 

# \- JDK 17 or higher

# \- Gradle 8.x

# \- Docker (optional)

# 

# \### Local Run

# ```bash

# \# Clone the repository

# git clone https://github.com/meirzhanAsk/kubernates.git

# cd kubernates

# 

# \# Build the project

# ./gradlew build

# 

# \# Run the application

# ./gradlew bootRun

# ```

# 

# The application will be available at: `http://localhost:8080`

# 

# \### Run with Docker

# ```bash

# \# Build the image

# docker build -t snowflake-id-generator:latest .

# 

# \# Run the container

# docker run -d \\

# &nbsp; --name snowflake-service \\

# &nbsp; -p 8080:8080 \\

# &nbsp; -e DATACENTER\_ID=1 \\

# &nbsp; -e WORKER\_ID=1 \\

# &nbsp; snowflake-id-generator:latest

# ```

# 

# \### Run with Docker Compose

# ```bash

# docker-compose up -d

# ```

# 

# \### Health Check

# ```bash

# GET /actuator/health

# 

# \# Response

# {

# &nbsp; "status": "UP"

# }

# ```

# 

# 

# 

# 

