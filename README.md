# ai-fx-scanner
forex AI scanner based on signals
# Native X AI &bull; Institutional Quant & Forex Terminal

<div align="center">

![Terminal Version](https://img.shields.io/badge/version-v2.8-cyan?style=for-the-badge)
![Liquid Glass UI](https://img.shields.io/badge/UI-Liquid%20Glass-blueviolet?style=for-the-badge)
![Node.js](https://img.shields.io/badge/Backend-Node.js%20%2F%20Express-green?style=for-the-badge)
![OpenAI](https://img.shields.io/badge/AI-GPT--4o%20Integrated-orange?style=for-the-badge)

**An elite, futuristic institutional quantitative trading dashboard featuring AI-driven chart screenshot scanning, real-time market data streaming, multi-strategy confluences (ICC, MSNR, ICT/CRT, CISD, SMC), and automated macro news filtering.**

</div>

---

## 🚀 Key Features

* **Liquid Glass UI/UX**: Multi-layered frosted glass panels, ambient fluid glow backdrops, and refractive light highlights designed for high-end quant desks.
* **AI Chart Screenshot Scanner**: Upload mobile or desktop chart screenshots for instant institutional breakdown (Entry, Stop Loss, Take Profit 1 & 2, R:R calculation, and AI reasoning).
* **Multi-Strategy Confluences**: Filter setups by Inducement/CHoCH (ICC), V-Shape Reversals (MSNR), Range Theory (ICT/CRT), Delivery State (CISD), and Smart Money Order Blocks (SMC).
* **Macro Economic News Guard**: Real-time filtering and risk warnings for high-impact events (FOMC, NFP, ECB rate decisions).
* **Visual Trade Journal & Analytics**: Track win rates, average risk-reward ratios, strategy performance breakdowns, and visual image archives side-by-side.

---

## 🛠️ Tech Stack

* **Frontend**: HTML5, Tailwind CSS (with custom Liquid Glass theme extensions), Lucide Icons, JetBrains Mono & Plus Jakarta Sans typography.
* **Backend**: Node.js, Express.js, Multer (for secure chart screenshot uploads), Axios.
* **APIs & Integrations**: Twelve Data API (real-time forex and market feeds) & OpenAI API (`gpt-4o` quantitative analysis).

---

## 📦 Project Structure

```text
ai_forex_scanner/
├── backend/
│   ├── uploads/           # Stored chart screenshots and trade images
│   ├── .env               # Environment configuration & API keys
│   ├── server.js          # Main Express API server & AI orchestrator
│   └── package.json       # Backend dependencies
└── frontend/
    ├── index.html         # Liquid Glass institutional dashboard UI
    └── styles.css         # Custom glassmorphism stylesheet & animations
