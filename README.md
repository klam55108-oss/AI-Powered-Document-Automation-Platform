# 🤖 AI-Powered-Document-Automation-Platform (MVP)

## Production-Grade Retrieval-Augmented Generation (RAG) & Document Governance

This repository showcases the complete AI-Powered Document Automation Platform developed during the Outamation Advanced AI-Powered Document Insights and Data Extraction Externship. The platform is designed to help businesses improve, automate, and architect critical tasks like document handling and data management, leading to thousands of hours saved and significantly boosted accuracy. This platform is a high-performance solution designed for complex, high-volume document environments such as Real Estate, Healtcare, Legal, Finance, and HR. Unlike generic RAG systems that often suffer from "Context Contamination," this system uses **Intelligent Boundary Detection** and **Metadata-Rich Chunking** to isolate and retrieve precise document segments with surgical accuracy.

<br>

------------- 
### 🛠️ MVP Objectives

- **Contextual Fidelity:** Eliminates hallucinations by segregating the vector space based on document classification.
- **Intelligent Automation:** Automatically splits bulk "blob" PDFs (e.g., a 50-page file containing multiple distinct contracts) into logical units.
- **Hardware-Aware Versatility:** Dynamic toggling between Gemini 2.0 (API), Mistral 7B, and Phi-2 (Local) with automated VRAM "Deep Purges" to - maintain stability on T4 GPUs.
- **Audit-Ready Compliance:** Every response undergoes a Quality Audit Gate (measuring Faithfulness, Relevance, and Context Density) before being displayed.

<br>

-------------
### 🏗️ Technical Architecture

The system follows a modular Six-Stage Execution Cycle:
- **Ingestion Layer:** Hybrid OCR (PyMuPDF + Tesseract) extracts text and images while preserving spatial metadata.
- **Intelligence Layer:** LLM-based classification into a custom taxonomy (e.g., Invoices, Land Deeds, Pay Slips) and automated page boundary detection.
- **Storage Layer:** LlamaIndex + FAISS create Segregated Silos using metadata filters to prevent data leakage between different document types.
- **Orchestration Layer:** A Python-generator-based "Thinking Loop" manages asynchronous status updates and hardware state safety.
- **Audit Layer:** Automated calculation of the RAG Triad metrics and real-time performance tracking.
- **Presentation Layer:** An Obsidian-themed Gradio UI featuring real-time PDF previews and exportable PDF audit reports.

<br> 

-------------
### 🔄 End-to-End Workflow

 The platform manages the complete document lifecycle through a specialized four-stage pipeline:

  * **1. Document Discovery & Classification (S2, S7)**
    * Automatically ingests unstructured PDF "blobs" (bulk uploads).
    * Cleans, applies OCR,and segments files into logical categories (Pay Stubs, IDs, Contracts) using intelligent boundary detection to ensure zero data leakage.

* **2. Heuristic Data Extraction (S3, S4)**
    * Employs specialized Python heuristics and layout-aware OCR engines.
    * Transforms raw text into structured JSON/DataFrames, capturing critical fields like loan amounts and names with high precision.

* **3. Semantic Context Retrieval (S5, S6)**
    * Powered by a fine-tuned RAG pipeline utilizing LlamaIndex.
    * Enables deep-context querying, allowing users to ask complex questions across the entire repository without manual searching.

* **4. Human-in-the-Loop Interface (S8)**
    * A production-ready Gradio web interface providing a familiar, chat-based UX.
    * Features real-time source citations and document previews for instant verification of AI responses.

<br>

-------------
### 🌟 Core Capabilities

- **Multi-Modal Routing:** Automatically detects if a query relates to "Financial Amounts" vs. "Legal Terms" and targets the specific document silo.
- **VRAM Management:** Implements "Safety Gate" logic (deep_purge_gpu) to allow seamless switching between heavy local models and API-based models without system crashes.
- **Source Attribution:** Every AI response includes clickable citations (e.g., "Source: Invoice (p. 4)") to ensure human-in-the-loop verification.
- **Exportable Audits:** Generate professional PDF summaries of chat history and performance metrics for compliance records.

<br>

-------------
### 🛠️ Tools & Technologies

