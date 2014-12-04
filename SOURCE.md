#Robert Wettlaufer
> Here's a quick rundown of my repos

##Current (Languishing) Project - `journal`
#####write random things, thoughts, blogs, or whatever with the CLI app backed by firebase with an angular front-end, inspired by [jrnl](http://maebert.github.io/jrnl/). Because there's no backend needed, you can host this on the github project page [as I do here](http://robert-wett.github.io/journal). One of the main objectives of this project is to create a rich experience without having to run any servers. All actions are first backed by a sqlite db, then persisted to a firebase store. At this time, firebase doesn't support a text-search so you have to pull down the entire collection and iterate through them which isn't super cool. This is a work in progress that just might be currently abandoned ;)
 - Node.js
 - Firebase + SQLite
 - Angular

----------

##Completed'ish Stuff
 > Stuff that's pretty much done, or in a 'viewable' state

###[Email Tracker](https://github.com/Robert-Wett/EmailTracker)
#####I hurriedly built this in 5 days of free-time for an interview challenge, with really no prior knowledge of how email tracking was implemented (because honestly, unless you need to who cares?). It's a proof of concept email tracking server that stores `Campaign`'s or unique sales events (Unique to the string level with this POC), like "Wikipedia's 50th donation begging" and maps them to individual `CampaignEmail`'s which are sent to specific `User`'s in the form of indivdual `UserRequest`'s that we track. At the moment, we track blanket information about every request we subsequently get from users under the corresponding `UserRequest` object, and enforce basic security in that a specific user can only redeem a given campaign once. Shortcuts used due to time constraint: Every endpoint is a `GET`, file structure is non-existent as everything is in [emailutils.js](https://github.com/Robert-Wett/EmailTracker/blob/master/lib/emailutils.js), and there's plenty of logic in [routes.js](https://github.com/Robert-Wett/EmailTracker/blob/master/routes.js).
 - Node.js + Express
 - Mongo

###[SimpleDB](https://github.com/Robert-Wett/SimpleDB)
#####A basic implementation of a key/value database with write-ahead logging and persistence. Command set is based on redis commands. This was another time-constrained assignment for an interview so it's not exactly super polished.
 - Python 3
 

###[Crypto Alert](https://github.com/Robert-Wett/cryptoalert)
#####Listen to a live feed of the latest Bitcoin, Litecoin, or Dogecoin prices and send an email alert if the value drops below a given point in USD.
 - Node.js
 - Firebase + nodemailer

###[EmoticonScraper](https://github.com/Robert-Wett/EmoticonScraper)
#####This project listens to Twitter's public [filter](https://dev.twitter.com/docs/api/1.1/post/statuses/filter) stream for defined [emoticons](https://github.com/Robert-Wett/EmoticonScraper/blob/master/modules%2Femoticons.js). It keeps track of the number of occurences of each emoticon, and displays the most-used emoticon at the top. The bottom portion changes each time a different emoticon is detected, and shows the last 25 tweets that triggered it.
 - Node.js + Express
 - Socket.io
 - EJS + Bootstrap

###[CorrectHorseBatteryStaple](https://github.com/Robert-Wett/CorrectHorseBatteryStaple)
#####This simple web-app was built in a couple of days preceeding the heartbleed bug. You can see a subtle nod to the [famous comic](http://imgs.xkcd.com/comics/password_strength.png) in the last cell of the comic [here](http://xkcd.com/1354/). There is some back-end API functionality that isn't documented or fully fleshed out.
 - Node.js
 - EJS + Bootstrap/jQuery
 
