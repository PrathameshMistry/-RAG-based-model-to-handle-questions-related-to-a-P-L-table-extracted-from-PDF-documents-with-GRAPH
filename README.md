
## 🚀 Overview
An AI-powered tool to analyze financial documents (e.g., P&L statements), extract metrics, answer questions, and visualize data using:
- **RAG Architecture** (Retrieval-Augmented Generation)
- **Mixtral-8x7B LLM** for QA
- **ChromaDB** for vector storage
- **Regex-based financial data extraction**
- **Sentiment Analysis** & **Auto-Graphing**

---

## ✨ Features
- 📁 **PDF Document Analysis**: Extract text from financial reports
- 💬 **Conversational QA**: Context-aware question answering
- 📈 **Auto-Visualization**: Generate bar charts for metrics comparisons
- 📊 **Financial Metrics Extraction**: Revenue, EBITDA, Net Profit, etc.
- 🎭 **Sentiment Analysis**: Classify answers as Positive/Negative/Neutral

---

## 🛠️ Installation
```bash
!pip install -q langchain-community langchain chromadb PyPDF2 pandas tiktoken sentence-transformers huggingface_hub python-dotenv matplotlib seaborn

🏃♂️ Quick Start
Set Hugging Face Token:


hf_token = "YOUR_HUGGINGFACE_API_TOKEN"  # Get yours at huggingface.co/settings/tokens
Run the System:

python
Copy
python main.py
Upload PDF when prompted (e.g., annual report)

📖 User Guide
1. Upload Documents
Supported format: PDF (text-based)

Example file: Annual_Report_2024.pdf

2. Ask Questions
python
Copy
"What is FY2024 revenue growth?"
"Compare Q1 2024 net income vs operating expenses"
"Show EBITDA trends as a graph"
3. Interpret Responses
Answer: Context-aware financial insights

Sentiment: Confidence-scored sentiment label

Sources: Document pages used for answer

Visualizations: Auto-generated comparative charts

🌟 Example Interactions
Example 1: Metric Extraction
Input: "Show key FY2024 metrics"
Output:

Copy
✅ Key Financial Metrics:
| Metric       | FY2024   | FY2023   |
|--------------|----------|----------|
| Revenue      | 100,000  | 90,000   |
| Net Profit   | 20,000   | 18,000   |
Example 2: Visualization
Input: "Graph net income vs expenses Q1 2024"
Output:
Net Income vs Expenses

🧠 System Architecture
mermaid

graph TD
    A[User] --> B[Upload PDF]
    B --> C[Text Extraction & Normalization]
    C --> D[ChromaDB Vector Store]
    D --> E[Query Processing]
    E --> F[LLM Answer Generation]
    F --> G[Sentiment Analysis]
    G --> H[Visualization Engine]
    H --> I[Output]
🚨 Troubleshooting
Issue	Solution
401 Unauthorized Error	Verify Hugging Face token
Empty PDF Results	Use OCR for image-based PDFs
Missing Metrics	Check document structure
📜 License
MIT License - See LICENSE for details

🤝 Contributing
Fork the repository

Create your feature branch (git checkout -b feature/AmazingFeature)

Commit changes (git commit -m 'Add some AmazingFeature')

Push to branch (git push origin feature/AmazingFeature)

Open a Pull Request

Note: Replace placeholder values (YOUR_HUGGINGFACE_API_TOKEN) with your actual credentials before use.

Copy

This README provides:
1. Clear visual hierarchy with emojis and sections
2. Easy-to-follow installation/usage instructions
3. Interactive elements (Colab link, architecture diagram)
4. Professional branding with contact info
5. Contribution guidelines for open-source development

To use:
1. Save as `README.md` in your GitHub repo
2. Add screenshots in `/images` folder
3. Update license file
4. Add CI/CD badges later if needed
