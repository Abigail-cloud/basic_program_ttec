# basic_program_ttec
A Tutorial series by Toluwalase



# The Internet, the Web, and HTML: A Comprehensive Introduction

## What is the Internet?

The internet is a global network of interconnected computers and devices that communicate with each other using standardized protocols. It is a vast infrastructure that enables the transfer of data, information, and services across the world. The internet is not owned by any single entity but is a decentralized network of networks, maintained by various organizations, governments, and private entities.

At its core, the internet is built on the concept of packet switching, where data is broken down into smaller packets, sent across the network, and reassembled at the destination. This allows for efficient and reliable communication between devices, even if some parts of the network are congested or fail.

The internet supports a wide range of services, including email, file transfer, online gaming, and, most notably, the World Wide Web (WWW). The web is just one of many services that run on top of the internet, but it is the most widely used and recognizable.

## How Does the Web Work?

The World Wide Web, commonly referred to as the web, is a system of interlinked hypertext documents and multimedia content that can be accessed via the internet. The web operates on a client-server model, where clients (typically web browsers) request resources from servers, which then respond with the requested data.

### Role of Browsers and How They Render Web Pages

A web browser is a software application that allows users to access and view web pages. Popular browsers include Google Chrome, Mozilla Firefox, Safari, and Microsoft Edge. When you enter a URL (Uniform Resource Locator) into the browser's address bar, the browser performs several steps to render the web page:

1. **DNS Lookup**: The browser first needs to resolve the domain name (e.g., www.example.com) into an IP address. This is done using the Domain Name System (DNS), which acts like a phone book for the internet, translating human-readable domain names into machine-readable IP addresses.

2. **HTTP Request**: Once the browser has the IP address, it sends an HTTP (Hypertext Transfer Protocol) request to the server hosting the website. HTTP is the protocol used for transferring web pages and other resources over the internet.

3. **Server Response**: The server processes the request and sends back an HTTP response, which includes the requested resource (e.g., an HTML file) along with metadata such as status codes (e.g., 200 for success, 404 for not found).

4. **Rendering**: The browser receives the HTML file and begins to parse it. As it encounters additional resources like CSS files, JavaScript, and images, it sends additional requests to the server to fetch these resources. The browser then renders the page by combining the HTML, CSS, and JavaScript to create the final visual representation of the web page.

### Client vs. Server, DNS, HTTP, and URLs

- **Client**: The client is the device or software (usually a web browser) that requests and displays web content. It initiates communication with the server by sending HTTP requests.

- **Server**: The server is a computer or software that hosts web resources and responds to client requests. It processes requests and sends back the appropriate resources, such as HTML files, images, or videos.

- **DNS (Domain Name System)**: DNS is a system that translates human-readable domain names (e.g., www.example.com) into IP addresses (e.g., 192.0.2.1) that computers use to identify each other on the network.

- **HTTP (Hypertext Transfer Protocol)**: HTTP is the protocol used for transferring web pages and other resources over the internet. It defines how messages are formatted and transmitted, and how servers and browsers should respond to various commands.

- **URL (Uniform Resource Locator)**: A URL is the address used to access a resource on the web. It typically consists of several parts, including the protocol (e.g., http://), the domain name (e.g., www.example.com), and the path to the resource (e.g., /index.html).

## Introduction to HTML

HTML (Hypertext Markup Language) is the standard markup language used to create web pages. It provides the structure and content of a web page by using a system of tags and attributes. HTML documents are plain text files that can be created and edited with any text editor.

### Basic HTML Tags

- **`<html>`**: The root element of an HTML document. All other elements are contained within this tag.
- **`<head>`**: Contains meta-information about the document, such as the title, character set, and links to external resources like CSS files.
- **`<body>`**: Contains the content of the web page that is displayed in the browser.
- **Headings (`<h1>` to `<h6>`)**: Used to define headings, with `<h1>` being the highest level and `<h6>` the lowest.
- **Paragraphs (`<p>`)**: Used to define paragraphs of text.
- **Links (`<a>`)**: Used to create hyperlinks to other web pages or resources. The `href` attribute specifies the URL of the linked resource.
- **Images (`<img>`)**: Used to embed images in a web page. The `src` attribute specifies the path to the image file, and the `alt` attribute provides alternative text for screen readers and if the image fails to load.

## Hands-on Practice: Creating a Simple HTML Page

Let's create a simple HTML page that includes a heading, a paragraph, and an image.

1. **Open a Text Editor**: Open any text editor (e.g., Notepad, VS Code, Sublime Text).

2. **Create the HTML Structure**:
   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>My First Web Page</title>
   </head>
   <body>
       <h1>Welcome to My Web Page</h1>
       <p>This is a simple HTML page with a heading, a paragraph, and an image.</p>
       <img src="https://via.placeholder.com/150" alt="Placeholder Image">
   </body>
   </html>
