# esp8266-evil-twin
Attempt to phish wifi passwords with a captive portal!

This script is originally by 125k -> https://www.github.com/125k/ESP8266_WiFi_Captive_Portal

I, Anon505950, made some edits to make it look like the victims router firmware is out of date. The user inputs their password to their router to 'update', and that password gets sent to the creds page. 

The way that I use this is with a nodemcu deauther paired with a captive portal deauther. To find the latest and greatest deauther code, go to Spacehuhn's github -> https://github.com/spacehuhn/esp8266_deauther

# What does it do?
This script makes 3 pages:
1. Index - The page that pops up on the victims device with the password prompt. - 172.0.0.1
2. Verification - The post screen that the victim see's once they have inputed the password. - 172.0.0.1/post
3. Credentials - This is the screen that the attacker navigates to in order to see inputted passwords. - 172.0.0.1/creds

# Usage
First, rename values in the .ino file to fit specific attacker parameters. 
Second, set up the portal as well as a deauther and target a specific ssid.
Third, wait! People should start handing there wifi password right over to you!

# Disclamer
This script is for educational purposes only, don't hack anybody that didn't give you explicit permission to hack them. I am not responsible for any damages or repercussions that you may face using this code! 
