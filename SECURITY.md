# Security Policy — BoloAI

BoloAI is a voice-first AI assistant with optional integrations for speech, AI reasoning, search, telephony and SMS. Not every provider is connected in demo mode.

## Data and service safety

- Keep all provider API credentials, signing secrets and external service tokens in deployment environment variables.
- Never commit or publish real calls, telephone numbers, transcripts, user messages or private documents.
- Demo/mock output must not be described as verified live provider data.
- Require confirmation before actions that send messages, spend money or affect external systems.
- Review webhook signature verification, authentication, authorization and request throttling before enabling a public telephony deployment.
- Use synthetic credentials and numbers in examples and automated tests.

## Reporting a vulnerability

Do not publish credentials, personal information or exploit details in public issues. Contact the maintainer privately through [@rajsalonia](https://github.com/rajsalonia), or GitHub private vulnerability reporting when available. Include concise reproduction steps using dummy records.

See [README.md](README.md) for provider requirements and [CONTRIBUTING.md](CONTRIBUTING.md) for testing guidelines.
