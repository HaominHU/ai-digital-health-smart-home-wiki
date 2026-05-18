---
title: Research Wiki Memory
type: memory
status: draft
privacy: private
last_updated: 2026-05-18
---

# Research Wiki Memory

## Current State

This repo has been initialized as a private Karpathy-style LLM Wiki for AI-driven digital health and smart home technologies in caregiving, chronic conditions, disability, and aging.

The repo is intentionally Markdown-first and Obsidian-compatible. No database, embedding system, or custom retrieval tooling has been added.

## Core Purpose

The wiki should support:

- General knowledge answers grounded in accumulated research context.
- Evidence-aware research writing.
- System design reasoning.
- AI-ready prompts for research, writing, coding, design, or specification work.
- Knowledge support for agent reasoning.

The wiki must not act as a clinical decision-maker, diagnostic system, treatment recommender, or substitute for professional medical, ethical, privacy, security, or IRB review.

## Architecture Decisions

- Raw sources live under `sources/` and are treated as immutable.
- Maintained wiki pages live under `wiki/`.
- Generated previews, briefs, prompts, and reports live under `outputs/`.
- Sensitive scratch notes live under `private_notes/`.
- `AGENTS.md` governs agent behavior.
- `INDEX.md` is the content-oriented map.
- `LOG.md` is the chronological timeline.
- `MEMORY.md` is the compressed current-state digest.

## Domain Model

- Conditions are overlays.
- Caregiving challenges are reusable hubs.
- Care recipient needs are tracked separately from caregiver needs.
- Technologies are reusable intervention lenses.
- Aging-related functional decline and age-associated disease development must be distinguished.
- Evidence, interpretation, personal insight, and speculative design direction must remain separate.

## Privacy and Security Baseline

The repo is private by default, but identifiable or sensitive healthcare/study data should not be stored unless the user explicitly provides a safe handling policy.

Default behavior:

- Avoid PHI and identifiable participant information.
- De-identify before wiki integration.
- Mark sensitive source material clearly.
- Include privacy, security, consent, ethics, data minimization, and human oversight considerations in healthcare-related prompts and specs.

## Source Storage and Git Baseline

The user manually handles commits and git management.

Raw source files may be stored locally under `sources/`, but they are ignored by git by default. The tracked wiki should preserve source-derived knowledge through source IDs, source context, evidence labels, and durable Markdown synthesis.

Recommended raw source ID and filename pattern:

`YYYY-MM-DD_author-or-org_short-title.ext`

Periodic lint checks should flag locally stored raw sources that may be removable after their contents have been well digested into the wiki. Do not delete raw sources automatically.

## Next Useful Step

Ingest the first real source or note using `wiki/commands/ingest_source.md` or `wiki/commands/quick_note.md`.
