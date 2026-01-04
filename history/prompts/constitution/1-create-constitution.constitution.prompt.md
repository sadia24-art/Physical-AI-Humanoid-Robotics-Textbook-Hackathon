---
id: 1
title: "Create Constitution"
stage: "constitution"
date_iso: "2026-01-04"
surface: "agent"
model: "claude-sonnet-4-5-20250929"
feature: "none"
branch: "master"
user: "user"
command: "/sp.constitution"
labels: ["constitution", "spec-driven", "ai-book"]
spec: null
ticket: null
adr: null
pr: null
files_yaml: |
  - .specify/memory/constitution.md
tests_yaml: |
  - none
prompt_text: |
  /sp.constitution

  Project: AI-Spec-Driven Book with Integrated RAG Chatbot

  Purpose:
  Define the mandatory constitutional rules governing the end-to-end creation of a unified technical book and its embedded RAG chatbot using Spec-Kit Plus and Claude Code.

  =================================================================

  CORE PRINCIPLES

  1. Spec-Driven Development (Mandatory)
  - No code, content, or infrastructure may be created without an approved specification.
  - All work must strictly follow the order:
    Constitution → Specs → Plan → Tasks → Implementation
  - Specs are the single source of truth.

  2. AI-Native Authorship
  - All book content, specs, plans, tasks, and code must be produced via Claude Code or AI agents.
  - Humans may review, approve, or reject outputs but may not manually write implementation artifacts.

  3. Accuracy & Verifiability
  - All technical claims must be correct, reproducible, and verifiable.
  - No speculative or unverifiable statements are allowed.

  4. Modularity & Traceability
  - Every chapter, feature, API, and chatbot capability must map to:
    - A spec section
    - A task ID
  - No orphan content or code is permitted.

  =================================================================

  BOOK STANDARDS

  - Platform: Docusaurus
  - Deployment: GitHub Pages
  - Structure:
    - Modular chapters
    - Clear navigation
    - Version-controlled documentation
  - Writing Style:
    - Clear, concise, technical
    - Target audience: software engineers & AI practitioners
  - Content Rules:
    - No placeholder text
    - No undocumented assumptions
    - All examples must be runnable or logically complete

  =================================================================

  RAG CHATBOT STANDARDS

  - Architecture:
    - OpenAI Agents / ChatKit SDKs
    - FastAPI backend
    - Neon Serverless Postgres (metadata + conversations)
    - Qdrant Cloud (Free Tier) for vector search
  - Capabilities (Mandatory):
    - Answer questions about the full book content
    - Answer questions based only on user-selected text
    - Cite retrieved sections in responses
  - Constraints:
    - No hallucinated answers
    - If context is missing, the bot must say so explicitly
  - Embedding:
    - Chatbot must be embedded directly within the Docusaurus site

  =================================================================

  INFRASTRUCTURE & CODE RULES

  - Backend:
    - FastAPI only
    - Clean, typed, modular Python code
  - Data:
    - Explicit schemas for embeddings, documents, and chats
  - Security:
    - No hardcoded secrets
    - Environment-based configuration only
  - Testing:
    - Core logic must be testable
    - No untested critical paths

  =================================================================

  PROHIBITIONS

  - No manual coding by humans
  - No implementation before approved specs
  - No undocumented features
  - No copy-pasted content from external sources
  - No hallucinated APIs, SDKs, or services

  =================================================================

  SUCCESS CRITERIA

  The project is considered complete only if:

  - The book is live on GitHub Pages
  - All content follows approved specs
  - The RAG chatbot:
    - Correctly retrieves and answers from book content
    - Correctly limits answers to selected text when required
  - Every artifact is traceable to a spec and task
  - No constitutional rule violations exist

  =================================================================

  ENFORCEMENT

  Any violation of this constitution invalidates the affected work
  and requires rollback to the last compliant state.
response_text: |
  Created the project constitution file .specify/memory/constitution.md with all the specified principles and requirements. The constitution includes:
  - Core Principles: Spec-Driven Development, AI-Native Authorship, Accuracy & Verifiability, Modularity & Traceability
  - Book Standards: Docusaurus platform, GitHub Pages deployment, modular structure
  - RAG Chatbot Standards: Architecture with OpenAI Agents, FastAPI, Neon Postgres, Qdrant Cloud
  - Infrastructure & Code Rules: FastAPI backend, clean code, security requirements
  - Prohibitions: No manual coding, implementation before specs, undocumented features
  - Success Criteria: Book live on GitHub Pages, RAG chatbot functionality, traceability
  - Enforcement: Violations require rollback to compliant state
outcome: |
  Constitution file created successfully at .specify/memory/constitution.md with version 1.0.0, ratification date 2026-01-04.
evaluation: |
  The constitution file has been created with all required principles and standards. All placeholder tokens have been replaced with the specific requirements provided by the user. The file follows the required structure and includes governance information.
---

# Create Constitution

## Summary
Created the project constitution for the AI-Spec-Driven Book with Integrated RAG Chatbot project with all specified principles and requirements.

## Details
The constitution file (.specify/memory/constitution.md) has been created with the following key sections:
- Core Principles including Spec-Driven Development, AI-Native Authorship, Accuracy & Verifiability, and Modularity & Traceability
- Book Standards specifying Docusaurus platform and GitHub Pages deployment
- RAG Chatbot Standards with architecture details using OpenAI Agents, FastAPI, and Qdrant Cloud
- Infrastructure & Code Rules for backend development
- Prohibitions against manual coding and implementation before specs
- Success Criteria for project completion
- Enforcement mechanisms for constitutional compliance

## Next Steps
- Proceed with creating specifications based on this constitution
- Ensure all future work follows the constitutional principles
- Create plan and tasks following the Spec-Driven Development workflow