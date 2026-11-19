# Enterprise Cloud Security Lab — Architecture

## 1. Purpose

Design and progressively implement an enterprise-style cloud security environment that demonstrates secure infrastructure architecture, network segmentation, identity protection, monitoring, and infrastructure automation.

The primary cloud platform will be Microsoft Azure, followed by AWS.

## 2. Architecture Status

**Status: Planned — Not Deployed**

The final architecture will be refined after inspecting existing Azure resources, subscriptions, virtual networks, address spaces, identity configurations, and security policies.

## 3. Planned Network Architecture

The initial Azure design will use a hub-and-spoke network topology.

### Hub Network

The hub will provide shared networking and security services, including:

- Azure Firewall
- Centralized routing
- DNS services
- VPN connectivity
- Security monitoring and logging

### Spoke Networks

Three logically separated environments are planned:

- **Development:** Infrastructure experiments and controlled security testing.
- **Testing:** Validation of infrastructure configurations and security policies.
- **Production-Like:** A more restrictive environment simulating enterprise production security requirements.

## 4. Initial Security Principles

- Least-privilege access
- Network segmentation
- Defense in depth
- Centralized monitoring
- Secure infrastructure automation
- Explicit security validation
- Controlled change management

## 5. Open Architecture Decisions

The following decisions must be made before infrastructure deployment:

- Azure subscription and management group organization
- Network IP addressing and subnet allocation
- VNet peering and routing design
- Firewall policy and traffic inspection requirements
- Identity and RBAC boundaries
- Logging and monitoring architecture
- Terraform state management
- Cost monitoring and resource cleanup

## 6. Future Expansion

The architecture will progressively incorporate advanced Azure security services, Docker, Kubernetes, AKS, AWS infrastructure security, and EKS.

All deployments and security controls will be documented and validated before being marked complete.
