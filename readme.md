# LinkedIn Profile Scraper

This project utilizes the ScrapeTables.com API to extract information from LinkedIn profiles using their URLs. It's designed to process a large number of LinkedIn profile URLs efficiently and safely.

## Project Overview

The LinkedIn Profile Scraper does the following:

1. Reads LinkedIn profile URLs from a CSV file
2. Uses the ScrapeTables.com API to fetch data for each profile
3. Processes URLs in batches of 50
4. Implements a 2-minute pause between batches to avoid overloading the API
5. Saves the scraped data to a CSV file

## Setup

1. Clone this repository to your local machine.
2. Install the required dependencies (list them if there are any specific requirements).
3. Create a `config.yaml` file in the root directory with your ScrapeTables.com API key:

   ```yaml
   api_key: 'your_api_key_here'
   ```

4. Create a `data` folder in the root directory.
5. Place your input CSV file containing LinkedIn URLs in the `data` folder.

## Input Data Format

The input CSV file should have a column named "LinkedIn URL" containing the profile URLs you want to scrape. For example: