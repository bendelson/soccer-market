# Title
Soccer inflation

# Short description
Project during Lede Bootcamp 2025 to show the discrepancy between overall inflation and price development of male soccer's transfer market

# Goal of data collection
The goal of this project is to scrape the website Transfermarkt.de to analyze the development of the male soccer's transfer market and then put the data in comparison with the overall inflation. 
To keep it concisely and manageable, I only tried to find the average player's value for each season. Otherwise, it would have been 12 to 20 different club's datasets for each league for each season.

# Findings
The findings of this project are, that for the last twenty years, there has been an immense increase in the price level of male soccer players for every league I analyzed: English Premier League and Championship One, German Bundesliga and 2nd Bundesliga, French Ligue 1, Spanisch La Liga, Italian Serie A, American MLS and Saudi-Arabien SPL. After being more or less in line with overall inflation for the first years of the analysis, the transfer market values dettached from the normal economy in all of these leagues.

# Summary of the data collection process
Since the data on Transfermarkt.de is shown in a table, I first tried pandas to get the average-element in the html-table. But I just recieved 403-errors. Then I tried to get the element with Playwright, but was still denied. Only after simulating an actual computer with specific information on the browser used etc, I was able to scrape some of the pages I was iterating through.
But all of that took alot of time, even though I "only" tried to scrape 180 websites. The breakthrough was, when I found out, I could use a while loop to save the found elements and retry the websites, where I couldn't find the element on the previous try. That's how I finally got all the numbers for each league.

# New skills + approaches
I definitely understand Playwright better, now. Unterstanding to use a while-loop within a scraper was and is a real gamechanger for me, when it comes to websites, that are not scraper-friendly. 
Also, building this webpage from scratch really helped me to get more into html-css-writing. 
For the visual part, I tried out Flourish for the first time, because I wanted to show moving line charts with symbols in them. I'm going to use Flourish more often now, for sure. And I enhanced on my Figma work for the soccer illustrations.

# What didn't work or where I would like to continue
What didn't work at first, obviously, was the scraping part. Transfermarkt.de is known to be not too scraper-friendly and it took me a while to figure out the while-loop-method for this case.
I also would have loved to turn the Github webpage into a scrollytelling but I didn't find the time to get into the details of webpage-building with scrollable elements.

Continuing from here, I would like to integrate different other sports into the analysis to give it a broader approach. For once, our mentor Jasmine told me to look for basketball or football data. And I found some databases on salary caps for different US sports, such as basketball, baseball, football. That's where I would go next to find more financial sports data to scrape, wrangle and visualize.
