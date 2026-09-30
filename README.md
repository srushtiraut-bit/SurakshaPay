# SurakshaPay

A voice-based UPI assistant that helps first-time users pay safely in their own language.

Built for the **Drunix Hackathon** (NPCI x Citi) under the **Financial Inclusion** track.

## The problem

A lot of people in India still avoid UPI, or use it nervously: grandparents, small-town shopkeepers, anyone who recently got their first smartphone. Most payment apps expect you to read English, move through several screens and be sure about what you're tapping. If you're unsure, there's usually nobody to ask.

Scams make it worse. Fake collect requests, fake QR codes and phishing messages mostly hit people who are new to digital payments. One wrong payment is often enough for them to go back to cash for good.

## What we're building

- **Voice-guided payments** in Hindi, Marathi and English
- **Spoken confirmation** of the payee and amount before any payment goes through
- **Plain-language scam warnings** when a request or payee looks suspicious
- **Trusted-contact alerts** so a family member can be notified about risky payments
- **Practice mode** where new users try payments with simulated money first

## How it works

1. The user says who to pay and how much.
2. The app understands the request and reads the payee and amount back out loud.
3. A risk check runs in the background (rule-based checks first, with a small ML model on top).
4. If something looks off, the user hears a simple warning instead of a technical error.
5. The user confirms by voice, and the payment goes through.

## Tech stack

| Part | Tools |
|---|---|
| Frontend | React (mobile-friendly web app) |
| Backend | Node.js, Express, FastAPI |
| Voice | Whisper / Bhashini, text-to-speech |
| Risk engine | Python, scikit-learn |
| Database | MySQL |
| Testing and deployment | Postman, Docker |

## Project structure

```
SurakshaPay/
├── docs/          proposal and design notes
├── frontend/      user interface
├── backend/       payment flow and APIs
└── ml-engine/     scam-risk scoring
```

## Status

Early stage. We are currently talking to real users and setting up the project. Nothing here is finished yet, and this README will be updated as we build.

## Roadmap

- [ ] User research with first-time UPI users
- [ ] Voice pipeline (Hindi and Marathi first)
- [ ] Payment flow with NPCI/Drunix APIs
- [ ] Scam-risk engine
- [ ] Trusted-contact alerts and practice mode
- [ ] Usability testing and fixes
- [ ] Deployment and demo

## Team

- Srushti Pramod Raut.
- Himani Ashish Gupta.

Cummins College of Engineering for Women, Pune

## License

MIT
