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

2. Identity Claims, Roles and API Compatibility
Retrieving user roles and ensuring that identity claims could be correctly interpreted by the existing backend was another challenge. This involved investigating token claims, additional API calls, and how role information could be used during the authorisation process.

Integrating ZITADEL with the existing backend required understanding how the different APIs could communicate and exchange information. This involved identifying compatibility issues, adapting integration approaches, and esnuring that the necessary authentication information could be processed correctly.

3. API Deprecation and Long-Term Compatibility
During development, I identified that one of the ZITADEL API endpoints used to retrieve user roles had been deprecated. I investigated the recommended alternatives and updated the integration to use the newer ListAuthorizations API, helping maintain compatibility with future ZITADEL updates and reducing the risk of relying on outdated functionality.

4. Email delivery and SMTP Integration
Configuring email delivery through ZITADEL introduced unexpected challenges during the integration. I investigated the existing email setup across different platforms to identify the appropriate configuration and help resolve an issue that was blocking progress. Working with my supervisor, we identified and addressed a potential email delivery issue, allowing us to complete the SMTP integration, test invitation emails, and customise their branding for the SSO experience.

5. Identity Provider Configuration and Security Recommendations
One of the final challenges was determining which configuration settings would be most appropriate and secure for enterprise customers using their existing identity providers. We configured an identity provider, created test users, and extensively tested different settings with the integrated SSO solution to evaluate their impact on security and user experience. After reviewing the results and discussing our findings with senior developers and management, we agreed on a set of recommended configuration practices to include in the customer documentation.
 
# Lessons Learned
1. The Vaue of Curiosity and Initiavtive
Something I've learned from working on different projects is the value of following my curiosity and exploring ideas beyond immediate requirements.

Sometimes, taking a little extra time to investigate a technology or a possible approach can become unexpectedly useful later on.

This happened with Terraform during the SSO project. Having explored its capabilities earlier, I was able to apply that knowledge when we needed an infrastructure provisioning solution under time pressure.

This experience reinforced something I had already started learning from previous projects: following an idea a little further can make a real difference when unexpected challenges arise.

2. Learning Through Challenging Conversations
One of the most valuable lessons I learned was to become more comfortable with challenging technical discussions. Even when I arrived at meetings well-prepared, conversations with senior developers often introduced concepts beyond my experience. Although uncomfortable at times, these moments became some of my greatest learning opportunities.

Over time, I gained confidence in sharing my observations, asking questions, and contributing ideas based on my research and testing. I learned that growth often comes from being willing to engage in discussions where I don't have all the answers, staying curious, and being open to feedback.

## Confidentiality
This repository provides an overview of my professional contributions and the technical concepts explored during the project.

No proprietary source code, internal configurations, customer information, credentials, or confidential architectural details are included.

The descriptions focus on general engineering racties and publicly document technologies rather than the company's internal implementation.