###[Reddit Sentiment Analysis](https://github.com/Robert-Wett/RedditSentimentAnalysis)
As seen on [blockspring](https://api.blockspring.com/users/robert-wett/blocks/24665639b10e5da3d6d3c5a4952b936e)

#####Grab a reddit user's latest comments on reddit, and run them against the popular TextBlob (NLTK-based) python library to get an overall "Sentiment" rating (postive or negative statements). The top 10 rated positive comments and their sentiment ranking, as well as the top 10 negative comments will be shown as well as the overall `are you happy` score. 

###[BoundedQueue](https://github.com/Robert-Wett/BoundedQueue)
#####Implements a FIFO queue that is optionally capacity bound. The queue also enforces type safety for all entries by designating the queue object class type in the constructor. ActionScript 3 does not intrinsically support templates/generics other than the Vector class but this convention serves the same purpose for this object.
 - ActionScript 3
 
###[What's Trending?](https://github.com/Robert-Wett/WhatsTrending)
*Unfortunately, this app was deprecated via Twitter's switch to [API V1.1](https://dev.twitter.com/docs/rate-limiting/1.1/limits) which killed the API end-point needed for this to function.*

#####The words in the title are the current top ten trending terms on twitter, for whatever location you choose in the drop-down (by default we are using U.S.A.). Underneath are the results we get when we cross-reference UrbanDictionary. The original idea was to try and make sense of some of the random people, places, terms, and things that trend on twitter throughout the day that might not exactly be in Merriam-Webster. The results can be funny, informative, random, useless (#hardtosplit), offensive, or a healthy mixture of them all. On the right-hand side, you'll see a table (not on mobile) that holds all the trends you've loaded in the session. You can click on "Location", or "Trend Name" to sort them descending/ascending alphabetically. Try loading different locations from the drop-down at the top and see what trends they share, and which ones are 'local'.
 - javascript
 - Bootstrap/jQuery

###[Daily Programmer](https://github.com/Robert-Wett/dailyprogrammer)
##### These are my solutions to various [/r/dailyprogrammer](http://www.reddit.com/r/dailyprogrammer) challenges, in 5 different languages. This is mostly for algorithm/problem-solving practice, or to learn a new language. The languages used are:
 - C#
 - JavaScript
 - Python
 - Ruby
 - ActionScript 3
 


----------
##Fun/Learning
 > Here are the projects that I did for the sole purpose (well, all my projects are for learning) of learning a specific technology or concept.

###[Tinder Keyword Swiper](https://github.com/Robert-Wett/TinderKeywordSwiper)
#####Automate tinder swiping behavior in a smarter way by defining positive and negative keywords (and subsequent weights for each) and swiping left or right based on matches. This relies on using [clarafai's](http://clarifai.com/) image recognition API, and only the POC has been built as of now.

###[GraphJS](https://github.com/Robert-Wett/GraphJS)
#####Working through graph-related CS problems in JavaScript. Algorithms are (somewhat loosely) transcribed from the Python code in  `Problem Solving with Algorithms and Data Structures`.

###[PyBraille](https://github.com/Robert-Wett/PyBraille)
As seen on [blockspring](https://api.blockspring.com/robert-wett/319bfef4aad7f3477745048a2da3ae6a).
#####Reads in a string and converts it into 2x3 delimited Braille characters (using standard English Braille). This was an experiment to learn more about using python in a more object-oriented, re-usable manner that one would expect from a command-line utility. This was based on my [DailyProgrammer solution](https://github.com/Robert-Wett/dailyprogrammer/blob/master/143_Braille.py).

###[EphemeralPhoto](https://github.com/Robert-Wett/ephemeralphoto)
#####Web-App that allows users to upload images, and denote the exact time the file will be un-hosted and the file deleted.
 - Node.js + Express

###[ManicPixieDreamQuote](https://github.com/Robert-Wett/ManicPixieDreamQuote)
#####Web-app that satirized the [Manic Pixie Dream Girl](http://tvtropes.org/pmwiki/pmwiki.php/Main/ManicPixieDreamGirl) trope using actual quotes from Tinder. This app was primarily done to get practice using **MongoDB** + **Redis**. The original (POC) version can be seen [here](http://blooming-stream-5857.herokuapp.com).
 - Node.js + Express

###[ng-subredditviewer](https://github.com/Robert-Wett/ng-subredditviewer)
#####Just pulling the jsonp results from a specified subreddit and displaying the top level entries as links. You can add comments on each of the entries, but there's no backend persistence so they'll be wiped out on refresh. This was a project to re-fresh my **Angular.js** skills. Check out the [bl.ocks.org](http://bl.ocks.org/Robert-Wett/27fad6eb3e74ba7c83ef) display to give it a try.
 - Angular

###[String To Comment](https://github.com/Robert-Wett/StringToComment)
#####Sublime Text 2 Plugin. StringToComment allows you to highlight a string and convert it into an 80-char delimited block comment in the language currently set in the view.
