# Deprecation Warning
This version of JukeBot is no longer maintained and shouldn't be used. Use the [Kotlin version](https://github.com/Devoxin/JukeBot) of JukeBot instead. 

------

# Welcome to JukeBot's repository!
requires a mere 3 dependencies *not including the dependencies of those dependencies*

doesn't require ffmpeg/avconv, very low CPU & RAM usage because of the low dependency count & the fact that it'll only play opus format

soundcloud is probably broken because of the strict opus-only stuff


## Self-Hosting: Getting Started

You'll need several things:

[A Discord Account (duh)](https://discordapp.com)

[A Discord Bot Account](https://discordapp.com/developers/applications/me)

[A Google API Key](https://console.developers.google.com)

[NodeJS 7.x](https://nodejs.org/en/download/current/)

[Git](https://git-scm.com/)

## Self-Hosting: Configuring & Running

Once you have the basics done above, begin by creating a folder somewhere accessible (E.g. your desktop).

Open your newly created folder, and shift+right-click inside. Select 'Open Command Window Here'.

In the command window, type in the following command:
```
git clone https://github.com/Devoxin/JukeBot.git
```
![](http://i.imgur.com/qwJPsMP.png, "Screenshot 1")

In the new 'JukeBot' folder that's just been created, head into /src/, rename config.example.json to config.json and open it.

Inside config.json, enter your youtube key, bot token, desired prefix & paste your ID (in quotations, don't use your 4 digit discriminator) in the owner array, like so:
![](http://i.imgur.com/na21QnO.png, "Screenshot 2")

(You can get a youtube key from the Google API page. Create a project & enable the 'YouTube Data API v3' for it).

Property Breakdown: 
```
token      - This is your bot token
owners     - This acts as a bot override ensuring full permissions.
youtube    - This is your Google API key, used for accessing YouTube data
soundcloud - This is your SoundCloud API key, used for accessing SoundCloud data
prefix     - This is the character users will need to prefix their messages with to use the bot
version    - DO NOT CHANGE. This helps diagnose issues should you encounter any.
hardblock  - Users blocked from using the bot everywhere
```

Once you've filled in config.json with the relevant info, return to your command window and type in
```
npm install && npm start
```
![](http://i.imgur.com/easejxp.png, "Screenshot 3")

This will install the necessary modules and start JukeBot.

The last step is inviting the bot to your server. [Head Here](https://finitereality.github.io/permissions/?v=36793345) and paste your bot's client ID from the discord developers page into the box at the bottom left, and then click on the generated link. You'll be taken to the Discord page to invite the bot to your server, select the appropriate server and hit Authorize! You may now begin using the bot :)
