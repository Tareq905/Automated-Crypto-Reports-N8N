AUTOMATED CRYPTO REPORTING SYSTEM
SYSTEM ARCHITECTURE DOCUMENT

PROJECT OVERVIEW
This project is an automated crypto market reporting system developed using n8n. The system fetches live cryptocurrency market data, processes and formats the data, generates AI-based market analysis, builds professional HTML reports, and distributes them automatically via email. The architecture is modular, scalable, and designed with read-only data access to ensure safety and reliability.

TRIGGER LAYER
The workflow starts with a Manual Trigger node. This trigger is used to start the automation manually for testing and development purposes. In production, this trigger can be replaced with a Schedule Trigger to run the workflow automatically at defined intervals.

DATA EXTRACTION LAYER
The system fetches market data from the CoinGecko public API. This API does not require an API key for the used endpoints. The workflow retrieves real-time cryptocurrency market data such as current price, 24-hour high and low, volume, all-time high, all-time low, and supply-related metrics. The architecture allows easy expansion to support multiple cryptocurrencies.

DATA PROCESSING LAYER
JavaScript Code nodes are used to process the raw API responses. This layer extracts the required fields, handles missing or undefined values, formats numeric values, and standardizes the output structure. The processed data becomes clean, consistent, and ready for analysis and reporting.

PROMPT PREPARATION LAYER
A dedicated node prepares structured textual input using the processed data. This text is formatted as a prompt for AI-based analysis. It includes market values, timestamps, and contextual instructions to generate concise and professional insights.

AI ANALYSIS LAYER
An AI language model is used to generate short market analysis text. The AI analyzes price behavior, volatility, liquidity, risk, and overall market sentiment. This layer focuses only on textual interpretation and does not modify or calculate numerical data.

POST-PROCESSING LAYER
Additional JavaScript processing ensures that the AI-generated text is clean and free from unwanted characters or formatting issues. This step guarantees compatibility with email and HTML rendering.

REPORT GENERATION LAYER
The system generates a professional HTML report using JavaScript. The report includes structured sections such as price overview, liquidity and volume, all-time levels, and supply information. The output is designed to be email-ready and visually clear.

DISTRIBUTION LAYER
The final HTML report is sent automatically using email services such as Gmail or Outlook. This layer ensures that the generated report reaches the intended recipients without manual intervention.

DATA FLOW SUMMARY
Trigger initiates workflow. Market data is fetched from CoinGecko. Data is cleaned and formatted. A prompt is generated for AI analysis. AI produces market insights. Output text is cleaned. An HTML report is generated. The report is delivered via email.

DESIGN PRINCIPLES
The system follows read-only data access, separation of concerns, modular workflow design, and easy extensibility. It is suitable for production automation as well as portfolio and CV demonstration.

POSSIBLE EXTENSIONS
The workflow can be extended with scheduled execution, support for multiple cryptocurrencies, data storage in databases or spreadsheets, Slack or Telegram notifications, and dashboard integration.

PROJECT DESCRIPTION FOR PORTFOLIO
Automated Crypto Market Reporting and Analysis System built with n8n, R
