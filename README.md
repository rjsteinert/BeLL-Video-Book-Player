# What this is and why it's useful
Video books cost little to produce (the example book was produced using Quicktime which comes for free with Mac OS X) and requires very little skill of the person generating the video book (only knowledge of how to start a screencast navigating PDFs required). This app builds on this concept by looking for an optional .cuepoints.json file that describes when the pages turn in the video book.  This allows the app to show what page of a video book the viewer is on and also to navigate between pages.  When file size of a video book is of concern, video books are best suited for early grade reading levels where picture books have large text.  This translates to only a small increase in file size between the PDF of the book and actual video file of the book. For example, the example book's PDF is 3.9mb while the video file is 5.4mb. 

![Screenshot](https://raw.github.com/rjsteinert/BeLL-Video-Book-Player/master/docs/screenshot.png)

# Getting started

To get started, put a WEBM video file at a URL accessible location, open the index.html in a browser, and add to the url the location of the WEBM video file.  For example:

http://127.0.0.1/bell-video-book-reader/index.html?url=http://127.0.0.1/example-book/patricks-birthday-party.webmsd.webm

# About Video Book formats
At the moment this code is hardcoded for the WEBM standard which is Android browser friendly and supported by most other major browsers.  It could however use any number of formats, you would just need to change the type parameter in the dynamically generated source tag.

# How to generate cuepoints for a video book.
From the url parameter provided, this code appends ".cuepoints.json" to it to find a cuepoints file that consists of a JSON array where each entry in the array is the precise second at which a page turns. See the cuepoints file for the example book to see exactly what I mean. At the moment this cuepoints file needs to be generated by observing at which second the page turns occur and recording that in the list of page turns in the cuepoints file.


# credits

BeLL Video Book Player by R.J. Steinert, Open Learning Exchange (http://ole.org)

FlowPlayer by FlowPlayer LTD (https://github.com/flowplayer/flowplayer) 

Kevin's Birthday book by Rubbish Books
