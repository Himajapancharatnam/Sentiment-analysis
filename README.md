# 🧠 SentimenTA - AI Sentiment Dashboard

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)

A professional-grade Sentiment Analysis Dashboard that uses **Google's Gemini 2.5 Flash API** to analyze customer reviews in real-time. Upload CSV, JSON, or TXT files to visualize sentiment distribution, confidence metrics, and key insights.

## ✨ Features

- **🤖 AI-Powered Analysis**: Leverages Google Gemini 2.5 Flash for high-accuracy sentiment detection.
- **📊 Interactive Visualization**: Beautiful interactive pie charts and metrics using Recharts.
- **📁 Multi-Format Support**: Drag & drop support for `.csv`, `.json`, and `.txt` files.
- **📈 Key Metrics**: Automatically calculates Accuracy, F1 Score, and Sentiment Distribution.
- **⚡ Fast & Responsive**: Built with Vite and Tailwind CSS for instant feedback and mobile responsiveness.

## 🚀 Quick Start

### Prerequisites
- Node.js (v18 or higher)
- A Google Gemini API Key (Get one [here](https://aistudio.google.com/app/apikey))

### 1. Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/sentiment-dashboard.git
cd sentiment-dashboard
npm install
```

### 2. Configuration

Create a `.env` file in the root directory:

```bash
touch .env
```

Add your Google Gemini API Key to the `.env` file:

```env
API_KEY=your_actual_api_key_here
```

### 3. Run Locally

Start the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 📂 Project Structure

```
src/
├── components/       # Reusable UI components (Charts, Cards, Buttons)
├── services/        # API integration (Gemini AI service)
├── utils/           # Helper functions (File parsing, ID generation)
├── types.ts         # TypeScript interfaces
├── App.tsx          # Main application logic
└── index.tsx        # Entry point
```

## 🛠️ Tech Stack

- **Frontend**: React 18, TypeScript
- **Styling**: Tailwind CSS, Lucide Icons
- **AI Model**: Google Gemini 2.5 Flash (`@google/genai`)
- **Charts**: Recharts
- **Build Tool**: Vite

## 📦 Building for Production

To create a production-ready build:

```bash
npm run build
```

This will generate a `dist` folder that you can deploy to Vercel, Netlify, or any static host.

---

**Note**: This is a frontend-only demonstration. For production use with sensitive API keys, it is recommended to move the API calls (`services/gemini.ts`) to a backend server to keep your keys secure.
