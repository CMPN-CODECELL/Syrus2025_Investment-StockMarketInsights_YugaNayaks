**Project Implementation and Workflow Documentation**

**Project Overview**

This document provides a detailed explanation of the project implementation along with a comprehensive breakdown of its workflow. The project, titled **InvestmentGuardian**, leverages advanced AI methodologies to create an impactful solution in the financial sector using Agentic AI. The goal is to develop a system that efficiently automates, optimizes, and streamlines financial operations while ensuring robustness, security, and compliance.

**Implementation Details**

Technology Stack
Frontend: React, TailwindCSS
Backend: Uptiq, OpenAPIs

**Unique Features**
1. AI-Powered Fraud Detection Engine
- Uses anomaly detection and behavioral analytics to identify suspicious transactions.
- Automatically flags and notifies users in case of fraudulent activities.
- Enhances security through multi-layered authentication and blockchain verification.

2. Predictive Market Analysis
- Integrates real-time stock market trends, financial news, and social sentiment analysis.
- Uses AI-based predictive modeling to forecast stock performance.
- Provides detailed insights into economic indicators affecting investment decisions.

And many more!

InvestmentGuardian is an AI-driven financial management system with specialized sub-agents for fraud detection, investment insights, risk assessment, and compliance reporting.
🔹 FraudHunter – Detects scams using NLP & anomaly detection. 
🔹 StockGuru – Provides investment insights with risk-based filters. 
🔹 RiskSentinel – Monitors portfolio risks & alerts on volatility. 
🔹 SEBIBot – Ensures compliance with SEBI regulations via API.
![image](https://github.com/user-attachments/assets/77860a70-4243-47d0-afe2-fc323f060c2b)

Features:  
Automated monitoring & real-time alerts  
AI-powered market analysis  
Seamless integration with NSE/BSE & broker APIs
![image](https://github.com/user-attachments/assets/a733990b-a470-41a5-b631-735c37d4f4e9)


**Future Objectives**
AI-Powered Predictive Analytics – Employ deep learning to predict market trends and identify nascent fraud patterns before they scale. 
Blockchain-Driven Transparency – Harness blockchain to provide tamper-proof investment histories and safe fraud reporting.
Autonomous Portfolio Management – Allow AI-driven, auto-tuning investment portfolios depending on market conditions and user risk levels.
Quantum Computing for Simulation of the Market – Leverage quantum algorithms to forecast stock market patterns for extremely precise risk calculation.
![image](https://github.com/user-attachments/assets/371bdb70-6489-401e-bb59-884339777674)


**Detail Workflow For Stock Guru Agent**
- Market Analysis Agent Workflow
  1. Start Node (Workflow Initiation)
    a. This node begins the market analysis workflow.
    b. It collects user input, such as stock ticker symbols, sectors, or financial metrics of interest.
    c. Tagged as Conversational and InvestmentGuardian, indicating it is designed for financial insights.
  2. Prompt (LLM Processing)
    a. A Large Language Model (LLM) processes the user’s request.
    b. It interprets financial terms, refines queries, and generates structured requests for data retrieval.
![image](https://github.com/user-attachments/assets/9d4557a7-1993-4eb5-9a70-2056540be894)

  3. API Call (Fetch Market Data)
    a. The workflow sends a request to Alpha Vantage (https://www.alphavantage.co/query).
    b. Retrieves real-time stock prices, forex data, cryptocurrency details, and market indicators.
    c. Uses parameters like stock ticker symbols and timeframes based on user input.
  4. JavaScript Processing (Data Handling & Computation)
    a. Executes JavaScript to process the API response.
    b. Extracts relevant data, such as price trends and volume.
    c. Performs additional calculations or formatting for better visualization.
  5. Display Nodes (Presenting Data to the User)
    - Two display nodes show the results:
      a. Main Display: Presents refined financial insights.
      b. Secondary Display: Could show raw API responses or intermediate calculations.
  6. Conditional Paths (Handling Success or Failure)
    a. Success Path: If the API call works, data moves to the JavaScript node for processing.
    b. Failure Path: If the API fails (e.g., invalid stock ticker or API limit exceeded), an error message is displayed.

Working Of Agent
![image](https://github.com/user-attachments/assets/17714f5d-4100-4fbe-a8e2-6b7a0292cb76)
**Observations from Execution Logs**
1. Intent Matching: The agent correctly identified the query as related to Market Analysis, meaning the LLM successfully understood the context.
2. Stock Symbol Recognition: The system retrieved multiple stock listings for Tesla Inc. across different exchanges:
TSLA | Equity (NASDAQ)
TL0.DEX | Equity (Likely a European exchange)
3. Detailed Summary Report: The AI agent generates an in-depth analysis of Tesla's stock performance, including:
  a. Price trends over the past year
  b. Key highs and lows
  c. Volatility and trading volume
  d. Market sentiment analysis

4. Debug Mode Enabled: This means you can track how the agent processes the query, making it easier to troubleshoot issues if needed.
![image](https://github.com/user-attachments/assets/626bb52b-5dd3-4ca1-9e90-540f117940d2)

**Execution Steps Involved In Working**
- Execution Flow 
 1. User Input (TSLA Query)Time: 9:36 PM
 2. The agent asks for the stock symbol (TSLA).
 3. Loader (Loading State) Displayed a "Loading..." message to inform the user that data retrieval is in progress.
 4. API Call (Alpha Vantage)Time: 9:37 PMThe agent makes a request to Alpha Vantage (https://www.alphavantage.co/query) to fetch Tesla stock data.
5. Loader (Second Loading Message)Another loading message appears, likely due to a second API request or data processing.
 6. API Call (Second API Request)Another request to Alpha Vantage, possibly fetching different time frames (e.g., historical vs. real-time).
7. Prompt (GPT-4 Processing)Time: 9:37 PMThe AI agent processes the fetched data and formats it into a summary.
8. Display (Final Response)The AI generates a structured response and displays it in the chat
![image](https://github.com/user-attachments/assets/b97b5ac3-f013-441d-9f40-f66b6c27ef28)

**Front-End Screen Shots:**

![image](https://github.com/user-attachments/assets/d52cb595-281d-48e9-a02b-2b8bdf9dfd30)
![image](https://github.com/user-attachments/assets/c9624ee0-6982-41a7-ae7b-c677eb61e47f)
![image](https://github.com/user-attachments/assets/697ad946-d4b3-4fa6-a885-69411b676f35)
