# Closet Pilot — Project Guidelines (`GEMINI.md`)

## Overview
**Closet Pilot** is an AI-powered web application that helps users declutter and sell unwanted clothing by analyzing garment photos, coaching photo quality, recommending platforms and pricing based on sold comps, surfacing required measurements, generating marketplace listings, and tracking inventory status.

## Core Principles
- **Beginner-Friendly & Transparent**: Keep the architecture clean, well-documented, and easy to run locally.
- **Security First**: Never hardcode API keys or secrets in source files. Always use `.env` / `.env.local` (which are excluded via `.gitignore`).
- **Iterative Development**: Build and verify one slice of functionality at a time, committing working checkpoints to Git.

## Core Modules
1. **Photo Analysis & Quality Coach**: Multimodal AI inspection of garment & tag photos + actionable photography feedback.
2. **Market & Platform Advisor**: "Sell vs. Consign vs. Donate" triage, platform matching (Poshmark, eBay, Depop, Grailed, etc.), and sold-comp price guidance.
3. **Measurement Assistant**: Garment-specific measurement checklists and sizing reference.
4. **Listing Copy Generator**: Marketplace-tailored titles, descriptions, and tags.
5. **Inventory Pipeline**: Status tracking (`Draft`, `Listed`, `Sold`, `Donate`).
