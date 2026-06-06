# Convertus AI Suite — Proposal & Demo

A single static site that pitches an AI platform for Convertus Group and links to a clickable, role-based demo. Built to deploy on Vercel.

## Pages

| URL | File | Description |
|-----|------|-------------|
| `/` | `index.html` | Sales presentation / landing page |
| `/ceo` | `app.html` | CEO — Executive Cockpit |
| `/regional` | `app.html` | Regional Manager — Operations Command Center |
| `/sales` | `app.html` | District Sales Manager — Sales Dashboard |

The demo is a single-page app; the role is resolved from the URL (`/ceo`, `/regional`, `/sales`, or `?role=` / `#` for local testing). A role switcher (top-right) and a cross-role Comms Center connect the three tiers.

## What's inside

23 AI tools across five domains — Corporate & Admin, Growth & Sales, Operations, Site Safety, and Leadership & Strategy — distributed across the three role dashboards.

> Prototype: data and AI responses are realistic samples to demonstrate the workflow, not connected to live systems.

## Deploy (Vercel)

It's a static site — no build step.

1. vercel.com → **Add New → Project**
2. Import this repo (or drag the folder in)
3. Set the project name to **convertus-ai-suite** so URLs match the links
4. Deploy

`vercel.json` provides clean-URL rewrites for `/ceo`, `/regional`, and `/sales`.

## Local preview

Open `index.html` in a browser. The clean `/ceo` paths only resolve once deployed; to preview a dashboard locally, open `app.html?role=ceo` (or `#gm`, `#rm`).