- **Frameworks:** LlamaIndex (Orchestration), Gradio (UI), FAISS (Vector DB).
- **OCR Engines:** Tesseract, PyMuPDF.
- **Models:** Gemini 2.0 Flash, Mistral 7B, Phi-2.
- **Environment:** Google Colab, Python 3.x.

<br>

-------------

<h1>ABOUT EXTERNSHIP</h1>

## The Business Challenge
Every day, companies handle thousands of complex, unstructured documents (e.g., loan applications, contracts). Extracting information quickly and accurately is a major challenge, as documents vary in format, often contain missing data, or require specialized layout-aware processing.

This project delivers an end-to-end, modular system that addresses these challenges by applying advanced AI, OCR, and Retrieval-Augmented Generation (RAG) techniques to mortgage documents.

<h1></h1>

## Project Overview (Modules)
The platform was built through a sequence of nine intensive sprints, progressing from foundational data preparation to final system integration and user interface development.

<h1></h1>

## Learning Python

I am currently upskilling my software engineering and product management skills by applying focused Python labs to real-world AI challenges. My journey to build the AI-Powered Document Automation Platform has been a comprehensive deep dive into three critical areas:

- <b>Data Extraction & Preparation:</b> I began by building robust pipelines for document data ingestion. This involved mastering tools like PyMuPDF to parse and transform raw, messy PDF structures into clean, standardized data—the essential first step for any reliable AI application.

- <b>RAG System Foundation:</b> I rapidly acquired knowledge of the Retrieval-Augmented Generation (RAG) system architecture, implementing the core components (LlamaIndex, Vector Indexing, LLMs) to create a functional knowledge base that powers semantic search.

- <b>Optimizing RAG Pipelines:</b> Finally, I focused on high-performance optimization, fine-tuning my pipeline's efficiency by selecting fast models like Gemini 2.5 Flash, implementing advanced chunking strategies, and deploying a memory-aware, conversational interface.
<br><br>

This practical experience has solidified my ability to move beyond theoretical concepts and architect, build, and deploy production-ready AI solutions for document intelligence.

