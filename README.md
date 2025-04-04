# MLK "I Have a Dream" Speech Analysis

This project analyzes the word frequency in Martin Luther King Jr.'s "I Have a Dream" speech. It uses Python and several libraries to fetch the speech from a website, clean the text, and count the occurrences of each word. The results are then saved to a CSV file.

## How it Works

1. **Fetching the Speech:**
   - The code uses the `requests` library to fetch the HTML content of the webpage containing the speech.
   - The `BeautifulSoup` library is used to parse the HTML and extract the relevant text.

2. **Cleaning the Text:**
   - Newline characters and punctuation are removed from the text.
   - The text is converted to lowercase for case-insensitive analysis.
   - The text is split into individual words.

3. **Analyzing Word Frequency:**
   - A pandas DataFrame is created from the list of words.
   - The `value_counts()` method is used to count the occurrences of each word.

4. **Saving the Results:**
   - The word counts are saved to a CSV file in Google Drive.

## Libraries Used

- `requests`: For fetching web pages.
- `BeautifulSoup`: For parsing HTML content.
- `re`: For regular expressions (used for text cleaning).
- `pandas`: For data manipulation and analysis.
- `google.colab.drive`: To mount Google Drive (if running in Google Colab).

## Usage

1. Make sure you have the necessary libraries installed. You can install them using `pip`:

# Automated Web Scraper, Bitcoin Price (Hourly Cadence)

This Python script automates the process of scraping the current price of Bitcoin from CoinMarketCap and saving it to a CSV file on Google Drive. It uses the requests library to fetch the website's HTML, BeautifulSoup to parse the HTML and extract the price, and pandas to create a DataFrame for storing the data. The script is designed to run continuously in a Google Colab environment, updating the CSV file every hour. This provides a convenient way to track the price of Bitcoin over time for analysis or personal use.

## Automated Data Collection (Commented Out for Cleanliness)

This project was initially designed to automatically collect and update Bitcoin price data every hour. However, to prevent unintended execution and ensure a clean GitHub repository, the automation loop has been commented out.

**Intended Automation Functionality:**

The intended automation was designed to perform the following steps at hourly intervals:

1. **Data Retrieval:** The script fetches the current Bitcoin price from a reliable source using the `requests` and `BeautifulSoup` libraries.
2. **Data Processing:** The retrieved data is parsed and extracted to obtain the relevant Bitcoin price information.
3. **Data Storage:** The extracted data, along with a timestamp, is then appended to a CSV file named `bit_coin_scraped.csv` stored in the user's Google Drive.

**Libraries Used for Automation:**

The following libraries were utilized for implementing the automation:

- `time`: For introducing delays and controlling the frequency of data collection.
- `schedule`: For scheduling the automation to run at specific intervals (e.g., hourly).
- `requests`: For making HTTP requests to fetch the Bitcoin price data.
- `BeautifulSoup`: For parsing the HTML content and extracting the relevant information.
- `pandas`: For creating and manipulating dataframes to store the collected data.
- `google.colab`: For interacting with Google Colab environment and mounting Google Drive.

**How to Reactivate Automation (for Testing):**

To reactivate the automation for testing purposes, follow these steps:

1. Locate the commented-out automation loop within the script (typically denoted by `# while True:`).
2. Uncomment the loop by removing the `#` symbols at the beginning of each line within the loop.
3. Execute the script. The automation loop will then run indefinitely, collecting and updating Bitcoin price data at the specified interval.

**Note:** It is recommended to thoroughly test and monitor the automation in a controlled environment before deploying it in a production setting.

# Web Scraper, World Population

Web scraping using Python and the BeautifulSoup library. It extracts data from the Worldometer website on world population by country, cleans the data, and saves it to a CSV file. 

**Description**
This project utilizes Python libraries like requests, BeautifulSoup, and pandas to scrape population data from the Worldometer website. It extracts information such as country name, population, yearly change, etc., organizes it into a pandas DataFrame, and then saves it as a CSV file. This data can be used for further analysis or visualization.

# Google Drive File Sorter

This Python script helps organize files in Google Drive into specific folders based on file types. It supports sorting of CSV files, text files, and image files into their respective directories. This project is particularly useful for data analysts who frequently handle various types of data files and need an automated way to keep their Google Drive organized.

**Contents:**

FileSorter.py: The main Python script that mounts Google Drive, checks for specified file types, and moves them into designated folders.

Installation: Clone this repository and run the script in a Google Colab notebook, as it uses Colab's specific library to mount Google Drive

**Dependencies:**

Google Colab
Python libraries: os, shutil

**Usage:**

Open the script in Google Colab.

Run the script. It will prompt you to authenticate your Google Drive.

Once authenticated, the script will organize the files in the specified "FileSorter" directory on your Google Drive.

## Acknowledgements

This project was completed as part of the Data Analysis with Python course on Analyst Builder. I would like to thank Alex The Analyst and the Analyst Builder team for providing the resources and guidance for this project. You can learn more about Analyst Builder at [https://analystbuilder.com/](https://analystbuilder.com/).

Google Colab team for providing the platform to easily interact with Google Drive using Python


