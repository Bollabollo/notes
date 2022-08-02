# Web Browser
A software that take in files from a remote server (or local directory) and render them for user interactions. When a file with ```.html``` extension is created, it signals to the browser engine to interpret the file as a HTML document.

## Web Browser Engine
A software the figures out what to do with the file that's sent to the client from the server. Mozilla's WBE is Gecko, for Chrome, it's Blink.

## The Process of opening a HTML document by a browser
When a client requests a HTML document, the server sends packets (bytes of data) over the internet. The raw bytes of data are then converted into characters based on the HTML document encoding (UTF-8). These characters are then further parsed into tokens ( small units of parsing). Tokens are then converted into _nodes_ and then linked to the **DOM**. This processs needs to be done before CSS and JS files are rendered.
![image](https://user-images.githubusercontent.com/84720339/182420213-7ef7c1ed-3ccb-4faa-ab3c-03b7ae5c3bf0.png)


## Fetching the CSS file
While the browser receives the raw bytes of data and begins DOM construction, it also makes a request to fetch the CSS file linked. The process is similar to the HTML process but instead of the DOM, the constructed tree model is **CSSOM (CSS Object Model).**
![image](https://user-images.githubusercontent.com/84720339/182420837-c8075b78-4f5f-47e5-b83c-f4c93a35381d.png)



