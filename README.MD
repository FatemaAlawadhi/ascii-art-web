## Ascii-art-web

## Description:
Ascii-Art-Web is a server-based application that allows users to generate ASCII art banners using different styles. It provides a web GUI (graphical user interface) for easy interaction with the application.

## Usage: 
How to Run: 
1. Start the server: 
```
go run main.go
```
2. Open a web browser and visit:
```
http://localhost:8119
```

## Implementation Details:
The Ascii-Art-Web application is built using the following technologies and concepts:
- Go programming language for the server-side implementation.
- HTML, CSS, and JavaScript for the frontend user interface.
- Go templates for rendering dynamic HTML pages.
- HTTP endpoints for handling different actions and requests.

The server provides the following HTTP endpoints:
- GET /: Returns the main HTML page, which includes a form for inputting text and selecting a banner style.
- POST /ascii-art: Accepts data from the client, including the user's text and selected banner style, and generates the corresponding ASCII art.

HTTP Status Codes:
- 200 OK: Returned when the request is successful and the ASCII art is generated without errors.
- 404 Not Found: Returned when necessary templates or banners are not found.
- 400 Bad Request: Returned when the request is incorrect or missing required parameters.
- 500 Internal Server Error: Returned when unhandled errors occur during the server-side processing.

Algorithm:
The algorithm for generating ASCII art banners involves the following steps:
1. Receive the user's text and selected banner style from the client.
2. Validate the input data to ensure it is correct and complete.
3. Retrieve the corresponding ASCII art banner template based on the selected style.
4. Replace specific characters in the template with the user's text to generate the final ASCII art.
5. Return the ASCII art as a response to the client.

## AUTHORS

* Fatema Alawadhi
* Asma Ahmed


## LICENSES
This program developed within the scope of Reboot.