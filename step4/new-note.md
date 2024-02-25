sequenceDiagram
    participant browser
    participant server

    browser->>server: The user submits the form, sending a HTTP POST request to the server
    activate server
    server-->>browser: The server responds with a HTTP status code 302, asking for a page reload
    deactivate server

    browser->>server: The browser reloads and issues another GET request, fetching the style, the JS and the data
    activate server
