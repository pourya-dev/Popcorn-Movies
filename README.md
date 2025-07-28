Movie Recommender Telegram Bot 🍿
A sophisticated Telegram Bot that provides detailed movie information and personalized recommendations, powered by a custom-built database and a content-based machine learning engine. This project was developed for the Advanced Programming (AP) course at Sharif University of Technology, International Campus.

Table of Contents
Overview

Features

Project Architecture

Setup and Installation

Usage

Project Documentation

Authors

License

Overview 📝
This project is an intelligent Telegram Bot designed for a comprehensive movie discovery experience. It integrates a vast movie database, created through a multi-stage scraping pipeline, with a machine learning engine to offer users two powerful ways to find movies:

Movie Information Retrieval: Users can search for any movie title to get detailed information.

Intelligent Recommendations:

Movie-to-Movie: Get recommendations for movies similar to a specific title.

Keyword-Based: Discover movies using keywords like genre, country of origin, or actor/director names.

Features ✨
✨ Powerful Inline Mode: Search for movies and get recommendations directly from any chat without having to talk to the bot directly.

💬 Conversational Discovery: A guided "Discover" mode that prompts you for keywords and delivers tailored results.

❤️ Favorites Management: Add, view, and delete your favorite movies, which are saved to your user account.

🚀 Deep Linking: Recommendation messages contain clickable links that take you directly to the movie's information page within the bot.

🧠 Modular & Resilient Architecture: The project is built with a clear separation of concerns, from the fault-tolerant data scrapers to the object-oriented recommendation engine.

Project Architecture 🏛️
The project is divided into three main components, each with its own set of scripts:

Data Scraping Pipeline:

wiki_extractor.py: A lightweight scraper to generate a list of movie titles from Wikipedia.

Scraper.py: A robust, stateful API scraper that enriches the title list with detailed data from the OMDb API. It features automatic API key rotation and graceful shutdown.

Machine Learning Engine:

engine.py: An object-oriented, content-based recommendation engine. It uses scikit-learn and Pandas to perform TF-IDF vectorization and calculate cosine similarity between movies based on their features (genre, director, actors, etc.).

The Telegram Bot:

bot.py: The main application that integrates all components and handles user interactions.

Explorer.py: A helper module for loading and searching the scraped movie data from memory.

user_management.py: An object-oriented module for creating and managing persistent user data (like favorites) in a CSV file.

bot_logger.py: A simple utility for logging bot activity to the console and a bot.log file.

Setup and Installation ⚙️
Follow these steps to get the project running on your local machine.

1. Prerequisites
Python 3.8 or higher

Git

2. Clone the Repository
Bash

git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
3. Set up a Virtual Environment (Recommended)
Bash

# For Windows
python -m venv venv
.\venv\Scripts\activate

# For macOS/Linux
python3 -m venv venv
source venv/bin/activate
4. Install Dependencies
Create a file named requirements.txt with the following content:

requests
beautifulsoup4
pandas
scikit-learn
selenium
webdriver-manager
python-telegram-bot
tqdm
numpy
scipy
Then, install the libraries using pip:

Bash

pip install -r requirements.txt
5. Configure the Bot
Get a Telegram Bot Token: Talk to @BotFather on Telegram to create a new bot and get your unique token.

Edit bot.py: Open the bot.py file and replace "YOUR_TELEGRAM_BOT_TOKEN_HERE" with the actual token you received.

Prepare API Keys: Create a file named api_keys.txt and add your OMDb API keys, one per line.

Prepare Data Files: Ensure you have your initial movie data file (e.g., movies.csv) in the root directory for the ML engine to use.

Usage ▶️
Build the Database (if needed):

Run the wiki_extractor.py to generate the initial movie_titles.txt.

Run the Scraper.py to process this list and generate the final Extdata.txt database.

Run the Bot:

Once your configuration is complete, start the bot by running the main script:

Bash

python bot.py
The bot will print a startup message and will begin polling for updates from Telegram.

Interact with the Bot on Telegram:

Find your bot on Telegram and send the /start command to see the main menu.

Use the inline mode (@your_bot_username movie title) in any chat to search for movies or get recommendations.

Project Documentation 📄
This repository contains a comprehensive Jupyter Notebook, Project_Documentation.ipynb, which provides a deep dive into the architecture, development history, and technical details of every script in this project.

Authors ✍️
Pourya Salimi

Computer Engineering Student, Sharif University of Technology, International Campus

Telegram: @PSALIMI80

Seyed Armin Saadatnia

Computer Engineering Student, Sharif University of Technology, International Campus

Telegram: (Contact information available upon request)

License ⚖️
This project is licensed under the MIT License - see the LICENSE.md file for details.
