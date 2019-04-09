# UiPath-Data-Scraper
UiPath short but useful automation I used to extract phone numbers from Craigslist for an Amazon Mechanical Turk HIT. 

1. The bot takes the URL from the Amazon HIT, opens a new browser window with this URL. 
2. Checks if the ad was removed, if it was, it closes the window and Returns the HIT. 
3. Else the ad is live, it scrapes the phone number, closes the window.
4. Checks if Amazon is asking for a Captcha. If it is, it reads the captcha image using Microsoft OCR and enters the sting into the      text box and clicks submit.
5. Finally, it enters the phone number into the text box and clicks submit.
6. Loops back to step 1.
