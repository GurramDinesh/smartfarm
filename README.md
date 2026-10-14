# SmartFarm 🌱
> **"Smarter Farming, Better Harvests."**

SmartFarm is a lightweight, responsive, and bilingual (English & Telugu) agricultural advisory web platform built for college hackathons. It provides instant, evidence-backed crop recommendations, plant disease management tips, and water-conservation techniques without requiring complex backends, paid APIs, or external setup.

---

## 🚀 How to Run & Preview the Website

### Option 1: Direct Browser Preview (Instant & Simplest)
1. Open your File Explorer and navigate to:
   ```
   d:\SmartFarm\
   ```
2. **Double-click on [`index.html`](file:///d:/SmartFarm/index.html)**.
3. It will open instantly in your default web browser (Chrome, Edge, Firefox, Brave). Everything runs 100% locally with zero setup!

### Option 2: Using Python Local Server
If you prefer running a local development server:
1. Open PowerShell or Command Prompt in `d:\SmartFarm`:
   ```powershell
   python -m http.server 8000
   ```
2. Open your web browser and visit:
   ```
   http://localhost:8000
   ```

---

## 🎯 Features Included for Hackathon Demo

### 1. 🌾 Smart Crop Advisor
- **User Inputs:** Select from 6 soil types (*Black Cotton, Red, Alluvial, Loamy, Sandy, Clay*) and 3 seasons (*Kharif / Monsoon, Rabi / Winter, Zaid / Summer*).
- **Output Cards:** Shows suitable crops with water requirements, growth duration, estimated yield, agronomic rationale, and practical farming tips.
- **Judge Presets:** One-click demo buttons (*Black Soil + Kharif*, *Red Soil + Rabi*, *Loamy Soil + Zaid*) so judges can test instantly.

### 2. 🛡️ Crop Disease & Pest Guide
- **Live Search:** Instant live filtering by crop name, disease name, or visible symptom (e.g., *blast, rot, curl, leaf spots*).
- **Crop Filters:** Quick filter pills (*All, Rice, Cotton, Tomato, Wheat, Chili, Groundnut*).
- **Actionable Guidance:** Key symptoms, pathogen type, risk severity badge, and prevention/organic treatment tips.

### 3. 💧 Water-Saving Strategies & Interactive Calculator
- **Actionable Techniques:** Field-tested guides on Drip Irrigation, Organic/Plastic Mulching, Alternate Wetting & Drying (AWD) for paddy, and Farm Ponds (*Panta Kunta*).
- **Interactive Calculator:** Enter farm acreage and select irrigation methods (Flood, Furrow, Drip, Sprinklers) to estimate:
  - Annual water saved (in Lakh Liters / Gallons)
  - Pumping electricity saved (in kWh)
  - Potential crop yield boost (+15% to +25%)

### 4. 🌐 Bilingual Support (English & Telugu)
- Toggle button in the navigation bar (`🇮🇳 తెలుగు` / `🌐 English`) switches all UI elements, headings, card contents, recommendations, and labels in real time.
- State persists in your browser (`localStorage`).

### 5. 📖 About & Problem-Solution Breakdown
- Outlines the grassroots challenges faced by smallholder farmers (irrigation stress, unscientific crop choices, delayed disease identification).
- Highlights SmartFarm's lightweight, zero-barrier digital intervention.

---

## 📂 Project Structure

```
d:\SmartFarm\
├── index.html            # Main semantic HTML structure & layout
├── css\
│   └── styles.css        # Green & White clean responsive styling
├── js\
│   ├── translations.js   # Full bilingual dictionaries (English & Telugu)
│   ├── data.js           # Curated agronomic database (Crops, Diseases, Water Tips)
│   └── app.js            # Interactive logic, live search, calculator & language toggle
└── README.md             # Project documentation & presentation guide
```

---

## 💡 Quick Tips for Hackathon Presentation
1. **Start with the Problem:** Explain how smallholder farmers struggle with water scarcity and lack accessible advice in their regional language.
2. **Show the Telugu Toggle:** Click the `🇮🇳 తెలుగు` button in the navbar to show inclusivity for local farmers.
3. **Click a Judge Preset:** In the Crop Advisor, click **"Black Soil + Kharif"** to instantly display Cotton and Soybean with growth requirements.
4. **Demonstrate Live Disease Search:** In the Disease Guide, type `"curl"` or `"spots"` to show instant symptom matching.
5. **Demonstrate Water Calculator:** Change farm size to 5 acres to showcase millions of liters of groundwater saved.
