Create a complete, production-ready **Java Sentiment Analysis Tool** for customer reviews as a resume project. Target: Infosys/Accenture software engineer interviews. Use **Java 17+, Spring Boot 3.x, Maven**. Generate ALL files with full code, folder structure, and documentation.

## 🎯 PROJECT REQUIREMENTS
- **Input**: Text reviews or CSV file upload (Kaggle Amazon reviews dataset recommended)
- **Output**: Sentiment classification (POSITIVE/NEUTRAL/NEGATIVE) with confidence scores
- **Target Accuracy**: 88%+ on 5,000+ review test set
- **Features**:
  - REST API endpoints (/analyze, /upload, /stats)
  - Simple HTML dashboard with Chart.js pie charts
  - Confusion matrix & accuracy metrics display
  - Save analyses to H2 database (in-memory)

## 🛠️ TECHNICAL STACK (MANDATORY)
pom.xml dependencies:
├── spring-boot-starter-web
├── spring-boot-starter-data-jpa  
├── spring-boot-starter-thymeleaf
├── h2-database
├── deeplearning4j-core OR opennlp-tools
├── commons-csv (file parsing)
├── chart.js (via CDN)
└── lombok

## 📁 EXACT FOLDER STRUCTURE TO GENERATE
sentiment-analysis-tool/
├── pom.xml
├── src/
│   ├── main/
│   │   ├── java/com/resume/sentiment/
│   │   │   ├── SentimentApplication.java
│   │   │   ├── controller/SentimentController.java
│   │   │   ├── model/Review.java
│   │   │   │   └── Sentiment.java (enum)
│   │   │   ├── service/SentimentService.java
│   │   │   ├── ml/SentimentAnalyzer.java (Naive Bayes + TF-IDF)
│   │   │   └── repository/AnalysisRepository.java
│   │   └── resources/
│   │       ├── application.properties
│   │       ├── static/css/style.css
│   │       ├── static/js/charts.js
│   │       └── templates/index.html
├── README.md
├── demo.gif (describe how to create)
└── sample-reviews.csv

## 🔧 CORE IMPLEMENTATION DETAILS
1. **Preprocessing**: Tokenize, lowercase, remove stopwords/punctuation, TF-IDF vectorization
2. **Model**: Train Naive Bayes classifier OR use pre-trained OpenNLP; include train/test split
3. **API Endpoints**:
   POST /api/analyze → {"text": "Great product!", "sentiment": "POSITIVE", "confidence": 0.92}
   POST /api/upload → Process CSV file, return stats
   GET /api/stats → {"accuracy": 88.5, "confusionMatrix": [...]}
   GET / → HTML dashboard
4. **Metrics**: Precision, Recall, F1-score, Confusion Matrix visualization
5. **Database**: Store predictions with timestamps

## 📄 README REQUIREMENTS
# Java Sentiment Analysis Tool
[![Accuracy](badge)](demo.gif)

## Features
- 88% accuracy on 5K+ reviews
- Spring Boot REST API + Dashboard
- Deeplearning4j/OpenNLP powered

## Quick Start
