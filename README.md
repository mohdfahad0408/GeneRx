# 🧬 PharmaGuard (geneRx)
### AI-Powered Pharmacogenomic Risk Prediction System

PharmaGuard is a privacy-first web application that analyzes genomic VCF files to predict drug response risks based on pharmacogenomic variants.

Built for Precision Medicine and clinical decision support.

---

## 🚨 Problem

Adverse Drug Reactions (ADRs) cause thousands of preventable deaths every year.

Many of these reactions occur because patients metabolize drugs differently due to genetic variations in key pharmacogenes like:

- CYP2D6
- CYP2C19
- CYP2C9
- SLCO1B1
- TPMT
- DPYD

However, clinicians often lack simple tools to interpret raw genomic (VCF) files quickly and safely.

---

## 💡 Solution

PharmaGuard is a fully client-side AI web app that:

- Parses real VCF (v4.1/v4.2) files
- Extracts pharmacogenomic variants
- Classifies drug response risk
- Assigns clinical labels:
  - Safe
  - Adjust Dosage
  - Toxic
  - Ineffective
  - Unknown
- Generates structured JSON clinical reports
- Optionally provides AI-based explanations (Gemini integration)

All processing happens in the browser — ensuring complete patient data privacy.

---

## ✨ Features

- ✅ VCF file upload & parsing
- ✅ Gene variant detection
- ✅ Drug-specific risk prediction
- ✅ Confidence scoring
- ✅ Structured JSON output
- ✅ Optional AI explainability
- ✅ Privacy-first architecture

---

## 🛠 Tech Stack

- React 18
- TypeScript
- Vite
- Tailwind CSS
- shadcn/ui
- Vitest
- Google Gemini API (optional)

---

## 📂 Project Structure

```
geneRx/
│
├── src/
│   ├── components/
│   ├── lib/
│   │   └── pharmacogenomics.ts
│   ├── hooks/
│   └── pages/
│
├── public/
├── package.json
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/mohdfahad0408/geneRx.git
cd geneRx
```

### 2. Install dependencies

```bash
npm install
```

### 3. Run development server

```bash
npm run dev
```

Open your browser at:

```
http://localhost:5173
```

---


## 📊 Example Output

```json
{
  "patient_id": "PG-001",
  "drug": "CODEINE",
  "risk_label": "Toxic",
  "confidence_score": 0.95,
  "gene": "CYP2D6",
  "phenotype": "Poor Metabolizer"
}
```

---

## 🔐 Privacy

- All genomic analysis runs in the browser
- No data is stored on servers
- No backend required

---

