# AI-Powered-Document-Automation-Platform


## AI-Powered Document Automation Platform
This repository showcases the complete AI-Powered Document Automation Platform developed during the Outamation Advanced AI-Powered Document Insights and Data Extraction Externship. The platform is designed to help businesses improve, automate, and architect critical tasks like document handling and data management, leading to thousands of hours saved and significantly boosted accuracy.

## The Business Challenge
Every day, companies handle thousands of complex, unstructured documents (e.g., loan applications, contracts). Extracting information quickly and accurately is a major challenge, as documents vary in format, often contain missing data, or require specialized layout-aware processing.

This project delivers an end-to-end, modular system that addresses these challenges by applying advanced AI, OCR, and Retrieval-Augmented Generation (RAG) techniques to mortgage documents.

## Project Overview (Modules)
The platform was built through a sequence of nine intensive projects, progressing from foundational data preparation to final system integration and user interface development.

## Module	Title	Core Focus / Outcome

### Project 1
Outamation Advanced AI Externship	Setting the Stage and Core Objectives

### Project 2
<b>Python & Google Colab:</b> Preparing Mortgage Data for AI	Data cleaning, standardization, and image processing to ensure clean input for AI models.

### Project 3
Advanced Data Extraction from PDFs using Python	Using Python tools (PyMuPDF, pdfplumber) and heuristics (regex, anchor phrases) to extract key fields from digital and scanned PDFs.

### Project 4
<b>OCR Showdown:</b> Comparing Tesseract, PaddleOCR, and EasyOCR	Evaluating and selecting the optimal OCR engine, focusing on layout-aware extraction for complex scanned documents.

### Project 5
Introduction to Retrieval-Augmented Generation (RAG)	Building a Retrieval-Augmented Generation (RAG) pipeline using LlamaIndex to enable AI to retrieve contextually relevant data.

### Project 6
<b>Advanced RAG:</b> Tuning, Chunking, and Metadata Filtering	Optimizing RAG through advanced chunking, metadata filtering, and experimentation with open-source LLMs (Mistral, Phi-2).

### Project 7
Unlocking Unstructured Data:</b> Blob Processing and Classification	Designing a modular system to automatically split, classify, and route documents from massive, unstructured "blobs" (e.g., pay slips, contracts).

### Project 8
Building an Interactive Chatbot with Gradio and RAG	Integrating the RAG pipeline into a user-friendly, web-based Q&A interface using Gradio for seamless user interaction.

### Project 9
<b>Final Integration:</b> Building the End-to-End AI System	Assembling all components into a complete, rigorously tested, and evaluated platform ready for demonstration and deployment.

## Core Architecture and Features
The platform is designed as an end-to-end pipeline covering the full document lifecycle:

- <b>Preprocessing & Classification (P2, P7):</b> Ingesting large, unstructured PDF "blobs," cleaning the data, applying OCR, and classifying individual documents (e.g., Pay Stubs, IDs, Contracts).

- <b>Extraction & Structuring (P3, P4):</b> Applying specialized extraction logic (Python heuristics, optimal OCR engine) to pull structured data (name, loan amount, salary) from each classified document.

- <b>Intelligent Retrieval (P5, P6):</b> Utilizing a fine-tuned RAG pipeline to allow users to ask complex, context-aware questions about the entire set of documents.

- <b>User Interface (P8):</b> Providing a clean Gradio web interface that allows users to chat with the document set, mirroring the user experience of tools like ChatGPT.

## Running the Project
Details on setting up the virtual environment, required dependencies, and running the individual project notebooks are located within the dedicated project folders.

- <b>Tools Used:</b> Python, Google Colab, Tesseract, PaddleOCR, EasyOCR, LlamaIndex, Gradio, PyMuPDF, pdfplumber.

- <b>Models Explored:</b> Open-source LLMs (Mistral, Phi-2) for RAG comparison.
