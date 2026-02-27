# Keeper Project -- Interview Discussion Questions & Answers

------------------------------------------------------------------------

## 1. Platform Persistence

**Q:** Is the document platform persistent, or is it session-based where
documents disappear after the user session ends?

**Answer:**\
The platform should be persistent. Documents must be stored in a durable
storage layer such as Azure Blob Storage or SharePoint and indexed in
Azure AI Search.\
Session-based storage would not be suitable for enterprise use
because: - Documents must remain available across sessions - Metadata,
embeddings, and access controls need persistence - Audit logging and
compliance require long-term storage

A persistent architecture ensures scalability, reliability, and
compliance.

------------------------------------------------------------------------

## 2. Replacing Copilot Studio

**Q:** How would you design and build an API-driven solution to replace
Copilot Studio?

**Answer:**\
Design a layered architecture:

**Architecture Layers:** - Web Front-End (React / Angular) - API
Gateway - Service Layer (Azure Functions or App Service) - Azure AI
Search - Document Source of Record (Blob, SharePoint, etc.) - Azure
OpenAI

**Flow:** 1. User sends query from front-end. 2. API calls service
layer. 3. Service queries Azure AI Search for relevant documents. 4.
Retrieved content is sent to Azure OpenAI for response generation. 5.
Response returned to UI.

This approach ensures modularity, scalability, and reusability.

------------------------------------------------------------------------

## 3. Document Segmentation by Role

**Q:** How would you separate 40,000+ documents by role?

**Answer:**\
Use Role-Based Access Control (RBAC) combined with metadata filtering.

**Implementation:** - Tag each document with metadata (department, role,
region). - Use Azure AI Search filters to enforce role-based queries. -
Integrate with Azure AD for identity validation. - Apply security
trimming at query time.

Overlapping access can be handled by assigning multiple role tags to
documents.

------------------------------------------------------------------------

## 4. Azure Networking Issue (Function → Storage Firewall)

**Q:** How would you resolve Function communication with a
firewall-protected Storage Account?

**Answer:**

Options:

1.  Enable VNet Integration for Azure Function.
2.  Use Private Endpoints for Storage Account.
3.  Deploy Function in Premium Plan (supports VNet and NAT Gateway).
4.  Use NAT Gateway to assign static outbound IP.
5.  Add trusted Microsoft services exception (if applicable).

Best practice: Use VNet Integration + Private Endpoint for secure
internal communication.

------------------------------------------------------------------------

## 5. Transition to a Reusable Service Layer

**Q:** How would you evolve from chatbot to reusable AI service?

**Answer:**

-   Extract AI logic into centralized microservices.
-   Expose REST APIs.
-   Implement API versioning.
-   Add logging, monitoring, and telemetry.
-   Support multiple clients (web, mobile, internal systems).

This creates a scalable enterprise AI platform instead of a single
chatbot solution.

------------------------------------------------------------------------

## 6. Real-Time Transcript Use Case

**Q:** How would you support near real-time transcript assistance?

**Answer:**

**Architecture:** - Real-time transcript ingestion (WebSocket or Event
Hub). - Stream processing layer (Azure Functions). - Query Azure AI
Search continuously. - Return ranked documents in near real-time.

Use caching and streaming techniques to reduce latency.

------------------------------------------------------------------------

## 7. Expanding Beyond Q&A

**Q:** How would you support broader enterprise AI capabilities?

**Answer:**

-   Modular AI architecture
-   Support summarization, classification, sentiment analysis
-   Workflow automation integration
-   Knowledge graph implementation
-   Centralized embedding and indexing strategy

Design system as AI platform, not just Q&A engine.

------------------------------------------------------------------------

## 8. Azure Maturity in a Google-Centric Environment

**Q:** How would you guide Azure maturity?

**Answer:**

-   Define Azure Landing Zone architecture
-   Establish governance and cost controls
-   Implement CI/CD pipelines
-   Security best practices (RBAC, Key Vault, Private Endpoints)
-   Documentation and training sessions
-   Gradual migration strategy

Focus on enabling best practices while aligning with existing Google
ecosystem where required.

------------------------------------------------------------------------

# End of Document
