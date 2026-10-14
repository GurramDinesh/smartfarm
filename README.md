# SmartFarm PRO 🌱
> **"Smarter Farming, Better Harvests."**

SmartFarm is a lightweight, responsive, and bilingual (English & Telugu) agricultural advisory web platform built for college hackathons. It provides instant, evidence-backed crop recommendations, plant disease management tips, water-conservation techniques, and an interactive **Farm Assistant (రైతు మిత్ర)** without requiring complex backends, paid APIs, or external setup.

---

## 🚀 How to Run & Preview the Website

### Option 1: Direct Browser Preview (Instant & Zero-Setup)
1. Open your File Explorer and navigate to:
   ```
   d:\SmartFarm\
   ```
2. **Double-click on [`index.html`](file:///d:/SmartFarm/index.html)**.
3. It will open immediately in your web browser. All features run 100% locally with zero configuration!

### Option 2: Using Python Local Server
If you prefer running through a local development server:
1. Open PowerShell or Command Prompt in `d:\SmartFarm`:
   ```powershell
   python -m http.server 8000
   ```
2. Open your web browser and visit:
   ```
   http://localhost:8000
   ```

---

## 🎯 Key Features Built for Hackathon Demonstration

### 1. 🌾 4-Dimension Smart Crop Advisor
- **User Inputs:**
  1. Soil Type (*Black Cotton, Red, Alluvial, Loamy, Sandy, Clay*)
  2. Cropping Season (*Kharif, Rabi, Zaid*)
  3. Location / State (*Andhra Pradesh, Telangana, Karnataka, Maharashtra, Tamil Nadu, Punjab & Haryana, Uttar Pradesh, Pan-India*)
  4. Available Water Level (*Rainfed <500mm, Moderate 500-900mm, High >900mm*)
- **Output Cards:** Suitable crops with water requirements, growth duration, estimated yield, agronomic rationale, growing considerations, and practical farming tips.
- **Judge Presets:** One-click demo chips (*Black Soil + Kharif*, *Red Soil + Rabi*, *Loamy Soil + Zaid*) so judges can test instantly.

### 2. 🛡️ Crop Disease & Pest Guide with Diagnostic Caution
- **Diagnostic Caution Banner:** Explicit safety note advising farmers that visual symptoms alone cannot confirm diagnosis and recommending local KVK/AEO consultation before applying chemicals.
- **Live Search:** Instant live filtering by crop name, disease name, or visible symptom (e.g., *blast, rot, curl, leaf spots*).
- **Crop Filters:** Quick filter pills (*All, Rice, Cotton, Tomato, Wheat, Chili, Groundnut*).
- **Actionable Guidance:** Key symptoms, pathogen type, risk severity badge, organic prevention, and appropriate next steps.

### 3. 🤖 Farm Assistant (రైతు మిత్ర) Q&A Chatbot
- **Interactive Chat Interface:** Ask questions on crops, soil management, irrigation, organic Jeevamrutham, pests, and government helplines.
- **Bilingual Intelligence:** Supports queries in both English and Telugu.
- **Offline Knowledge Engine:** Built-in fuzzy keyword matching engine that runs without needing any API key or paid subscription.
- **Vercel Serverless Ready:** Pre-configured `/api/chat.js` proxy for optional Gemini/OpenAI server-side integration (keeps API keys completely hidden from client).
- **Suggested Question Chips:** One-click query chips for quick demonstrations.

### 4. 💧 Water-Saving Strategies & Interactive Calculator
- **Actionable Techniques:** Field-tested guides on Drip Irrigation, Organic/Plastic Mulching, Alternate Wetting & Drying (AWD) for paddy, and Farm Ponds (*Panta Kunta*).
- **Interactive Calculator:** Enter farm acreage and select irrigation methods (Flood, Furrow, Drip, Sprinklers) to estimate:
  - Annual water saved (in Lakh Liters / Gallons)
  - Pumping electricity saved (in kWh)
  - Potential crop yield boost (+15% to +25%)

### 5. 🌐 100% Bilingual Support (English & Telugu)
- Toggle button in the navigation bar (`🇮🇳 తెలుగు` / `🌐 English`) switches all UI elements, headings, card contents, recommendations, and labels in real time.
- State persists in your browser (`localStorage`) without losing user inputs or refreshing the page.

---

## 📂 Project Architecture

```
d:\SmartFarm\
├── index.html            # Main semantic HTML structure & layout
├── vercel.json           # Vercel deployment configuration (clean URLs, headers)
├── api\
│   └── chat.js           # Serverless proxy for optional AI query answering
├── css\
│   └── styles.css        # Forest green, leaf green, warm cream & gold design system
├── js\
│   ├── translations.js   # 100% synchronized bilingual dictionary (136 keys)
│   ├── data.js           # Curated agronomic database (Crops, Diseases, Water Tips)
│   ├── knowledge.js      # Offline Q&A knowledge engine for Farm Assistant
│   └── app.js            # Core interactive controller
└── README.md             # Project documentation & presentation cheat-sheet
```

---

## 💡 Quick Tips for Hackathon Presentation
1. **The Hook:** *"Over 80% of smallholder farmers face crop failure from unscientific crop choices and lack access to timely advice in their native language."*
2. **Show Telugu Inclusivity:** Click **`🇮🇳 తెలుగు`** in the navbar to show that local farmers can use the platform comfortably.
3. **Show 4-Dimension Advisor:** Click the **"Black Soil + Kharif"** preset. Point out the growing considerations and water requirements.
4. **Demonstrate Live Disease Search:** Type `"curl"` or `"spots"` in the search bar to demonstrate instant symptom diagnosis and next steps.
5. **Show Farm Assistant (రైతు మిత్ర):** Click a suggested chip like **"How to prepare Jeevamrutham?"** or ask in Telugu **"వరి పొలంలో నీటిని ఎలా ఆదా చేయాలి?"** to demonstrate instant conversational guidance.
6. **Show Water Calculator:** Adjust the slider to 5 acres to showcase saving over **62 Lakh Liters** of water annually.
