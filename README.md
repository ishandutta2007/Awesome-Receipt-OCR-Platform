# Awesome-Receipt-OCR-Platform

Edit
Top Receipt OCR Tools Ecosystem

Curated List of SaaS Products & Open-Source GitHub Projects
Focused on Receipt OCR, Expense Data Extraction, Document AI & Financial Document Automation
Last updated: August 2026

This repository tracks notable SaaS/Hosted platforms and open-source projects for Receipt OCR. These tools convert receipt images, scans, and PDFs into structured data such as merchant names, transaction dates, currencies, taxes, totals, payment details, and line items for expense management, accounting, ERP, fintech, tax, and reimbursement workflows.

Examples include Veryfi, OCR.Space, Mindee, Klippa, Nanonets, Amazon Textract, Azure AI Document Intelligence, Google Document AI, Docsumo, and Taggun.

Open-source emphasis: The open-source ecosystem is particularly useful for organizations that want to process receipts locally or build their own extraction pipeline. Rather than relying only on turnkey receipt APIs, developers can combine PaddleOCR, Tesseract, EasyOCR, docTR, OCRmyPDF, OpenCV, LayoutParser, Surya, OpenReceipts, Open Receipt OCR, and receipt-specific extraction projects to create self-hosted receipt-processing systems.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites or repositories.

Table of Contents

SaaS/Hosted Platforms

Open-Source GitHub Projects

Additional Strong Open-Source Options

How to Contribute

Disclaimer

SaaS/Hosted Platforms

Veryfi
AI-powered receipt and invoice OCR API that extracts structured JSON including merchant information, line items, taxes, totals, currencies, and other financial fields. Veryfi states that its receipt API supports 91 currencies and 38 languages.

OCR.Space
Cloud OCR API providing image and PDF text extraction with an API-oriented workflow suitable for applications that need straightforward OCR processing.

Mindee
Developer-focused document AI platform with a pre-trained Receipt model capable of extracting merchant information, totals, dates, line items, and other receipt fields. Its receipt model is designed for receipts from more than 50 countries.

Klippa
Intelligent document processing platform providing OCR, document classification, data extraction, and receipt/expense processing capabilities.

Nanonets
AI-powered document processing platform supporting OCR and structured extraction from receipts, invoices, and other financial documents.

Amazon Textract
AWS managed document-analysis service that extracts printed text, forms, tables, and structured information from scanned documents and images.

Azure AI Document Intelligence
Microsoft's document-processing platform for OCR, prebuilt document models, custom extraction, forms, invoices, receipts, and other structured-document workloads.

Google Document AI
Google's document understanding platform providing OCR, classification, parsing, extraction, and specialized processors for financial and business documents.

Docsumo
Intelligent document processing platform for extracting structured information from receipts, invoices, financial documents, and other semi-structured documents.

Taggun
Receipt OCR and data-extraction API focused on extracting structured receipt information for expense management, accounting, loyalty, and financial applications.

Rossum
Cloud-native intelligent document processing platform using AI-based document understanding and extraction for financial and business documents.

Veryfi OCR API
Specialized receipt and invoice extraction API returning structured JSON, including line items, taxes, totals, vendor details, and OCR text.

Mindee Receipt API
Specialized receipt extraction workflow with configurable fields and structured output for merchant, date, total, expense category, quantities, prices, and line items.

Veryfi Mobile OCR SDK
Mobile-oriented document capture and OCR infrastructure for applications that need receipt and expense-document ingestion.

Dext
Receipt and invoice capture platform focused on automating bookkeeping and accounting workflows from photographed or uploaded financial documents.

Expensify
Expense-management platform incorporating receipt scanning and automated expense-data extraction into reimbursement and accounting workflows.

Receipt Bank
Receipt and financial-document capture capabilities now provided through the Dext ecosystem, with extraction designed for accounting workflows.

Rossum
AI document-processing platform that can be used for automated extraction and processing of receipts and other transaction documents.

Receipt OCR platforms generally fall into several layers: image capture → image preprocessing → OCR → document/layout understanding → field extraction → line-item parsing → validation → structured JSON → accounting/ERP integration.

Open-Source GitHub Projects

PaddleOCR
One of the strongest open-source OCR/document-AI foundations for receipt processing. It supports multilingual OCR and document parsing and can transform images and PDFs into structured, AI-friendly data. The project is Apache-2.0 licensed.

Tesseract OCR
Widely used open-source OCR engine for converting receipt images and scanned documents into machine-readable text. It is particularly useful as the OCR layer inside custom receipt-extraction pipelines.

EasyOCR
Open-source deep-learning OCR library supporting many languages and providing a relatively simple API for extracting text from receipt photographs and other images.

docTR
Open-source document text-recognition toolkit from Mindee combining text detection and recognition models. It can serve as a modern OCR layer in self-hosted receipt-processing systems.

OpenCV
Open-source computer-vision library widely useful for receipt preprocessing such as cropping, perspective correction, denoising, thresholding, rotation, and image enhancement.

OCRmyPDF
Open-source tool that adds OCR text layers to scanned PDFs using Tesseract and related PDF-processing infrastructure. Useful when receipt archives are stored as scanned PDFs.

