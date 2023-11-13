# IMDb Web Scraper

This Python script scrapes the top 250 movies from IMDb and updates a MySQL database with the movie titles and ratings.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/GROSANIA/imdb-webscraps.git
    cd imdb-web-scraper
    ```

2. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

3. Set up your MySQL database:

    - Create a database named `imdb_scrapping`.
    - Update the database connection details in `app.py` (host, user, password).


## Usage

1. Run the Flask web scraper:

    ```bash
    python app.py
    ```

    This will start the Flask app, and you can access the scraped top movies at `http://127.0.0.1:5000/top_movies`.

2. Observe the terminal for any errors or messages.

3. The MySQL database will be populated with the top 250 movies. If a movie already exists in the database, it will be updated.

## Notes

- Ensure that your MySQL server is running before running the scraper.
- Make sure to have the correct version of ChromeDriver for your Chrome browser.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
