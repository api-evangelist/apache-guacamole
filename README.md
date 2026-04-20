# Apache Guacamole (apache-guacamole)
Apache Guacamole is a clientless remote desktop gateway that supports standard protocols like VNC, RDP, and SSH. It requires no plugins or client software and provides access to remote desktops through a web browser with a comprehensive REST API for connection, user, and session management.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Apache, Open Source, RDP, Remote Access, Remote Desktop, SSH, VNC, Web Gateway

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-04-19

## APIs

### Apache Guacamole REST API
REST API for managing connections, users, groups, and active sessions in Apache Guacamole remote desktop gateway, with token-based authentication and per-data-source resource management.

**Human URL:** [https://guacamole.apache.org/doc/gug/guacamole-rest-api.html](https://guacamole.apache.org/doc/gug/guacamole-rest-api.html)

#### Tags:

 - Authentication, Connections, Remote Desktop, REST, Users

#### Properties

- [Documentation](https://guacamole.apache.org/doc/gug/guacamole-rest-api.html)
- [OpenAPI](openapi/apache-guacamole-rest-openapi.yml)
- [JSONSchema](json-schema/guacamole-rest-auth-token-schema.json)
- [JSON-LD](json-ld/apache-guacamole-rest-context.jsonld)

### Apache Guacamole JavaScript Client API
JavaScript client library for embedding the Guacamole remote desktop client in web applications, with APIs for protocol tunneling, display rendering, and user input handling.

**Human URL:** [https://guacamole.apache.org/doc/gug/writing-you-own-guacamole-app.html](https://guacamole.apache.org/doc/gug/writing-you-own-guacamole-app.html)

#### Tags:

 - JavaScript, Remote Desktop, SDK

#### Properties

- [Documentation](https://guacamole.apache.org/doc/gug/writing-you-own-guacamole-app.html)

## Common Properties

- [Documentation](https://guacamole.apache.org/doc/gug/)
- [GettingStarted](https://guacamole.apache.org/doc/gug/users-guide.html)
- [GitHubOrganization](https://github.com/apache)
- [GitHubRepository](https://github.com/apache/guacamole-client)

## Features

| Name | Description |
|------|-------------|
| Clientless Remote Desktop | Access remote desktops through any HTML5 web browser with no client software or plugins required. |
| Multi-Protocol Support | Supports VNC, RDP, SSH, and Telnet protocols through a unified web gateway. |
| Token-Based Authentication | Stateless REST API authentication using time-limited tokens from the /api/tokens endpoint. |
| Connection Management | REST API for creating, updating, and organizing remote desktop connections and connection groups. |
| User and Group Management | Fine-grained user and group permissions for controlling access to connections and administrative functions. |
| Active Session Monitoring | Monitor and terminate active remote desktop sessions through the REST API. |
| Connection History | Audit log of all remote desktop sessions with timestamps and user attribution. |
| Extension API | Java extension API for implementing custom authentication providers, event listeners, and protocol extensions. |

## Use Cases

| Name | Description |
|------|-------------|
| Remote Desktop Access | Provide browser-based access to Linux and Windows desktops for remote workers. |
| Cloud Server Management | Access cloud VMs and servers through SSH and RDP via browser without installing VPN or client software. |
| Secure Bastion Host | Use Guacamole as a protocol-proxying bastion host to isolate internal systems from direct network access. |
| Development Environment Access | Provide developers with browser-based access to containerized or virtualized development environments. |
| IT Support Tooling | Enable IT helpdesk teams to access and troubleshoot user desktops through the browser. |

## Integrations

| Name | Description |
|------|-------------|
| Apache Tomcat | Runs as a Java web application on Apache Tomcat or any Java Servlet container. |
| LDAP / Active Directory | LDAP extension for authenticating users against directory services like Active Directory. |
| TOTP / Duo MFA | Multi-factor authentication extensions supporting TOTP apps and Duo Security. |
| MySQL / PostgreSQL | Database authentication extensions for storing connections and users in relational databases. |
| Kubernetes | Guacamole can be deployed on Kubernetes with the guacamole-client Docker image. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Apache Guacamole REST API](openapi/apache-guacamole-rest-openapi.yml)

### JSON Schema

- 7 schema files in [json-schema/](json-schema/)

### JSON Structure

- 7 structure files in [json-structure/](json-structure/)

### JSON-LD

- [Apache Guacamole REST Context](json-ld/apache-guacamole-rest-context.jsonld)

### Examples

- 7 example files in [examples/](examples/)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Apache Guacamole REST API](capabilities/shared/guacamole-rest.yaml) — 5 operations for connection and session management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Apache Guacamole Remote Access](capabilities/guacamole-remote-access.yaml) | guacamole-rest | 5 | DevOps Engineer |

## Vocabulary

- [Apache Guacamole Vocabulary](vocabulary/apache-guacamole-vocabulary.yaml) — Unified taxonomy mapping 4 resources, 5 actions, 1 workflow, and 1 persona across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Apache Guacamole Spectral Rules](rules/apache-guacamole-spectral-rules.yml) — 10 rules across 5 categories enforcing Apache Guacamole API conventions

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
