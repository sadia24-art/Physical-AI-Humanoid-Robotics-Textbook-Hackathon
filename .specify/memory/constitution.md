<!-- SYNC IMPACT REPORT:
Version change: N/A (initial creation) → 1.0.0
Modified principles: N/A
Added sections: All principles and sections based on user requirements
Removed sections: N/A
Templates requiring updates:
- .specify/templates/plan-template.md ✅ updated
- .specify/templates/spec-template.md ✅ updated
- .specify/templates/tasks-template.md ✅ updated
- .specify/templates/commands/*.md ⚠ pending review
Follow-up TODOs: None
-->
# AI-Spec-Driven Book with Integrated RAG Chatbot Constitution

## Core Principles

### I. Spec-Driven Development (Mandatory)
No code, content, or infrastructure may be created without an approved specification. All work must strictly follow the order: Constitution → Specs → Plan → Tasks → Implementation. Specs are the single source of truth.

### II. AI-Native Authorship
All book content, specs, plans, tasks, and code must be produced via Claude Code or AI agents. Humans may review, approve, or reject outputs but may not manually write implementation artifacts.

### III. Accuracy & Verifiability
All technical claims must be correct, reproducible, and verifiable. No speculative or unverifiable statements are allowed.

### IV. Modularity & Traceability
Every chapter, feature, API, and chatbot capability must map to a spec section and a task ID. No orphan content or code is permitted.

## Book Standards

Platform: Docusaurus
Deployment: GitHub Pages
Structure: Modular chapters, clear navigation, version-controlled documentation
Writing Style: Clear, concise, technical targeting software engineers & AI practitioners
Content Rules: No placeholder text, no undocumented assumptions, all examples must be runnable or logically complete

## RAG Chatbot Standards

Architecture: OpenAI Agents / ChatKit SDKs, FastAPI backend, Neon Serverless Postgres (metadata + conversations), Qdrant Cloud (Free Tier) for vector search
Capabilities (Mandatory): Answer questions about the full book content, answer questions based only on user-selected text, cite retrieved sections in responses
Constraints: No hallucinated answers, if context is missing, the bot must say so explicitly
Embedding: Chatbot must be embedded directly within the Docusaurus site

## Infrastructure & Code Rules

Backend: FastAPI only, clean, typed, modular Python code
Data: Explicit schemas for embeddings, documents, and chats
Security: No hardcoded secrets, environment-based configuration only
Testing: Core logic must be testable, no untested critical paths

## Prohibitions

No manual coding by humans
No implementation before approved specs
No undocumented features
No copy-pasted content from external sources
No hallucinated APIs, SDKs, or services

## Success Criteria

The project is considered complete only if:

- The book is live on GitHub Pages
- All content follows approved specs
- The RAG chatbot correctly retrieves and answers from book content and correctly limits answers to selected text when required
- Every artifact is traceable to a spec and task
- No constitutional rule violations exist

## Enforcement

Any violation of this constitution invalidates the affected work and requires rollback to the last compliant state.

## Governance

This constitution supersedes all other practices. All implementation work must strictly follow these principles. Amendments require explicit documentation, approval process, and migration plan for existing artifacts. All development must verify compliance with these rules. Any work that violates these principles must be rolled back to the last compliant state.

**Version**: 1.0.0 | **Ratified**: 2026-01-04 | **Last Amended**: 2026-01-04