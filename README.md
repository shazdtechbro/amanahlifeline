# Amana Lifeline — Next.js prototype

An emergency-first, voice-first agentic healthcare lifeline for underserved Nigerian communities. This is a React/Next.js application, not an HTML embed.

## Run locally

Use Node.js 20.9 or later. Run `npm install`, then `npm run dev`. Open http://127.0.0.1:3000. Run `npm run build` and `npm start` to serve a production build.

## Demonstrations

- Emergency, ambulance, hospital-readiness, routine-appointment and follow-up call journeys; manual stepping, automatic playback and optional browser speech.
- A generated character with six acted poses: listening, thinking, working, transport coordination, hospital readiness and connected care.
- A specialist-agent gallery with selectable roles and states, animated waveform and ambulance/coordinator illustrations, scroll reveals, hero parallax and reduced-motion support.
- English, Yoruba, Hausa, Igbo and Nigerian Pidgin example conversations. These are scripted examples, not validated multilingual speech recognition.
- Searchable illustrative providers, visit-request form validation, patient visits and cancellation, provider routine queue actions, handoff acknowledgement/decline and intake status.

## Entering the demonstration

Choose a patient or care-team role, then use **Fill demo credentials** on the sign-in screen. The application displays synthetic test values for form validation. There are no real user accounts, authentication service or protected backend behind this prototype.

## Suggested walkthrough

1. Use **Try a care call** and play or step through an emergency scenario.
2. Select a specialist and switch its acted states.
3. Switch language examples and compare the caller/agent text.
4. Search the provider directory and create a routine request with fictional details.
5. Sign in as patient to view/cancel the request.
6. Open **For care teams**, sign in as provider, acknowledge the pending handoff, and add/serve a routine queue entry.
7. Sign back in as patient and inspect the changed handoff status.

## Scope and data

Calls, providers, costs, availability, care records and partner responses are simulated. There is no live Amana telephone line, microphone capture, dispatch API, hospital integration, diagnosis or real appointment booking. Do not use the prototype for an actual emergency.

Only visit metadata is saved to browser-tab sessionStorage. Name and phone inputs are validated but not retained. Provider status, reminders, referral status and queue actions are in memory and reset on reload. No patient details are posted to a backend. Clear demo records in the care space or privacy dialog. Optional speech uses the browser’s speech synthesis implementation. Google Fonts supplies typography with local fallbacks.

## Research

Sources and scoped historic statistics are in `app/research.js`; full context is in the parent deliverable `Amana-emergency-research.md`. Historic study figures and national targets are not Amana outcomes or guarantees.

## Artwork

`public/images/amana-hero.webp` and `amana-states.webp` are generated custom character assets. PNG originals and the prompt/layout notes are retained. Sprite selection uses CSS; the characters also float and respond through state changes. No external character-image dependency is required.

## Deploy

Deploy this directory as a Next.js project on Vercel. No environment variables or backend services are required for this front-end demonstration. Install project dependencies locally rather than relying on any unrelated ancestor `node_modules` folder.
