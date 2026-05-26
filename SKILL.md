---
name: grok-vercel-react-best-practices
description: React and Next.js performance optimization guidelines from Vercel Engineering, enhanced for Grok users. Use for writing, reviewing, refactoring React/Next.js code to achieve optimal performance. Triggers on React components, Next.js pages, data fetching, bundle optimization, re-renders, performance audits, or any request involving Grok for React/Next.js speed improvements. Works with Grok native skills and real-time X community insights.
license: MIT
metadata:
  author: vercel + grok-optimization
  version: 1.1.0
  compatibility: grok, claude, codex, cursor
---

# Grok-Optimized Vercel React Best Practices

**Vercel Engineering + Grok enhancements** — 70+ performance rules across 8 priority categories. Originally from Vercel, now tuned for seamless use with Grok (including real-time X data for latest React patterns).

## When to Activate (Grok Triggers)
- Writing new React components or Next.js pages
- Implementing or optimizing data fetching (client/server)
- Reviewing code for performance bottlenecks
- Refactoring for bundle size, re-renders, or load times
- Asking Grok: "optimize this React code", "fix Next.js performance", "make my app faster"
- Any performance audit or "best practices" request in React/Next.js

**Grok Advantage**: Combine with Grok's native X search for fresh community discussions, benchmarks, or edge cases not in static rules.

## Rule Categories by Priority (Quick Reference)

| Priority | Category                  | Impact       | Prefix     | # Rules |
|----------|---------------------------|--------------|------------|---------|
| 1        | Eliminating Waterfalls    | CRITICAL     | async-     | 6       |
| 2        | Bundle Size Optimization  | CRITICAL     | bundle-    | 6       |
| 3        | Server-Side Performance   | HIGH         | server-    | 10      |
| 4        | Client-Side Data Fetching | MEDIUM-HIGH  | client-    | 4       |
| 5        | Re-render Optimization    | MEDIUM       | rerender-  | 16      |
| 6        | Rendering Performance     | MEDIUM       | rendering- | 11      |
| 7        | JavaScript Performance    | LOW-MEDIUM   | js-        | 12      |
| 8        | Advanced Patterns         | LOW          | advanced-  | 4       |

**Total: 70 rules** — Prioritized by real-world impact from Vercel production codebases.

### Top Quick Wins (Start Here in Grok)
1. **Eliminate waterfalls** — Use `Promise.all()` and Suspense boundaries (`async-parallel`, `async-suspense-boundaries`)
2. **Avoid barrel imports** — Direct imports only (`bundle-barrel-imports`)
3. **Parallelize server fetches** — Restructure for concurrent data loading (`server-parallel-fetching`)
4. **Memoize expensive renders** — Extract to memoized components (`rerender-memo`)
5. **Use content-visibility** for long lists (`rendering-content-visibility`)

## How to Use with Grok
1. Install in your Grok environment (or reference this skill).
2. When chatting with Grok about React/Next.js, it automatically activates for relevant tasks.
3. For deeper dives: Ask Grok to "apply vercel-react-best-practices to this code" or "check against all categories".
4. **Pro Tip**: Pair with Grok's real-time X search — e.g., "latest React 19 performance patterns from X + these rules".

**Detailed rules & examples**: See `rules/` directory in the original repo (each rule has bad/good code + explanation). For full list, reference the original Vercel repo or ask Grok to expand specific categories.

## Grok-Specific Enhancements (v1.1)
- Added explicit Grok trigger phrases for better activation.
- Integrated guidance for combining with Grok X data (fresh community benchmarks, new patterns).
- Improved table for quick scanning in Grok responses.
- Added "Quick Wins" section for faster agent decision-making.
- Metadata updated for multi-agent compatibility (Grok priority).

## Anti-Patterns to Avoid
- Never ignore priority — always tackle CRITICAL (waterfalls, bundles) first.
- Don't apply rules in isolation — consider full component tree impact.
- Avoid over-optimizing LOW priority before HIGH impact areas.

**Source**: Optimized from Vercel Labs agent-skills (original ~389K+ installs on skills.sh leaderboard). This Grok edition improves discoverability and real-time utility while preserving all original value.

**License & Credits**: MIT (Vercel) + enhancements by Grok optimization workflow. Original: https://github.com/vercel-labs/agent-skills/tree/main/skills/react-best-practices

For updates or contributions, fork and PR to the community version.