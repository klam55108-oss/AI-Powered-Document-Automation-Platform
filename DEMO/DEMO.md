# DEMO: AI-Powered Document Automation Platform

<img src="https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/DEMO/DEMO%20AI-Powered%20Document%20Automation%20Platform.png" width="800" height="600" alt="DEMO PNG">




## Table of Contents

- [UI WalkThrough](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/DEMO/DEMO.md#demo-ui-walkthrough)

- [Gemini - Document Ingestion & Hardcoded Prompts](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/DEMO/DEMO.md#demo-gemini-ingestion--harcoded-prompts)

- [Gemini Export Chat History PDF](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/DEMO/DEMO.md#demo-gemini-export-chat-history-pdf)

- [Switch LLM & Mistral - Docuement Ingestion with Hardcoded Prompts](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/DEMO/DEMO.md#switch-llm--mistral---document-ingestion-with-hardcoded-prompts)

- [Switch LLM & Phi2 - Docuement Ingestion with Hardcoded Prompts](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/DEMO/DEMO.md#switch-llm--phi2---document-ingestion-with-hardcoded-prompt)

- [Gemini  RAG Configuration, JSON,  & Document Type Filter](https://github.com/LashawnFofung/AI-Powered-Document-Automation-Platform/blob/main/DEMO/DEMO.md#gemini--rag-configuration-json---document-type-filter)

---------------

 ## DEMO: UI WalkThrough
 
 - <i>Review DEMO Video:</i> [HERE](https://youtu.be/T4zju8HCFMM)
      
A quick look at the UI layout and functional design of my AI-Powered Document Intelligence Platform. This MVP is built to handle complex document structures (Real Estate, Finance, Legal) by bridging the gap between raw LLM power and granular administrative control.

<br>

<b>👩🏽‍💻⚙️Tab 1: Chat Operations</b>

The first tab serves as the primary Interactive AI Workspace, featuring a clean, dual-column chat interface designed for real-time document interrogation. On the left, users can select their preferred LLM—switching between the high-reasoning Gemini 2.0 Flash, the balanced Mistral, or the lightweight Phi-2—and utilize a dedicated upload zone to ingest new files into the system. The right side is dedicated to the conversation window, where users can ask complex natural language questions and receive grounded responses based on the uploaded data.

<br>

<b>👩🏽‍💻⚙️Tab 2: Configuration & Filters</b>

The second tab, labeled System Configuration & Metadata, provides a deep dive into the platform’s "under-the-hood" logic and data governance. It features a JSON viewer that displays the document's underlying structure and metadata tags, alongside a configuration panel for tuning the RAG engine's performance. Here, users can manually adjust chunk sizes and overlap parameters or apply strict Document Type Filters to isolate specific silos, ensuring the AI only retrieves data from relevant sources like "Lender Fee Sheets" while ignoring extraneous files.

<br>

<b>👩🏽‍💻⚙️Tab 3: Performance Audit</b>

The third tab is the Audit Performance Dashboard, a specialized diagnostic environment used to validate the accuracy and reliability of the AI’s outputs. This layout presents a series of analytical cards and tables that track the "RAG Triad" metrics: Faithfulness, Relevance, and Context Density. By reviewing these scores alongside average latency data, engineers can pinpoint exactly why a specific query might have underperformed, allowing for data-driven refinements to the retrieval pipeline without guessing.
    
<h1></h1>


## DEMO: Gemini Document Ingestion & Harcoded Prompts
 
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

<h1></h1>


## DEMO: Gemini Export Chat History PDF
 
- <i>Review DEMO Video:</i> [HERE](https://youtu.be/JwXRt7PwbmE) 

In this demo of the AI-Powered Document Automation Platform 🤖, we explore the Document Governance & Compliance layer of the platform by showcasing the PDF Export Functionality 📄. In production-grade AI automation, having a "black box" conversation isn't enough because enterprises require a verifiable paper trail 📑. This feature allows users to transform their entire AI-powered research session into a professional, portable document with a single click! 🖱️✨

The export engine does more than just copy-paste text; it performs a Structured Data Reconstruction of the chat history 🛠️. When the export is triggered, the platform parses the conversation thread including the specific LLM used (Gemini, Mistral, or Phi-2 🧠), the retrieved document citations, and the extracted financial data 💰, and then formats it into a clean, paginated PDF. This ensures that any responses generated during the session are preserved in a fixed format that can be instantly shared with stakeholders, auditors, or legal teams ⚖️🤝.

The layout for this feature is integrated directly into the Chat Operations tab 💬, featuring a dedicated "Export Session" utility that bridges the gap between dynamic AI exploration and static record-keeping 🌉. By capturing the metadata of the conversation such as timestamps and the specific document silos queried 🔍, the exported PDF serves as a comprehensive Audit Trail ✅. This ensures full transparency, allowing anyone reviewing the document to see exactly which sources the AI referenced to reach its conclusions 🎯.

<h1></h1>


## DEMO: Switch LLM & Mistral - Document Ingestion with Hardcoded Prompts
 
- <i>Review DEMO Video:</i> [HERE](https://youtu.be/_qzGlJbhN5U)

In this demo of the AI-Powered Document Intelligence Automation Platform 🤖, we showcase the seamless process of switching the core engine to the Mistral LLM 🧠. High-performance document automation requires flexibility, and this layout demonstrates how users can instantly toggle between models to find the perfect balance of reasoning and speed for their specific datasets. By selecting Mistral from the control panel, the platform reconfigures its processing logic to leverage Mistral’s unique capabilities for the tasks ahead ⚡.

The second part of the walkthrough focuses on the Document Ingestion and Indexing pipeline 📥. Watch as a complex document is uploaded and immediately put through our intelligent boundary detection system. The platform doesn't just store the text; it creates a metadata-rich index that maps out the document's structure in real-time 🔍. This indexing phase is critical because it ensures that when we query the system later, the Mistral model can retrieve the exact "Document Silos" needed without getting lost in unrelated data 🏗️.

Finally, we put the system to work using Hardcoded Business Prompts 📝. Instead of typing manual queries, we trigger automated logic gates designed for professional workflows, such as high-level document summarization and precision amount extraction 💰. You will see the Mistral LLM parse the indexed data to identify key financial figures and provide a concise executive summary with zero manual intervention. This demonstration highlights how pre-configured prompts can turn a raw PDF into structured, actionable intelligence in seconds 🚀.

<h1></h1>


## DEMO: Switch LLM & Phi2 - Document Ingestion with Hardcoded Prompt
 
- <i>Review DEMO Video:</i> [HERE](https://youtu.be/KewimB_I_k8)

In this demo of the AI-Powered Document Intelligence Automation Platform 🤖, we showcase the versatility of our Multi-LLM Switching feature by activating the Phi-2 engine 🧠. Designed by Microsoft, Phi-2 is a lightweight yet powerful model that we’ve integrated for scenarios requiring high-speed processing and low-latency extraction ⚡. You’ll see how the system’s "Hardware-Aware" architecture allows us to toggle to this local model on a T4 GPU without a hitch, using our VRAM Deep Purge logic to ensure a crash-free experience while maintaining top-tier performance 🛡️.

The second part of the walkthrough demonstrates the Document Ingestion and Indexing pipeline 📥 specifically tuned for small-context models. Watch as we upload a document and the system automatically triggers its Intelligent Boundary Detection to classify and index the content into isolated "Document Silos" 🏗️. For Phi-2, our indexing logic applies specialized Metadata-Rich Chunking, ensuring that every retrieved fragment is optimized with precise page and source tags, which prevents the model from being overwhelmed by unnecessary noise 🔍.

Finally, we test the efficiency of Phi-2 using Hardcoded Business Prompts 📝 tailored for rapid intelligence gathering. We trigger automated workflows for Document Summarization and a specialized Find Amounts extraction 💰. Despite its smaller size, you will see Phi-2 leverage our Model-Aware Retrieval settings to pull 8 contextual chunks instead of the standard 5, allowing it to provide accurate financial figures and concise summaries with clickable source citations 🚀. This demo highlights how even a lightweight model can deliver professional-grade RAG results when paired with a smart, metadata-driven architecture 🎯.

<h1></h1>


## DEMO: Gemini  RAG Configuration, JSON,  & Document Type Filter
 
- <i>Review DEMO Video:</i> [HERE](https://youtu.be/rNTbHpflirk)

This technical demonstration provides a streamlined, visual-only walkthrough of the AI-Powered Document Automation Platform, focusing on high-level system transparency and advanced document governance. The video highlights the backend logic and interface design used to manage complex, multi-siloed RAG (Retrieval-Augmented Generation) environments using the Gemini 2.0 Flash engine.

The Configuration & Filters tab, where the system’s "Siloed Vector Space" architecture is put into action. By toggling specific Document Type Filters, we demonstrate how the platform isolates the vector search to a specific business category—such as Mortgage Contracts or Tax Documents. This process is critical for preventing "Context Contamination," ensuring that the AI only retrieves data relevant to the selected document silo while maintaining a 100% routing confidence score.

The Document Structure and Metadata Transparency layers. We visualize the logical segmentation of uploaded files, showing how the "Intelligence Layer" has successfully partitioned a bulk PDF into distinct, searchable units with clear page boundaries. The deep dive into the Raw JSON Output reveals the underlying dataclasses, including unique DocIDs and Page mappings, which serve as the foundation for the system's high-fidelity source attribution and evidence-based answers.

The structured metadata objects facilitate professional document auditing. By peeling back the UI, we see that the AI isn't just generating text; it is performing precise queries against a highly structured knowledge brain. This "Glass Box" approach allows human auditors to verify the RAG Triad—Faithfulness, Relevance, and Context Density—directly through the dashboard, ensuring full transparency in automated business workflows.

<h1></h1>


