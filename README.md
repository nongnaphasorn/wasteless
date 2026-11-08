# Wasteless: Sales Forecasting and Food Waste Prevention Platform

Wasteless is a web-based operational dashboard engineered for cafés and restaurants to optimize inventory management, accurately predict daily demand, and systematically prevent food waste. The platform correlates historical sales data with external environmental factors—such as weather patterns and local events—to generate actionable procurement and sales forecasts.

---

## Key Features

- **Executive Analytics Dashboard**
  Provides high-level operational visibility through key performance indicators (KPIs), including revenue trends, waste reduction metrics, forecast accuracy backtests, and real-time alerts for ingredients nearing expiration.

- **Predictive Demand Forecasting Engine**
  Calculates item-level sales projections by analyzing historical Point of Sale (POS) data against weather forecasts, day classifications (weekday vs. weekend/holiday), and localized event impacts.

- **Automated Bill of Materials (BOM) & Procurement**
  Generates supplier-specific reorder recommendations by matching forecasted dish volume against recipe formulations, current inventory levels, and configurable safety stock buffers.

- **Waste Mitigation & Promotional Campaign Engine**
  Identifies surplus stock nearing shelf-life limits and recommends promotional pricing strategies that maximize ingredient utilization while enforcing minimum profit margin thresholds.

- **Inventory and Recipe Formulation Management**
  Tracks raw material inventory across batches, monitors shelf-life status, calculates recipe Costs of Goods Sold (COGS), and supports full data import/export via CSV format.

- **Artificial Intelligence Assistant**
  Integrates Google's Gemini API to offer an interactive natural language interface capable of querying operational data, inventory risks, and stock recommendations.

- **Digital Signage & Operational Briefings**
  Features a built-in preview interface for in-store promotional displays (Store TV) and automated daily briefing summaries for store managers.

---

## Technical Architecture

- **Frontend Framework:** Native HTML5, Modern JavaScript (ES6+)
- **Styling & Layout:** Tailwind CSS
- **Data Visualization:** Chart.js
- **CSV Data Ingestion:** PapaParse
- **Artificial Intelligence Engine:** Google Gemini API Integration
- **Customer Chat:** Botnoi Customer Chat widget

## Botnoi Chat Integration

Both `index.html` and `wasteless_demo_chatbot.html` load the Botnoi customer chat widget using bot ID `6ad663fa0437519b47c20f14`. The widget uses the Wasteless blue theme, Thai locale, and starts closed. The existing “Ask Wasteless” assistant button is positioned at the lower left to keep it clear of Botnoi’s launcher.

To change the displayed name, greetings, theme, or language, edit the `bn-customerchat` attributes near the end of each HTML file. The widget loads from `https://console.botnoi.ai/customerchat/index.js`, so the page needs an internet connection and the Botnoi bot must be available for the deployment domain.

---

## Installation and Deployment

This application operates as a client-side Web Application and requires no server-side build steps or database deployment.

### Local Development

1. Clone the repository:
   ```bash
   git clone [https://github.com/puifai-tt/wasteless.git](https://github.com/puifai-tt/wasteless.git)
