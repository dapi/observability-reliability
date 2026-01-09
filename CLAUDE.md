# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

**ВАЖНО: Всегда отвечайте на русском языке.**

## Repository Overview

This is the Site Reliability Specifications (SRS) repository - a collection of technical specifications that define best practices and standards for building reliable, scalable applications and services. The repository contains no executable code, only markdown documentation.

## Specification Format

- Each specification follows the naming pattern: `SRS-XXX Title.md`
- Specifications support versioning: `SRS-XXX-Y` where Y is the version number
- Status workflow: DRAFT → PROPOSED → APPROVED → DEPRECATED
- Written in Russian and English

## Multilingual Documentation Rules

### File Naming Conventions
- **English specifications**: `SRS-XXX Title.md` (default)
- **Russian specifications**: `SRS-XXX Title.ru.md` (with `.ru.md` extension)
- **English README**: `README.md`
- **Russian README**: `README.ru.md`

### Link Rules
- **README.md (English)** must link to English specifications (`.md` files)
- **README.ru.md (Russian)** must link to Russian specifications (`.ru.md` files)
- Each README should include a language switcher link at the top:
  - English README: `:ru: [Русская версия](README.ru.md)`
  - Russian README: `:gb: [English version](README.md)`

### Creating Bilingual Specifications
1. Create the English version first: `SRS-XXX Title.md`
2. Create the Russian version: `SRS-XXX Title.ru.md`
3. Both files should have the same structure but in respective languages
4. Update both README files with links to the appropriate language version

### Updating Specifications
When updating content:
- Update both language versions to maintain consistency
- Ensure links in both README files point to correct language versions

## Key Specifications

The repository contains 38 specifications covering:
- **Microservices patterns**: Circuit Breaker (SRS-012), Retry mechanisms (SRS-020), Fallback (SRS-022)
- **Observability**: Logging (SRS-008), Error Tracking (SRS-009), Liveness Probes (SRS-010, SRS-021)
- **Reliability**: Graceful Shutdown (SRS-014), Jobs Management (SRS-001), Blocking Timeouts (SRS-015), Idempotency, Rate Limiting
- **Scalability**: Scaling and State (SRS-003), Deadline Propagation (SRS-017)
- **DevOps practices**: Versioning (SRS-005, SRS-007), Environment Variables (SRS-004), Stand-Independent Images (SRS-019)

## Common Tasks

### Creating a New Specification
1. Create a new file following the naming pattern: `SRS-XXX Title.md`
2. Start with status DRAFT
3. Follow the approval process outlined in specs/README.md

### Updating Specifications
- Create a new version by adding version number: `SRS-XXX-Y Title.md`
- Maintain backward compatibility notes in the specification
- Update the Google Sheets tracking document mentioned in specs/README.md

### Reviewing Specifications
- Check for consistency with existing specifications
- Ensure proper status labeling (DRAFT/PROPOSED/APPROVED/DEPRECATED)
- Verify links between related specifications are correct

## Important Notes

- This is a documentation-only repository - no build or test commands needed
- Specifications are primarily in Russian with some English content
- All specifications should reference related specifications when applicable
- The Google Sheets document mentioned in specs/README.md tracks implementation across services