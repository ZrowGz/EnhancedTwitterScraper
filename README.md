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

**Currently, this app only outputs files as a .csv and only scrapes twitter hashtags. Future versions will include ability to scrape by usernames.**

*If you're scraping a potentially large dataset, it is recommended to run multiple instances of this in multiple terminals, each pulling from different date ranges to enhance tweets found per second. For example, this pulls approximately 35-50 tweets per second, but 6 months of `#Bitcoin` yields over 3 million tweets. As you can see, that could take a long time to collect through only one instance!*


Open the CLI and run:
`python TweetScraperQuest.py`

You will be prompted to fill out the data you wish to scrape, as well as which attributes of a tweet you wish to collect.
- Enter the desired file path and name, with no quotes: `tweetDemo.csv`
- Currently, this does not integrate with pandas, so only select `Yes` when asked about output file type.
- Enter the hashtag you wish to search for with no `#` in front: `bitcoin`
- Selecting all tweet attributes to scrape can generate large file sizes! Otherwise, select the ones you care about.
- Enter the start date, closest to today as `2021-10-01` (not inclusive)
- Enter the end of the date range to scrape as `2021-01-01` (inclusive)
- Select tweet stats frequency, `100` to `250` is good for medium to large sized data sets
- Can include a limit to the number of tweets found. 
- Sit back and enjoy!

---

## Credit

- snscrape source code was utilized in this app. Follow the links in the Installation section for more details
- MartinBeckUT's Python Wrapped TwitterScraper is the core of how snscrape was integrated into this project.
- Idea and troubleshooting for this came up during a project with [Lisa](https://github.com/balllisaann) and [Meghan](https://github.com/megkennedy)
