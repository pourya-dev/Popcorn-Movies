# 🎬 **Movie Recommender Telegram Bot** 🤖🍿
### Final Project for Advanced Programming (AP)

**Institution:** Sharif University of Technology, International Campus

**Project Members:**
- 👨‍💻 **Pourya Salimi** — Scraping Pipeline, Telegram Bot Development, Documentation  
- 🤖 **Seyed Armin Saadatnia** — Machine Learning and Recommendation Engine  

<p align="center"><em>📅 July 2025</em></p>

---

## 🏷️ Badges

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Platform](https://img.shields.io/badge/Platform-Telegram-lightgrey?logo=telegram)
![ML](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange?logo=scikit-learn)

---

## 📜 Table of Contents

1. [🎯 Introduction](#1-introduction)
2. [🔍 The Data Scraping Pipeline](#2-the-data-scraping-pipeline)
3. [🧠 Machine Learning & Recommendation Engine](#3-machine-learning--recommendation-engine)
4. [💬 The Telegram Bot](#4-the-telegram-bot)
5. [📸 Screenshots](#5-screenshots)
6. [🔗 Links and References](#6-links-and-references)
7. [⚖️ License](#7-license)
---

## 1. 🎯 Introduction

This project presents an intelligent **Telegram Bot** for movie discovery and recommendation. It is powered by:

- 🧰 A custom-built movie dataset (from IMDb & TMDb)
- 🧠 A machine learning engine for smart recommendations

---

## 2. 🔍 The Data Scraping Pipeline

Our pipeline collects and preprocesses movie data:

- 🌐 Scraped over **20,000** movies
- 🎭 Collected features like **title**, **genre**, **director**, **cast**, and **ratings**
- 🧼 Cleaned and structured into a CSV format
- 📁 Used in both training and live recommendations

---

## 3. 🧠 Machine Learning & Recommendation Engine

Using content-based filtering:

- ✅ Feature vectorization with **TF-IDF**
- 📏 **Cosine similarity** for recommendations
- 🧪 Built with `scikit-learn`, `pandas`, and `numpy`

---

## 4. 💬 The Telegram Bot

Built with the `python-telegram-bot` API, this bot:

- 💡 Recommends movies based on user input
- 🔎 Supports search queries
- 🧵 Conversational and interactive

### 🤖 Commands

/recommend <movie_name> → Suggest similar movies
/search <keyword> → Find movies by keyword
/help → Show command list


---

## 5. 📸 Screenshots

| User Input | Bot Response |
|------------|--------------|
| ![screenshot1](https://via.placeholder.com/300x200?text=/recommend+Inception) | ![screenshot2](https://via.placeholder.com/300x200?text=Bot+Recommends+Shutter+Island+...) |
| ![screenshot3](https://via.placeholder.com/300x200?text=/search+Batman) | ![screenshot4](https://via.placeholder.com/300x200?text=Batman+Begins+%7C+The+Dark+Knight) |


---

## 6. 🔗 Links and References

- 🌐 [IMDb](https://www.imdb.com)
- 🎞️ [TMDb API](https://www.themoviedb.org)
- 🛠️ [Scikit-learn](https://scikit-learn.org/)
- 💬 [python-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot)

---

## ⚖️ License

This project is licensed under the **MIT License**.  
Feel free to fork, modify, and share! ⭐

---

> 🧠 *Built with love, data, and caffeine.*

👉 Try the bot here: [@popcorn_moviezbot](https://t.me/popcorn_moviezbot)
