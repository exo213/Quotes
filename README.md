# 🌿 Zen Quote

A minimalist, relaxing single-page website that displays a new quote every 3 hours. Designed with a premium "Cloud Dancer" aesthetic, glassmorphism UI, and kinetic typography.

## ✨ Features

- **Zen Aesthetic**: Soft, multi-tonal background gradient ("Cloud Dancer").
- **Glassmorphism**: A frosted-glass quote card using `backdrop-filter`.
- **Premium Typography**: Uses the variable serif font **Playfair Display**.
- **Kinetic Typography**: Smooth 2-second fade-in animations for quotes and authors.
- **Smart Caching**: Uses `localStorage` to ensure a new quote is only fetched every 3 hours, respecting API limits and providing instant load times.
- **Responsive**: Fully responsive and mobile-friendly design.

## 🛠️ Built With

- **HTML5 & CSS3**: Vanilla implementation for maximum performance.
- **JavaScript (ES6)**: Pure client-side logic with `localStorage` caching.
- **ZenQuotes API**: Source for inspiring quotes.
- **AllOrigins Proxy**: Ensures smooth API fetching without CORS issues.

## 🕒 The 3-Hour Rule

This project implements a strict caching logic:
1. On page load, it checks if a quote is stored in `localStorage`.
2. It compares the current timestamp with the saved timestamp.
3. If less than 10,800 seconds (3 hours) have passed, it displays the cached quote.
4. If more than 3 hours have passed, it fetches a fresh quote and resets the timer.

## 🚀 Deployment

This project is optimized for deployment on **Vercel** or **GitHub Pages**. Simply upload the files to a repository and connect it to your favorite hosting platform.

## 📜 Attribution

Quotes are provided by [ZenQuotes API](https://zenquotes.io/).

---

*“True peace comes from within.”*
