# Installation Guide

## Overview

This guide explains how to set up and run the Automotive FAQ Assistant project locally. The project consists of a FastAPI backend and a React frontend.

---

## Prerequisites

Make sure the following software is installed:

- Python 3.9 or above
- Node.js (v16 or above)
- npm or yarn
- Git

---

## Clone the Repository

Clone the project from GitHub:

git clone https://github.com/Ahzam-Hamza-Karat/automotive-faq-assistant.git
cd automotive-faq-assistant

---

# Backend Setup (FastAPI)

## Step 1: Navigate to Backend Directory

cd backend

## Step 2: Create a Virtual Environment

python -m venv venv

## Step 3: Activate Virtual Environment

On Windows:
venv\Scripts\activate

On Mac/Linux:
source venv/bin/activate

## Step 4: Install Dependencies

pip install -r requirements.txt

## Step 5: Run the Backend Server

uvicorn app.main:app --reload

The backend server will run at:
http://localhost:8000

API documentation (Swagger UI):
http://localhost:8000/docs

---

# Frontend Setup (React)

## Step 1: Navigate to Frontend Directory

cd frontend

## Step 2: Install Dependencies

npm install

## Step 3: Start the Development Server

npm start

The frontend application will run at:
http://localhost:3000

---

# Running the Full Application

1. Start the backend server.
2. Start the frontend server.
3. Open your browser at http://localhost:3000.
4. Enter a VIN or ask a question to interact with the system.
