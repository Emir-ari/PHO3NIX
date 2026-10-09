# PHO3NIX Architecture

PHO3NIX is a modular AI-assisted cybersecurity assessment and security automation platform.

## System Overview

The platform is designed around a central orchestration layer that coordinates discovery, asset profiling, security assessment, validation, evidence collection and reporting.

## Main Components

### 1. Operator Layer
- CLI
- Dashboard
- API

### 2. Core Orchestration
- Task coordination
- Workflow management
- State handling
- Module execution
- Assessment lifecycle

### 3. AI Reasoning Layer
- Context analysis
- Planning
- Prioritisation
- Finding analysis
- Knowledge retrieval
- Report assistance

### 4. Asset & Attack Surface Management
- Hosts
- IP addresses
- Domains
- Subdomains
- Services
- APIs
- Cloud assets
- Identity systems
- Applications

### 5. Reconnaissance
- Passive discovery
- Active discovery
- DNS analysis
- Service discovery
- Web discovery
- Asset enrichment

### 6. Security Capability Modules
- Network
- Web
- API
- Identity
- Active Directory
- Cloud
- Containers
- Kubernetes
- Wireless
- Mobile
- IoT
- DevOps
- Supply Chain

### 7. Validation Engine
- Finding correlation
- Confidence scoring
- Reproduction data
- Evidence handling

### 8. Execution Fabric
- Jobs
- Workers
- Queues
- Module execution
- Runtime management

### 9. Threat Intelligence
- CVE enrichment
- CVSS
- EPSS
- Vulnerability intelligence
- Exploit mapping

### 10. Reporting
- Findings
- Evidence
- Timelines
- Remediation
- Structured reports

### 11. Knowledge Layer
- Assessment history
- Asset relationships
- Security findings
- Context storage
- Reusable knowledge

## High-Level Flow

```mermaid
flowchart TD

    A[Operator] --> B[CLI / Dashboard / API]

    B --> C[Core Orchestrator]

    C --> D[Asset Profiling]
    C --> E[Reconnaissance]
    C --> F[AI Reasoning]
    C --> G[Security Modules]

    G --> G1[Network]
    G --> G2[Web]
    G --> G3[API]
    G --> G4[Identity / AD]
    G --> G5[Cloud]
    G --> G6[Containers]
    G --> G7[Wireless]
    G --> G8[Mobile / IoT]
    G --> G9[DevOps]

    D --> H[Knowledge Layer]
    E --> H
    F --> H
    G --> I[Validation Engine]

    I --> J[Evidence Collection]
    J --> K[Reporting Engine]

    H --> F
