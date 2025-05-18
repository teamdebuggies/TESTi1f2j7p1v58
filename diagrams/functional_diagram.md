graph TD;
    A[User] -->|Access| B[Web Application];
    B -->|Fetch Data| C[Microservices];
    C -->|Read/Write| D[Database];
    C -->|Notification| E[Message Queue];
    B -->|Authentication| F[Auth Service];
    F -->|Token| A;
    D -->|Logs| G[Log Management];
    D -->|Monitoring| H[Monitoring Service];