- <b>View Repo:</b>
  - [Python Document Preparation & Extraction](https://github.com/LashawnFofung/Python-Document-Preparation-and-Extraction)
  - [RAG Pipelines](https://github.com/LashawnFofung/RAG-Pipelines)
    - AI-Powered Document Automation Platform: A RAG Journey 🚀
    - This repository documents my technical evolution from writing basic LLM prompts to engineering a production-ready Retrieval-Augmented Generation (RAG) Proof of Concept (PoC). Each folder and notebook represents a critical milestone in mastering LlamaIndex, open-source model deployment, and intelligent document orchestration.  

<h1></h1>

## Module	Title	Core Focus / Outcome

### 🟩 Sprint 1 (S1)
  - <b>AI Document Intelligence:</b> Setting the stage and Core Objectives

  - <i>Status Update:</i> [Sprint 1 (S1)](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Status%20Updates/Status%20Update%20Sprint%201%20AI-Powered%20Document%20Automation%20Platform.pdf)

### 🟩 Sprint 2 (S2)
  - <b>Python & Google Colab:</b> Preparing Mortgage Data for AI	Data cleaning, standardization, and image processing to ensure clean input for AI models.

  - <i>Status Update:</i> [Sprint 2(S2)](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Status%20Updates/Status%20Update%20Sprint%202%20AI-Powered%20Document%20Automation%20Platform-2.pdf)

### 🟩 Sprint 3 (S3)
  - Python Data Extraction from PDFs using Python	Using Python tools (PyMuPDF, pdfplumber) and heuristics (regex, anchor phrases) to extract key fields from digital and scanned PDFs.

  - <i>Status Update:</i> [Sprint 3(S3)](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Status%20Updates/Status%20Update%20Sprint%203%20AI-Powered%20Document%20Automation%20Platform.pdf)

### 🟩 Sprint 4 (S4)
  - <b>Optimizing OCR:</b> Comparing Tesseract, PaddleOCR, and EasyOCR	Evaluating and selecting the optimal OCR engine, focusing on layout-aware extraction for complex scanned documents.
  - <i>Status Update:</i> [Sprint 4(S4)](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Status%20Updates/Status%20Update%20Sprint%204%20AI-Powered%20Document%20Automation%20Platform.pdf)

### 🟩 Sprint 5 (S5)
  - <b>Implementing RAG:</b> Introduction to Retrieval-Augmented Generation (RAG).	Building a Retrieval-Augmented Generation (RAG) pipeline using LlamaIndex to enable AI to retrieve contextually relevant data.
  - <i>Status Update:</i> [Sprint 5(S5)](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Status%20Updates/Status%20Update%20Sprint%205%20AI-Powered%20Document%20Automation%20Platform.pdf)

### 🟩 Sprint 6 (S6)
  - <b>Optimizing RAG Pipelines:</b> Tuning, Chunking, and Metadata Filtering	Optimizing RAG through advanced chunking, metadata filtering, and experimentation with open-source LLMs (Mistral, Phi-2).
  - <i>Technical Evaluation Report:</i> [Embedding Model Scorecard Analysis](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Technical%20Evaluation%20Reports/Embedding%20Model%20Scorecard%20Analysis.pdf)
  - <i>Technical Evaluation Report:</i> [Comparative Analysis of Large Language Models for Retrieval-Augumented Generation (RAG)](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Technical%20Evaluation%20Reports/Comparative%20Analysis%20of%20Large%20Language%20Models%20%20for%20Retrieval-Augmented%20Generation%20(RAG).pdf)
  - <i>Status Update:</i> [Sprint 6(S6)](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Status%20Updates/Status%20Update%20Sprint%206%20AI-Powered%20Document%20Automation%20Platform.pdf)

### 🟩 Sprint 7 (S7)
  - <b>Blob Processing and Classification:</b> Unlocking Unstructured Data. Designing a modular system to automatically split, classify, and route documents from massive, unstructured "blobs" (e.g., pay slips, contracts).
  - <i>Status Update:</i> [Sprint 7(S7)](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Status%20Updates/Status%20Update%20Sprint%207%20AI-Powered%20Document%20Automation%20Platform.pdf)

### 🟩 Sprint 8 (S8)
  - <b>Interactive Chatbot:</b> Building an Interactive Chatbot with Gradio and RAG	Integrating the RAG pipeline into a user-friendly, web-based Q&A interface using Gradio for seamless user interaction.
  - <i>Status Update:</i> [Sprint 8(S8)](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/Status%20Updates/Status%20Update%20Sprint%208%20AI-Powered%20Document%20Automation%20Platform.pdf)
  - <i>view:</i> [Colab Notebook: Full RAG Pipeline with Interactive Gradio Chatbot](https://github.com/LashawnFofung/RAG-Pipelines/blob/main/Gradio/Task_Full_RAG_Pipeline_with_Interactive_Gradio_Chatbot.ipynb)
   - <i>view:</i> [Presentation PDF: Full RAG Pipeline with Interactive Gradio Chatbot](https://github.com/LashawnFofung/RAG-Pipelines/blob/main/Presentation/Full%20RAG%20Pipeline%20with%20Interactive%20Gradio%20Chatbot%20-%20Demo%20and%20Reflection.pdf)
   - <i>view:</i> [Proof of Concept (POC) Colab Notebook: AI-Powered Document Intelligence Automation Platform with Gradio Chatbot](https://github.com/LashawnFofung/RAG-Pipelines/blob/main/POC/Task_Enhanced_Document_Q%26A_System_with_Intelligent_RAG_Pipeline.ipynb)
   - <i>view:</i> [Proof of Concept (POC) Presentation PDF: AI-Powered Document Intelligence Automation Platform with Gradio Chatbot](https://github.com/LashawnFofung/RAG-Pipelines/blob/main/Presentation/AI-Powered%20Document%20Intelligence%20Automation%20Platform%20with%20Gradio%20Chatbot%20-%20Demo%20and%20Reflection.pdf)
   - <i>View Web-based POC:</i> [Live POC](https://huggingface.co/spaces/lfofung/AI-Powered-Document-Intelligence-Automation-Platform)

### 🟩 Sprint 9 (S9)
  - <b>AI-Powered Document Automation Platform:</b> Final Integration. Building the End-to-End AI System	Assembling all components into a complete, rigorously tested, and evaluated platform ready for demonstration and deployment.
  - <i>Status Update:</i> [Sprint 9(S9)]()
  - <i>view:</i> [Colab Notebook: AI-Powered Document Auotmation Platform](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/src/AI_Powered_Document_Intelligence_Automation_Platform_MVP.ipynb)

<h1></h1>



