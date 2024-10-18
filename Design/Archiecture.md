
# Architecture

```mermaid

graph TD
    A[Main Page UI] -->|view| B[Customer UI]
    A -->|view| G[Service Provider UI]
    
    B --> C{Performs Actions}
    C --> D[Book Service Appointments]
    C --> E[Choose Date and Time]
    C --> F[Confirm Code]
    F --> |View or Modify| H[ Reservations]

    G[Service Provider UI] --> |view, update, delete, and call| H








