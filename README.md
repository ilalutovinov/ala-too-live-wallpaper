# 🇰🇬 Ala-Too Live Stream Wallpaper 🇰🇬

A lightweight, optimized live wallpaper for **Wallpaper Engine** featuring a real-time stream of Ala-Too Square in Bishkek, Kyrgyzstan.

[![](https://img.shields.io/badge/View-Live_Demo-brightgreen?style=for-the-badge&logo=youtube)](https://ilalutovinov.github.io/ala-too-live-wallpaper/)

---

## 🛠 How It Was Made
To create this wallpaper, I captured the direct video stream from the official city camera at [kg.camera](https://kg.camera/ru/camera/Bishkek_Ala-Too_Square).
* **Finding the Stream:** Using browser developer tools (**F12 -> Network tab**), I analyzed the page traffic to locate the direct HLS video stream URL.
* **CSS Cropping:** The original camera page is cluttered with UI elements, watermarks, and branding. To achieve a clean, professional look for your desktop, I implemented a CSS-based cropping method. By using a container with `overflow: hidden` and precise positioning, I effectively masked all unnecessary interface elements, leaving only the live view.

## 🚀 How to Set Up in Wallpaper Engine

1. Copy your GitHub Pages site URL (e.g., `https://ilalutovinov.github.io/ala-too-live-wallpaper/`).
2. Open **Wallpaper Engine**.
3. Click the **"Open URL"** button.
4. Paste the link into the URL field.
5. **IMPORTANT:** Ensure the **"Use Streaming Mode"** checkbox is selected.
6. Click **"OK"** and enjoy your live view!

## ⚙️ Customize for Your Own City
You can easily clone this repository to display a live feed from any location:

1. **Fork/Clone** this repository to your local machine.
2. Open `index.html` in any code editor.
3. **Replace the video stream URL** with the direct link to your chosen camera.
4. Adjust the CSS properties (like `clip-path` or margins) if your new stream has a different aspect ratio or requires different cropping.
5. Push your changes back to GitHub, and your personalized live wallpaper will be live.

## 🧠 How the Code Works
* **Video Rendering:** The page utilizes a standard HTML5 player to stream the video content directly.
* **Auto-Recovery System:** To prevent common issues such as buffer buildup, memory leaks, or the stream freezing after the PC wakes from sleep mode, I implemented a JavaScript function that **automatically refreshes the page every 10 minutes**. This ensures the feed stays fluid and stable.
* **Optimization:** The code is stripped of heavy frameworks and unnecessary scripts. This keeps CPU and GPU usage at a minimum, ensuring the wallpaper remains smooth and never interferes with your gaming or work performance.

---

*Bring a piece of your favorite location to your desktop!*
