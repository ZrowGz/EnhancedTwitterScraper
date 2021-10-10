# EnhancedTwitterScraper
Repacking of a wrapped interface of snscrape.

---

## Requirements

Install the developer edition of snscrape.
- "wrapped version" (recommended): [TwitterScraper](https://github.com/MartinBeckUT/TwitterScraper.git)

Python
- python 3.8
- questionary
- csv
- pathlib

---

## Use

Generating multiple instances of this running in parallel allows significant numbers of Tweets to be scraped.

Output file currently only works as a .csv file.

Displays fun statistics about the rate of tweets discovered along the way


Open the CLI and run:
`python TweetScraperQuest.py`

You will be prompted to fill out the data you wish to scrape, as well as which attributes of a tweet you wish to collect.

---

## Credit

- snscrape source code was utilized in this app. Follow the links in the Installation section for more details
- MartinBeckUT's Python Wrapped TwitterScraper is the core of how snscrape was integrated into this project.
