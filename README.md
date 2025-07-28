IT Help Desk Ticket Analysis System
This project is a complete, end-to-end prototype of an IT service management (ITSM) system. It demonstrates the full lifecycle of business systems analysis, from initial requirements gathering and system architecture design to the development of a functional, data-driven application.

The system features a user-facing form for submitting IT help desk tickets and a real-time management dashboard that visualizes key performance indicators (KPIs) and analytical insights from the ticket data.

View the Live Demo Here

Table of Contents
Project Overview

System Architecture

Key Features

Tech Stack

Configuration & Setup

How to Run Locally

Project Overview
In many organizations, IT help desk data is logged but not effectively analyzed, leading to recurring issues and inefficient resource allocation. This project was designed to solve that problem by creating a system that not only captures ticket information but also provides immediate, actionable insights for management.

The core objective was to design and build a system that could:

Provide an intuitive interface for users to submit support tickets.

Persist this data in a real-time, scalable database.

Analyze the aggregated data to identify trends and bottlenecks.

Visualize these findings on a live dashboard for IT managers and stakeholders.

System Architecture
This application was designed with a modern, decoupled architecture, representing the different layers of a business system:

Presentation Layer (Frontend): A user-facing interface built with HTML, styled with Tailwind CSS, and made interactive with vanilla JavaScript. This includes the ticket submission form and the management dashboard.

Business Logic Layer: A set of JavaScript functions that handle form validation, data processing, and the analytical calculations required to aggregate the ticket data for the dashboard charts.

Data Persistence Layer (Backend): The system uses Google Firebase's Firestore, a NoSQL cloud database, to store all ticket information in real-time. This allows the dashboard to update instantly as new tickets are submitted, demonstrating a reactive, event-driven system.

Authentication Layer: To manage user sessions securely, the application uses Firebase Anonymous Authentication.

Key Features
Real-Time Dashboard: The dashboard updates automatically as new tickets are submitted, providing a live look at the IT support queue.

KPI Visualization: Key metrics like "Total Open Tickets" and "High Urgency Tickets" are displayed prominently for quick assessment.

Interactive Charts: The dashboard features doughnut and bar charts (built with Chart.js) that visualize the breakdown of tickets by category and urgency.

Dynamic Data Analysis: The application's JavaScript engine continuously analyzes the ticket data from Firestore to calculate and display insights.

Error Handling & User Guidance: The system includes robust error handling to guide the user through setup if the Firebase configuration is missing or incorrect.
