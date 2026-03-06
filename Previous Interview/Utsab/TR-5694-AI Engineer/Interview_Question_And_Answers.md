AI Engineer (SAP Managed Services) – Interview Q&A
1. Are you currently working? Can you talk about yourself and your background?

Answer

Yes, I am currently working at Health First as a Software Engineer. I have around 13 years of experience in software engineering, primarily focused on backend development using Python and building scalable cloud-based platforms.

Over the last few years, my work has shifted more toward AI-driven automation and LLM-based systems. In my current role, I work on building AI-powered operational automation platforms that integrate with enterprise systems and healthcare data services.

One of the key projects I worked on was an AI-based incident diagnostics assistant that analyzes system alerts, operational logs, and ServiceNow tickets. The AI agent provides root cause analysis and remediation suggestions, which significantly reduces manual triage effort for support engineers.

The system runs on AWS using containerized services and serverless components, and I was responsible for designing the AI orchestration layer, enterprise integrations, and deployment pipelines.

2. Which cloud platform are you familiar with? AWS or Azure?

Answer

My primary experience is with AWS.

In my current role, we deploy most of our AI services and backend applications on AWS. We use AWS for compute resources, storage, monitoring, and scalable deployments.

The AI systems are deployed using containerized services and cloud-managed infrastructure, ensuring scalability, reliability, and secure operations.

Although my hands-on experience is mainly with AWS, I am familiar with general cloud architecture principles such as container orchestration, serverless computing, and secure API integrations, which are applicable to Azure environments as well.

3. What is your SAP experience?

Answer

My SAP experience is mainly from an integration and architecture perspective, rather than working directly within specific SAP modules like HR, Finance, or Supply Chain.

Most of my work has focused on building AI-driven systems that integrate with enterprise platforms using APIs and structured data services. This is very similar to how SAP exposes business data through OData services and enterprise APIs.

In my current projects, AI agents retrieve structured enterprise data, operational logs, and incident information, process it using retrieval pipelines and LLM reasoning, and generate insights or remediation steps.

While I have not implemented ABAP development or SAP RAP directly, my expertise lies in building AI systems that integrate with enterprise platforms, which can easily extend to SAP systems using OData services and enterprise APIs.

4. Is your strong point SAP or AI?

Answer

My strong point is AI engineering.

I specialize in building AI agents, LLM-based automation systems, and enterprise AI platforms that integrate with existing enterprise systems.

SAP in this role would be the enterprise platform that the AI systems integrate with, while my expertise focuses on AI architecture, agent orchestration, retrieval pipelines, and cloud deployment.

5. Do you design MCP architecture?

Answer

Yes, I have experience designing AI agent orchestration architectures, including MCP-style integration patterns.

The architecture typically includes a retrieval layer, reasoning layer, and tool integration layer. The AI agent retrieves enterprise data, interacts with APIs or external tools, and combines that information with LLM reasoning to generate responses.

My role usually involves designing the agent workflow, defining tool interfaces, and integrating the system with enterprise platforms and cloud infrastructure.

6. What are the pros and cons of MCP?
Pros

Standardized integration between LLMs and external tools

Modular architecture for adding new services

Better enterprise data access

Supports complex AI agent workflows

Scalable for enterprise environments

Cons

Architecture complexity

Potential latency from multiple tool calls

Security concerns with enterprise APIs

Context management challenges

Operational overhead for monitoring and governance

7. Can you explain Redbook integration?

Answer

Redbook integration refers to connecting AI systems with runbooks or operational knowledge repositories.

When an incident occurs, the AI agent retrieves alerts, logs, and incident data. It then queries the runbook repository to retrieve relevant troubleshooting procedures.

Using semantic search and retrieval pipelines, the AI finds the most relevant documentation and combines it with the incident context to generate recommended diagnostic steps and remediation guidance.

8. What is webhook integration?

Answer

Webhook integration enables event-driven communication between systems.

For example, when a new incident is created in ServiceNow, the platform sends a webhook event to our backend service.

That event triggers the AI workflow, which retrieves the incident details, analyzes logs and alerts, and generates diagnostics or remediation suggestions.

Webhook architecture enables real-time automation and loosely coupled system integration.

9. Are you working as a full stack developer?

Answer

Yes, I work in a full-stack capacity, although my primary focus is on backend and AI services.

On the frontend side, I work mainly with React to build interfaces and dashboards that allow users to interact with AI agents or review system insights.

The React frontend communicates with backend APIs, which connect to the AI processing services and enterprise integrations.

10. Can you give an example of using Docker and Kubernetes?

Answer

We use Docker to containerize AI services and backend APIs.

Each component of the system, such as AI agent services, retrieval pipelines, and API layers, runs in a Docker container. This ensures consistent environments across development, staging, and production.

We deploy these containers into a Kubernetes cluster, which manages orchestration, scaling, and system health.

Kubernetes provides:

Auto-scaling when workload increases

Self-healing when containers fail

Rolling deployments for updates without downtime

Load balancing across services

This architecture ensures high availability and scalability for AI workloads.

11. Do you lead a team or work independently?

Answer

I work in a lead full-stack capacity, where I handle both system design and hands-on development.

I collaborate with backend engineers, frontend developers, and platform teams. My responsibilities include:

Designing AI architecture

Defining integration workflows

Implementing backend services

Conducting code reviews and peer reviews

We follow a pull-request based workflow using Git, where every change goes through peer review before merging.

12. Have you worked with Oracle data services?

Answer

Yes, I have worked with Oracle-based data services from a data integration and backend services perspective.

Our backend systems retrieve structured enterprise data stored in Oracle databases, often using SQL queries, stored procedures, or service APIs.

This data is then processed by AI pipelines or analytics systems to generate insights or support operational workflows.

13. Have you worked with OData services?

Answer

Yes, I have experience working with OData services from an integration perspective.

OData is commonly used in enterprise platforms like SAP to expose structured business data through RESTful APIs.

Our backend systems call OData endpoints to retrieve enterprise data, process the data through application workflows or AI pipelines, and generate insights or automation actions.

14. What do you know about CDS Views?

Answer

CDS Views (Core Data Services) are used in SAP to define semantic data models on top of database tables.

They allow developers to create structured representations of business entities, which can then be exposed through OData services.

External systems, including AI services, can retrieve this data through APIs and use it for analysis, automation, or workflow orchestration.

While I have not implemented CDS views directly in SAP, I understand how they are used to model enterprise data and expose it for integrations.