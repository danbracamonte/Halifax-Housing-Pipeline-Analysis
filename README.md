# AI-Powered Analysis of Halifax's Housing Development Pipeline

[![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)](https://www.python.org/)
[![GitHub last commit](https://github.com/danbracamonte/Halifax-Housing-Pipeline-Analysis)](https://github.com/danbracamonte/Halifax-Housing-Pipeline-Analysis)

## Project Overview
This repository contains my capstone project for the **Growth: Data Analytics & AI - Skills for Hire Atlantic** program. It goes beyond a simple dashboard to create an **intelligent system** that analyzes, predicts, and queries Halifax's housing development pipeline using public building permit data.

The core goal is to demonstrate a full-stack data science workflow:
- **Data Processing:** Cleaning, geospatial analysis, and feature engineering.
- **Machine Learning:** Time series forecasting (Prophet/SARIMA), development type classification (XGBoost), and neighborhood clustering (K-Means).
- **Generative AI (RAG):** A question-answering chatbot that allows users to query the permit data using natural language.

## Business Questions Answered
*   How have permit volumes and values evolved over time? (Time Series Analysis)
*   Where is new housing supply geographically concentrated? (Spatial Analysis)
*   Can we predict the volume of new permits for the next 6-12 months? (Forecasting)
*   Can we identify natural "development pattern" clusters across neighborhoods? (Clustering)
*   **Can we ask questions like "Show me all multi-unit permits in the Peninsula from 2023" in plain English?** (RAG System)

## Technical Stack
*   **Core:** Python (Pandas, GeoPandas, NumPy)
*   **Visualization:** Matplotlib, Plotly, Folium
*   **Machine Learning:** Scikit-learn (Clustering), XGBoost (Classification), Prophet/SARIMA (Forecasting)
*   **Generative AI (RAG):** LangChain, OpenAI/Claude API, ChromaDB/FAISS
*   **App & Deployment:** Streamlit (for demo), Git/GitHub

## Project Structure
Halifax-Housing-Pipeline-Analysis/
├── data/ # Data files (raw/ - gitignored, processed/)
├── notebooks/ # Jupyter notebooks for each step (01_processing 02_eda, 03_clustering, 04_forecast, 05_rag_demo)
├── src/ # Reusable Python scripts (data_processor.py, rag_system.py)
├── app/ # Streamlit application (app.py)
├── outputs/ # Generated figures and reports
├── docs/ # Additional documentation
├── .gitignore
├── LICENSE (MIT)
├── requirements.txt
└── README.md


## How to Run This Project
1.  **Clone the repo:** `git clone https://github.com/danbracamonte/Halifax-Housing-Pipeline-Analysis.git`
2.  **Set up environment:** `python -m venv venv` and activate it.
3.  **Install dependencies:** `pip install -r requirements.txt`
4.  **Get the data:** Download the raw data from the [Halifax Open Data Catalogue](https://catalogue-hrm.opendata.arcgis.com/) (links in `docs/data_sources.md` or notebook 01) and place it in `data/raw/`.
5.  **Run the notebooks:** Execute the notebooks in order (`01_processing.ipynb`, etc.).
6.  **Launch the app (optional):** `streamlit run app/streamlit_app.py`

## Contributing / Contact
This is a personal portfolio project. Created by [**Daniel Bracamonte**].
*   **LinkedIn:** [\[Daniel Bracamonte\]](https://www.linkedin.com/in/danielbracamonte/)
*   **Email:** [dbracamonte@gmail.com]
*   **Project Link:** [[Project Link](https://github.com/danbracamonte/Halifax-Housing-Pipeline-Analysis.git)]

## License
This project is open source and available under the [[MIT License](https://choosealicense.com/licenses/mit/)].
