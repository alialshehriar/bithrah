# Bithrah Technical Architecture

## Overview

Bithrah is built with a modern, scalable architecture designed for the Saudi Arabian market.

## Stack

```
┌──────────────────────────────────────────────┐
│                  Frontend                     │
│  Next.js 15 + React 19 + TypeScript          │
│  TailwindCSS + Framer Motion                 │
│  Bilingual: Arabic (RTL) + English (LTR)     │
└──────────────────┬───────────────────────────┘
                   │ REST API
┌──────────────────┴───────────────────────────┐
│                  Backend                      │
│  FastAPI (Python) + PostgreSQL               │
│  Authentication + Authorization              │
│  AI/ML Pipeline                              │
└──────────────────┬───────────────────────────┘
                   │
┌──────────────────┴───────────────────────────┐
│              AI/ML Engine                     │
│  Idea Analysis + Validation                  │
│  Community Matching                          │
│  Recommendation Engine                       │
│  Performance Analytics                       │
└──────────────────────────────────────────────┘
```

## Key Technical Decisions

### Why Next.js 15?
- Server-side rendering for SEO
- Static export capability for CDN distribution
- React 19 with latest features
- Excellent Arabic RTL support

### Why FastAPI?
- High-performance async Python backend
- Native support for ML/AI libraries
- Automatic API documentation
- Type safety with Pydantic

### Why PostgreSQL?
- Robust relational database
- Full-text search (Arabic + English)
- JSON support for flexible schemas
- Proven scalability

## AI Components

### Idea Analyzer
Evaluates submitted ideas across:
- Market viability
- Innovation score
- Community potential
- Similar project comparison

### Community Matcher
Uses ML to connect ideas with:
- Relevant supporter communities
- Domain experts
- Potential collaborators

### Recommendation Engine
Provides creators with:
- Improvement suggestions
- Optimal timing for campaigns
- Reward structure recommendations

## Security

- JWT-based authentication
- Rate limiting
- Input validation (Zod)
- HTTPS everywhere
- Saudi data residency compliance
