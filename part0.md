# 0.5: Single page app diagram

```mermaid
sequenceDiagram;
    title Single Page App (SPA) Load Flow
    participant Browser
    participant Server

    Browser->>Server: GET /exampleapp/spa
    activate Server
    Server-->>Browser: HTML document
    deactivate Server

    Browser->>Server: GET /exampleapp/main.css
    activate Server
    Server-->>Browser: main.css
    deactivate Server

    Browser->>Server: GET /exampleapp/spa.js
    activate Server
    Server-->>Browser: spa.js
    deactivate Server

    Browser->>Server: GET /exampleapp/data.json
    activate Server
    Server-->>Browser: JSON data
    deactivate Server
```

# 0.6 New note in Single page app diagram

```mermaid
sequenceDiagram;
    title New note in SPA
    participant Browser
    participant Server

    Browser->>Server: POST /new_note_spa
    activate Server
    Server-->>Browser: 201 Created
    deactivate Server
```
