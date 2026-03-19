# 🌙 Eid Salami Wheel of Fortune

> **A fun, interactive spin-the-wheel web app for gifting Eid Salami — built with pure HTML, CSS & JavaScript. Free for everyone under the MIT License.**

---

## ✨ Live Demo

> Deploy via GitHub Pages and paste your link here.  
> `https://<your-username>.github.io/eid-salami-wheel/`

---

## 📖 About the Project

Eid Salami is a beloved Bengali tradition where elders gift money to younger family members during Eid celebrations. This project brings that tradition into the digital world with a twist of fun!

**Eid Salami Wheel** is a single-page web app where each visitor spins a beautifully designed prize wheel and wins a randomized Eid Salami amount. The wheel is weighted — smaller amounts appear more frequently, while larger amounts are rarer, just like real life! Each device is limited to one spin, keeping things fair and exciting.

This project was built as a lighthearted gift for friends and family to enjoy during **Eid ul Fitr**. It is completely free, open-source, and requires no backend, no database, and no installation.

---

## 🎯 Features

- 🎡 **Animated Spin Wheel** — Smooth canvas-based spinning with easing animation
- 🎰 **Weighted Prize Distribution** — Higher amounts are rarer; lower amounts appear more often
- 🔒 **One Spin Per Device** — Uses `localStorage` to prevent multiple spins on the same device
- 🎊 **Confetti Celebration** — Burst of confetti on every win
- 🔊 **Sound Effects** — Tick sounds while spinning, winning fanfare on result
- 🌙 **Eid-Themed UI** — Deep green & gold Islamic aesthetic with twinkling stars
- 📱 **Fully Responsive** — Works beautifully on mobile, tablet, and desktop
- ⚡ **Zero Dependencies** — Pure HTML, CSS, and Vanilla JavaScript — no frameworks, no npm

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| HTML5 Canvas | Wheel drawing and animation |
| Vanilla JavaScript | Spin logic, audio, confetti |
| CSS3 | Animations, responsive layout, theming |
| Web Audio API | Tick sounds and win fanfare |
| localStorage | One-spin-per-device enforcement |
| Google Fonts | Cinzel Decorative & Amiri typefaces |

---

## 🚀 Getting Started

### Option 1 — Just open the file

No build tools or servers needed. Simply download and open:

```bash
git clone https://github.com/<your-username>/eid-salami-wheel.git
cd eid-salami-wheel
# Open index.html in any modern browser
```

### Option 2 — GitHub Pages (Recommended)

1. Fork or clone this repository
2. Go to your repository **Settings → Pages**
3. Under **Source**, select `main` branch and `/ (root)` folder
4. Click **Save** — your site will be live at `https://<your-username>.github.io/eid-salami-wheel/`

### Option 3 — Any Static Host

Upload `index.html` to any static hosting service:
- [Netlify](https://netlify.com)
- [Vercel](https://vercel.com)
- [Cloudflare Pages](https://pages.cloudflare.com)

---

## 📂 Project Structure

```
eid-salami-wheel/
│
├── index.html        # The entire app — all HTML, CSS, and JS in one file
├── README.md         # This file
└── LICENSE           # MIT License
```

The whole project lives in a **single HTML file** — no build steps, no dependencies, no configuration.

---

## 🎨 Customization

Want to personalize it? Everything is in `index.html` and easy to modify.

### Change Prize Amounts

Find the `BASE_AMOUNTS` array in the `<script>` section:

```javascript
const BASE_AMOUNTS = [
  { amount: 11,   label: '৳11',   emoji: '🌙', msg: 'Lucky 11! Mashallah, a charming Salami!' },
  { amount: 50,   label: '৳50',   emoji: '⭐',  msg: 'Fifty taka! A generous blessing!' },
  // Add or edit entries here
];
```

Each entry has:
- `amount` — numeric value (used to calculate rarity weight)
- `label` — text displayed on the wheel
- `emoji` — shown on the result card
- `msg` — congratulatory message shown after winning

> **Weight Logic:** The wheel automatically makes higher amounts rarer. A prize worth `৳55` will appear far less frequently than one worth `৳5`. No manual weight configuration needed.

### Change the Currency Symbol

Replace `৳` (Bangladeshi Taka sign) with your preferred symbol:

```javascript
label: '$10'   // US Dollar
label: '£10'   // British Pound
label: '€10'   // Euro
label: '₹10'   // Indian Rupee
```

### Reset the Spin Lock (for testing)

Open your browser's developer console and run:

```javascript
localStorage.removeItem('eidSalamiPlayed_v2');
```

This resets the one-spin lock for your device.

---

## 📸 Screenshots

| Wheel | Result Card |
|---|---|
| *(Add a screenshot of the wheel here)* | *(Add a screenshot of the result overlay here)* |

> To add screenshots: take a screenshot, upload to your repo under `/screenshots/`, and update the links above.

---

## 🙌 Contributing

Contributions are warmly welcome! Whether it's a bug fix, a new feature, or a UI improvement — feel free to open a pull request.

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

Please keep the spirit of the project in mind — it should remain fun, lightweight, and dependency-free.

---

## 📬 Contact

Created with ❤️ by **Asif Aman Jihad**

📧 Email: [asifaman.jihad10@gmail.com](mailto:asifaman.jihad10@gmail.com)  
🐙 GitHub: [@your-username](https://github.com/your-username)

Feel free to reach out for questions, suggestions, or just to say Eid Mubarak! 🌙

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for full details.

```
MIT License

Copyright (c) 2025 Asif Aman Jihad

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

<div align="center">

**ঈদ মোবারক — Eid Mubarak 🌙**

*May this little wheel bring smiles, laughter, and blessings to everyone who spins it.*

⭐ If you enjoyed this project, please consider giving it a star on GitHub!

</div>
