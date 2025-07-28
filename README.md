# **Movie Recommender Telegram Bot**
### Final Project for Advanced Programming (AP)

**Institution:** Sharif University of Technology, International Campus

**Project Members:**
* **Pourya Salimi:** Scraping Pipeline, Telegram Bot Development, Documentation  
* **Seyed Armin Saadatnia:** Machine Learning and Recommendation Engine  

<p align="center"><em>July 2025</em></p>

---

## **Table of Contents** 📜

1. [**Introduction**](#1-introduction)
2. [**The Data Scraping Pipeline**](#2-the-data-scraping-pipeline)
3. [**Machine Learning & Recommendation Engine**](#3-machine-learning--recommendation-engine)
4. [**The Telegram Bot**](#4-the-telegram-bot)
5. [**Links and References**](#5-links-and-references)

---

## **1. Introduction**

This project details the development of an intelligent **Telegram Bot** designed to provide users with a comprehensive movie discovery and recommendation experience. The system is built on two core pillars: a vast, self-constructed movie database and a sophisticated machine learning engine that drives its recommendations.

---

## **2. The Data Scraping Pipeline**

A fully functional web scraping pipeline was developed to collect real-world movie data from reliable sources such as IMDb and TMDb. The pipeline includes:

- Crawling over 20,000 movie titles
- Extracting relevant features (genres, cast, crew, ratings, etc.)
- Cleaning and storing the data in structured formats
- Saving the dataset as a CSV file for further processing

---

## **3. Machine Learning & Recommendation Engine**

The engine is trained to provide high-quality, personalized recommendations using:

- **Content-based filtering**: Recommendations based on movie metadata similarity (e.g., genre, director, etc.)
- **Cosine similarity**: To find the most relevant movies
- Efficient model implementation with `scikit-learn` and `pandas`

---

## **4. The Telegram Bot**

The Telegram Bot acts as the front-end interface for users:

- Built using `python-telegram-bot` API
- Responsive to multiple commands:
  - `/recommend <movie_name>` – Suggests similar movies
  - `/search <keyword>` – Searches for matching titles
- Deployed and accessible via a Telegram link (insert link here if deployed)

---

## **5. Links and References**

- IMDb: https://www.imdb.com
- TMDb API: https://www.themoviedb.org
- [Scikit-learn Documentation](https://scikit-learn.org/)
- [Python Telegram Bot Library](https://github.com/python-telegram-bot/python-telegram-bot)

---

> **Note:** This project was developed for educational purposes only. The content used from third-party sources belongs to their respective owners.

