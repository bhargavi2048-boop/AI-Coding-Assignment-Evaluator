🤖 AI Coding Assignment Evaluator

A professional, recruiter-grade web application that simulates an AI-powered coding assignment evaluation system with structured scoring, performance analytics, and actionable feedback.

Designed as a hackathon prototype, this project demonstrates how automated evaluation can deliver fairness, transparency, scalability, and recruiter-aligned assessment standards.

🚀 Overview

The AI Coding Assignment Evaluator is a fully client-side web application that enables users to:

Submit code (Python, C++, Java, JavaScript)

Upload coding assignment PDFs

Receive multi-metric performance scoring

View strengths and improvement insights

Track evaluation history

Export structured reports (CSV)

Customize evaluation parameters and UI settings

The system simulates an AI-based assessment engine that evaluates submissions across multiple industry-relevant dimensions.

✨ Key Features
🔎 Smart Submission Handling

Direct code input via textarea

PDF upload support (coding assignments)

Input validation for file types and empty submissions

📊 Multi-Dimensional Evaluation

Each submission is scored across:

✅ Correctness

⚡ Time Efficiency

💾 Space Efficiency

📖 Readability

🧩 Modularity

🧠 Edge Case Handling

🏆 Best Practices

🔍 Plagiarism Detection

An overall score (0–100) is computed using weighted aggregation.

📈 Visual Analytics Dashboard

Animated circular score indicator

Dynamic progress bars

Metric-by-metric breakdown

Structured performance insights

💬 Intelligent Feedback Engine

Automatically generates:

Strengths (high-performing areas)

Areas for improvement

Recruiter-style actionable recommendations

📜 Evaluation History

Session-based history tracking

Timestamped evaluation records

Performance comparison across runs

📤 Exportable Reports

CSV export functionality

Structured for academic or recruiter review

Suitable for documentation and analysis

⚙️ Customizable Settings

Users can personalize:

🌙 Dark Mode

🔠 Font Size

📊 Evaluation Weights

✨ Animation Effects

🧮 Scoring Algorithm

The overall score is calculated using weighted metrics:

Overall Score =
(Correctness × 25%) +
(Time Efficiency × 15%) +
(Space Efficiency × 10%) +
(Readability × 15%) +
(Modularity × 10%) +
(Edge Case Handling × 10%) +
(Best Practices × 10%) +
(Plagiarism × 5%)


Evaluation weights can be modified through the Settings panel for customized assessment strategies.

🏗 Architecture

This is a fully self-contained front-end application:

AI Coding Assignment Evaluator.html
│
├── HTML (UI Structure)
├── CSS (Animations, Responsive Design, Dark Mode)
└── JavaScript
    ├── Tab Management
    ├── Validation Engine
    ├── Scoring Logic
    ├── Feedback Generator
    ├── History Manager
    └── CSV Export Module

Technical Characteristics

Pure HTML5, CSS3, and Vanilla JavaScript

No external dependencies

No backend required

Lightweight and portable

Runs on any modern browser

🎯 Problem It Solves

Traditional coding evaluations often suffer from:

Delayed feedback

Superficial scoring

Lack of transparency

Scalability challenges

Inconsistent evaluation standards

This project demonstrates how AI-powered systems can deliver:

Instant performance breakdown

Structured feedback

Fair and repeatable scoring

Recruiter-aligned evaluation criteria

Scalable assessment design

⚠️ Current Limitations

Scores are prototype-based (simulated logic)

No live test-case execution engine

No persistent database storage

No real AI model integration (yet)

🔮 Future Enhancements

Real AI/LLM-based code analysis

Backend integration with persistent storage

Automated test-case execution

Advanced plagiarism detection system

Authentication & user dashboard

API-based institutional integration

Cloud scalability

🧪 How to Run

Download the HTML file.

Open it in any modern browser (Chrome, Edge, Firefox, Safari).

No installation, server, or dependencies required.

👩‍💻 Author

Bhargavi N

“Code is like poetry; every line should sing with clarity.”
