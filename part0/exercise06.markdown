sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server->>browser: HTML document
    deactivate server

    browser->>browser: JavaScript code executes
    Note right of browser: The browser executes the JavaScript code that renders the notes again after a new note is added

