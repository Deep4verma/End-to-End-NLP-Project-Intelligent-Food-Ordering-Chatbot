# AI Food Ordering Chatbot
## Project Overview

Developed an intelligent food ordering chatbot that enables customers to place, modify, and track restaurant orders through natural language conversations. The system integrates Dialogflow for intent recognition, FastAPI for backend services, and MySQL for order management and tracking.

The chatbot streamlines the ordering process by understanding customer requests, maintaining conversation context, processing orders, and providing real-time order status updates.

# Objective

Build an end-to-end conversational AI solution that:

Accepts food orders through natural language conversations.
Allows customers to add or remove items from ongoing orders.
Processes and stores orders in a MySQL database.
Tracks order status using unique order IDs.
Provides a seamless restaurant ordering experience.
Tech Stack
Python
FastAPI
Dialogflow ES
MySQL
Uvicorn
Ngrok
REST APIs
# Project Architecture
├── backend/
│   ├── main.py
│   ├── db_helper.py
│   ├── generic_helper.py
│   └── requirements.txt
│
├── frontend/
│   └── Website Interface
│
├── dialogflow_assets/
│   └── Intents, Training Phrases & Entities
│
└── db/
    └── MySQL Database Dump
# Key Features
Order Management
Add multiple food items to an order.
Update existing orders dynamically.
Remove selected items from ongoing orders.
Maintain session-wise order history during conversations.
Conversational AI
Intent detection using Dialogflow.
Context-aware conversations.
Natural language understanding for food ordering workflows.
Database Integration
MySQL database for storing orders.
Stored procedures for order insertion.
Automated order ID generation.
Order tracking status management.
Order Tracking
Unique order ID generation.
Real-time order status retrieval.
Customer order progress monitoring.
# Workflow
1. User Interaction

Customers interact with the chatbot through Dialogflow.

2. Intent Recognition

Dialogflow identifies user intents such as:

Add Order
Remove Order
Complete Order
Track Order
3. Backend Processing

FastAPI webhook receives requests and routes them to the appropriate intent handler.

4. Database Operations
Order details are stored in MySQL.
Order tracking records are created.
Pricing information is calculated automatically.
5. Response Generation

The chatbot returns confirmation messages, order summaries, and tracking updates.

Implemented Intents
Intent	Description
Order Add	Add food items to cart
Order Remove	Remove food items from cart
Order Complete	Finalize and place order
Track Order	Check current order status
Database Design
Orders Table

Stores:

Order ID
Food Item
Quantity
Order Tracking Table

Stores:

Order ID
Current Status
Delivery Progress
Stored Procedures and Functions
insert_order_item()
get_total_order_price()
API Endpoint
POST /

# Handles Dialogflow webhook requests for:

Food ordering
Order modification
Order completion
Order tracking
# Results
Successfully built an end-to-end AI-powered food ordering chatbot.
Integrated Dialogflow with FastAPI using webhook architecture.
Implemented session-based order management for multi-turn conversations.
Developed real-time order tracking functionality.
Connected conversational AI workflows with MySQL database operations.
# Future Improvements
User authentication and profile management.
Payment gateway integration.
Delivery time estimation.
Menu recommendation system.
Cloud deployment using AWS, Azure, or GCP.
Voice-enabled food ordering support.
