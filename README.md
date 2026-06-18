# 🌏 WanderAI - AI Travel Planner

A professional, production-ready AI-powered travel itinerary planner with premium design, built for Bangladesh and international destinations.

## ✨ Features

### Core Features
- **AI-Powered Itinerary Generation** - Uses Groq API (Llama 3.3 70B) for intelligent trip planning
- **9 Interactive Tabs**:
  - 📍 Itinerary - Day-by-day activities with costs and tips
  - 🗺️ Map - Interactive Leaflet map with activity markers
  - 🌤️ Weather - 7-day forecast with emojis
  - 💰 Budget - Visual charts and currency converter
  - 💳 Expenses - Real-time expense tracker
  - 🎒 Packing - AI-generated checklist
  - 🗣️ Phrases - Local phrases with text-to-speech
  - 🏨 Hotels - Recommendations with booking links
  - 🚨 Emergency - Emergency contacts and safety info

### Design Features
- **Premium Glassmorphism UI** - Modern, professional aesthetics
- **Gradient Animations** - Smooth, eye-catching transitions
- **Dark Mode** - Full dark theme support
- **Responsive Design** - Works on all devices
- **Print-Friendly** - Optimized for printing itineraries

### Bangladesh & International Support
- **BDT Currency** - Bangladeshi Taka support
- **Local Destinations** - Cox's Bazar, Sylhet, Rangamati, Bandarban, Dhaka, Saint Martin's Island
- **International Cities** - Paris, Tokyo, Bali, Dubai, New York, London
- **Multi-Currency** - USD, BDT, EUR, GBP support

## 🔑 API Keys (Pre-Configured)

All API keys are already configured and ready to use:

- **Groq API**: `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`
  - Free tier: 30 requests/minute
  - Used for: AI itinerary generation
  
- **ExchangeRate API**: `ce805b42334c58b129da6b49`
  - Free tier: 1,500 requests/month
  - Used for: Currency conversion

- **Open-Meteo**: No key required (completely free)
  - Used for: Weather forecasts

- **OpenStreetMap + Leaflet**: No key required (completely free)
  - Used for: Interactive maps

## 🚀 Deployment to GitHub Pages

### Step 1: Create Repository
```bash
# On GitHub.com, create a new repository
# Name it: wanderai (or any name you prefer)
# Make it Public
```

### Step 2: Upload Files
```bash
# Clone your repository
git clone https://github.com/YOUR_USERNAME/wanderai.git
cd wanderai

# Copy the files
cp /path/to/index.html .
cp /path/to/README.md .

# Commit and push
git add .
git commit -m "Initial commit: WanderAI Travel Planner"
git push origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under "Source", select **Deploy from branch**
4. Branch: **main**, Folder: **/(root)**
5. Click **Save**
6. Wait 1-2 minutes
7. Your site will be live at: `https://YOUR_USERNAME.github.io/wanderai/`

## 📱 How to Use

1. **Open the deployed site**
2. **Enter destination** - Type or click quick-select (Cox's Bazar, Paris, etc.)
3. **Set trip details**:
   - Start date
   - Duration (1-14 days)
   - Daily budget (with currency selection)
   - Number of travelers
4. **Select interests** - Culture, food, adventure, beach, etc.
5. **Click "Generate My Itinerary"**
6. **Explore results** across 9 tabs:
   - View day-by-day itinerary with activities and meals
   - Check interactive map with all locations
   - See weather forecast
   - Review budget breakdown with charts
   - Track expenses during your trip
   - Check packing list
   - Learn local phrases (with audio!)
   - Browse hotel recommendations
   - View emergency contacts

## 🎯 Technical Stack

- **HTML5** - Semantic structure
- **Tailwind CSS** - Utility-first styling
- **Vanilla JavaScript** - No framework dependencies
- **Leaflet.js** - Interactive maps
- **Chart.js** - Data visualization
- **Groq API** - AI-powered content generation
- **Open-Meteo API** - Weather data
- **ExchangeRate API** - Currency conversion

## 📊 File Statistics

- **Total Lines**: 1,791
- **File Size**: 90.98 KB
- **Single File**: Just `index.html` - no build step needed
- **Zero Dependencies**: All libraries loaded from CDN

## 🔒 Security & Privacy

- ✅ All API calls are client-side
- ✅ No user data collected
- ✅ No cookies or tracking
- ✅ No ads
- ✅ 100% free to use

## 🎨 Design Highlights

- **Glassmorphism** - Modern frosted glass effects
- **Gradient Text** - Eye-catching color transitions
- **Smooth Animations** - Professional micro-interactions
- **Premium Cards** - Elevated UI components
- **Responsive Grid** - Adapts to all screen sizes
- **Dark Mode** - Full theme support

## 🌟 Key Differentiators

1. **Bangladesh-First** - Built with BDT currency and local destinations
2. **9 Comprehensive Tabs** - More features than any competitor
3. **Expense Tracker** - Real-time budget management
4. **Local Phrases** - With text-to-speech pronunciation
5. **Emergency Info** - Safety contacts for travelers
6. **Countdown Timer** - Trip anticipation feature
7. **Zero Setup** - API keys pre-configured

## 📝 Customization

### Change API Keys
Edit the constants at the top of the `<script>` section:
```javascript
const GROQ_API_KEY = 'your_key_here';
const EXCHANGE_API_KEY = 'your_key_here';
```

### Add More Destinations
Edit the destination cards in the HTML:
```html
<div class="destination-card" onclick="quickSelect('Your City, Country')">
```

### Customize Colors
Edit the Tailwind config in the `<script>` section:
```javascript
colors: {
    primary: { /* your colors */ },
    accent: { /* your colors */ }
}
```

## 🐛 Troubleshooting

**Issue**: API calls failing
- **Solution**: Check your internet connection. API keys are rate-limited.

**Issue**: Map not loading
- **Solution**: Ensure Leaflet CSS and JS are loading from CDN.

**Issue**: Dark mode not working
- **Solution**: Click the moon/sun icon in the top navigation.

**Issue**: Currency converter not working
- **Solution**: ExchangeRate API has a 1,500 request/month limit.

## 📄 License

MIT License - Free to use, modify, and distribute.

## 🤝 Contributing

Contributions welcome! Feel free to:
- Add more destination presets
- Improve UI/UX
- Add new features
- Fix bugs
- Improve documentation

## 📧 Contact

- **Email**: Aryanrifat1@gmail.com
- **WhatsApp**: +880 1947-653255
- **Instagram**: @tawsif_tibro
- **Facebook**: [Profile Link](https://www.facebook.com/share/17iGBRuHxW/)
- **LinkedIn**: [Profile Link](https://www.linkedin.com/in/your-profile/)

## 🙏 Acknowledgments

- **Groq** - For fast, free AI inference
- **Open-Meteo** - For free weather data
- **OpenStreetMap** - For free map data
- **Leaflet** - For excellent map library
- **Chart.js** - For beautiful charts
- **Tailwind CSS** - For utility-first CSS

---

**Made with ❤️ for travelers worldwide**

*100% Free • No Ads • No Tracking • Open Source*
