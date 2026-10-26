# 📊 Stock Valuation Report – DCF Model

<p align="center">
  <img src="https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java 21"/>
  <img src="https://img.shields.io/badge/Spring_Boot-3-green?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot"/>
  <img src="https://img.shields.io/badge/React-Vite-blue?style=for-the-badge&logo=react&logoColor=white" alt="React"/>
  <img src="https://img.shields.io/badge/DCF-Valuation-purple?style=for-the-badge" alt="DCF Valuation"/>
</p>

<p align="center">
  <b>A full-stack financial analysis application for estimating a company's intrinsic stock value using the Discounted Cash Flow (DCF) method.</b>
</p>

---

## 🚀 About the Project

The **Stock Valuation Report** is a Java Full Stack web application designed to analyze financial performance and estimate the intrinsic value of a company's stock using the Discounted Cash Flow (DCF) method.

The application combines a **Java Spring Boot backend** with a **React frontend** to calculate projected cash flows, estimate company valuation, and analyze how changes in financial assumptions affect the results.

## ✨ Features

- 📈 Forecast revenue and free cash flow for five years.
- 💰 Calculate intrinsic stock value using the DCF method.
- 🧮 Calculate Weighted Average Cost of Capital (WACC).
- 🏢 Estimate terminal value, enterprise value, and equity value.
- 📊 Analyze valuation sensitivity using different WACC and terminal growth assumptions.
- 📉 Visualize revenue and cash-flow forecasts through interactive charts.
- 📥 Export forecast data as a CSV file.
- ⚙️ Update financial assumptions and recalculate the valuation.

## 🛠️ Tech Stack

### 🔹 Backend
- ☕ Java 21
- 🌱 Spring Boot
- 🔗 Spring Web
- ✅ Bean Validation
- 🔌 REST APIs

### 🔹 Frontend
- ⚛️ React
- ⚡ Vite
- 📊 Recharts
- 🎨 HTML and CSS

### 🔹 Development Tools
- 📦 Maven
- 🐙 Git and GitHub
- 💻 VS Code / IntelliJ IDEA

## 📁 Project Structure

```text
DCF_Stock_Valuation_Java_FullStack/
│
├── backend/
│   ├── src/
│   │   ├── main/
│   │   └── test/
│   └── pom.xml
│
├── frontend/
│   ├── src/
│   ├── package.json
│   └── vite.config.js
│
├── docs/
│   ├── investment_thesis_template.md
│   └── data_source_checklist.md
│
├── screenshots/
└── README.md
```

## ⚙️ How to Run the Project

### 1️⃣ Start the Backend

Open a terminal inside the `backend` directory and execute:

```bash
mvn spring-boot:run
```

Backend URL: `http://localhost:8080`

### 2️⃣ Start the Frontend

Open another terminal inside the `frontend` directory and execute:

```bash
npm install
npm run dev
```

Open the local URL displayed in the terminal, usually:

`http://localhost:5173`

**Note:** Keep both terminals running while using the application.

## 🔌 API Endpoints

| Method | Endpoint | Description |
|:---:|---|---|
| 🟢 GET | `/api/health` | Check backend status |
| 🟢 GET | `/api/valuation/default` | Load default valuation inputs |
| 🔵 POST | `/api/valuation/calculate` | Calculate DCF valuation |
| 🔵 POST | `/api/valuation/sensitivity` | Generate sensitivity analysis |

## 📈 DCF Model

### 💵 Free Cash Flow

```text
UFCF = EBIT × (1 − Tax Rate) + D&A − CapEx − Change in NWC
```

### 🧮 Terminal Value

```text
Terminal Value = Final Forecast UFCF × (1 + Growth Rate)
                 / (WACC − Growth Rate)
```

The model discounts forecast cash flows to estimate enterprise value, adjusts for cash and debt to estimate equity value, and calculates the implied value per share.

## 📸 Screenshots

Add screenshots of the running application to the `screenshots/` folder and display them here.

### 🖥️ Dashboard Overview

![Dashboard Overview](screenshots/01-dashboard-overview.png)

### 📊 Five-Year DCF Forecast

![Five-Year DCF Forecast](screenshots/02-five-year-dcf-forecast.png)

### 📉 Sensitivity Analysis

![Sensitivity Analysis](screenshots/03-sensitivity-analysis.png)

## 🔮 Future Improvements

- 📡 Integrate verified financial data from company annual reports.
- 📊 Add bull, base, and bear valuation scenarios.
- 🏦 Introduce comparable-company valuation using P/E and EV/EBITDA.
- 🧪 Expand automated testing and error handling.
- ☁️ Deploy the application online.

## 👨‍💻 Author

**Your Name**

💼 Java Full Stack Developer | Spring Boot | Apache Kafka | REST APIs | SQL

- 🐙 GitHub: https://github.com/phaneendrak-gif
- 💼 LinkedIn: https://www.linkedin.com/in/phaneendra1345/
> Replace the placeholders with your actual name and profile links before publishing.

## 📄 License

This project is available under the MIT License if you include an MIT `LICENSE` file in the repository. Otherwise, specify the license you actually intend to use.

---

<p align="center">
  ⭐ If you find this project useful, consider giving the repository a star!
</p>
