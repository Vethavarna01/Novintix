**WORKING LINK**

https://colab.research.google.com/drive/1dElI8grKjJDI6w29QAmJAivzRtNR4ME3?usp=sharing


**Dataset**

Dataset used: Wind Turbine SCADA Dataset from Kaggle

Features:
Date/Time
LV Active Power (kW)
Wind Speed (m/s)
Theoretical Power Curve (kWh)
Wind Direction (°)

**Tech Stack**
Python
Pandas, NumPy
Matplotlib, Seaborn, Plotly
TensorFlow (LSTM)
Scikit-learn
FAISS (Vector Database)
Sentence Transformers
Gradio (UI)


**Task 1 — Exploratory Data Analysis (EDA)**
✔ What is done:
Converted dataset into time-series format
Handled missing values using forward fill
Plotted time-series graphs for all parameters
Visualized wind speed vs power curve

🎯 Outcome:
Identified trends and seasonal patterns
Observed turbine power curve behavior
Detected abnormal or noisy data points


**Task 2 — Time Series Forecasting**
✔ What is done:
Created windowed dataset for sequential learning
Built LSTM model for multivariate forecasting

Predicted all 4 parameters:
LV Active Power
Wind Speed
Theoretical Power
Wind Direction

📈 Evaluation:
Used Mean Squared Error (MSE)
Plotted predicted vs actual values

🎯 Outcome:
Captured temporal dependencies
Forecasted turbine behavior


**Task 3 — Anomaly Detection**
✔ What is done:
Calculated deviation between actual power and theoretical power
Defined threshold using statistical method
Flagged abnormal points

🎯 Outcome:
Identified underperformance zones
Detected inefficient turbine operation


**Task 4 — AI Performance Score Generator**
✔ What is done:
Calculated performance score:
Score = (Actual Power / Theoretical Power) × 100
Scaled between 0–100
Categorized:
Good (>80)
Moderate (50–80)
Poor (<50)
Generated automated suggestions

🎯 Outcome:
Provided interpretable turbine health metric
Enabled decision-making for maintenance


**Task 5 — RAG-Based AI System**
✔ What is done:
Uploaded turbine manuals (PDF/DOCX/TXT)
Extracted text and split into chunks
Converted text into embeddings
Stored embeddings in FAISS vector database
Built retrieval-based question answering system

💬 Example Queries:
What causes gearbox failure?
How to maintain a wind turbine?

🎯 Outcome:
Intelligent document-based Q&A system
Domain-specific knowledge retrieval


**Gradio UI Implementation**
✔ Features:
Dropdown to select turbine parameters
Time-series visualization
Prediction vs actual graphs
RAG chatbot interface

🎯 Outcome:
Interactive and user-friendly dashboard
Real-time visualization and querying



**How to Run (Google Colab)**
Install dependencies
Upload dataset and PDF file
Run all cells
Launch Gradio UI
