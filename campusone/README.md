# CampusOne

A modern, responsive CampusOne frontend prototype built with React + Vite.

## Included in this prototype
- Responsive dashboard and navigation
- Persistent light/dark mode preference
- Dynamic date and time-of-day welcome
- Dynamic membership age calculated from the account creation timestamp
- Marketplace search, category, institution, location, budget and sort filters
- Accommodation listings included in marketplace filtering
- Course search and institution filter
- People search, institution filter, follow/unfollow controls and follower counts
- Basic profile and settings screens

## Run locally

Requirements: Node.js 20+

```bash
npm install
npm run dev
```

Build for production:

```bash
npm run build
```

## Deploy to Cloudflare Pages

1. Push this repository to GitHub.
2. In Cloudflare Dashboard, open Workers & Pages and create a Pages project connected to the GitHub repository.
3. Select the repository and production branch.
4. Build command: `npm run build`
5. Build output directory: `dist`
6. Deploy.

This is a Vite static frontend. It can be deployed to Cloudflare Pages without a Worker for this prototype.

## Important prototype limitations

This build is a frontend prototype. Demo marketplace listings, people, and courses are sample data. Follow state, theme preference and demo profile are stored in the browser's localStorage. Authentication, cross-device social follows, real follower counts, listing creation, messaging, payments, file uploads, AI, moderation and institution-wide shared data still require the production backend and database. Do not treat the demo UI as a live marketplace or production account system.

Before public launch, connect secure backend APIs, server-side authorization, PostgreSQL, managed file storage, verified payment webhooks, abuse reporting and moderation. Do not put AI provider secrets in frontend code.
