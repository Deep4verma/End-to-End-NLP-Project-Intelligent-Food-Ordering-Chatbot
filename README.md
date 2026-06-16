# AI Food Ordering Chatbot

## Project Overview

Developed an intelligent food ordering chatbot that enables customers to place, modify, and track restaurant orders through natural language conversations. The system integrates Dialogflow for intent recognition, FastAPI for backend services, and MySQL for order management and tracking.

The chatbot streamlines the ordering process by understanding customer requests, maintaining conversation context, processing orders, and providing real-time order status updates.

## Objective

Build an end-to-end conversational AI solution that:

- Accepts food orders through natural language conversations.
- Allows customers to add or remove items from ongoing orders.
- Processes and stores orders in a MySQL database.
- Tracks order status using unique order IDs.
- Provides a seamless restaurant ordering experience.

## Tech Stack

- Python
- FastAPI
- Dialogflow ES
- MySQL
- Uvicorn
- Ngrok
- REST APIs

## Key Features

### Order Management

- Add multiple food items to an order.
- Update existing orders dynamically.
- Remove selected items from ongoing orders.
- Maintain session-wise order history during conversations.

### Conversational AI

- Intent detection using Dialogflow.
- Context-aware conversations.
- Natural language understanding for food ordering workflows.

### Database Integration

- MySQL database for storing orders.
- Stored procedures for order insertion.
- Automated order ID generation.
- Order tracking status management.

### Order Tracking

- Unique order ID generation.
- Real-time order status retrieval.
- Customer order progress monitoring.

## Workflow

### User Interaction

Customers interact with the chatbot through Dialogflow.

### Intent Recognition

The chatbot identifies user intents such as:

- Add Order
- Remove Order
- Complete Order
- Track Order

### Backend Processing

FastAPI receives webhook requests and routes them to the appropriate handler.

### Database Operations

- Stores order details in MySQL.
- Creates order tracking records.
- Calculates total order amount.

### Response Generation

Returns order confirmations and tracking updates to customers.

## Results

- Built a complete AI-powered food ordering chatbot.
- Integrated Dialogflow with FastAPI using webhook architecture.
- Implemented session-based order management.
- Developed real-time order tracking functionality.
- Connected conversational AI workflows with MySQL database operations.

## Future Improvements

- User authentication and profile management.
- Online payment integration.
- Delivery time estimation.
- Menu recommendation system.
- Cloud deployment.
- Voice-based ordering support.
