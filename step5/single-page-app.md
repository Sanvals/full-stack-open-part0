sequenceDiagram
    participant browser
    participant server

    browser->>server: The user sends a GET request to fetch the page from the server
    activate server
    server-->>browser: The server delivers the HTML page and JSON data to the browser
    deactivate server

    browser->>server: The browser fetches the JSON data and manipulates the HTML
    activate server
