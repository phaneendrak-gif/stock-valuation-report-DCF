# 📊 Stock Valuation Report – DCF Model

<h2 style="color:#2563eb;">🚀 About the Project</h2>

The Stock Valuation Report is a full-stack web application built to analyze a company's financial performance and estimate its intrinsic stock value using the Discounted Cash Flow (DCF) method.

<h2 style="color:#16a34a;">✨ Features</h2>

- Calculate intrinsic stock value using the DCF method.
- Forecast revenue and free cash flow for five years.
- Calculate Weighted Average Cost of Capital (WACC).
- Estimate terminal value, enterprise value, and equity value.
- Perform sensitivity analysis using different financial assumptions.
- Visualize financial forecasts through interactive charts.
- Export forecast data as a CSV file.

<h2 style="color:#9333ea;">🛠️ Tech Stack</h2>

**Backend**
- Java 21
- Spring Boot
- Spring Web
- Bean Validation
- REST APIs

**Frontend**
- React
- Vite
- Recharts
- HTML and CSS

**Tools**
- Maven
- Git and GitHub
- VS Code / IntelliJ IDEA

<h2 style="color:#0891b2;">📁 Project Structure</h2>

```text
DCF_Stock_Valuation_Java_FullStack/
├── backend/
├── frontend/
├── docs/
├── screenshots/
└── README.md
```

<h2 style="color:#ea580c;">⚙️ How to Run the Project</h2>

**1. Start the backend**

Open a terminal in the `backend` directory:

```bash
mvn spring-boot:run
```

Backend URL: `http://localhost:8080`

**2. Start the frontend**

Open another terminal in the `frontend` directory:

```bash
npm install
npm run dev
```

Open the local URL shown in the terminal, usually `http://localhost:5173`.

<h2 style="color:#db2777;">🔌 API Endpoints</h2>

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/health` | Check backend status |
| GET | `/api/valuation/default` | Load default inputs |
| POST | `/api/valuation/calculate` | Calculate DCF valuation |
| POST | `/api/valuation/sensitivity` | Generate sensitivity analysis |

<h2 style="color:#0f766e;">📈 DCF Model</h2>

**Free Cash Flow**

`UFCF = EBIT × (1 − Tax Rate) + D&A − CapEx − Change in NWC`

**Terminal Value**

`Terminal Value = Final Forecast UFCF × (1 + Growth Rate) / (WACC − Growth Rate)`

<h2 style="color:#4f46e5;">🔮 Future Improvements</h2>

- Integrate verified financial data from company annual reports.
- Add bull, base, and bear valuation scenarios.
- Introduce comparable-company valuation.
- Improve automated testing and error handling.
- Deploy the application and add screenshots.

<h2 style="color:#64748b;">⚠️ Disclaimer</h2>

This project is intended for educational purposes. Default company inputs are illustrative and have not been verified as current reported financial data. The model is assumption-sensitive and should not be treated as investment advice.
