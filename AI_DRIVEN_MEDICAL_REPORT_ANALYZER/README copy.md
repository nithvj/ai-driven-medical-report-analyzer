# 🩺 Blood Report Analysis

## Overview

The Medical Report Analysis app is a comprehensive tool designed to analyze  reports from PDF files. Built using the Streamlit framework, this application processes the data extracted from the PDF and delivers a detailed analysis, which includes key medical findings, potential health concerns, recommended follow-up tests, actionable lifestyle advice, and references to trusted medical resources. The goal of this application is to provide users with insights into their health based on their blood test reports and to offer guidance on necessary steps for improving or maintaining their health.

## Features

- **PDF Upload:** Users can upload their blood test reports in PDF format, which the app will analyze.
- **Detailed Analysis:** The app leverages the CrewAI framework, involving specialized agents, to parse and analyze the report data, providing a comprehensive summary of the results.
- **Health Recommendations:** Based on the analysis, the app generates personalized health advice, including lifestyle modifications and suggested medical follow-ups.
- **Trusted Resources:** The app includes references to high-quality medical articles and resources, allowing users to further understand their health conditions.

## Application Workflow

1. **Data Extraction:** The app uses PyPDF2 to extract text data from the uploaded PDF files.
2. **Analysis:** Leveraging CrewAI, the app processes the data through various agents, each responsible for specific tasks such as summarizing key findings, identifying health concerns, and providing recommendations.
3. **Output:** The processed data is then displayed on the Streamlit interface, categorized into key findings, main health concerns, additional tests or follow-ups, lifestyle advice, and trusted medical resources.

## Installation

### Prerequisites

Ensure that you have Python 3.8 or above installed on your machine.

### Step-by-Step Guide

Run the Application:**
   Launch the Streamlit application by running the following command:
   ```bash
   streamlit run main.py
   ```

5. **Access the App:**
   Once the app is running, open the provided URL in your web browser to access the application.

## Usage

1. **Uploading a PDF Report:**
   - Navigate to the app in your web browser.
   - Upload your blood test report using the provided file uploader.
   
2. **Analyzing the Report:**
   - Click the "Analyze Report" button to start the analysis.
   - The app will process the report and provide detailed insights, including:
     - **Summary of Key Findings:** Highlighting the essential observations from the blood test.
     - **Main Health Concerns:** Listing potential health issues based on the test results.
     - **Recommended Additional Tests or Follow-Ups:** Suggesting further medical tests or follow-ups if needed.
     - **Actionable Lifestyle Advice:** Offering advice on lifestyle changes that could improve or maintain your health.
     - **References to Medical Resources:** Providing links to trusted medical articles for further reading.

## Project Structure

```
medical-report-analysis/
│
├── app.py               # Main application script
├── agents.py            # Definitions of CrewAI agents
├── tasks.py             # Task definitions for CrewAI
├── requirements.txt     # List of Python dependencies
├── .env                 # Environment variables
├── README.md            # Project documentation

```




