#### What a service?
- Make information available
- Perform transactions
- Solve business problem
- Independent of technology or product
- Can connect to multiple "clients"

#### SOA - Service-Oriented Architecture
- Normally larger services based on features
- Need to ESB
- Single point of failure
- Common Shared Database
```
   Sistema       Usuarios
     ||             ||
     \/             \/
 --------------------------
 |Enterprise   Service Bus|
 --------------------------
     ||             ||
     \/             \/ 
   Service        Service
     ||             ||
     \/             \/
          Database
```

#### Microservice-based Architecture
- Small services with less responsibility
- Greater fault tolerance
- Totally independent 
- Each service has it own database
- Synchronous or Asynchronous communication
```
    Site       Intern System
     ||             ||
     \/             ||
   Service -------> ||
     ||             ||
     \/             \/
   Service <----- Service
```
##### Disadvantage
- Complex architecture
- High cost
- Need more teams to maintain
- The system needs be large enough to justify
- Generate new problems
- Complex monitoring