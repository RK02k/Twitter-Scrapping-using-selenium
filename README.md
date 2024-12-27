# Twitter Trending Topics Scraper

This repository contains a Python-based web scraping application that uses Selenium to read Twitter’s homepage and extract the top 5 trending topics from the "What’s Happening" section.

## Technologies Involved:
1. **Selenium**: A widely-used tool for automating web browser actions. It is employed in this project for scraping, enabling interaction with the Twitter website to retrieve trending topics.
2. **MongoDB**: A NoSQL database used for storing the scraped trending topics, providing data persistence.
3. **HTML & Jinja**: HTML is used for structuring web pages, while Jinja, a templating engine for Python, is used alongside Flask to generate dynamic HTML content.
4. **Python-Dotenv**: A Python library that loads environment variables from a `.env` file, helping to securely manage sensitive credentials.
5. **Flask**: A lightweight web framework written in Python, utilized to build the web application and define routes for handling HTTP requests.

## Key Features:
1. **Automated Web Scraping**: Using Selenium and BeautifulSoup, the application scrapes Twitter’s homepage to gather the top trending topics in real-time.
2. **MongoDB Integration**: The application stores the extracted trending topics in a MongoDB database for future reference.
3. **Flask Web Interface**: A user-friendly interface that allows users to trigger the scraping process and view the collected data.

## Files Included:
1. **web.py**: A Flask-based Python script that manages routes to trigger the scraping process and display the scraped data.
2. **twitter_scraping.py**: A Python script that utilizes Selenium to scrape Twitter and store the trending topics in a MongoDB database.
3. **requirements.txt**: A file that lists the necessary Python dependencies for the project.
4. **index.html**: An HTML template file used to render the user interface.
5. **.env**: A configuration file that holds environment variables, including credentials for third-party services.

## Installation Instructions

To get started, clone the repository to your local machine:

```bash
git clone https://github.com/RK02k/Twitter-Scrapping-using-selenium.git


### Installation
Clone the repository to your local machine:

```bash
git clone https://github.com/RK02k/Twitter-Scrapping-using-selenium.git
```
Navigate to the project directory:

```bash
cd twitter-scraping-app
```
Install the required dependencies using pip:

```bash
pip install -r requirements.txt
```
Set up your environment variables by creating a .env file in the project directory and adding the necessary credentials:

```makefile
proxymesh_user=your_proxymesh_username
proxymesh_pass=your_proxymesh_password
X_EMAIL=your_twitter_email
X_PASS=your_twitter_password
X_USER=your_twitter_username
MONGODB_URI=your_mongodb_uri
```
Usage
Run the Flask application:

```bash
python Web.py
```
Open your web browser and go to http://localhost:5000 to access the web interface.

Click the "Scrape Data" button to trigger the scraping process.

Once the scraping is complete, the trending topics will be displayed on the webpage.
