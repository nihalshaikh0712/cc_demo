
# 🍽️ CityWise | Premium Food Explorer

CityWise is a **high-end, real-time web application** built for food lovers and travelers to discover **curated dining experiences** across major Indian cities.  
It combines a **premium UI**, **smart filtering**, and **seamless user feedback**, all powered by **Flask**.

---

## 🚀 Key Features

### 🔍 Real-Time Restaurant Discovery
- Instant search across **180+ restaurants**
- Covers major Indian cities:
  - Sangli
  - Kolhapur
  - Pune
  - Mumbai
  - Bangalore
- Fast client-side rendering using structured datasets

---

### 🎛️ Advanced Multi-Filtering System
- **Budget Slider**  
  Filter restaurants by *price per person*

- **Rating Filters**  
  Choose minimum quality thresholds:
  - 3.5 ★
  - 4.0 ★
  - 4.5 ★

- **Cuisine Filtering**  
  Narrow results by cuisine type (Indian, Chinese, etc.)

---

### ⚡ Smart Search Logic
- Results load **only after clicking “Explore Now”**  
  → Prevents accidental or unnecessary loading
- Once results are visible:
  - Meal filters (**Breakfast / Lunch / Dinner**) update **instantly**

---

### 💬 Seamless Feedback System
- Custom-themed **Feedback Modal**
- Integrated with **Formspree**
- Sends user feedback directly to email
- No page reloads (smooth UX)

---

## 🛠️ Tech Stack

### Frontend
- HTML5
- CSS3 (Custom Premium Theme)
- Bootstrap 5
- JavaScript (Vanilla)
- Font Awesome 6

### Backend
- Python
- Flask

### APIs & Services
- Formspree (Feedback handling)
- Google Maps (Navigation)

---

```markdown
## 📂 Project Structure



CITYWISE_EXPLORER/
├── app.py                  # Main Flask application
├── static/
│   └── js/
│       └── restaurants.js  # Dataset of 180+ restaurant entries
├── templates/
│   └── index.html          # Main UI template
├── requirements.txt        # Python dependencies
├── .env                    # Environment variables
└── venv/                   # Virtual environment

```

---

## 💻 Installation & Local Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/citywise-explorer.git
cd citywise-explorer
````

---

### 2️⃣ Create & Activate Virtual Environment

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

#### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4️⃣ Configure Feedback (Formspree)

1. Visit 👉 [https://formspree.io](https://formspree.io)
2. Create a free account
3. Create a **New Form**
4. Copy your **Form ID**

Open `templates/index.html` and update:

```js
const FORMSPREE_URL = "https://formspree.io/f/YOUR_ID_HERE";
```

Replace `YOUR_ID_HERE` with your actual Formspree ID.

---

### 5️⃣ Run the Application

```bash
python app.py
```

Open your browser and visit:

```
http://127.0.0.1:5000
```

---

## 📋 Usage Guide

1. Select a **Destination** from the dropdown
2. Choose a **Meal Type** (All / Breakfast / Lunch / Dinner)
3. Click **Explore Now** to load restaurants
4. Use **Advanced Filters** to refine results
5. Click **View on Map** to open Google Maps

---

## 📦 Requirements

Minimal required Python libraries:

```
Flask
```

---
