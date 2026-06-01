# AI E-commerce Support Agent

![n8n](https://img.shields.io/badge/n8n-Automation-FF6D5A)
![Google Gemini](https://img.shields.io/badge/Google-Gemini-4285F4)
![Google Sheets](https://img.shields.io/badge/Google-Sheets-34A853)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E)
![License](https://img.shields.io/badge/License-MIT-green)

AI-powered customer support workflow built with n8n, Google Gemini and Google Sheets.

## Workflow Overview

![Workflow Overview](workflow%20inteiro.png)

---

## Overview

This project automates customer support for an e-commerce business using Artificial Intelligence.

The workflow receives customer messages, identifies customer intent, routes requests to the correct process, retrieves order information from Google Sheets when necessary, and generates personalized responses using Google Gemini.

---

## Features

- Intent Classification using Google Gemini
- Order Tracking Automation
- Return Request Handling
- FAQ Automation
- Human Support Escalation
- Google Sheets Integration
- AI-Generated Responses
- Webhook-Based API
- Error Handling for Missing Orders

---

## Technologies

- n8n
- Google Gemini
- Google Sheets
- JavaScript
- Webhooks

---

## Workflow Architecture

```text
Customer Message
        ↓
Intent Classifier
        ↓
Intent Router
    ├── Track Order
    ├── Return Product
    ├── FAQ
    └── Human Support
        ↓
Response Generator
        ↓
API Response
```

## Supported Intents

| Intent | Description |
|----------|-------------|
| TRACK_ORDER | Track customer orders |
| RETURN_PRODUCT | Handle product return requests |
| FAQ | Answer frequently asked questions |
| HUMAN_SUPPORT | Escalate requests to a human agent |

---

## Demo Video

A complete workflow demonstration is available in the repository.

Video file:

- `2026-06-01 11-54-40.mp4`

---

## Workflow File

The complete n8n workflow can be imported directly into n8n.

Workflow file:

- `AI E-commerce Support Agent.json`

---

## Example Request

```json
{
  "message": "Where is my order 12345?"
}
```

## Example Response

```json
{
  "reply": "Your order #12345 is currently in transit and expected to arrive soon."
}
```

---

## Screenshots

### Track Order Flow

![Track Order](TRACK_ORDER.png)

### Track Order Response

![Track Order Response](TRACK%20ORDER%20RESPONSE.png)

### FAQ Flow

![FAQ](FAQ.png)

### FAQ Response

![FAQ Response](FAQ%20RESPONSE.png)

### Return Product Flow

![Return Product](RETURN%20PRODUCT%20.png)

### Return Product Response

![Return Product Response](RETURN_PRODUCT%20RESPONSE.png)

### Human Support Flow

![Human Support](HUMAN_SUPPORT.png)

### Human Support Response

![Human Support Response](HUMAN_SUPPORT%20RESPONSE.png)

### Order Not Found Flow

![Order Not Found](NOT%20FOUND.png)

### Order Not Found Response

![Order Not Found Response](NOT%20FOUND%20RESPONSE.png)

---

## How It Works

1. Customer sends a message through the API.
2. Google Gemini classifies the customer's intent.
3. The workflow routes the request to the correct path.
4. For tracking requests, Google Sheets is queried.
5. Gemini generates a contextual response.
6. The API returns the final response.

---

## Future Improvements

- WhatsApp Integration (Evolution API)
- CRM Integration
- Database Integration
- Customer Authentication
- Order History Retrieval
- Multi-language Support

---

## Project Highlights

- AI-powered customer support automation
- Intent classification and routing
- Dynamic response generation
- External data lookup via Google Sheets
- Modular workflow architecture
- Real-world business use case

---

## Author

**João Gabriel Nazzi**

GitHub: https://github.com/NZ2901

---

## License

This project is licensed under the MIT License.
