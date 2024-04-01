# Image-Scraping-from-Google-Images (Fork)
Now  scrape as many images as you want, from google images using Python, Chromedriver and Selenium

**Dependencies needed**
1) Module Installations:
Install as `pip install -U -r requirements.txt`
2) [Python 3+](https://www.python.org/download/releases/3.0/?) - Pyhton 3.6+ verion
3) Paste the script inside a folder, open your terminal (Command Prompt for Windows) from that location and execute the script by typing `python googe_image_scraping_script.py`

The `error_clicks` parameter is to stop when there are no more results to show and end of the page is reached in Google Images search.

Line 82 is the timeout, which is set to 60 seconds. Sometimes while scraping the loop gets stuck forever when downloading an image, so the timer will resolve that issue and skip to next image automatically

Line 105 change the queries you want to search: `queries = ["Manchester City", "Manchester United", 'Barcelona', 'Real Madrid']` in my case

Line 110 `links = fetch_image_urls(query,500,wd)`, 500 denotes no. of images you want to download 

   > Open your terminal (`cmd` in Windows) execute the following query:
     `python google_image_scraping_script.py`
     Now in that same directory, you will see a folder `datasets` inside which you will see a folder for each name of search text that you put in. In my case the folder names will be the list of queries that I have passed.

References: https://medium.com/@wwwanandsuresh/web-scraping-images-from-google-9084545808a2

