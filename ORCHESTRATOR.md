# FeedLink — Orchestrator Execution Guide

## Purpose
FeedLink connects food donors with receivers to reduce food waste and help direct surplus food to people who need it.

## Main Workflow
1. A user opens the platform and signs in.
2. The user selects the appropriate role: Donor or Receiver.
3. Donors submit food donation details; receivers provide their food requirements.
4. The backend validates incoming requests and retrieves relevant records from the database.
5. The matching workflow evaluates eligibility and compatibility using available information such as food type, quantity, location, and urgency.
6. AI assistance can provide contextual analysis when configured and available.
7. The system returns suitable matches and communicates relevant results through the platform.
8. Errors or unavailable AI services should be handled safely, using the available fallback logic.

## Architecture
- Frontend: React, TypeScript, Vite, and Tailwind CSS.
- Backend: Node.js and TypeScript.
- Database: PostgreSQL hosted on Neon.
- Backend deployment: Render.
- Frontend deployment: Vercel.
- AI integration: Google Generative AI SDK, configured through environment variables.

## Execution Principles
- Validate and sanitize user input.
- Keep credentials in environment variables; never commit real API keys.
- Use database records as the source of truth.
- Treat AI output as assistance, not as a replacement for eligibility checks.
- Handle database, API, and network failures gracefully.
- Return clear, useful responses to the frontend.

## Verification
Before a release, verify authentication, role selection, donation and receiver submissions, matching behavior, database connectivity, error handling, and deployment health.

Note: Actual runtime behavior depends on the implementation and deployment configuration.
