# 🧠 SentimenTA - AI Sentiment Analysis Dashboard

![Status](https://img.shields.io/badge/Status-Production%20Ready-success)
![AI Model](https://img.shields.io/badge/AI%20Model-Gemini%202.5%20Flash-violet)
![Tech](https://img.shields.io/badge/Stack-React%20%7C%20TypeScript%20%7C%20Tailwind-blue)

**SentimenTA** is a modern, high-performance dashboard designed to automate the process of analyzing customer feedback. By leveraging Google's **Gemini 2.5 Flash** model, it transforms raw text data into actionable business intelligence in seconds.

## 📖 Project Overview

In the age of big data, businesses receive thousands of reviews across multiple platforms. Manually processing this data is slow, bias-prone, and unscalable. 

**SentimenTA** solves this by providing an interface where users can upload bulk review datasets (CSV, JSON, TXT). The application processes this data through a Large Language Model (LLM) to determine:
1.  **Sentiment Polarity**: Positive, Negative, or Neutral.
2.  **Confidence Score**: How certain the AI is about its prediction.
3.  **Macro Trends**: Overall distribution of customer satisfaction.

## ✨ Key Features

### 1. 🤖 Advanced AI Analysis
- Utilizes **Google Gemini 2.5 Flash** for low-latency, high-accuracy classification.
- Capable of understanding nuance, sarcasm, and context better than traditional NLP libraries.

### 2. 📊 Real-Time Visualization
- **Interactive Pie Charts**: Visual breakdown of sentiment distribution.
- **Key Metrics Cards**: Instant view of Total Processed, Accuracy, F1 Score, and Positive Ratios.
- **Confidence Tracking**: Visual progress bars showing the model's certainty for every single review.

### 3. 📂 Universal File Support
- **Drag & Drop Interface**: Seamless file uploading.
- **Format Support**: 
  - `.csv` (Spreadsheets)
  - `.json` (Structured Data)
  - `.txt` (Raw Text Logs)

### 4. ⚡ Modern Architecture
- **Zero-Config Deployment**: Built to be deployed instantly to Vercel, Netlify, or Heroku.
- **Responsive Design**: Fully functional on desktop, tablet, and mobile devices.
- **Client-Side Optimization**: Efficient parsing logic to handle large files without crashing the browser.

## 🛠️ Technical Architecture

The application is built using a modern frontend stack emphasizing type safety and performance.

| Component | Technology | Description |
|-----------|------------|-------------|
| **Core Framework** | React 18 | Component-based UI architecture. |
| **Language** | TypeScript | Ensures type safety and reduces runtime errors. |
| **Styling** | Tailwind CSS | Utility-first CSS for rapid, responsive UI development. |
| **AI Integration** | Google GenAI SDK | Direct integration with Gemini 2.5 Flash API. |
| **Visualization** | Recharts | Composable charting library built on SVG components. |
| **Build Tool** | Vite | Next-generation frontend tooling for instant server start. |

## 🎯 Use Cases

- **Product Managers**: Quickly gauge reaction to a new feature launch.
- **Customer Support**: Identify negative reviews that require urgent attention.
- **Market Researchers**: Analyze competitor reviews to find market gaps.

## 🚀 Setup & Run

To run this project locally:

1.  **Install Dependencies**: `npm install`
2.  **Configure API Key**: Create a `.env` file and add `API_KEY=your_gemini_key`.
3.  **Start Application**: `npm run dev`

---
*Built by [Your Name] as a showcase of AI integration in modern web development.*
