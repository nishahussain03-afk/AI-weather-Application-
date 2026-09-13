# 🌦️ AI Weather Function Calling Application

An AI-powered weather application built using **Python, Streamlit, Hugging Face LLM, Function Calling, Geocoding API, and Weather API**.

This project demonstrates how a Large Language Model (LLM) can understand a user's natural-language weather query, decide when a function needs to be called, execute a Python function, retrieve real-time weather information from an external API, and generate a natural-language response.

---

## 📌 Project Overview

The **AI Weather Function Calling Application** allows users to ask weather-related questions in natural language.

For example:

> What is the weather in Chennai?

Instead of directly asking the user to enter latitude and longitude, the application automatically:

1. Understands the user's question using an LLM.
2. Identifies that weather information is required.
3. Calls the `get_weather()` Python function.
4. Converts the city name into geographical coordinates.
5. Retrieves current weather information.
6. Sends the weather data back to the LLM.
7. Generates a clear and natural response for the user.
8. Displays the result through a Streamlit interface.

<img width="855" height="491" alt="WhatsApp Image 2026-09-13 at 2 46 07 PM" src="https://github.com/user-attachments/assets/c908e2bb-0d88-4814-b2fe-634d6ca26bad" />


---

# 🎯 Objectives

The main objectives of this project are:

- To understand **LLM Function Calling**.
- To integrate an LLM with external APIs.
- To allow users to interact using natural language.
- To automatically identify when a tool/function is required.
- To retrieve real-time weather information.
- To understand the complete workflow of:
  
  `User → LLM → Function → API → Tool Result → LLM → Response`

- To build an interactive AI application using Streamlit.
- To demonstrate practical usage of Function Calling in an AI application.

---

# ✨ Key Features

- 🤖 AI-powered natural language interaction
- 🌦️ Real-time weather information
- 🔧 LLM Function Calling
- 📍 Automatic city-to-coordinate conversion
- 🌐 Geocoding API integration
- ☁️ Weather API integration
- 💬 Chat-based Streamlit interface
- 📊 Weather information displayed in an easy-to-understand format
- 🔐 Secure Hugging Face token handling using `.env`
- ⚠️ Error handling for invalid cities and API failures
- 🧠 LLM-generated natural language responses
- 📱 Interactive and user-friendly interface

---
                    ┌─────────────────────┐
                    │        USER         │
                    │ "Weather in Chennai"│
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       STREAMLIT     │
                    │    Chat Interface   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       LLM           │
                    │  Hugging Face Model │
                    └──────────┬──────────┘
                               │
                         Function Call
                               │
                               ▼
                    ┌─────────────────────┐
                    │   get_weather()     │
                    │   Python Function   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │  Geocoding API      │
                    │  City → Latitude    │
                    │       Longitude     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Weather API       │
                    │ Open-Meteo Forecast │
                    └──────────┬──────────┘
                               │
                         Weather Data
                               │
                               ▼
                    ┌─────────────────────┐
                    │     Tool Result     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       LLM           │
                    │ Final Response      │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │        USER         │
                    │ Natural Language    │
                    │ Weather Response    │
                    └─────────────────────┘
---                    

# 🧠 What is Function Calling?

Function Calling is a capability that allows an LLM to decide when it needs to use an external function or tool.

Normally, an LLM can generate text based on the information available to it.

However, an LLM may need external information such as:

- Current weather
- Stock prices
- Database information
- Search results
- Calculations
- External APIs

Function Calling allows the model to request a specific function.

---
## Author 

AFREEN NISHA M 
