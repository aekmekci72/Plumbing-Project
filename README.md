# Plumbing-Project

A web application built using a single React Native codebase (via React Native for Web). The application communicates with a Python Flask backend, uses Firebase for secure authentication and data storage, and integrates AI features powered by a large language model (LLM).

## Tech Stack Overview

#### Frontend

React Native (with React Native for Web) – Core UI framework for building apps from a single codebase, running on web browsers via React Native for Web (extension layer).
Expo – Provides build tools, device testing, and development environment
Tailwind CSS – Utility-first styling for fast and responsive UI design
Axios – Used for making HTTPS API requests to the backend

#### Backend

Python Flask – Lightweight server that exposes REST API endpoints
Communicates with the frontend via JSON-based API calls

#### Authentication & Database

Firebase Authentication
- Supports federated identity providers such as Google Sign-In
- Tokens are verified server-side using Firebase Admin SDK

Cloud Firestore (Firebase)
- NoSQL document-based database
- Stores application data (users, roles, books, etc.)

#### ORM / Data Layer

FireORM – Used to manage Firestore data with an object-model interface

#### AI / Caching

Redis – Used for caching responses and improving AI/LLM request performance
LLM Model Used: Mistral-7B-Instruct-v0.2
- Hosted on Hugging Face: https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2

#### PDF Generation

jsPDF – React library used for exporting and generating PDF documents
