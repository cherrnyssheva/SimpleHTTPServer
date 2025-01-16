# Simple HTTP Server

This project demonstrates a simple HTTP server built in Python using the `socket` library. The server supports basic request parsing, routing, and response generation.

## Features

- **Routing**: Handles requests to specific URLs (`/index` and `/blog`).
- **HTTP Methods**: Currently supports the `GET` method.
- **Error Handling**: Returns appropriate HTTP status codes and messages for unsupported methods or unknown URLs (e.g., 404 Not Found, 405 Method Not Allowed).
- **Custom Views**: Serves responses from predefined view functions.

## How It Works

1. The server listens for incoming connections on `localhost` and port `5000`.
2. Incoming requests are parsed to extract the HTTP method and URL.
3. Based on the URL and method, the server generates headers and content:
   - For known URLs, a predefined view function generates the content.
   - For unknown URLs or unsupported methods, the server returns an error message.
4. The response (headers + content) is sent back to the client.

## Possible Enhancements

- Add support for more HTTP methods (e.g., POST, DELETE).
- Implement asynchronous handling for multiple clients.
- Use template files for generating HTML content.
- Add logging and configuration options.

### The basis for writing the code was video from Oleg Molchanov
https://www.youtube.com/@zaemiel
