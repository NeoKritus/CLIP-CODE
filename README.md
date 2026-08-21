# CLIP&CODE — Multimodal UI Parsing & Code Generation Engine

CLIP&CODE is a multimodal design-to-code platform that converts UI screenshots into reusable React code. It combines visual understanding, local AI processing, and code generation to recreate interface designs as frontend components.

---

## Key Features

* **UI Screenshot Analysis**: Accepts interface screenshots and analyzes their layout, visual elements, typography, colors, and components.

* **Multimodal UI Understanding**: Uses a vision-language model to understand the visual structure and content of the uploaded interface.

* **React Code Generation**: Converts the analyzed UI information into structured React components and frontend code.

* **Reusable Code Output**: Generates organized frontend code that can be adapted and reused in development projects.

* **Local AI Processing**: Uses Ollama and locally available models for visual analysis and code generation without relying on paid AI APIs.

* **Interactive Code Interface**: Provides a web interface for submitting screenshots and viewing the generated UI description and code.

* **VS Code Integration**: Provides a VS Code extension that connects with the backend and enables the generation workflow directly within the development environment.

---

## Why This Architecture?

* **Design-to-Code Automation**: Reduces the manual effort required to recreate interfaces by combining screenshot understanding with automated code generation.

* **Local & Private AI**: Ollama can run the required AI models locally, keeping screenshots and generated content within the local environment.

* **Two-Stage Processing**: The system first understands the visual interface and then uses that understanding to generate the corresponding frontend code.

* **Developer-Friendly Integration**: The web interface and VS Code extension provide convenient ways to access the same code-generation workflow.

---

## System Architecture & Workflow (How It Works)

1. **Screenshot Input**: The user provides a UI screenshot through the web interface or VS Code extension.

2. **Visual Understanding**: A local vision model analyzes the screenshot and produces a structured understanding of the interface.

3. **Code Generation**: The visual information is passed to a local code-generation model to create the corresponding React implementation.

4. **Result Delivery**: The generated code and UI information are returned through the application for further development.

---

## Agent Workflow Design

### UI Understanding

`Screenshot → Vision Model → UI Description`

The vision model identifies the major visual and structural characteristics of the interface.

### Code Generation

`UI Description → Code Model → React Code`

The generated UI information is used to create the corresponding frontend implementation.

### Developer Integration

`Screenshot → VS Code Extension → Backend → Generated Code`

The VS Code extension provides a development-focused way to access the same generation workflow.

---

## Tech Stack

| Domain                  | Technologies                          |
| :---------------------- | :------------------------------------ |
| **Frontend**            | React, TypeScript, Vite, Tailwind CSS |
| **Backend & API**       | Python, FastAPI, Uvicorn, Pydantic    |
| **Local AI**            | Ollama                                |
| **Image Processing**    | Pillow                                |
| **VS Code Integration** | VS Code Extension API, TypeScript     |
| **API Communication**   | REST API, Axios                       |
| **Development**         | Git, GitHub, Node.js, npm             |

---

## Prerequisites

* Python 3.10+
* Node.js 18+
* npm
* Ollama
* A compatible local AI model
* Git
