# Contributing to BoloAI

BoloAI explores multilingual, voice-first assisted workflows in Hindi, Hinglish, and English.

## What matters
- Clearly distinguish **real provider integrations** from demo/mock fallback behavior.
- Preserve explicit user confirmation before actions that can incur costs or affect external accounts.
- Never hardcode or commit telephony, speech, AI model, SMS, or search API credentials.
- Prefer accessible, understandable errors for Hindi/Hinglish/English conversations.
- Use synthetic call records, numbers, messages, and transcripts for tests and examples.

## Development flow
1. Follow [README.md](README.md) to install the FastAPI app and configure `.env`.
2. Use `DEMO_MODE=true` for local development without external provider credentials.
3. Validate affected functionality using the test/evaluation commands documented in the README, where present in the checked-out branch.
4. Open a focused pull request with a summary, reproduction/demo steps, and details of which provider paths were tested.

## PR checklist
- [ ] Provider status is accurately surfaced in the UI/API
- [ ] Fallback behavior is documented
- [ ] No secrets or personal information in commits
- [ ] External side effects require informed confirmation
