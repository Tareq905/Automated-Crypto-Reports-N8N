<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Automated Crypto Reporting System</title>
  <style>
    body {
      font-family: Arial, Helvetica, sans-serif;
      background-color: #f5f7fb;
      margin: 0;
      padding: 0;
      color: #1f2937;
      line-height: 1.6;
    }
    .container {
      max-width: 900px;
      margin: 40px auto;
      background: #ffffff;
      padding: 40px;
      border-radius: 12px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.08);
    }
    header {
      border-bottom: 2px solid #e5e7eb;
      padding-bottom: 20px;
      margin-bottom: 30px;
    }
    header h1 {
      margin: 0;
      color: #4f46e5;
      font-size: 32px;
    }
    header p {
      margin-top: 8px;
      color: #6b7280;
      font-size: 16px;
    }
    section {
      margin-bottom: 32px;
    }
    section h2 {
      color: #4f46e5;
      font-size: 22px;
      margin-bottom: 12px;
    }
    ul {
      padding-left: 20px;
    }
    li {
      margin-bottom: 8px;
    }
    .architecture-step {
      background: #f9fafb;
      border-left: 4px solid #4f46e5;
      padding: 12px 16px;
      margin-bottom: 12px;
      border-radius: 6px;
    }
    footer {
      border-top: 1px solid #e5e7eb;
      padding-top: 20px;
      margin-top: 40px;
      font-size: 14px;
      color: #6b7280;
      text-align: center;
    }
    code {
      background: #eef2ff;
      padding: 2px 6px;
      border-radius: 4px;
      font-size: 14px;
    }
  </style>
</head>

<body>
  <div class="container">

    <header>
      <h1>Automated Crypto Reporting System</h1>
      <p>An end-to-end automation workflow built with n8n for crypto market analysis and reporting</p>
    </header>

    <section>
      <h2>Overview</h2>
      <p>
        This project demonstrates an <strong>end-to-end crypto market automation system</strong> built using <strong>n8n</strong>.
        It fetches live cryptocurrency market data, processes and formats the data, generates AI-based market analysis,
        creates professional HTML reports, and distributes them automatically via email.
      </p>
      <p>
        The system is designed with <strong>read-only data access</strong>, ensuring safety, reliability, and easy extensibility.
      </p>
    </section>

    <section>
      <h2>Features</h2>
      <ul>
        <li>Fetches live cryptocurrency market data (price, volume, ATH, ATL, supply metrics)</li>
        <li>Cleans and normalizes raw API data using JavaScript</li>
        <li>Generates AI-based market analysis</li>
        <li>Creates professional, email-ready HTML reports</li>
        <li>Automatically sends reports via Gmail or Outlook</li>
        <li>Modular and scalable workflow design</li>
      </ul>
    </section>

    <section>
      <h2>Architecture</h2>

      <div class="architecture-step">
        <strong>Trigger Layer:</strong>  
        Manual Trigger for development and testing. Can be replaced with a Schedule Trigger for automated execution.
      </div>

      <div class="architecture-step">
        <strong>Data Extraction Layer:</strong>  
        Fetches real-time market data from the CoinGecko Public API (no API key required).
      </div>

      <div class="architecture-step">
        <strong>Data Processing Layer:</strong>  
        JavaScript Code nodes clean, format, and normalize API responses.
      </div>

      <div class="architecture-step">
        <strong>Prompt Preparation Layer:</strong>  
        Prepares structured textual input for AI-based analysis.
      </div>

      <div class="architecture-step">
        <strong>AI Analysis Layer:</strong>  
        Generates concise market insights covering price behavior, volatility, liquidity, and sentiment.
      </div>

      <div class="architecture-step">
        <strong>Post-Processing Layer:</strong>  
        Cleans AI-generated output to ensure compatibility with HTML and email rendering.
      </div>

      <div class="architecture-step">
        <strong>Report Generation Layer:</strong>  
        Builds a professional HTML report with structured sections.
      </div>

      <div class="architecture-step">
        <strong>Distribution Layer:</strong>  
        Automatically delivers reports via email using Gmail or Outlook.
      </div>
    </section>

    <section>
      <h2>Data Flow</h2>
      <p>
        Trigger → CoinGecko API → Data Processing → Prompt Preparation → AI Analysis →
        Post-Processing → HTML Report Generation → Email Delivery
      </p>
    </section>

    <section>
      <h2>Design Principles</h2>
      <ul>
        <li>Read-only data access</li>
        <li>Separation of concerns</li>
        <li>Modular workflow structure</li>
        <li>Easy extensibility</li>
        <li>Production- and portfolio-ready design</li>
      </ul>
    </section>

    <section>
      <h2>Possible Extensions</h2>
      <ul>
        <li>Scheduled execution</li>
        <li>Support for multiple cryptocurrencies</li>
        <li>Data storage in Google Sheets or databases</li>
        <li>Slack or Telegram notifications</li>
        <li>Dashboard integration (Looker Studio)</li>
      </ul>
    </section>

    <section>
      <h2>Portfolio Description</h2>
      <p>
        <strong>Automated Crypto Market Reporting and Analysis System</strong> built with
        <code>n8n</code>, <code>REST APIs</code>, <code>JavaScript</code>, and
        <code>AI-based text generation</code>.
      </p>
    </section>

    <footer>
      © 2025 • Automated Crypto Reporting System • Built for learning, automation, and portfolio demonstration
    </footer>

  </div>
</body>
</html>
