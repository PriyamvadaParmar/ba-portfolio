# 03 — Functional Requirements Specification (FRS)

## Authentication
- The system shall support biometric login on eligible devices.
- The system shall enforce MFA for high-risk actions (add payee, high-value transfer).

## Onboarding & eKYC
- The system shall parse KYC documents using OCR.
- The system shall validate identity via government KYC APIs and return a decision within 30 seconds.
- The system shall allow resuming an incomplete application within 7 days.

## Chatbot
- The chatbot shall answer Tier-1 queries and escalate to human support with full context.

## Personalization
- The dashboard shall show categorized spends and personalized nudges based on user behavior.

## Reporting & Audit
- The system shall log user actions and admin overrides with timestamp, actor, and outcome.

## Non-Functional
- P95 page response time < 2s for key flows.
- 99.9% availability target for auth and transfers.
- Compliance with data privacy & security policies.