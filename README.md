# AI-Powered-Document-Automation-Platform

This repository showcases the complete AI-Powered Document Automation Platform developed during the Outamation Advanced AI-Powered Document Insights and Data Extraction Externship. The platform is designed to help businesses improve, automate, and architect critical tasks like document handling and data management, leading to thousands of hours saved and significantly boosted accuracy.

<h1></h1>

## The Business Challenge
Every day, companies handle thousands of complex, unstructured documents (e.g., loan applications, contracts). Extracting information quickly and accurately is a major challenge, as documents vary in format, often contain missing data, or require specialized layout-aware processing.

This project delivers an end-to-end, modular system that addresses these challenges by applying advanced AI, OCR, and Retrieval-Augmented Generation (RAG) techniques to mortgage documents.

<h1></h1>

## Project Overview (Modules)
The platform was built through a sequence of nine intensive sprints, progressing from foundational data preparation to final system integration and user interface development.

<h1></h1>

## Learning Python
I am currently augmenting my software engineering and product management skills by engaging in focused Python labs, specifically building robust pipelines for document data extraction and preparation.

[Python Document Preparation & Extraction](https://github.com/LashawnFofung/Python-Document-Preparation-and-Extraction)

<h1></h1>

## Module	Title	Core Focus / Outcome

### Sprint 1 (S1)
<b>AI Document Intelligence:</b> Setting the stage and Core Objectives

<i>Status Update:</i> [Sprint 1 (S1)](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Status%20Updates/Status%20Update%20Sprint%201%20AI-Powered%20Document%20Automation%20Platform.pdf)

### Sprint 2 (S2)
<b>Python & Google Colab:</b> Preparing Mortgage Data for AI	Data cleaning, standardization, and image processing to ensure clean input for AI models.

<i>Status Update:</i> [Sprint 2(S2)](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Status%20Updates/Status%20Update%20Sprint%202%20AI-Powered%20Document%20Automation%20Platform-2.pdf)

### Sprint 3 (S3)
Python Data Extraction from PDFs using Python	Using Python tools (PyMuPDF, pdfplumber) and heuristics (regex, anchor phrases) to extract key fields from digital and scanned PDFs.

### Sprint 4 (S4)
<b>Optimizing OCR:</b> Comparing Tesseract, PaddleOCR, and EasyOCR	Evaluating and selecting the optimal OCR engine, focusing on layout-aware extraction for complex scanned documents.

### Sprint 5 (S5)
<b>Implementing RAG:</b> Introduction to Retrieval-Augmented Generation (RAG).	Building a Retrieval-Augmented Generation (RAG) pipeline using LlamaIndex to enable AI to retrieve contextually relevant data.

### Sprint 6 (S6)
<b>Optimizing RAG Pipelines:</b> Tuning, Chunking, and Metadata Filtering	Optimizing RAG through advanced chunking, metadata filtering, and experimentation with open-source LLMs (Mistral, Phi-2).

### Sprint 7 (S7)
<b>Blob Processing and Classification:</b> Unlocking Unstructured Data. Designing a modular system to automatically split, classify, and route documents from massive, unstructured "blobs" (e.g., pay slips, contracts).

### Sprint 8 (S8)
<b>Interactive Chatbot:</b> Building an Interactive Chatbot with Gradio and RAG	Integrating the RAG pipeline into a user-friendly, web-based Q&A interface using Gradio for seamless user interaction.

### Sprint 9 (S9)
<b>AI-Powered Document Automation Platform:</b> Final Integration. Building the End-to-End AI System	Assembling all components into a complete, rigorously tested, and evaluated platform ready for demonstration and deployment.

<h1></h1>

## Core Architecture and Features
The platform is designed as an end-to-end pipeline covering the full document lifecycle:

- <b>Preprocessing & Classification (S2, S7):</b> Ingesting large, unstructured PDF "blobs," cleaning the data, applying OCR, and classifying individual documents (e.g., Pay Stubs, IDs, Contracts).

- <b>Extraction & Structuring (S3, S4):</b> Applying specialized extraction logic (Python heuristics, optimal OCR engine) to pull structured data (name, loan amount, salary) from each classified document.

- <b>Intelligent Retrieval (S5, S6):</b> Utilizing a fine-tuned RAG pipeline to allow users to ask complex, context-aware questions about the entire set of documents.

- <b>User Interface (S8):</b> Providing a clean Gradio web interface that allows users to chat with the document set, mirroring the user experience of tools like ChatGPT.

<h1></h1>

## Running the Project
<b>PENDING</b> Details on setting up the virtual environment, required dependencies, and running the individual project notebooks are located within the dedicated project folders.

- <b>Tools Used:</b> Python, Google Colab, Tesseract, PaddleOCR, EasyOCR, LlamaIndex, Gradio, PyMuPDF, pdfplumber.

- <b>Models Explored:</b> Open-source LLMs (Mistral, Phi-2) for RAG comparison.
