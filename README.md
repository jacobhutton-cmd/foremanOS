# ForemanOS

Mobile-first web platform for independent trade contractors — built on GitHub Pages + Supabase.

## Live App
https://jacobhutton-cmd.github.io/foremanOS/

## Stack
- **Frontend**: Single-file HTML/JS/CSS — GitHub Pages
- **Backend**: Supabase (Postgres + Auth + Storage + Edge Functions)
- **AI Layer**: Gemini 1.5 Pro via Supabase Edge Functions (Phase 2)

## Features
- 📋 **Client Intake Portal** — anonymous intake, trade selection, photo upload
- 🔧 **Technician Dashboard** — work order list, detail view, status updates
- 📥 **Intake Queue** — convert intake sessions to work orders
- 🤖 **Tech Briefings** — AI-generated first-trip summaries (Edge Function layer)
- 🏠 **Mechanical Biography** — equipment assets, specs, repair history per property

## Setup

1. **Supabase project**: `pnsyuuonddgfqcmjiitf` (already configured)
2. **GitHub Pages**: Enable in repo Settings → Pages → Source: GitHub Actions
3. **Storage buckets**: Create `intake-temp` and `audio-transcripts` in Supabase Storage
4. **Anon auth**: Enable Anonymous Sign-ins in Supabase Auth settings

## Deployment
Every push to `main` auto-deploys via GitHub Actions.
