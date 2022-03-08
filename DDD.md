<b><h1 align="center">Technical Papers On Domain-Driven Design </h1>
<h2 align="center">by SOHEL I. PATEL</h2></b>


## **Abstract** ##
Domain-Driven Design is a software design or development approach to resolving business logic. This design solves complex domain models, connecting to the core business concepts. Reducing friction between Domain experts, developers, and team members to interact and collaborate to achieve the Business goals.

## **1. Introduction**

 In Eric Evan's 2003 book  Domain-Driven Design: Tackling Complexity in the Heart of Software DDD concept was introduced.
Consider we have created software using all the latest tech and infrastructure now, our software design architecture looks pretty good but, when It is in the market, ultimately the end-user who decides whether our system is Excellent or not. Also, if the system does not solve business needs is of no use to anyone; No matter how pretty it looks or how well architecture its infrastructure. When we are developing software, our focus should not be primarily on technology; instead; It should be essentially on the business.

### **1.1  Domain logic and Model**  ###
Domain logic is the purpose of your modeling. Most commonly, it’s referred to as business logic. This is where business rules define the way data gets created, stored, and modified. Domain model includes the ideas, knowledge, data, metrics, and goals that revolve around that problem that they are trying to solve. It contains all the rules and patterns that will help you deal with complex business logic. Moreover, they will be useful to meet the requirements of your business.

## **2. Strategic Design** ##
The objective of DDD is to define the Bounded contexts, the Ubiquitous Language, and the Context Maps.

### **2.1 Bounded Context** ###
Bounded context is the boundaries of the context where a domain model is applicable. The large domain will have great difficulties because different people will use vocabulary, terms, and sentences. Outside of that limit will probably mean something different.

### **2.2 Ubiquitous Language** ###
It is the common language used by all team members to interact with all activities around the domain model. It brings together the domain experts, the technical team, and the others involved in the project.

### **2.3 Context Maps** ###
It shows the relationships between the different Bounded Contexts.

## **3. Tactical Patterns :** ##
It's mainly concerned with implementation details. It is a set of Technical resources used in the construction of the Domain Model, and these resources apply to work in a single Bounded Context.

### **3.1 Entity** ###
An Entity can be a changeable object which has a unique identifier. Entities have a life of their own within their Domain Model; An entity is like a class with some properties. The instance of these classes has a global identity and keeps the same identity throughout the lifespan.

### **3.2 Values Object** ###
These are immutable and do not have a unique identity, 
to update a Value Object, you must create a new instance to replace the old one which is a consequence of this immutability. (e.g. js object which non-primitive)

### **3.3 Services** ###
Services are stateless classes or objects that perform some logic that does not fit with an operation on an Entity or Value Object.
a service is functionality that exists somewhere between entities and values objects but it is neither related to an entity nor values objects.
They perform domain-specific operations, which can involve multiple domain objects.

###  **3.4 Aggregates** ### 
An aggregate is a collection of entities and values which come under a single transaction boundary.  Aggregates basically, control change and have a root entity called aggregate roots. The root entity governs the lifetime of other entities in aggregates.

### **3.5 Factories** ### 
Factories are used to handle aggregate. It provides an abstraction in the construction of an Object and can return an Aggregate Root, an Entity, or a Value Object. Factories help in managing the beginning of the lifecycle of aggregates Factories are an alternative for building objects that have complexity in a building via the constructor method.

###  **3.6 Repositories** ###  
Repositories handle aggregate. These are mainly used to deal with storage, they abstract concerns about data storage. They are responsible for persisting Aggregates. Repositories help in managing the middle and end of the lifecycle of an aggregate Repositories help in persisting aggregates. We should always create a repository per aggregate root but not for all entities.

## **4.Example Of DDD: Microservices** ##
Microservices is an architecture design model with a specific bounded context, configuration, and dependencies. These result from the architectural principles of domain-driven design and DevOps. 
The business goal is important to the business users, with a clear interface and functions. This way, the microservice can run independently from other microservices. 
Using microservices means creating applications from loosely coupled services. The application consists of several small services, each representing a separate business goal. They can be developed and easily maintained individually, after which they are joined in a complex application.

## **5. Conclusion** ##
Domain-driven design is the idea of solving problems of the organization through code. It improves our craft, provides flexibility, prefers domains over the interface, and reduces the communication gap between teams through Ubiquitous Language. Common terminology between the domain experts and the development team includes domain logic, subdomains, bounded contexts, context maps, domain models, and ubiquitous language as a way of collaborating and improving the application model and solving any domain-related challenges. With this article, I wanted to define the core concepts around domain-driven design. The downside of DDD is that It requires a professional who has strong domain expertise. It encourages the team to follow iterative practices.

## **6. Acknowledgements** ##
I would like Thanks to Google,youtuber Alpha code, wikipedia, Geekforgeeks, dev.to and medium.com

## **7. References**
<p>[1] https://en.wikipedia.org/wiki/Domain-driven_design</p>
<p>
[2] https://www.youtube.com/playlist?list=PLZBNtT95PIW3BPNYF5pYOi4MJjg_boXCG</p>
<p>
[3] https://www.domainlanguage.com/wp-content/uploads/2016/05/DDD_Reference_2015-03.pdf</p>
<p>
[4] https://thedomaindrivendesign.io/what-is-strategic-design/</p>
<p>
[5] https://thedomaindrivendesign.io/what-is-tactical-design/</p>
<p>
[6] https://www.geeksforgeeks.org/domain-driven-design-ddd/</p>
<p>
[7] https://dev.to/microtica/the-concept-of-domain-driven-design-explained-1ccn</p>

































