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

## SaaS/Hosted Platforms

| Platform / Product | Description & Capabilities | Starting Pricing | Free Tier / Trial Limits |
| :--- | :--- | :--- | :--- |
| **Veryfi OCR API & SDK** | AI-powered receipt, invoice, and bill OCR API extracting line items, taxes, totals, vendor details, and currency across 91 currencies and 38 languages. Includes Mobile Lens SDK. | **$500/month** (Starter tier; ~$0.08/receipt, $0.16/invoice up to ~6,250 receipts/month) | **Free forever:** 100 documents/month (with access to all document types & SDKs); **14-day free trial** for full-access platform features (no credit card required). |
| **OCR.Space** | Cloud OCR API supporting multi-engine text and table extraction from receipt images and PDFs with searchable structured output. | **$30/month** (PRO plan; includes 300,000 requests/month, SLA, up to 100 MB file size) | **Free forever:** 25,000 requests/month (max 500 requests/day per IP, 1 MB max file size, max 3 pages/PDF). |
| **Mindee (Receipt API)** | Developer-first document AI API with pre-trained receipt and invoice parsing models covering 50+ countries with line-item, merchant, and tax parsing. | **€44/month** (~$48/mo billed annually; Starter plan includes 500 pages/month or 6,000 annual credits) | **14-day free trial** with 200 pages included for testing (no credit card required; no permanent free tier). |
| **Azure AI Document Intelligence** | Microsoft managed document AI service offering prebuilt models for receipts and invoices with line-item extraction, key-value pairs, and confidence scores. | **$10.00 per 1,000 pages** ($0.010/page) on Standard S0 Pay-as-you-go tier for prebuilt Receipt & Invoice models | **Free forever (F0 tier):** 500 pages/month (max 2 pages per document, max 4 MB file size). |
| **Amazon Textract (Analyze Expense)** | AWS managed document analysis service featuring a specialized `AnalyzeExpense` API for parsing receipts and invoices with line-item and vendor recognition. | **$0.025 per page** for Analyze Expense API (first 100,000 pages/month; drops to $0.010/page beyond 100k; basic text OCR starts at $0.0015/page) | **3-month free trial:** 100 pages/month for Analyze Expense (and 1,000 pages/month for basic text detection). |
| **Google Cloud Document AI (Expense Parser)** | Google Cloud document understanding platform with a specialized Expense Parser for extracting receipt items, taxes, totals, and payment metadata. | **$0.10 per document count** (1 count = up to 10 pages, effectively $0.01–$0.10/page or $100/1k pages; basic OCR is $1.50/1k pages) | **90-day free trial:** $300 in Google Cloud trial credits for testing Document AI processors (no permanent free tier for Expense Parser). |
| **Taggun** | Real-time receipt OCR and data extraction API optimized for expense management, loyalty platforms, and accounting automation with fast JSON response. | **$28/month** (Developer tier; includes 500 receipt scans/month, overage at $0.056/scan) | **30-day free trial** with unlimited receipt scans in testing/sandbox mode (no credit card required). |
| **Nanonets** | Automated document processing platform with pre-trained receipt models, human-in-the-loop validation, and custom AI workflow automation. | **$100/month** (Starter tier; includes 100 workflow block runs; pay-as-you-go extraction blocks at $0.10–$0.30/run) | **Free trial credits:** $50 in free trial credits (up to ~500 document pages/block runs, up to 3 users, no credit card required). |
| **Docsumo** | Intelligent document processing platform for financial documents, extracting line items, tables, and key data points from complex receipts and invoices. | **$299/month** (Growth tier; includes ~1,000 documents/month, ~$0.30 per additional page) | **14-day free trial** with 100 document pages included (no credit card required; no permanent free tier). |
| **Rossum** | Cloud-native intelligent document automation platform using transactional AI for end-to-end receipt, invoice, and bill capture. | **$18,000/year** (~$1,500/month; Starter annual contract with unlimited seats and core API ingestion) | **14-day free trial** with custom sandbox and sample receipt workflow validation (no permanent free tier). |
| **Dext (formerly Receipt Bank)** | Accounting automation and bookkeeping platform designed to capture and extract receipts, bills, and invoices directly into Xero, QuickBooks, and Sage. | **$31.50/month** ($25.21/month billed annually; includes 5 user seats and up to 250 documents/month) | **14-day free trial** with full receipt capture and extraction access (no credit card required; no permanent free tier). |
| **Expensify** | Expense management and business card platform featuring SmartScan for automated receipt OCR, mileage tracking, and expense report generation. | **$5/user/month** (Collect plan with accounting sync) or **$9/user/month** (Control plan); Free for personal use | **Free forever:** Unlimited SmartScans for individual users and expense tracking; **6-week free trial** for company business plans. |
| **Klippa (DocHorizon / SpendControl)** | Intelligent document processing API and expense management suite for scanning, classifying, and extracting receipt and invoice data. | **€5/user/month** (SpendControl Expense) or **€95/month** (SpendControl AP Invoice up to 4,000 docs/yr); API priced on volume | **Free trial credits:** €25 in free API testing credits upon registration with a business email (or 14-day platform trial; no permanent free tier). |

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