Open Receipt OCR
Self-hosted receipt/document OCR platform specifically designed for receipt processing. It supports local providers including PaddleOCR and Tesseract.js, making it particularly relevant for privacy-focused deployments.

OpenReceipts
Free, private, open-source receipt scanner that extracts merchant, date, total, tax, and line-item information locally. It is designed to keep receipt images and extracted data on the user's own machine.

Receipt-OCR
Receipt-specific OCR project combining a Tesseract-based OCR module with higher-level structured receipt extraction. It includes a FastAPI service and can return fields such as merchant, transaction date, total, and line items.

receipt-ocr
Open-source receipt processing project providing both raw Tesseract OCR and structured receipt extraction workflows. It includes Docker/FastAPI deployment options.

LayoutParser
Open-source toolkit for document image analysis and layout detection. Useful for locating receipt regions such as headers, totals, merchant information, and line-item tables before extraction.

Surya
Open-source document OCR and layout-analysis toolkit useful for multilingual document processing, text detection, recognition, layout analysis, and related document-understanding tasks.

PaddleOCR-VL
Vision-language/document-parsing capabilities within the PaddleOCR ecosystem that can be used for more complex document understanding beyond traditional OCR.

Keras-OCR
Open-source OCR pipeline built around deep-learning text detection and recognition components, suitable for experimentation with receipt-image extraction.

Calamari OCR
Open-source OCR engine designed around neural-network-based recognition and useful for custom OCR model experimentation.

Kraken
Open-source OCR system with trainable recognition models and layout analysis capabilities, particularly useful when custom recognition models are required.

Additional Strong Open-Source Options

MMOCR for research and development involving text detection, recognition, and document OCR.

Detectron2 for custom receipt-region and object-detection models.

PaddlePaddle as the underlying deep-learning framework for PaddleOCR-based custom models.

PyMuPDF for extracting and manipulating receipt PDFs before OCR.

pdfplumber for extracting text and layout information from digitally generated receipt PDFs.

pdf2image for converting receipt PDFs into images before OCR.

Unstructured for document ingestion and preprocessing pipelines.

Marker for converting PDFs and documents into structured representations before downstream extraction.

Docling for open-source document conversion and document-structure understanding.

Haystack for building document-processing and extraction pipelines around OCR outputs.

LangChain for connecting OCR output to LLM-based structured extraction and validation.

LlamaIndex for building document ingestion and structured extraction pipelines.

Transformers for incorporating vision-language and document-understanding models into custom receipt pipelines.

FastAPI for exposing self-hosted receipt OCR as an internal REST API.

Apache Tika for generic document and metadata extraction in larger ingestion systems.

MinIO for self-hosted object storage of receipt images and extracted document artifacts.

PostgreSQL for storing structured receipt records, merchants, transactions, and extraction results.

Redis for queues, caching, deduplication, and asynchronous OCR workloads.

Celery for distributed asynchronous receipt-processing jobs.

Framework for building a custom open-source Receipt OCR platform: Combine OpenCV for image cleanup and perspective correction; PaddleOCR/Tesseract/EasyOCR/docTR for OCR; LayoutParser/Surya/Docling for document structure; OpenReceipts/Open Receipt OCR/Receipt-OCR for receipt-specific extraction patterns; and an LLM or rules engine for merchant normalization, line-item parsing, tax validation, and structured JSON output. Use FastAPI + Celery + Redis for the processing API and queue, with PostgreSQL + MinIO for persistence and document storage.

A particularly interesting architecture is to use multiple OCR engines as interchangeable providers. Open Receipt OCR already demonstrates this approach by supporting local OCR providers such as PaddleOCR and Tesseract.js, while receipt-specific projects such as Receipt-OCR combine raw OCR with structured extraction.

The biggest distinction from commercial APIs is that OCR is only the first layer. Veryfi, Mindee, Nanonets, Docsumo, and similar platforms provide substantial value through document-specific models, field normalization, confidence scoring, validation, line-item extraction, API infrastructure, and production operations. Open-source components provide the building blocks to reproduce much of this stack, but achieving enterprise-grade accuracy across countries, merchants, languages, layouts, and poor-quality photographs generally requires additional models, training data, validation logic, and monitoring.

How to Contribute

Fork the repo.

Add/edit entries in README.md (follow existing format).

Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

For open-source projects, preferably include the GitHub repository and license.

Submit PR with a short explanation.

Star the repo if you find it useful!

Disclaimer

This is a community-curated list — not exhaustive and not an endorsement.

Some open-source projects listed here are OCR engines or document-processing building blocks rather than direct replacements for commercial Receipt OCR platforms.

Always verify the current license, maintenance activity, model licenses, security posture, and production suitability before deployment.

Receipt OCR output can contain sensitive financial and personal information. Self-hosted deployments should use appropriate encryption, access control, retention policies, and audit logging.

OCR and extraction accuracy varies substantially with image quality, receipt layout, language, handwriting, fonts, lighting, and model configuration.

Financial records should be validated before being used for accounting, tax, reimbursement, payment, or other consequential workflows.

Made for fintech companies, expense-management platforms, accounting teams, developers, researchers, retailers, and document-AI builders.
Let's make receipt processing more open, private, accurate, and developer-friendly.
