# VedaMoviesBot

A Telegram bot that helps you discover information about movies and actors using the TMDb API.

## Features

* **Search by Movie Name:** Enter the name of a movie to get details like:
    * Title
    * Poster image
    * Overview/Synopsis
    * Release date
    * User rating
    * Top 5 cast members
    * Link to the official YouTube trailer (if available)

* **Search by Actor Name:** Enter the name of an actor to get details like:
    * Full name
    * Profile image
    * A list of their popular movies
    * Biography

## Setup Instructions

1.  **Get a Telegram Bot Token:**
    * Open Telegram and search for "BotFather".
    * Start a chat with BotFather by sending `/start`.
    * Create a new bot using the `/newbot` command. Follow the prompts to choose a name and username for your bot (e.g., Name: Veda Movies Bot, Username: VedaMoviesBot).
    * BotFather will provide you with an **API token**. Copy this token carefully.

2.  **Configure the API Key and Bot Token:**
    * Navigate to the `VedaMoviesBot` folder on your computer.
    * Open the `config.py` file using a text editor.
    * Replace the placeholder `"YOUR_BOT_TOKEN"` with the actual API token you received from BotFather. The TMDb API key is already included.

    ```python
    # VedaMoviesBot/config.py

    BOT_TOKEN = "YOUR_BOT_TOKEN"  # Replace with your BotFather token
    TMDB_API_KEY = "8baba8ab6b8bbe247645bcae7df63d0d"
    ```

    * **Important:** Keep your `BOT_TOKEN` private! Do not share it publicly.

3.  **Install Required Python Libraries:**
    * Open your terminal or command prompt.
    * Navigate to the `VedaMoviesBot` folder using the `cd` command (e.g., `cd path/to/VedaMoviesBot`).
    * Run the following command to install the necessary Python libraries:

    ```bash
    pip install -r requirements.txt
    ```

    This command will download and install the `python-telegram-bot` library for interacting with the Telegram API and the `requests` library for making HTTP requests to the TMDb API.

4.  **Run the Bot:**
    * In the same terminal or command prompt, execute the `main.py` file:

    ```bash
    python main.py
    ```

    Your bot should now be running and listening for commands on Telegram.

## Usage

1.  Open the Telegram app on your phone or desktop.
2.  Search for your bot using its username (e.g., `@VedaMoviesBot`) and start a chat.
3.  Use the `/start` command to see the initial options.
4.  Click on the "Search Movie" or "Search Actor" button.
5.  Type the name of the movie or actor you are interested in and send it to the bot.
6.  The bot will process your request and send you the relevant details.

## Folder Structure