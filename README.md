# Political Emails Analysis

### Description

The purpose of this project is to:
- 1.) Explore similarities in the text of the political emails broken out by country, party, time, and other categories.
- 2.) Discover patterns in the text of these emails and determine the relative importance of certain words.
- 3.) Determine if any latent groupings of emails exist.
- 4.) Build ML models to predict sentiment of emails


### Data

The data used for this analysis included:
- [Archive of Political Emails](https://politicalemails.org/)



### Challenges
- To conduct a sufficient analysis of the email database, I wanted to collect as many emails as possible, if not all of them.  The entire database contained over 800K emails, which would be more than enough.  However, the amount of space and time it would take to scrape all of these emails grew too quickly as I crossed over 100K.  Thus, I decided to only scrape the first 100K emails - some of which turned up empty links resulting in ~83K emails in total.
- I was unaware of Github's max size file upload limit of 100MB when I tried to upload the entire dataframe of ~83K emails which totaled ~300MB.  Splitting up the data into 4 smaller chunks was not an issue, but I needed to clean my Git history of the failed upload before pushing anything else to my repository.  This process took some time Googling/Stackoverflowing, but I eventually found a solution which entailed using the "git filter-branch ..." command.

