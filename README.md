# Zee Kelvin - Professional Trading Portfolio Web Application

**Zee Kelvin** is a professional, clean, minimalist, and highly interactive web application for tracking and analyzing a diversified trading portfolio. Designed for experienced traders, it offers a calm, organized, and data-rich environment.

---

## Features

### Core Sections
- **Portfolio Dashboard**: At-a-glance overview with key metrics and visualizations.
- **Trades History**: Detailed sortable, filterable, and expandable record of all transactions.
- **Performance Analytics**: Interactive charts and comparative metrics.
- **Watchlist**: Real-time price widgets for tracked assets (e.g., Gold, UKOIL, USOIL, SPX500, ESP35).
- **Settings**: User preferences, account management, import/export.
- **About**: Personal trading philosophy (optional).
- **Contact/Feedback**: Feedback form or direct contact link (optional).

### Data & Integration
- **Live Market Data**: Widgets for all portfolio/watchlist assets; ready for real-time market data API integration.
- **Trade Entry**: Interactive form with validation, future-ready for automated broker/API imports.

### Interactivity & UI
- **Charts**: TradingView-style, zoom/pan, multi-timeframe, technical indicators (MA, RSI, MACD, etc.), no-gap candles, tooltips, watermark.
- **Tables**: Sortable, searchable, filterable, expandable rows in Trades History and Watchlist.
- **Forms**: Real-time validation, date pickers, ticker suggestions, numeric steppers, confirmation modals.
- **Micro-interactions**: Subtle hover effects, smooth transitions, loading indicators, toast notifications.

### Visual & UX
- **Aesthetic**: Minimalist, professional, and calm. Dark mode primary with #1A1A1A background and #d0d4dc text.
- **Accent**: Muted blue-green (#678797) for highlights, positive/negative P&L, and active states.
- **Typography**: Readable sans-serif fonts.
- **Whitespace**: Generous spacing for clarity and calm.
- **Responsive**: Fully responsive for desktop, tablet, and mobile.

### Inspiration
- [TradingView.com](https://www.tradingview.com): For charts & clean UI.
- [Forex.com](https://www.forex.com), [FXCM](https://www.fxcm.com): For dashboard and portfolio layouts.

---

## Tech Stack

- **Frontend**: React + Vite (or Next.js, if SSR desired)
- **Styling**: Tailwind CSS (for rapid, consistent dark-mode theming)
- **Charts**: Lightweight wrapper around [TradingView Charting Library](https://www.tradingview.com/charting-library/) or [Recharts](https://recharts.org/) / [Chart.js](https://www.chartjs.org/)
- **State Management**: Zustand or Redux Toolkit
- **API**: Ready for real-time market data API integration (Alpaca, Finnhub, etc.)
- **Deployment**: Vercel, Netlify, or Firebase Hosting

---

## Project Structure

```
zee-kelvin/
├── public/
│   └── favicon.ico
├── src/
│   ├── assets/
│   ├── components/
│   │   ├── charts/
│   │   ├── tables/
│   │   ├── forms/
│   │   ├── navigation/
│   │   └── ui/
│   ├── pages/
│   │   ├── Dashboard.jsx
│   │   ├── TradesHistory.jsx
│   │   ├── Analytics.jsx
│   │   ├── Watchlist.jsx
│   │   ├── Settings.jsx
│   │   ├── About.jsx
│   │   └── Contact.jsx
│   ├── styles/
│   │   └── tailwind.css
│   ├── App.jsx
│   ├── main.jsx
│   └── utils/
├── .env.example
├── package.json
└── README.md
```

---

## Quick Start

1. **Install dependencies**
   ```bash
   npm install
   # or
   yarn
   ```

2. **Run development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

3. **Build for production**
   ```bash
   npm run build
   # or
   yarn build
   ```

4. **Deploy** to Vercel, Netlify, or Firebase Hosting.

---

## Live Market Data Integration

- Integrate your preferred market data API (Alpaca, Finnhub, IEX Cloud, etc.) via `.env` configuration.
- See `src/utils/marketData.js` for integration points.

---

## Customization

- To adjust color themes, update `tailwind.config.js` and `src/styles/tailwind.css`.
- To add new asset types or chart features, see `src/components/charts/` and `src/components/forms/AssetForm.jsx`.
- For future broker API integration, see comments in `src/utils/brokerIntegration.js`.

---

## License

MIT

---

## Contact

For feedback, suggestions, or feature requests, please use the Contact form in the application or open an issue on GitHub.
