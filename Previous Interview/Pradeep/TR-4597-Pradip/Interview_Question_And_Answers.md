# Professional Dynamics 365 CRM Interview Preparation

## Introduction

**Answer:**\
Hi, my name is Pradip Rimal. I have over 11 years of experience as a
Microsoft Dynamics 365 CRM and D365 CE Developer, with strong expertise
in Power Platform, C#.NET, and Azure integrations.

Currently, I'm working as a Lead CRM and Power Platform Developer at
Health Book, where I design and deliver end-to-end CRM solutions,
including integrations using Azure Data Factory, Azure Functions, and
APIs.

I have hands-on experience with plugin development, custom workflows,
Power Automate, Dataverse customizations, JavaScript form scripting, and
large-scale data migrations using SSIS.

Overall, I focus on building scalable, secure, and high-performance
Dynamics 365 solutions while owning the full lifecycle from design to
deployment and support.

------------------------------------------------------------------------

## 1️⃣ C# Strategy for Performing Multiple Data Updates Without Causing Timeouts in Dynamics 365

**Question:** How do you perform multiple data updates in Dynamics 365
using C# in real-time and manual scenarios without causing performance
issues or timeouts?

**Answer:**\
When performing multiple data updates in Dynamics 365 using C#, I focus
on separating real-time processing from bulk or manual updates to avoid
timeouts and platform impact.

For real-time or user-driven scenarios, I keep synchronous plugins
extremely lightweight and use them only for validations or critical
updates. Any heavy processing is moved to asynchronous plugins, Azure
Functions, or background services.

For bulk or manual updates, I never update records one by one. I use
**ExecuteMultipleRequest** to batch records together and reduce service
calls. I also control the batch size, usually between **100 and 500
records**, to stay within Dataverse throttling limits.

For very large data volumes or external system updates, I prefer **Azure
Functions** or **Azure Data Factory**. These services run outside
Dynamics, support retries and logging, and update Dataverse through the
Web API in a controlled and scalable manner.

I also disable unnecessary plugins, workflows, and Power Automate flows
during bulk operations whenever possible. Overall, batching,
asynchronous processing, and offloading heavy logic outside Dynamics
helps me perform updates safely without timeouts.

------------------------------------------------------------------------

## 2️⃣ Securing Client ID and Client Secret for Application User Authentication

**Question:** How do you securely manage the client ID and client secret
required for application user authentication in Dynamics 365?

**Answer:**\
To securely manage the client ID and client secret, I never hard-code
credentials in the application or store them in plain configuration
files.

I register the application in **Azure Active Directory** and store
secrets securely in **Azure Key Vault**. The application accesses Key
Vault using a **managed identity**, so no credentials are exposed in the
code.

At runtime, the app retrieves the secret securely from Key Vault and
uses it to request an access token from Azure AD. Whenever possible, I
prefer **certificate-based authentication** over client secrets for
higher security.

I also rotate secrets regularly, apply **least-privilege permissions**
for the application user in Dynamics 365, and restrict Key Vault access
using **RBAC and private endpoints**. This ensures credentials remain
secure, auditable, and compliant.

------------------------------------------------------------------------

## 3️⃣ Importance of Authentication Type in a Custom Connector

**Question:** When creating a custom connector that integrates with an
external API, why is the authentication type important and how do you
secure it?

**Answer:**\
The authentication type is a critical setting when creating a custom
connector because it defines how securely the external API is accessed
and how credentials are managed.

I choose the authentication type based on the API's security model. For
enterprise systems, I prefer **OAuth 2.0** or **Azure AD
authentication**. API keys are used only when OAuth is not supported.

For OAuth-based connectors, I use Azure AD app registration and define
proper scopes and permissions. Token handling and refresh are
automatically managed by the Power Platform, reducing security risks.

If secrets or API keys are required, I store them securely using
**environment variables** or **Azure Key Vault** and restrict access
using **role-based security** and least-privilege principles.

I also enforce token expiration, rotate secrets regularly, and limit
connector usage to specific environments and users. This ensures the
connector remains secure, compliant, and production-ready.
