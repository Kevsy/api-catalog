Sequence diagram test

```mermaid
sequenceDiagram
    participant UA as “User App”
    participant AB as “App (backend)”
    participant AGO1 as “API GW OP1”
    participant AGO2 as “API GW OP2”
    participant OP2 as “Operator 2”

    note over UA,AB,AGO1,AGO2,OP2: Identity and Routing
    note over UA: Self identity<br/>and routing

    UA->>AB: Send identity and routing
```
