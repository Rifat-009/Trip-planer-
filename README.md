# 🌏 WanderAI - AI Travel Planner

<div align="center">

![WanderAI](https://img.shields.io/badge/WanderAI-Travel%20Planner-blue?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxMDAgMTAwIj48dGV4dCB5PSIuOWVtIiBmb250LXNpemU9IjkwIj7wn4yPPC90ZXh0Pjwvc3ZnPg==)
![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)
![Responsive](https://img.shields.io/badge/Responsive-Yes-success?style=for-the-badge)
![PWA](https://img.shields.io/badge/PWA-Ready-blueviolet?style=for-the-badge)

**AI-powered travel itinerary planner for Bangladesh and worldwide destinations**

[Live Demo](https://rifat-009.github.io/Trip-planer-/) • [Report Bug](https://github.com/Rifat-009/Trip-planer-/issues) • [Request Feature](https://github.com/Rifat-009/Trip-planer-/issues)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [API Integration](#-api-integration)
- [Installation](#-installation)
- [Usage](#-usage)
- [Responsive Design](#-responsive-design)
- [Project Structure](#-project-structure)
- [Browser Support](#-browser-support)
- [Contributing](#-contributing)
- [License](#-license)
- [Credits](#-credits)

---

## 🌟 Overview

WanderAI is a comprehensive AI-powered travel planning application that creates personalized itineraries for destinations worldwide. Built with modern web technologies, it offers a seamless experience across all devices with offline capabilities through PWA support.

### ✨ Key Highlights

- 🤖 **AI-Powered Planning** - Generate detailed itineraries using Groq's Llama 3.3 70B model
- 🌍 **Global Coverage** - Plan trips to any destination worldwide
- 📱 **Fully Responsive** - Optimized for mobile, tablet, and desktop
- 📴 **Offline Support** - PWA with service worker for offline access
- 💰 **Budget Tracking** - Real-time expense tracking with visual charts
- 🎤 **Voice Guide** - Text-to-speech narration for activities
- 📸 **Photo Journal** - Capture and organize travel memories
- 🔄 **Smart Rescheduling** - Auto-adjust plans based on weather

---

## 🚀 Features

### Core Features

#### 🗺️ Trip Planning
- **AI Itinerary Generation** - Detailed day-by-day plans with activities, meals, and costs
- **Interactive Maps** - Leaflet maps with activity markers and location details
- **Weather Forecasts** - 16-day forecast from Open-Meteo API
- **Hotel Recommendations** - AI-suggested accommodations with booking links
- **Emergency Contacts** - Local emergency numbers for your destination

#### 💰 Budget & Expenses
- **Budget Overview** - Track total budget vs actual spending
- **Expense Tracker** - Add expenses with categories (food, transport, activity, shopping)
- **Category Charts** - Visual breakdown of spending by category using Chart.js
- **Real Cost Data** - AI-estimated prices for 12 common items at your destination
- **Currency Converter** - Real-time currency conversion using ExchangeRate API

#### 📱 Travel Tools
- **Packing List** - Interactive checklist with checkboxes
- **Phrasebook** - Useful phrases with translations and pronunciation
- **Photo Journal** - Upload photos, write entries, save memories
- **Local Events** - AI-generated events and festivals during travel dates
- **Voice-Guided Tours** - Text-to-speech narration for each activity

#### 🔄 Advanced Features
- **Smart Weather Rescheduling** - Detect bad weather and auto-swap to indoor activities
- **Collaborative Sharing** - Generate share codes for travel companions
- **Social Share Cards** - Generate downloadable PNG images of your trip
- **Place Explorer** - Search destinations with Wikipedia integration, country data, and images
- **Save Trips** - Save itineraries to localStorage for later access

---

## 🛠️ Technologies Used

### Frontend
- **HTML5** - Semantic markup
- **CSS3** - Modern styling with gradients, glassmorphism, animations
- **JavaScript (ES6+)** - Vanilla JS, no frameworks
- **Tailwind CSS** - Utility-first CSS framework (via CDN)
- **Font Awesome 6.5.1** - Icon library

### Libraries & APIs
- **Leaflet 1.9.4** - Interactive maps
- **OpenStreetMap** - Map tiles and geocoding
- **Chart.js 4.4.1** - Data visualization
- **html2canvas 1.4.1** - Screenshot generation for share cards

### APIs (All Free)
- **Groq API** - AI itinerary generation (Llama 3.3 70B)
- **Open-Meteo** - Weather forecasts and geocoding
- **ExchangeRate API** - Currency conversion
- **Wikipedia API** - Place descriptions and images
- **REST Countries API** - Country information (population, languages, currency)

---

## 🔑 API Integration

### Pre-configured API Keys

The application comes with pre-configured API keys for immediate use:

```javascript
// Groq API (AI Generation)
const DEFAULT_GROQ_KEY = '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';

// ExchangeRate API (Currency Conversion)
const DEFAULT_EXCHANGE_KEY = 'ce805b42334c58b129da6b49';
```

### Free API Services Used

| Service | Purpose | Rate Limit |
|---------|---------|------------|
| **Groq** | AI itinerary generation | 30 requests/minute |
| **Open-Meteo** | Weather & geocoding | 10,000 requests/day |
| **ExchangeRate** | Currency conversion | 1,500 requests/month |
| **Wikipedia** | Place descriptions | Unlimited |
| **REST Countries** | Country data | Unlimited |
| **OpenStreetMap** | Maps & tiles | Fair use policy |

### Custom API Keys

Users can add their own API keys via the Settings modal:
1. Click the gear icon in the navigation
2. Enter your Groq API key (get one at [console.groq.com](https://console.groq.com))
3. Enter your ExchangeRate API key (get one at [exchangerate-api.com](https://www.exchangerate-api.com))
4. Click "Save Settings"

---

## 📦 Installation

### Option 1: GitHub Pages (Recommended)

1. **Fork or Clone the Repository**
   ```bash
   git clone https://github.com/Rifat-009/Trip-planer-.git
   cd Trip-planer-
   ```

2. **Upload to GitHub**
   - Create a new repository on GitHub
   - Upload all files from the `output/` folder:
     - `index.html`
     - `manifest.json`
     - `sw.js`

3. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Source: Deploy from branch
   - Branch: `main` / `root`
   - Save

4. **Access Your Site**
   - Your site will be live at: `https://yourusername.github.io/repository-name/`

### Option 2: Local Development

1. **Download Files**
   ```bash
   git clone https://github.com/Rifat-009/Trip-planer-.git
   cd Trip-planer-
   ```

2. **Start Local Server**
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve
   
   # Using PHP
   php -S localhost:8000
   ```

3. **Open in Browser**
   - Navigate to `http://localhost:8000`

---

## 📖 Usage

### Planning a Trip

1. **Enter Destination**
   - Type any city, country, or landmark
   - Use quick-select buttons for popular destinations

2. **Set Trip Details**
   - **Start Date**: Choose your travel date
   - **Duration**: 1-14 days
   - **Budget**: Daily budget in your preferred currency (USD, BDT, EUR, GBP)
   - **Travelers**: Solo, couple, family, or group

3. **Select Interests**
   - Choose from: Culture, Food, Adventure, Nature, Beach, Shopping, History, Photography

4. **Generate Itinerary**
   - Click "Generate My Itinerary"
   - Wait for AI to create your personalized plan (usually 10-30 seconds)

### Exploring Your Itinerary

After generation, you'll see 13 tabs:

| Tab | Description |
|-----|-------------|
| **Itinerary** | Day-by-day activities with times, costs, and descriptions |
| **Map** | Interactive map with all activity locations |
| **Weather** | 16-day weather forecast with icons |
| **Budget** | Total budget overview |
| **Expenses** | Track spending with charts and real cost data |
| **Hotels** | AI-recommended accommodations |
| **Packing** | Interactive checklist |
| **Phrases** | Useful local phrases with pronunciation |
| **Currency** | Real-time currency converter |
| **Journal** | Photo diary with entries |
| **Events** | Local festivals and events |
| **Voice Guide** | Audio narration for activities |
| **Emergency** | Local emergency contacts |

### Advanced Features

#### Place Explorer
- Search any destination in the "Explore Any Place" section
- View Wikipedia description, country info, coordinates
- See population, languages, currency
- Click "Plan Trip Here" to quickly fill the planner

#### Photo Journal
- Navigate to the Journal tab
- Upload photos (automatically compressed)
- Add titles and descriptions
- Entries saved to localStorage

#### Smart Weather Rescheduling
- If bad weather is detected, a banner appears
- Click "Auto-Reschedule" to swap outdoor activities for indoor alternatives
- AI generates appropriate indoor activities

#### Collaborative Sharing
- Click "Collaborate" button
- Generate a unique share code
- Share the code with travel companions
- They can import the trip using the code

#### Social Share Cards
- Click "Share Card" button
- Generates a 1080x1080 PNG image
- Includes destination, duration, budget, and highlights
- Downloads automatically

---

## 📱 Responsive Design

### Breakpoints

| Device | Width | Optimizations |
|--------|-------|---------------|
| **Mobile** | < 768px | Single column, larger touch targets, reduced padding |
| **Tablet** | 768px - 1024px | 2-column grids, balanced spacing |
| **Desktop** | > 1024px | Full features, multi-column layouts |
| **Large Desktop** | > 1440px | Maximum content width, enhanced spacing |

### Mobile-Specific Features

- **Touch-Friendly** - Minimum 44px touch targets
- **Horizontal Scroll Tabs** - Swipe through tabs on small screens
- **Optimized Chat** - Full-width chat panel on mobile
- **Reduced Animations** - Smoother performance on mobile
- **Landscape Support** - Adjusted layout for landscape orientation

### Responsive Images

- All images use `loading="lazy"` for performance
- Responsive sizing with `max-width: 100%`
- Optimized for different screen densities

---

## 📁 Project Structure

```
Trip-planer-/
│
├── index.html          # Main application (2,518 lines)
│   ├── HTML structure
│   ├── CSS styles (inline)
│   └── JavaScript (inline)
│
├── manifest.json       # PWA manifest
│   ├── App metadata
│   ├── Icons
│   └── Theme colors
│
├── sw.js              # Service Worker
│   ├── Cache management
│   ├── Offline support
│   └── Fetch handling
│
└── README.md          # Documentation (this file)
```

### Code Organization

The `index.html` file is organized into sections:

1. **Head Section** (Lines 1-31)
   - Meta tags
   - CDN links
   - External libraries

2. **CSS Styles** (Lines 32-1000)
   - Base styles
   - Component styles
   - Responsive media queries
   - Animations

3. **HTML Body** (Lines 1001-1400)
   - Navigation
   - Settings modal
   - Hero section
   - Place Explorer
   - Trip Planner form
   - Results section with 13 tabs
   - Chat widget
   - Share modal
   - Footer

4. **JavaScript** (Lines 1401-2518)
   - State management
   - API key configuration
   - Form handlers
   - Render functions (13 tabs)
   - Feature implementations
   - Event listeners

---

## 🌐 Browser Support

| Browser | Version | Status |
|---------|---------|--------|
| **Chrome** | 90+ | ✅ Full support |
| **Firefox** | 88+ | ✅ Full support |
| **Safari** | 14+ | ✅ Full support |
| **Edge** | 90+ | ✅ Full support |
| **Opera** | 76+ | ✅ Full support |
| **Samsung Internet** | 15+ | ✅ Full support |

### Required Features

- ES6+ JavaScript
- CSS Grid & Flexbox
- Fetch API
- LocalStorage
- Service Workers (for PWA)
- Web Speech API (for voice guide)

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

### Reporting Bugs

1. Check existing [issues](https://github.com/Rifat-009/Trip-planer-/issues)
2. Create a new issue with:
   - Clear description
   - Steps to reproduce
   - Expected vs actual behavior
   - Browser and device info

### Suggesting Features

1. Open a [feature request](https://github.com/Rifat-009/Trip-planer-/issues/new)
2. Describe the feature
3. Explain the use case
4. Provide examples if possible

### Pull Requests

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see below for details:

```
MIT License

Copyright (c) 2025 WanderAI

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🙏 Credits

### Developer
- **Tawsif Tibro** - [GitHub](https://github.com/Rifat-009)

### APIs & Services
- [Groq](https://groq.com/) - AI inference platform
- [Open-Meteo](https://open-meteo.com/) - Free weather API
- [ExchangeRate-API](https://www.exchangerate-api.com/) - Currency conversion
- [Wikipedia](https://www.wikipedia.org/) - Place descriptions
- [REST Countries](https://restcountries.com/) - Country data
- [OpenStreetMap](https://www.openstreetmap.org/) - Map data
- [Leaflet](https://leafletjs.com/) - Interactive maps

### Libraries
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS
- [Font Awesome](https://fontawesome.com/) - Icons
- [Chart.js](https://www.chartjs.org/) - Data visualization
- [html2canvas](https://html2canvas.hertzen.com/) - Screenshot generation

### Design Inspiration
- Modern glassmorphism UI
- Gradient color schemes
- Smooth animations and transitions

---

## 📞 Contact & Support

### Social Links
- **Instagram**: [@tawsif_tibro](https://www.instagram.com/tawsif_tibro)
- **Facebook**: [Tawsif Tibro](https://www.facebook.com/share/17iGBRuHxW/)
- **LinkedIn**: [Tawsif Tibro](https://www.linkedin.com/in/tawsif-tibro)
- **WhatsApp**: [+880 1947-653255](https://wa.me/8801947653255)

### Email
- **Contact**: tawsiftibro@gmail.com

---

## 🗺️ Roadmap

### Planned Features
- [ ] Multi-language support
- [ ] Flight search integration
- [ ] Restaurant recommendations
- [ ] Offline map downloads
- [ ] Trip cost estimation before generation
- [ ] Social features (share trips publicly)
- [ ] Mobile app (React Native)
- [ ] Backend for user accounts

### In Progress
- [ ] Enhanced AI prompts for better itineraries
- [ ] More destination-specific data
- [ ] Improved offline capabilities

---

## 📊 Statistics

- **Total Lines of Code**: 2,518
- **Features**: 13 main tabs + 10 advanced features
- **APIs Integrated**: 6 free APIs
- **Responsive Breakpoints**: 4 (mobile, tablet, desktop, large)
- **Browser Support**: 6 major browsers
- **PWA Ready**: Yes (with service worker)

---

## 🎯 Quick Start

1. **Visit the Live Demo**: [https://rifat-009.github.io/Trip-planer-/](https://rifat-009.github.io/Trip-planer-/)
2. **Enter a Destination**: Try "Cox's Bazar" or "Paris"
3. **Set Your Preferences**: Duration, budget, interests
4. **Generate Itinerary**: Click the magic button
5. **Explore**: Navigate through all 13 tabs
6. **Save & Share**: Use the action buttons

---

<div align="center">

**Made with ❤️ for travelers worldwide**

⭐ Star this repo if you find it useful!

[Live Demo](https://rifat-009.github.io/Trip-planer-/) • [Report Bug](https://github.com/Rifat-009/Trip-planer-/issues) • [Request Feature](https://github.com/Rifat-009/Trip-planer-/issues)

</div>
