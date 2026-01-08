# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

**ВАЖНО: Всегда отвечайте на русском языке.**

## Repository Overview

This is the SafeBlock Specifications (SFS) repository - a collection of technical specifications that define best practices and standards for building reliable, scalable applications and services. The repository contains no executable code, only markdown documentation.

## Specification Format

- Each specification follows the naming pattern: `SFS-XXX Title.md`
- Specifications support versioning: `SFS-XXX-Y` where Y is the version number
- Status workflow: DRAFT → PROPOSED → APPROVED → DEPRECATED
- Written in Russian and English

## Key Specifications

The repository contains 17 specifications covering:
- **Microservices patterns**: Circuit Breaker (SFS-012), Retry mechanisms (SFS-020), Fallback (SFS-022)
- **Observability**: Logging (SFS-008), Error Tracking (SFS-009), Liveness Probes (SFS-010, SFS-021)
- **Reliability**: Graceful Shutdown (SFS-014), Jobs Management (SFS-001), Blocking Timeouts (SFS-015)
- **Scalability**: Scaling and State (SFS-003), Deadline Propagation (SFS-017)
- **DevOps practices**: Versioning (SFS-005, SFS-007), Environment Variables (SFS-004), Stand-Independent Images (SFS-019)

## Common Tasks

### Creating a New Specification
1. Create a new file following the naming pattern: `SFS-XXX Title.md`
2. Start with status DRAFT
3. Follow the approval process outlined in specs/README.md

### Updating Specifications
- Create a new version by adding version number: `SFS-XXX-Y Title.md`
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