# 05 — Process Flows (Mermaid)

## As-Is: Onboarding (high level)
```mermaid
flowchart LR
A[Start] --> B[Download App]
B --> C[Register Account]
C --> D[Manual Form Entry]
D --> E[Upload KYC Docs]
E --> F[Manual Verification]
F -->|1-3 days| G[Decision]
G --> H[Activate Account]
```
## To-Be: Onboarding with OCR eKYC
```mermaid
flowchart LR
A[Start] --> B[Register Account]
B --> C[Scan ID (OCR)]
C --> D[Auto-fill + Validate]
D --> E[KYC API Check]
E -->|< 30s| F[Decision]
F --> G[Activate Account]
```
## To-Be: Support Deflection
```mermaid
flowchart LR
A[User Query] --> B[AI Chatbot Tier-1]
B -->|Resolved| C[End]
B -->|Not Resolved| D[Human Agent]
D --> E[Close with Notes]
```