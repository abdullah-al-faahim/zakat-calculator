# 🕌 যাকাত ক্যালকুলেটর — Islamic Zakat Calculator (Bangla)

> **কুরআন ও সুন্নাহর আলোকে নির্ভুল যাকাত হিসাব — সম্পূর্ণ বাংলায়**  
> A comprehensive, Shariah-compliant Zakat Calculator in the Bengali language — built as a single, dependency-free HTML file.

---

## 🌙 Live Demo

[![Open Calculator](https://img.shields.io/badge/Open-Calculator-0d4a2f?style=for-the-badge&logo=html5&logoColor=white)](https://abdullahalfahim.bd)

---

## ✨ Features

- **📖 Quran & Hadith References** — Every rule is sourced from authentic Islamic texts (Bukhari, Muslim, Abu Dawud, Tirmidhi) with Ayah and Hadith numbers displayed in the UI
- **⚖️ Silver Nisab Standard** — Uses the 612.36g silver nisab (the most inclusive, widely accepted standard among scholars)
- **💰 6 Asset Categories** — Full coverage of all zakatable wealth:
  - নগদ অর্থ ও ব্যাংক সঞ্চয় (Cash & Bank Savings) — 2.5%
  - সোনা ও রূপা (Gold & Silver) — 2.5%
  - ব্যবসায়িক মালামাল (Business Inventory & Stock) — 2.5%
  - বিনিয়োগ ও শেয়ার (Investments & Shares) — 2.5%
  - কৃষি উৎপাদন (Agricultural Produce) — 10% rain-fed / 5% irrigated
  - গবাদি পশু (Livestock: Goat, Cattle, Camel) — Shariah-based rules
- **📡 Today's Live Prices** — Gold & silver prices (BDT/gram) sourced via Google Search and pre-loaded automatically on page open
- **✏️ Manual Override** — Users can edit any price; fields show 🟢 Live or ✏️ Manual badges
- **🧮 Detailed Breakdown** — Each asset category shows individual Zakat amount with rate
- **✅ Nisab Eligibility Check** — Instantly tells whether Zakat is obligatory or not
- **📱 Fully Responsive** — Works on mobile, tablet, and desktop
- **🚫 Zero Dependencies** — Pure HTML, CSS & JavaScript. No frameworks, no npm, no build step.

---

## 📐 Islamic Ruling References

| বিষয় | দলিল | বিধান |
|---|---|---|
| যাকাত ফরজ | সূরা তাওবাহ ৯:১০৩ | সকল মুসলিমের উপর ফরজ |
| নিসাব (রূপা) | আবু দাউদ ১৫৭৪ | ৬১২.৩৬ গ্রাম রূপার মূল্য |
| নিসাব (সোনা) | আবু দাউদ ১৫৭৪ | ৮৭.৪৮ গ্রাম সোনার মূল্য |
| নগদ / সঞ্চয় | তিরমিযী ৬২০ | ২.৫% (রুবু'উল উশর) |
| সোনা ও রূপা | সহীহ বুখারী ১৪৫৪ | ২.৫% |
| ব্যবসায়িক মাল | আবু দাউদ ১৫৬২ | ২.৫% (পাইকারি মূল্যে) |
| বৃষ্টির ফসল | সহীহ বুখারী ১৪৮৩ | ১০% (উশর) |
| সেচের ফসল | সহীহ বুখারী ১৪৮৩ | ৫% (নিসফ উশর) |
| ছাগল / ভেড়া | সহীহ বুখারী ১৪৫৪ | ৪০টিতে ১টি ছাগল |
| গরু / মহিষ | সহীহ বুখারী ১৪৫৪ | ৩০টিতে ১টি বকর |
| উট | সহীহ বুখারী ১৪৫৪ | ৫টিতে ১টি ছাগল |

---

## 🚀 Getting Started

No installation or build process required.

### Option 1 — Open Directly in Browser

```bash
# Clone the repo
git clone https://github.com/your-username/zakat-calculator.git

# Open in your browser
open zakat-calculator.html
```

### Option 2 — GitHub Pages (Recommended)

1. Fork or clone this repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Your calculator will be live at `https://your-username.github.io/zakat-calculator/`

### Option 3 — Any Static Host

Upload `zakat-calculator.html` to any static hosting service:
- **Netlify** — drag & drop the file
- **Vercel** — `vercel deploy`
- **Cloudflare Pages** — connect your repo

---

## 🗂️ Project Structure

```
zakat-calculator/
│
├── zakat-calculator.html   # The entire app — HTML + CSS + JS in one file
└── README.md               # This file
```

---

## 💡 How to Update Gold & Silver Prices

Prices are pre-loaded from Google Search. To update them for a new date:

1. Open `zakat-calculator.html` in any text editor
2. Find the `LIVE_PRICES` object near the bottom of the `<script>` tag:

```javascript
const LIVE_PRICES = {
  gold_per_gram:   20922.61,   // Update this → BDT per gram (24K)
  silver_per_gram:   366.64,   // Update this → BDT per gram
  date:          '৪ মার্চ ২০২৬',
  source:        'goldpricez.com'
};
```

3. Replace the values with today's prices (search **"Bangladesh gold price per gram BDT today"** on Google)
4. Save the file — done!

> 💡 **Tip:** 1 ভরি (Vori) = 11.664 grams. If you find prices per vori, divide by 11.664 to get per-gram price.

---

## 🎨 Design Highlights

- **Font:** Noto Serif Bengali — consistent across all UI elements
- **Color Palette:** Deep emerald green (`#0d4a2f`) + Islamic gold (`#c9a84c`) + warm cream (`#fdf8ee`)
- **Motifs:** Geometric Islamic star/hexagon patterns in backgrounds
- **Arabic Calligraphy:** Amiri font for Quranic Ayahs in the header and banners
- **Animations:** Staggered card fade-up on page load; smooth scroll to results

---

## 🤲 Zakat Recipients (সূরা তাওবাহ ৯:৬০)

Zakat must be distributed to the **8 categories** specified in the Quran:

1. **ফকির** — The very poor
2. **মিসকীন** — The needy
3. **আমিল** — Zakat collectors/administrators
4. **মুয়াল্লাফাতুল কুলুব** — New Muslims
5. **রিকাব** — Freeing of slaves/captives
6. **গারিমীন** — Those burdened by debt
7. **ফি সাবিলিল্লাহ** — In the cause of Allah
8. **ইবনুস সাবিল** — Stranded travellers

---

## ⚠️ Disclaimer

This calculator is provided for **educational and general guidance purposes only**. For complex financial situations, multiple asset types, or scholarly disputes, please consult a qualified Islamic scholar or Mufti. Gold and silver prices fluctuate daily — always verify with current market rates before calculating your Zakat.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙏 Contributing

Contributions are welcome! If you find a fiqh error, pricing issue, or UI bug:

1. Fork the repository
2. Create a branch: `git checkout -b fix/your-fix-name`
3. Commit your changes: `git commit -m 'Fix: description'`
4. Push and open a Pull Request

---

<div align="center">

Made with 🩵 by **[Abdullah Al Fahim](https://abdullahalfahim.bd)**

</div>
