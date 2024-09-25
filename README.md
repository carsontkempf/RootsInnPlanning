# RootsInn Project

## Overview
RootsInn is a Django-based application for booking and managing treehouse accommodations. The project includes a complete database design, app implementation, and deployment on AWS. It aims to streamline the booking process while ensuring data integrity and reducing cloud costs.

## Table of Contents
1. [Project Description](#project-description)
2. [Database Design](#database-design)
3. [Django App Development](#django-app-development)
4. [Deployment](#deployment)
5. [AWS Integration](#aws-integration)
6. [Usage](#usage)
7. [License](#license)

## Project Description
RootsInn is a modular Django project that supports user authentication, treehouse library management, booking functionality, and payment integration through Stripe. The project leverages AWS for hosting and deployment, focusing on scalability and cost optimization.

## Database Design
### Entity-Relationship Diagram
![Entity Tables](./Entity%20Tables.png)

### Relational Tables
![Relation Tables](./Relation%20Tables.png)

### State Planning
![State Planning](./State%20Planning.png)

### Transition Mapping
![Transition Mapping](./Transition%20Mapping.png)

The database schema is designed to capture detailed relationships and transitions, supporting efficient queries and data manipulation for the booking process.

## Django App Development
### Key Applications
- **Booking Logic:** Facilitates booking treehouses, with checks for availability and validation of booking requests.
- **User Authentication:** Secure user login and registration using Django's built-in authentication system.
- **Treehouse Library:** Manages the collection of treehouses, allowing users to view detailed information about each property.
- **Payment Integration:** Utilizes Stripe API for secure payments, enabling users to book and pay directly on the site.

### Modularity and Optimization
The project is being refactored to increase modularity, allowing for easy integration of individual Django apps into other projects. Efforts are also made to optimize the project to reduce AWS costs through database optimization and server scheduling.

## Deployment
### AWS Services
- **Elastic Beanstalk:** Used for easy deployment and management of the Django application.
- **RDS:** Manages the PostgreSQL database for high performance and reliability.
- **EC2:** Supports scalable server infrastructure.
- **Server Scheduling:** Reduces costs by managing server uptime based on demand.

### CI/CD Workflow
The project includes a GitHub Actions workflow for testing the application locally and automating deployment to AWS.

## AWS Integration
### AWS RDS and S3
- Configured RDS for the PostgreSQL database to ensure high performance and data integrity.
- Utilized S3 for storing static and media files, enabling efficient content delivery.

### Stripe Integration
Stripe API endpoints are set up for secure payment processing. The project will become open-source once user and payment data are fully secured.

## Usage
- **Treehouse Library:** Users can browse available treehouses and view detailed descriptions and availability.
- **Booking:** Users can select available dates and book their stay.
- **Payments:** Integrated with Stripe, allowing users to complete payments securely.

## License
This project is currently in the planning stage and will become open-source once security measures for user information and payments are fully implemented. License details will be provided upon release.
