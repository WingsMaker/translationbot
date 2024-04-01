# translationbot
google translation telegram bot

![image](https://github.com/WingsMaker/translationbot/assets/32192638/e5ced06f-4a3c-4655-bed0-757f479943dc)
<br>
Demo 
https://t.me/WingsMakerBot

<hr>

# Introduction 
How to create serverless telegram chatbot to perform google translation. (default language : English)

![image](https://github.com/WingsMaker/translationbot/assets/32192638/3478fcc7-fedc-466a-ada2-bf0d29c6c8e4)
<br>


# Requirements
- Google Gmail account ( where your android playstore account is )
- Telegram chatbot token, see https://t.me/BotFather
<br>

# Getting Started - Google App Script Project
[1] Goto https://script.google.com/home , click "New Project" 

[2] Write the scripts, copy paste from below template url :

https://raw.githubusercontent.com/WingsMaker/translationbot/main/google_translate_gas.txt

[3] Rename the project

Click on the "Untitled project" to rename the project as something else. Example, "GoogleTranslate".

![image](https://github.com/WingsMaker/translationbot/assets/32192638/3ab3fae4-0591-4279-b5a9-662600760a90)
<br>

[4] Deploy as google web app

In the Google App Script project, go to "Publish" in the top navigation bar. 
Under "Deploy as web app", select "Deploy". This will open a pop-up window. 
Your web app URL will be listed in the "Current web app URL" field.

Click on the "Deploy - New Deployment"

![image](https://user-images.githubusercontent.com/32192638/209758084-a48fdfd0-4eb8-45be-af04-1642c3c05ed8.png)

Click "Select type - Web App"

![image](https://user-images.githubusercontent.com/32192638/209758240-b3d00b5c-09de-4355-be1d-b6193269409f.png)
<br>

Fill in the form and click "Deploy".
( for more see https://www.youtube.com/watch?v=-AlstV1PAaA )

![image](https://user-images.githubusercontent.com/32192638/209758768-29dda612-80c7-425e-8a39-e3e80d2fe5bc.png)
<br>

Copy the web app url to the clipboard for later use.

[5] Update the values of weburi in the script.

Remove the substrings "https://script.google.com/macros/s/" and "/exec" of url. Copy the result to clipboard.
Change the value of statement, paste the weburi address into here.

var weburi  = "__paste_here__";

[6] Update the values of token in the script.

Find your Telegram chatbot token by logging into the BotFather in Telegram, selecting your bot, and clicking the "API Token" button.
( see https://www.youtube.com/watch?v=aNmRNjME6mE )
Change the value of statement, paste the bot token into here.

var token = "__replace_here__";

Save the project.

[7] Run the "start_bot" function for only once to make sure actual telegram bot able to callback this google web app.

![image](https://github.com/WingsMaker/chatgptbot/assets/32192638/416ecbda-30bb-4d63-adb3-d3a24da7822f)

Your telegram bot is ready !


