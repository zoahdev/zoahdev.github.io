# What is authorization for Physical AI?

Physical AI authorization is the process of deciding and proving whether a specific agent may cause a specific machine to perform a specific real-world action, for a defined purpose and limited time.

KineGrant is an experimental open protocol for that permission boundary. The canonical path is:

Action Request -> Policy Evaluation -> Short-lived Capability -> Local Action Gate -> Physical Action -> Signed Receipt

The local gate verifies the trusted issuer, signature, exact request binding, scope, expiry, and one-time nonce immediately before the actuator boundary. A valid capability is consumed atomically so replay is rejected.

KineGrant complements IAM, PKI, API credentials, network controls, ROS 2/SROS2, OPC UA, Matter, and native safety systems. It does not replace them. It is not a robot operating system, motion planner, functional-safety controller, legal authority, recognized standard, or safety certification.

Official status: KGP-001 Experimental Open Draft 0.1. Reference implementation v0.1.1. Apache-2.0.

Primary source: https://zoahdev.github.io/physical-ai-authorization
Specification: https://github.com/zoahdev/kinegrant-protocol/blob/main/spec/KGP-001.md
Threat model: https://github.com/zoahdev/kinegrant-protocol/blob/main/spec/THREAT-MODEL.md
Executable evidence: https://zoahdev.github.io/challenge
