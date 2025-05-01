# 🎨 Advanced Color Picker Chrome Extension

A sleek and powerful Chrome Extension that lets you pick colors, view their complementary shades, and save your favorite palettes — built entirely with HTML, CSS, and JavaScript.

---

## ✨ Features

- 🎨 **Color Picker Input** – Select any HEX color
- 🌈 **Live Background Update** – Changes the background in real-time
- 🔁 **Complementary Color Generator** – Instantly shows the contrast/opposite color
- 📋 **Copy HEX Code** – Copy the selected color code with one click *(planned)*
- 💾 **Save Favorite Colors** – Store and view your favorite color combinations *(planned)*

---

``

``

## 🚀 How to Use

1. Clone or Download the repo
2. Go to `chrome://extensions`
3. Enable **Developer Mode**
4. Click on **Load Unpacked**
5. Select the project folder
6. Click the extension icon and start picking colors!

---

## 🧠 How Complementary Color Works

This app calculates the complementary color by inverting the HEX value using XOR logic:

```js
const base = parseInt(hexColor.slice(1), 16);
const complement = (0xFFFFFF ^ base).toString(16).padStart(6, '0');
