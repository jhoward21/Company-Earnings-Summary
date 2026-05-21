"# Company-Earnings-Summary" 
# Company Earnings Reader

An AI-powered web application that analyzes and summarizes company earnings reports. Built with a React + TypeScript frontend and a Python FastAPI backend, this project combines software engineering with financial domain knowledge to help users quickly extract key insights from earnings documents.

---

## Features (In Progress)

- Upload or paste a company's earnings report
- AI-powered summarization of key financial metrics
- Visual charts for revenue, EPS, and guidance data
- Sentiment analysis on management commentary
- Q&A mode — ask questions directly about the report

---

## Tech Stack

**Frontend**
- React + TypeScript
- Vite
- Tailwind CSS
- Recharts

**Backend**
- Python
- FastAPI
- Anthropic Claude API
- pdfplumber

**APIs**
- Anthropic Claude API (AI summarization)
- Financial Modeling Prep / Alpha Vantage *(planned)*

---

## Project Structure

```
company-earnings-reader/
├── frontend/
│   └── vite-earnings-report/
│       ├── src/
│       │   ├── components/
│       │   ├── pages/
│       │   └── api/
│       └── public/
└── backend/
    ├── main.py          # FastAPI routes
    ├── parser.py        # PDF/text parsing
    ├── ai_service.py    # Claude API integration
    ├── models.py        # Pydantic data models
    └── .env             # API keys (not committed)
```

---

## Getting Started

### Prerequisites
- Node.js v18+
- Python 3.10+
- Anthropic API key

### Frontend Setup
```bash
cd frontend/vite-earnings-report
npm install
npm run dev
```

### Backend Setup
```bash
cd backend
python -m venv venv

# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate

pip install fastapi uvicorn python-dotenv pdfplumber anthropic
uvicorn main:app --reload
```

### Environment Variables
Create a `.env` file in the `backend/` folder:
```
ANTHROPIC_API_KEY=your_api_key_here
```

---

## Roadmap

- [x] Project scaffolding (frontend + backend)
- [ ] PDF upload and parsing
- [ ] AI summarization via Claude API
- [ ] Frontend dashboard UI
- [ ] Financial charts and visualizations
- [ ] Live earnings data via financial API
- [ ] Multi-quarter comparison view
- [ ] Export summary as PDF

---

## About

This project was built to bridge the gap between raw financial data and actionable insights. As someone with a background in both software engineering and finance, I wanted to create a tool that cuts through the noise and surfaces what actually matters in an earnings report.

---

## Contact

Feel free to connect or reach out via [LinkedIn](#) or open an issue on this repo.