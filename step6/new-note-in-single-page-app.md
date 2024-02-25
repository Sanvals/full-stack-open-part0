sequenceDiagram
    participant browser
    participant server

    browser->>server: The user submits a sigle POST request with the data
    activate server
    server-->>browser: The server parses the data and responds with a 201 status code
    deactivate server

    browser->>server: The browser pervents the page reload and updates the content via JS
    activate server
