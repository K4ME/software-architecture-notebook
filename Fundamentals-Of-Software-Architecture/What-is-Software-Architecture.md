### "Technology architecture" or "enterprise architecture" 
Encompasses the overarching structure and layout of an organization's technological environment and infrastructure. 
It involves the design, arrangement, and integration of various technology components such as hardware, software, networks, data centers, cloud services, and IT systems.

"Corporate architecture" often refers to the broader structure and organization of an entire enterprise, including its business processes, strategies, goals, organizational structure, and 
how it aligns with its technological infrastructure. It aims to align technology solutions with the overall business strategy and objectives of the organization.
<br />

### Solution architecture
Refers to the design and structure of an individual system or application within an organization. 
It involves the creation of a comprehensive plan that defines how specific software components, modules, databases, interfaces, and technologies will work together to address a particular business problem or 
meet specific business requirements.

Solution architecture focuses on providing detailed technical specifications, frameworks, and guidelines for implementing and integrating various components into a cohesive and functional solution. 
It aims to ensure that the system or application meets performance, security, scalability, and other non-functional requirements while aligning with the broader enterprise architecture and business objectives.
<br />

### Software architecture
- Software architecture is a software engineering discipline.

**Software architecture** refers to the fundamental structure of a software system, including its components, relationships, design principles, and high-level decisions that guide software development. 
It defines the organization and interactions among different modules and layers of a system, ensuring that it meets functional and non-functional requirements. 
Software architecture is crucial for ensuring scalability, maintainability, and robustness of a system.
<br />

### The role of the software architect
The role of a software architect involves designing and overseeing the technical aspects of software development projects. 
Software architects are responsible for making high-level design choices, establishing technical standards, defining software structures, and ensuring that the software system meets the desired 
functional and non-functional requirements.

**Key responsibilities of a software architect include:**
- **Designing the System:** Creating a blueprint or architectural design for the software system, including defining components, interfaces, modules, and their interactions.
- **Technical Leadership:** Providing technical leadership and guidance to development teams, ensuring adherence to best practices, coding standards, and architectural principles.
- **Requirement Analysis:** Collaborating with stakeholders to gather and analyze requirements, understanding business needs, and translating them into technical solutions.
- **Risk Management:** Identifying potential risks, technical bottlenecks, and proposing mitigations or alternate solutions to ensure the success of the project.
- **Technology Evaluation:** Evaluating new technologies, tools, frameworks, and methodologies to determine their suitability for the project's requirements.
- **Documentation:** Creating architectural documentation, diagrams, and guidelines for developers to follow during implementation.
- **Collaboration and Communication:** Collaborating with cross-functional teams, including developers, testers, project managers, and business stakeholders, and effectively communicating technical decisions andtrade-offs.
- **Quality Assurance:** Ensuring that the software architecture supports scalability, maintainability, performance, security, and other quality attributes.
<br />

The "pillars" of software architecture generally refer to the fundamental principles that guide the design and development of software systems. 

**The key pillars of software architecture are often described as follows:**
- **Modularity:** The ability to divide a system into independent and interconnected components, facilitating software maintenance, reusability, and evolution.
- **Flexibility:** The system's capability to adapt to changes in requirements or the environment without significant structural modifications, while maintaining functionality and integrity.
- **Scalability:** The system's ability to handle increased load or demand, whether in terms of data volume, concurrent users, or processing, without compromising performance.
- **Security:** Ensuring data protection, prevention of unauthorized access, and system integrity against potential threats and vulnerabilities.
- **Performance:** Ensuring that the system performs its functions within acceptable parameters of speed, response time, and efficiency, meeting user needs.
- **Standards and Design Patterns:** Utilizing best practices, recognized design patterns, and compliance with software engineering principles to ensure a solid and consistent structure.
- **Ease of Maintenance:** Structuring the system in a way that makes it easy to identify, fix, or enhance specific parts of the software without affecting other areas.
<br />

## Resilience
- It is a set of strategies adopted intentionally to adapt a system when a failure occurs.
- Having resilience strategies allows us to minimize the risks of data loss and important transactions for the business.

### Strategies

#### Protect and be protected
- A system in a distributed architecture needs to adopt self-preservation mechanisms to ensure maximum quality operation.
- An accurate system cannot be selfish to the point of making more requests on a system that is failing.
- A slow system on air is often worse than a system off air. (Domino effect).

### Health check
- Without vital signs, it is not possible to know the health of a system.
- An unhealthy system has a chance of recovering if traffic stops being directed to it temporarily.
- Quality health check.

### Rate Limiting
- Protects the system based on what it was designed to support.
- Preference programmed by client type. (return 500 when the maximum number of requests is reached).

### Circuit Breaker
- Protects the system by causing requests made to it to be denied, Ex: 500.
- Closed circuit = Requests arrive normally.
- Open circuit = Requests do not reach the system. Instant error on the client.
- Half open = Allows a limited number of requests to check whether the system is able to return to the air completely.

### API Gateway
- It is a centralizer of all system requests.
- Ensures that "inappropriate" requests reach the system:
Ex: unauthenticated user.
- implements Rate Limiting, Health check, etc. policies.

### Service Mesh
- Controls network traffic.
- Avoids protection implementations by the system itself.
- mTLS (encryption).
- Circuit breaker, retry, timeout, fault injection, etc.

### Asynchronous communication
- Prevents data loss.
- There is no loss of data when sending a transaction if the server is down.
- Server can process the transaction in your time when online.
- Understand in depth the message broker / stream system.
