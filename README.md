# Enterprise Single Sign-On (SSO) Solution
Identity & Access Management | Authentication & Authorisation | Software Engineering
Case study covering identity federation and access management.

## Project Overview
This project included contributing to the design, development, implementation of an Enterprise Single Sign-On solution for a cybersecurity company.
The main objective was to simplify authentication for enterprise customers by giving them te option to use their own identity providers to authenticate their users while maintaining compatibility with their permissiona and access to resources.


## Technologies and Concepts
- Identity Management: ZITADEL
- Authentication OpenID Connect (OIDC), OAuth 2.0
- Backend Development: Go (Golang=
- Infrastructure as Code: Terraform
- Security: PKCE, JWT validation, Role-Based Access Control (RBAC)
- Architecture: Identity Federation, Multi-Tenant Access Management
- Cloud Infrastructure: AWS

## My Contributions
1. Research and Technical Evaluation
- Evaluated ZITADEL's capabilities and documentation to assess its compatibility with the existing backend and authentication requirements.
- Investigated possible integration approaches, considering implementation complexity, maintainability and compatibility with existing functionality.
- Explored the ZITADEL Go SDK and developed initial proof-of-concept integrations to understand authentication flows and token handling.
- Identified potential technical challenges and investigated approaches to address them.
- Worked on request signature validation to support secure communication between ZITADEL Actions and backend services.

2. Architecture and Initial Development
- Contributed to the initial technical design and proposed an implementation approach for the integration.
- Developed and tested an early prototype to validate key components and authentication concepts.
- Presented an initial demonstration to comany supervisors and discussed technical findings.
- Investigated compatibility issues and considered potential implications for security and customer experience.

3. Infrastructure and Configuration
- Developed Terraform configurations to support consistent environment provisioning.
- Worked on identity management configuration and integration testing across development and staging environments.
- Investigated configuration issues affecting federated authentcation with external identity providers.

4. Testing and Troubleshooting
- Created a test plan covering authentication flows, backend integration, infrastructure provisioning and CLI authentication.
- Performed integration and end-to-end testing across test and staging environments.
- Investigated and debugged authentication, configuration and compatibility issues.
- Collaborated with other developers to validate the behaviour of the solution.

5. Technical Documentation
- Produced internal step-by-step technical documentation to support the integration of the solution and fina delivery.
- Documented code changes and contributed to the deployment documentation.
- Documented configuration requirements, testing procedures and relevant considerations.

## Technical Challenges
1. Integration with Existing Authentication Systems
Introducing a new SSO solution into an existing pletform required maintaining compatibility with the previous authentication approaches during the transition without disrupting existing functionality.

2. Identity Claims and Role Management
Retrieving user roles and ensuring that identity claims could be correctly interpreted by the existing backend was another challenge. This involved investigating token claims, additional API calls, and how role information could be used during the authorisation process.

3. Backend Integration and API Compatibility
Integrating ZITADEL with the existing backend required understanding how the different APIs could communicate and exchange information. This involved identifying compatibility issues, adapting integration approaches, and esnuring that the necessary authentication information could be processed correctly.

4. Third-Party Identity Provider Integration
Supporting external identity providers introduced challenges related to configuration and compatibility. Different providers required testing and troubleshooting to ensure that enterprise users could authenticate through their existing identity systems.

5. API Deprecation and Long-Term Compatibility
During development, I identified that one of the ZITADEL API endpoints used to retrieve user roles had been deprecated. I investigated the recommended alternatives and updated the integration to use the newer ListAuthorizations API, helping maintain compatibility with future ZITADEL updates and reducing the risk of relying on outdated functionality.

6. Email delivery and SMTP Integration
Configuring email delivery through ZITADEL introduced unexpected challenges during the integration. I investigated the existing email setup across different platforms to identify the appropriate configuration and help resolve an issue that was blocking progress. Working with my supervisor, we identified and addressed a potential email delivery issue, allowing us to complete the SMTP integration, test invitation emails, and customise their branding for the SSO experience.

 
# Authentication and Authorisation
One of the key challenges was understanding how authenticated identities could be associated with the appropriate accounts and permissions.

This involved working with authentication tokens, identity claims and role-based access control concepts.

# Integration with Existing Systems

Introducing a new authentication solution into an established platform required careful consideration of compatibility and migration.

The aim was to support new authentication capabilities while maintaining continuity for existing users.

# Performance and Reliability

The integration also introduced considerations around backend communication, efficient account management and service reliability.

These challenges required evaluating potential performance implications and investigating ways to minimise unnecessary processing.

# Security and User Experience

This involved considering secure token management, access permissions, and authentication flows that would provide a straightforward experience for users and administrators without compromising security.

# Lessons Learned

To be completed.

## Confidentiality
This repository provides an overview of my professional contributions and the technical concepts explored during the project.

No proprietary source code, internal configurations, customer information, credentials, or confidential architectural details are included.

The descriptions focus on general engineering racties and publicly document technologies rather than the company's internal implementation.
