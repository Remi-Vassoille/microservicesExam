Part 1:
Commands for the docker file:
type nul > Dockerfile
docker build -t count-server .
docker run -dp 127.0.0.1:3000:3000 count-server

Part 2 :
Q1 – In a Microservices architecture for each process we have a different service, independent from the others. Services communicate with API’s. In a monolithic architecture, all processes are connected into one big block and are not independent from others.

Q2 – Microservices pros: scalability, flexibility, deployment independence, resilience, ease of sustainability.
Microservices cons: complex to manage, communication between services is complex
Monolithic pros: simple to develop, easy to deploy and manage, easy to test
Monolithic cons: Scalability is complex, single deployment for all applications, integration of new technologies is complex

Q3 – In a Microservices architecture, you need to have a service for each feature so that the services are independent. By doing this, the application is much easier to update and scale because if you need to change something, it only affects the relevant service.

Q4 – The CAP theorem says that you cannot guarantee Consistency, Availability, and partition Tolerance simultaneously. In microservices architecture, this is relevant because you need to choose which one you prefer to make your services interact and share data.

Q5 – Therefore, you must choose between Consistency and Availability when partitioning. You must also adapt error recovery strategies in the event of a failure due to the absence of one of the CAPs. Finally, systems must be designed to make them capable of operating in degraded mode.

Q6 – Microservices can enhance scalability in a cloud environnement by using continers to deploy independant services. These services can be automatically scalled if needed.

Q7 – In case of statelessness, each request is independent and the service does not save the state between them. This is important in microservices architecture because it allows any service instance to treat requests. So it’s more scalable and resilient.

Q8 – A gateway API is how external clients access the application. It routes requests to the right services, manages authentication, limits the flow and can filter data.