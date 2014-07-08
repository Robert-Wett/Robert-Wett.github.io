#Robert Wettlaufer
####Hi there! If you are here, you're probably looking for a breakdown of my github projects so you don't have to waste time seeing if I can actually code. I'll start with some "finished" projects.


----------
##Completed Stuff
 > Stuff that's pretty much done, or in a 'viewable' state


###[EmoticonScraper](https://github.com/Robert-Wett/EmoticonScraper)
####This project listens to Twitter's public [filter](https://dev.twitter.com/docs/api/1.1/post/statuses/filter) stream for defined [emoticons](https://github.com/Robert-Wett/EmoticonScraper/blob/master/modules%2Femoticons.js). It keeps track of the number of occurences of each emoticon, and displays the most-used emoticon at the top. The bottom portion changes each time a different emoticon is detected, and shows the last 25 tweets that triggered it.
 - Node.js
 - Socket.io

###[CorrectHorseBatteryStaple](https://github.com/Robert-Wett/CorrectHorseBatteryStaple)
####This simple web-app was built in a couple of days preceeding the heartbleed bug. You can see a subtle nod to the [famous comic](http://imgs.xkcd.com/comics/password_strength.png) in the last cell of the comic [here](http://xkcd.com/1354/). There is some back-end API functionality that isn't documented or fully fleshed out.
 - Node.js
 - Bootstrap/jQuery
 
###[BoundedQueue](https://github.com/Robert-Wett/BoundedQueue)
####Implements a FIFO queue that is optionally capacity bound. The queue also enforces type safety for all entries by designating the queue object class type in the constructor. ActionScript 3 does not intrinsically support templates/generics other than the Vector class but this convention serves the same purpose for this object.
 - ActionScript 3
 
###[What's Trending?](https://github.com/Robert-Wett/WhatsTrending)
####*Unfortunately, this app was deprecated via Twitter's switch to [API V1.1](https://dev.twitter.com/docs/rate-limiting/1.1/limits) which killed the API end-point needed for this to function.*

####The words in the title are the current top ten trending terms on twitter, for whatever location you choose in the drop-down (by default we are using U.S.A.). Underneath are the results we get when we cross-reference UrbanDictionary. The original idea was to try and make sense of some of the random people, places, terms, and things that trend on twitter throughout the day that might not exactly be in Merriam-Webster. The results can be funny, informative, random, useless (#hardtosplit), offensive, or a healthy mixture of them all. On the right-hand side, you'll see a table (not on mobile) that holds all the trends you've loaded in the session. You can click on "Location", or "Trend Name" to sort them descending/ascending alphabetically. Try loading different locations from the drop-down at the top and see what trends they share, and which ones are 'local'.
 - javascript
 - Bootstrap/jQuery

###[Daily Programmer](https://github.com/Robert-Wett/dailyprogrammer)
#### These are my solutions to various [/r/dailyprogrammer](http://www.reddit.com/r/dailyprogrammer) challenges, in 5 different languages. This is mostly for algorithm practice, or to learn a new language. The languages used are:
 - C#
 - JavaScript
 - Python
 - Ruby
 - ActionScript 3
 


----------
##In-Progress/Experiments
 > Here are the projects that I did for the sole purpose (well, all my projects are for learning) of learning a specific technology or concept.

<br>
###[GraphJS](https://github.com/Robert-Wett/GraphJS)
####Working through common graph-related CS problems in JavaScript. Algorithms are transcribed from `Problem Solving with Algorithms and Data Structures`, written in python.
<br>
###[EphemeralPhoto](https://github.com/Robert-Wett/ephemeralphoto)
####Web-App that allows users to upload images, and denote the exact time the file will be un-hosted and the file deleted.
<br>
###[ManicPixieDreamQuote](https://github.com/Robert-Wett/ManicPixieDreamQuote)
####Web-app that satirized the [Manic Pixie Dream Girl](http://tvtropes.org/pmwiki/pmwiki.php/Main/ManicPixieDreamGirl) trope using actual quotes from Tinder. This app was primarily done to get practice using **MongoDB** + **Redis**. The original (POC) version can be seen [here](http://blooming-stream-5857.herokuapp.com).
<br>
###[ng-subredditviewer](https://github.com/Robert-Wett/ng-subredditviewer)
####Just pulling the jsonp results from a specified subreddit and displaying the top level entries as links. You can add comments on each of the entries, but there's no backend persistence so they'll be wiped out on refresh. This was a project to re-fresh my **Angular.js** skills. Check out the [bl.ocks.org](http://bl.ocks.org/Robert-Wett/27fad6eb3e74ba7c83ef) display to give it a try.
<br>
###[Reddit Sentiment Analysis](https://github.com/Robert-Wett/RedditSentimentAnalysis)
####This is a script that takes in a reddit username as a parameter, then scrapes the first 100 comments of said user and determines the overall positivity ratio of the comments via TextBlob. As of now, it prints out the top 10 positive comments, then top 10 negative comments (these are sorted lists), then the overall ratio. This was primarily done to get more experience with **Python** and the **TextBlob** library.
<br>
###[PyBraille](https://github.com/Robert-Wett/PyBraille)
####Reads in a string and converts it into 2x6 delimited Braille characters (using standard English Braille). This was an experiment to learn more about **OOP Python**.
<br>
###[String To Comment](https://github.com/Robert-Wett/StringToComment)
####Sublime Text 2 Plugin. StringToComment allows you to highlight a string and convert it into an 80-char delimited block comment in the language currently set in the view.