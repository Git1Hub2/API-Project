sequenceDiagram
participant Client
participant API Gateway
participant Backend Service 1
participant Backend Service 2

Client->>API Gateway: API Request
API Gateway->>Backend Service 1: Forward Request
Backend Service 1->>API Gateway: Response
API Gateway->>Client: Forward Response

Client->>API Gateway: API Request
API Gateway->>Backend Service 2: Forward Request
Backend Service 2->>API Gateway: Response
API Gateway->>Client: Forward Response
