# Project Architecture

## Overview

Automotive FAQ Assistant is a full-stack web application built using FastAPI for the backend and React for the frontend. The system is designed with modular architecture and clear separation of concerns.

---

# Backend Architecture (FastAPI)

## Structure

backend/
│
├── app/
│   ├── api/
│   │   └── v1/
│   │       ├── vin.py
│   │       └── faq.py
│   ├── main.py
│   └── models/
│
├── requirements.txt

## Key Components

main.py  
- Entry point of the FastAPI application.  
- Registers routers and middleware.

vin.py  
- Contains VIN decoding logic and validation.

faq.py  
- Handles automotive FAQ question-answer logic.

Pydantic Models  
- Used for request validation and structured response formatting.

---

# Frontend Architecture (React)

## Structure

frontend/
│
├── src/
│   ├── components/
│   ├── App.js
│   └── index.js

## Responsibilities

- Captures user input (VIN or question).
- Sends HTTP requests to backend API.
- Displays structured responses.
- Handles error states and user feedback.

---

# Communication Flow

1. User enters a VIN or question in the frontend.
2. Frontend sends an HTTP request to the backend API.
3. Backend processes the request and returns a JSON response.
4. Frontend renders the response dynamically.

---

# Design Principles

- Modular routing
- Versioned API structure (/api/v1)
- Separation of backend and frontend
- Clear request and response models
- Scalable project organization
