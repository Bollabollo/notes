# Web Browser
A software that take in files from a remote server (or local directory) and render them for user interactions. When a file with ```.html``` extension is created, it signals to the browser engine to interpret the file as a HTML document.

## Web Browser Engine
A software the figures out what to do with the file that's sent to the client from the server. Mozilla's WBE is Gecko, for Chrome, it's Blink.

## The Process of opening a HTML document by a browser
When a client requests a HTML document, the server sends packets (bytes of data) over the internet. The raw bytes of data are then converted into characters based on the HTML document encoding (UTF-8). These characters are then further parsed into tokens ( small units of parsing). Tokens are then converted into _nodes_ and then linked to the **DOM**. 
