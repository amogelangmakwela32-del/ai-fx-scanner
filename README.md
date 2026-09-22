# AI FX Scanner

AI-powered forex chart analysis and market-scanning dashboard. Upload a trading-chart screenshot and receive a structured analysis containing potential entry zones, stop-loss and take-profit levels, risk-reward calculations, technical reasoning, and relevant market context.

> **Disclaimer:** This project is for research and educational purposes only. It does not provide financial advice, and its output should not be used as the sole basis for trading decisions. Always verify signals independently and manage risk responsibly.

## Features

- **AI chart analysis**  
  Upload desktop or mobile chart screenshots for automated technical analysis.

- **Trade setup extraction**  
  Identifies possible entries, stop-loss levels, take-profit targets, and estimated risk-reward ratios.

- **Multi-strategy analysis**  
  Supports configurable concepts such as:
  - Inducement and change of character
  - Market-structure shifts
  - ICT/CRT range analysis
  - CISD and delivery-state analysis
  - Smart-money concepts and order blocks

- **Market-news awareness**  
  Displays warnings for potentially high-impact events such as FOMC, NFP, and central-bank decisions.

- **Trade journal and analytics**  
  Record setups, review historical performance, and compare strategy results.

- **Responsive dashboard**  
  Designed for desktop and mobile chart-review workflows.

## Demo

Add a screenshot, hosted demo, or short video here:

```text
https://your-demo-url.example
```

![AI FX Scanner dashboard](docs/dashboard-screenshot.png)

## Tech stack

- **Frontend:** HTML, CSS, Tailwind CSS, Lucide Icons
- **Backend:** Node.js and Express
- **File uploads:** Multer
- **Market data:** Twelve Data API
- **AI analysis:** OpenAI API
- **HTTP client:** Axios

Update this list whenever the implementation changes.

## Project structure

```text
ai-fx-scanner/
├── backend/
│   ├── server.js
│   ├── package.json
│   ├── .env.example
│   └── uploads/
├── frontend/
│   ├── index.html
│   └── styles.css
├── docs/
│   └── dashboard-screenshot.png
├── .gitignore
└── README.md
```

Do not commit `.env`, API keys, or private uploaded chart images.

## Requirements

- Node.js 18 or newer
- npm
- An OpenAI API key
- A Twelve Data API key, if market-data features are enabled

## Installation

Clone the repository:

```bash
git clone https://github.com/amogelangmakwela32-del/ai-fx-scanner.git
cd ai-fx-scanner
```

Install backend dependencies:

```bash
cd backend
npm install
```

Create a local environment file:

```bash
cp .env.example .env
```

Configure the required values:

```env
PORT=3000
OPENAI_API_KEY=your_openai_api_key
TWELVE_DATA_API_KEY=your_twelve_data_api_key
```

Start the backend:

```bash
npm start
```

Then open the frontend according to the project's development setup.

If the project does not yet define an `npm start` script, add one to `backend/package.json` or document the correct command here.

## Environment variables

| Variable | Required | Description |
|---|---:|---|
| `PORT` | No | Port used by the Express server |
| `OPENAI_API_KEY` | Yes | Used for AI chart analysis |
| `TWELVE_DATA_API_KEY` | Optional | Used for forex and market data |
| `UPLOAD_DIR` | Optional | Directory used for uploaded images |

Never expose these values in frontend code or commit them to Git.

## API overview

Document the actual routes implemented by the backend. For example:

| Method | Endpoint | Description |
|---|---|---|
| `GET` | `/health` | Returns service health information |
| `POST` | `/api/scan` | Analyzes an uploaded chart image |
| `GET` | `/api/market-data` | Retrieves market data |
| `POST` | `/api/trades` | Saves a journal entry |

Replace these examples with the project's real endpoints and request formats.

## Upload and security considerations

Because the application accepts image uploads:

- Validate file type and file size on the server.
- Generate safe, unique filenames.
- Do not serve arbitrary uploaded files without access controls.
- Remove old or unused uploads.
- Add `backend/uploads/` to `.gitignore` unless sample images are intentionally tracked.
- Add authentication and rate limiting before deploying publicly.
- Avoid logging API keys or sensitive chart data.

## Development

Run the backend in development mode if a development script is available:

```bash
npm run dev
```

Before opening a pull request:

```bash
npm test
npm run lint
```

Add these scripts to `package.json` if they are not yet configured.

## Limitations

AI-generated chart analysis may be incomplete or incorrect. Results can be affected by:

- Low-resolution or cropped screenshots
- Missing timeframe or symbol information
- Ambiguous chart structures
- Delayed or unavailable market data
- Unexpected market volatility

Always validate the analysis against live charts and your own trading plan.

## Contributing

1. Create a feature branch.
2. Make focused changes.
3. Add or update tests where appropriate.
4. Update the documentation.
5. Open a pull request with a clear description of the change.

## License

Add the project's license here, for example:

```text
This project is licensed under the MIT License. See LICENSE for details.
```

If the project is not open source, state that clearly instead.
