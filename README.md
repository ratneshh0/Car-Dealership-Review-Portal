# Best Cars Dealership - Car Dealership Review Portal

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Setup and Installation](#setup-and-installation)
- [Containerization and Deployment](#containerization-and-deployment)
- [CI/CD Pipeline](#ci/cd-pipeline)
- [Kubernetes](#kubernetes)
- [Contributing](#contributing)
- [License](#license)

## Introduction

**Best Cars Dealership** is a comprehensive car dealership review portal that allows users to browse, review, and rate cars from various dealerships. The project is a full-stack application built with Django for the backend, React for the frontend, and other advanced technologies to ensure scalability, security, and ease of deployment.

The platform features a user-friendly interface, robust user management, and advanced containerization and deployment strategies, making it a modern solution for car dealerships aiming to improve customer feedback and engagement.

## Features

- **Full Stack Development:**
  - Backend developed with **Django** for REST API services.
  - Frontend built using **React**, with components for dealership reviews, car listings, and rating submissions.
  - Static pages such as Homepage, About Us, and Contact Us created with **HTML**, **CSS**, and **Bootstrap** for responsiveness and styling.

- **User Management:**
  - Secure and efficient user registration, login, and session management.
  - Authentication handled by **Django** in the backend and **React** on the frontend for seamless user experience.

- **Sentiment Analysis Microservice:**
  - A **Python** and **Flask** microservice deployed on IBM Cloud for analyzing customer reviews using sentiment analysis.
  - Provides real-time feedback on customer sentiment towards cars and dealerships.

- **Containerization & Microservices:**
  - Backend services built with **Node.js**, **Express**, and **MongoDB**, ensuring flexibility in handling data and logic.
  - All services containerized with **Docker**, ensuring environment consistency and ease of deployment.

- **CI/CD Pipeline:**
  - Continuous Integration and Continuous Delivery (CI/CD) pipeline implemented using **GitHub Actions**, automating testing, building, and deploying.
  - Codebase is continuously monitored for quality and correctness with automated testing during each commit.

- **Kubernetes for Scalability:**
  - Managed application deployment and scalability using **Kubernetes**.
  - Utilized serverless components on **IBM Cloud** for efficient scaling during high traffic.

## Technologies Used

### Backend
- **Django**: Backend web framework for handling RESTful API.
- **Node.js & Express**: Microservices for handling specific backend logic and MongoDB integration.
- **MongoDB**: NoSQL database for handling car listings and dealership data.
- **Flask**: Python framework used for the sentiment analysis microservice.

### Frontend
- **React**: Component-based JavaScript library for building the user interface.
- **HTML, CSS, Bootstrap**: Used for creating responsive static pages like Homepage, About Us, and Contact Us.

### DevOps
- **Docker**: Containerization of backend and microservices for consistent deployment.
- **Kubernetes**: For orchestrating containerized services and managing scalability.
- **IBM Cloud**: Deployment platform for microservices and serverless components.

### CI/CD
- **GitHub Actions**: CI/CD pipeline for automating testing, building, and deploying.

## Project Structure

```bash
Best-Cars-Dealership/
│
├── backend/
│   ├── app/
│   │   ├── models/
│   │   ├── views/
│   │   ├── serializers/
│   │   └── urls.py
│   ├── manage.py
│   └── settings.py
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── App.js
│   ├── public/
│   └── package.json
│
├── microservices/
│   ├── sentiment-analysis/
│   │   ├── app.py
│   │   ├── requirements.txt
│   └── Dockerfile
│
├── .github/workflows/
│   └── ci-cd.yml
│
└── Dockerfile
