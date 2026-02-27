```mermaid
flowchart TD

A[React Frontend\n(View Layer)]
B[Spring Boot Controller\n(REST API)]
C[Service Layer\n(Business Logic)]
D[Repository Layer\n(JPA)]
E[(PostgreSQL Database)]

A -->|HTTP Request (JSON)| B
B --> C
C --> D
D --> E
E --> D
D --> C
C --> B
B -->|JSON Response| A
```