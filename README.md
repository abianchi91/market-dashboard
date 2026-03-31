# Markets Dashboard 📈

A premium, minimalist, and real-time markets dashboard designed for easy monitoring. It is a Progressive Web App (PWA) that can be installed on mobile or desktop for a full-screen, native-like experience.

## Features
- **Real-time Data**: Fetches data directly from Public Market Quote Services.
- **Auto-Refresh**: Automatically updates all market quotes every 60 seconds.
- **PWA Ready**: Installable on iPhone, Android, and Desktop with a custom gold-themed icon.
- **Full-Screen Experience**: Optimized for an immersive, native-app feel when launched from the home screen.
- **Mobile First**: Vertically optimized layout that fits entire global markets on a single phone screen.

## How to Customize Tickers
You can easily modify which markets and instruments are shown by editing the `config.json` file. You **do not** need to touch the HTML code in `index.html`.

### 1. Change Regions or Symbols
Locate the `"regions"` object in `config.json`. Add or remove symbols from the arrays:
```json
"regions": {
  "Futures": ["@SP.1", "@ND.1", ".VIX"],
  "Asia": [".N225", ".SSEC", ...],
  "My New Region": ["SYMBOL1", "SYMBOL2"]
}
```

### 2. Update Labels
Map symbols to human-readable names in the `"symbolLabel"` object:
```json
"symbolLabel": {
  "@SP.1": "S&P",
  "SYMBOL1": "My Instrument Name"
}
```

### 3. Change Emojis
Assign flags or symbols in the `"symbolEmoji"` object:
```json
"symbolEmoji": {
  "@SP.1": "🇺🇸",
  "SYMBOL1": "🚀"
}
```