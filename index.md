#Assignment 1.1 - How a Website Works

## Explanatory Paragraph

When I type a URL into my browser, the browser acts as the client and sends a request to the server where the website is stored. This request travels over the internet using HTTP (HyperText Transfer Protocol), or HTTPS (HyperText Transfer Protocol Secure) if the connection is encrypted. This process is called the request-response cycle: the client sends a request and the server sends back a response. If the website is static, the server simply sends ready-made HTML, CSS and JavaScript files that are the same for every visitor. If the website is dynamic, the server runs backend code and gets data from a database, such as user details or products, to build a page for that visitor. The browser then reads the files it received and displays the webpage on my screen.

## Roles

- Browser / Client: the program I use (Chrome, Edge) that sends requests and shows the page.
- Server: a computer that stores the website and responds to requests.
- Database: where the server stores data such as users, products and orders.

## HTTP and HTTPS

- HTTP: the set of rules used to transfer web pages between a browser and a server.
- HTTPS: the secure version of HTTP. The data is encrypted so others cannot read it.

## Static vs Dynamic Website

| Static Website | Dynamic Website |
|---|---|
| Same content for every visitor | Content can change for each visitor |
| Uses fixed HTML, CSS and JavaScript files | Uses backend code and a database |
| Fast and simple | Slower and more complex |
| Example: a portfolio page | Example: Amazon, Instagram |

### What I observed

- I opened the Network tab on en.wikipedia.org and refreshed the page. The browser made 28 requests to load the single page.
- About 14.3 kB was transferred, and the total size of the resources was about 1.1 MB. Many files were loaded from the browser cache, which is why the transferred size is smaller.
- The Status column shows the result of each request. 200 means success, 304 means the file had not changed so the cached copy was used, and 202 means the request was accepted.
- The Type column shows the kinds of files loaded, such as images (webp, png, svg+xml) and scripts.
- The Time column shows how long each request took. Most cached files took about 0 to 1 ms, while a request to the server took longer (for example 160 ms).
- This shows that one webpage is made of many separate requests, and the browser combines all the responses to display the page.


