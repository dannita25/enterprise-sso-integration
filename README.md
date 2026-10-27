# Enterprise Single Sign-On (SSO) Solution
Identity & Access Management | Authentication & Authorisation | Software Engineering
Case study covering identity federation and access management.

## Project Overview
This project included contributing to the design, development, implementation of an Enterprise Single Sign-On solution for a cybersecurity company.
The main objective was to simplify authentication for enterprise customers by giving them te option to use their own identity providers to authenticate their users while maintaining compatibility with their permissiona and access to resources.


## Technologies and Concepts
- Identity Management Interface and third party provider: ZITADEL
- Authentication OpenID Connect (OIDC), OAuth 2.0
- Backend Development: Golang
- Infrastructure as Code: Terraform
- Security: PKCE, JWT token validation, role-based access control (RBAC)
- Architecture: Identity Federation,multi-tenant access management
- Database: AWS

## My Contributions
- Evaluating ZITADEL documentation to decide whether it worked for our current backend and could blend within our current PPAT system.
- Build a proposal on how to implement the base that will handle ans sustain the whole code.
- Tried out the ZITADEL Go SDK example, in our backend system, in order to return an http request with a token with claims that our backend can handle.
- Identified the main issue that con interfere with the implementation and implement a solution for that.
- Worked on the first code draft with all the key pieces and tested it.
- Displayed a first demo to company supervisors
- Troubleshoot compatibility issues and noted future possible issues, facing customer experience and customer security.
- Build a Terraform solution, to serve as a template for Testing, Staging and Deployment Instances
- Build a Test Plan for teh different parts of the project, CLI, Admin Service connected to ZITADEL and Terraform.
- Tested the whole flow on the Test and Staging Instances.
- Debug final configuration issues ofr thid arty authentciation with specific Customer Identity Providers 
- Build internal step-by-step documentation for final product delivery

## Technical Challenges
- Securly attach token claims, and find the user roles for all of the company roles
- Map and connect Zitadel APIs to Approov endpoints
- Investigated performance considerations related to account management and backend communications.
- Maintain compatibility with old service for migration of old service giving the option to unable or disable the new SSO solution
- Email delivery and test round to check all emails were delivered correctly and if not throw an issue
- Find the right set of ocnfiguration for maintaining user credentials private and secure for reduce attack possibilities
- 
## Confidentiality
This repository provides an overview of my professional contributions and the technical concepts explored during the project.

No proprietary source code, internal configurations, customer information, credentials, or confidential architectural details are included.

The descriptions focus on general engineering racties and publicly document technologies rather than the company's internal implementation.
