# FeedLink — Skills and Technical Capabilities

## Project Skills
- Frontend development using React, TypeScript, Vite, and Tailwind CSS.
- Backend API development using Node.js and TypeScript.
- Relational data storage using PostgreSQL and Neon.
- Deployment and hosting using Vercel and Render.
- AI integration through the Google Generative AI SDK.
- Food donation and receiver workflow management.
- Matching donors with receivers using relevant eligibility and compatibility criteria.
- Environment-based configuration and secure secret management.
- Error handling, testing, and maintainable project structure.

## AI and Matching
AI may assist with contextual interpretation, such as food urgency or request details, when the configured model is available. Deterministic rules should handle required eligibility checks and matching constraints. A fallback should be used when AI is unavailable.

## Engineering Guidelines
1. Keep frontend and backend responsibilities separate.
2. Validate inputs on the backend.
3. Never commit `.env` files or API keys.
4. Keep matching decisions explainable where possible.
5. Test important workflows and failure cases.
6. Document changes and keep deployment configuration consistent.

## Important
This document describes the intended project capabilities and engineering practices. Confirm each capability against the current implementation before presenting it as fully operational.
