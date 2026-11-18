# ⚖️ Weight & Price Two-Way Calculator

A fast, modern, and lightweight two-way retail weight and price calculator built with pure HTML, CSS, and Vanilla JavaScript.

Designed for shoppers, merchants, grocery stores, and everyday market calculations. Easily switch between calculating the **price for a given weight** or finding the **exact weight you get for a given budget**.

---

## 🚀 Live Demo

> **GitHub Pages:** `https://<your-username>.github.io/<repository-name>/`  
*(Follow the [Deployment Guide](#-deploy-to-github-pages) below to get your live link in 2 minutes)*

---

## ✨ Key Features

- **🔄 Two-Way Calculation Modes:**
  - **Weight → Price Mode:** Enter product rate per kg (e.g., ₹150/kg) and weight (e.g., 250 gm) → get total price (**₹37.50**).
  - **Price → Weight Mode:** Enter product rate per kg (e.g., ₹150/kg) and your budget (e.g., ₹50) → get exact weight (**333.33 gm** / **0.333 kg**).
- **⇄ Seamless Mode Switching:** Switch modes with one click or using the `⇄` swap button; your active inputs convert automatically.
- **⚡ Quick-Select Presets:**
  - **Weight Chips:** `25g`, `50g`, `100g`, `200g`, `250g`, `400g`, `500g (½ kg)`, `750g`, `1000g (1 kg)`.
  - **Price Chips:** `₹10`, `₹20`, `₹30`, `₹50`, `₹75`, `₹100`, `₹150`, `₹200`, `₹500`.
- **📊 Dynamic Reference Chart:**
  - In Weight Mode: Real-time price breakdown for different quantities.
  - In Price Mode: Real-time weight breakdown for different budget tiers.
  - Add custom quantities or budgets to the chart with one click.
  - Click any row in the chart to load that value into the main calculator.
- **📋 One-Click Copy:** Copy calculated price or weight directly to your clipboard.
- **🎯 Precision Control:** Easily switch between 0, 1, 2, or 3 decimal places.
- **📱 100% Responsive Design:** Smooth, modern UI with clean card layout, optimized for mobile phones, tablets, and desktop browsers.
- **⚡ Zero Dependencies:** Single standalone file. No frameworks, no build tools, no npm packages required. Runs anywhere offline.

---

## 📐 Calculation Logic & Formulas

### 1. Weight to Price (Find Price)
$$\text{Price (₹)} = \left(\frac{\text{Price per kg}}{1000}\right) \times \text{Weight in Grams}$$

* **Example:** Product is ₹150/kg, you want 250 grams:
  $$\text{Price} = \left(\frac{150}{1000}\right) \times 250 = 0.15 \times 250 = ₹37.50$$

---

### 2. Price to Weight (Find Quantity for Budget)
$$\text{Weight in Grams} = \left(\frac{\text{Budget (₹)}}{\text{Price per kg}}\right) \times 1000$$
$$\text{Weight in Kilograms} = \frac{\text{Budget (₹)}}{\text{Price per kg}}$$

* **Example:** Product is ₹150/kg, you have ₹50 budget:
  $$\text{Weight (gm)} = \left(\frac{50}{150}\right) \times 1000 = 333.33\text{ gm}$$
  $$\text{Weight (kg)} = \frac{50}{150} = 0.333\text{ kg}$$

---

## 📁 Project Structure

```text
├── index.html       # Main application file (ready for GitHub Pages)
├── price-calc.html  # Standalone copy of the calculator
└── README.md        # Project documentation
```

---

## 💻 Quick Start / Local Setup

No installation or build steps required!

1. Clone or download this repository:
   ```bash
   git clone https://github.com/<your-username>/<repository-name>.git
   ```
2. Open `index.html` (or `price-calc.html`) directly in any web browser (Chrome, Edge, Firefox, Safari).
3. Alternatively, serve with any local HTTP server:
   ```bash
   # Python 3
   python -m http.server 8000

   # Node.js (npx)
   npx serve .
   ```

---

## 🌐 Deploy to GitHub Pages (Step-by-Step)

Deploy this calculator for free on GitHub Pages in under 2 minutes:

### Option A: Using the GitHub Web Interface (Easiest)

1. Go to [GitHub](https://github.com) and click **New Repository**.
2. Name your repository (e.g. `price-calculator` or `weight-to-price-calc`).
3. Set the repository to **Public** and click **Create repository**.
4. In the repository page, click **"uploading an existing file"**.
5. Drag and drop `index.html` and `README.md` into GitHub, then click **Commit changes**.
6. Go to **Settings** (tab at the top of your repository).
7. In the left sidebar, click **Pages** (under "Code and automation").
8. Under **Build and deployment > Branch**:
   - Select `main` (or `master`) branch.
   - Leave the folder as `/ (root)`.
   - Click **Save**.
9. Wait 1–2 minutes, then refresh the page. Your live site URL will be displayed at the top:
   ```
   https://<your-username>.github.io/<repository-name>/
   ```

---

### Option B: Using Git CLI

```bash
# 1. Initialize git repository
git init

# 2. Add files
git add index.html README.md

# 3. Commit files
git commit -m "Initial commit: Weight & Price Two-Way Calculator"

# 4. Rename branch to main
git branch -M main

# 5. Add remote origin (replace with your repo URL)
git remote add origin https://github.com/<your-username>/<repository-name>.git

# 6. Push to GitHub
git push -u origin main
```
Then enable GitHub Pages under **Settings > Pages > Branch: main > Save**.

---

## 🛠️ Built With

- **HTML5** – Semantic markup and accessible form controls.
- **CSS3** – Modern flexbox/grid layout, CSS custom properties (variables), smooth transitions, and linear gradients.
- **Vanilla JavaScript (ES6+)** – Reactive two-way calculations, clipboard API integration, and dynamic DOM rendering.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE). Feel free to use, modify, and distribute it for personal or commercial projects.

