# DEMO: AI-Powered Document Automation Platform

<img src="https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/DEMO/DEMO%20AI-Powered%20Document%20Automation%20Platform.png" width="800" height="600" alt="DEMO PNG">




## Table of Contents

- [UI WalkThrough](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/DEMO/DEMO.md#demo-ui-walkthrough)

- [Gemini Ingestion & Hardcoded Prompts](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/DEMO/DEMO.md#demo-gemini-ingestion--harcoded-prompts)

- [Gemini Export Chat History PDF]()

---------------

 ## DEMO: UI WalkThrough
 
 - <i>Review DEMO Video:</i> [HERE](https://youtu.be/T4zju8HCFMM)
      
A quick look at the UI layout and functional design of my AI-Powered Document Intelligence Platform. This MVP is built to handle complex document structures (Real Estate, Finance, Legal) by bridging the gap between raw LLM power and granular administrative control.

<br>

<b>👩🏽‍💻⚙️Tab 1: Chat Operations</b>

The first tab serves as the primary Interactive AI Workspace, featuring a clean, dual-column chat interface designed for real-time document interrogation. On the left, users can select their preferred LLM—switching between the high-reasoning Gemini 2.0 Flash, the balanced Mistral, or the lightweight Phi-2—and utilize a dedicated upload zone to ingest new files into the system. The right side is dedicated to the conversation window, where users can ask complex natural language questions and receive grounded responses based on the uploaded data.

<br>

<b>👩🏽‍💻⚙️Tab 2: RAG Configuration</b>

The second tab, labeled System Configuration & Metadata, provides a deep dive into the platform’s "under-the-hood" logic and data governance. It features a JSON viewer that displays the document's underlying structure and metadata tags, alongside a configuration panel for tuning the RAG engine's performance. Here, users can manually adjust chunk sizes and overlap parameters or apply strict Document Type Filters to isolate specific silos, ensuring the AI only retrieves data from relevant sources like "Lender Fee Sheets" while ignoring extraneous files.

<br>

<b>👩🏽‍💻⚙️Tab 3: Performance Audit</b>

The third tab is the Audit Performance Dashboard, a specialized diagnostic environment used to validate the accuracy and reliability of the AI’s outputs. This layout presents a series of analytical cards and tables that track the "RAG Triad" metrics: Faithfulness, Relevance, and Context Density. By reviewing these scores alongside average latency data, engineers can pinpoint exactly why a specific query might have underperformed, allowing for data-driven refinements to the retrieval pipeline without guessing.
    
<h1></h1>


## DEMO: Gemini Ingestion & Harcoded Prompts
 
- <i>Review DEMO Video:</i> [HERE](https://youtu.be/FG8nZZfnJ78)

🟩 <b>Document Ingestion & Indexing</b>

The first section of the demo highlights the Seamless Ingestion & Indexing Pipeline, where raw documents are uploaded and transformed into machine-readable intelligence. As the file is processed, the system utilizes Gemini 2.0 Flash to perform intelligent boundary detection, segmenting the document into logical silos while simultaneously generating high-dimensional vector embeddings. This backend process ensures that every paragraph and data point is indexed with rich metadata, setting the stage for high-precision retrieval and eliminating the "context contamination" common in standard RAG systems.

🟩 <b>Document Viewer</b>

The second part of the layout features the Integrated Document Viewer, a specialized interface that allows for manual verification of the digital twin. This tab provides a high-fidelity, page-by-page view of the ingested document, allowing users to scroll through the original formatting while the AI works in the background. This visual anchor is crucial for transparency, as it allows the operator to cross-reference the AI’s extracted insights directly against the source material, ensuring that page numbers and physical layouts match the indexed data.

🟩 <b>Harcoded Prompts</b>

The final stage of the demo showcases Automated Intelligence via Hardcoded Prompts, where the power of Gemini is applied to specific business logic. We trigger two primary "One-Click" actions: a comprehensive Document Summary and a targeted "Find Amounts" query. The summary prompt instructs the LLM to condense complex clauses into actionable bullet points, while the amount extraction prompt utilizes specific reasoning to identify financial figures, fee schedules, and totals. This demonstrates how the platform moves beyond simple chat, providing structured, reliable data extraction at the push of a button.

🤖<b>Technical Deep Dive: Document Silos & Strategic Retrieval</b>

The core of the platform’s accuracy lies in its Metadata-Rich Vector Architecture. Unlike generic systems that throw all text into a single "bucket," this platform uses an Intelligent Router that classifies every uploaded page into a specific business taxonomy (e.g., Mortgage_Contract vs. Lender_Fee_Sheet). When you use the "Find Amounts" prompt, the system doesn't just perform a keyword search; it triggers a specialized Amount Extraction Pipeline:

- 🔍 <b>Silo-Specific Filtering</b> 

  The UI selection creates a hard metadata constraint at the database layer. If you filter for "Lender Fee Sheets," the vector engine physically ignores "Pay Slips" or "Bank Statements," even if they contain similar financial terminology. This eliminates "Context Contamination" and ensures the 32k context window of Gemini 2.0 Flash is populated only with relevant data.

- 🔗 <b>Deterministic Regex Hybridization</b> 

  To achieve the high Faithfulness scores required for finance, the platform combines LLM reasoning with Deterministic Regex Scanners. While Gemini interprets the meaning of a fee, the Regex engine ensures every decimal-accurate figure is captured from the raw text, cross-referencing them before generating the final response.

- ⭐️ <b>Page-Level Attribution</b> 

  Because the ingestion layer preserves the "Physical Layer" of the document, every amount found is tagged with a doc_id and page_num. This allows the "Find Amounts" feature to provide clickable citations, enabling a "Human-in-the-loop" to verify the AI's findings against the Document Viewer in real-time.



## DEMO: Gemini Export Chat History PDF
 
- <i>Review DEMO Video:</i> [HERE](https://youtu.be/Cr7QLuYJXtQ)

In this demo of the AI-Powered Document Automation Platform 🤖, we explore the Document Governance & Compliance layer of the platform by showcasing the PDF Export Functionality 📄. In production-grade AI automation, having a "black box" conversation isn't enough because enterprises require a verifiable paper trail 📑. This feature allows users to transform their entire AI-powered research session into a professional, portable document with a single click! 🖱️✨

The export engine does more than just copy-paste text; it performs a Structured Data Reconstruction of the chat history 🛠️. When the export is triggered, the platform parses the conversation thread including the specific LLM used (Gemini, Mistral, or Phi-2 🧠), the retrieved document citations, and the extracted financial data 💰, and then formats it into a clean, paginated PDF. This ensures that any responses generated during the session are preserved in a fixed format that can be instantly shared with stakeholders, auditors, or legal teams ⚖️🤝.

The layout for this feature is integrated directly into the Chat Operations tab 💬, featuring a dedicated "Export Session" utility that bridges the gap between dynamic AI exploration and static record-keeping 🌉. By capturing the metadata of the conversation such as timestamps and the specific document silos queried 🔍, the exported PDF serves as a comprehensive Audit Trail ✅. This ensures full transparency, allowing anyone reviewing the document to see exactly which sources the AI referenced to reach its conclusions 🎯.


## BELOW SECTIONS: PENDING 
 
- <i>Review DEMO Video:</i> [HERE]()

