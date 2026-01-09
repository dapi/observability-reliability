# Contributing to Site Reliability Specifications

Thank you for your interest in contributing to the Site Reliability Specifications! This document provides guidelines and processes for contributing to the project.

---

## Table of Contents

1. [Code of Conduct](#code-of-conduct)
2. [Language Strategy](#language-strategy)
3. [How to Contribute](#how-to-contribute)
4. [Specification Format](#specification-format)
5. [Creating a New Specification](#creating-a-new-specification)
6. [Review Process](#review-process)
7. [Standards and Conventions](#standards-and-conventions)
8. [Templates](#templates)
9. [Questions?](#questions)

---

## Code of Conduct

- Be respectful and constructive
- Focus on technical excellence
- Share knowledge generously
- Welcome newcomers and help them get started

---

## Language Strategy

### Repository Language Structure

This repository maintains **bilingual documentation** to serve both Russian-speaking and international teams:

1. **Specifications** (`specs/` directory):
   - `specs/SRS-XXX Title.md` → English version
   - `specs/SRS-XXX Title.ru.md` → Russian version
   - Always create both versions for new specifications

2. **README.md**:
   - Currently in **Russian** (main project description)
   - Project started for Russian-speaking team
   - Contains links to both English and Russian specification versions

3. **CONTRIBUTING.md** (this file):
   - In English (following open-source best practices)
   - Makes project accessible to international contributors

### When Contributing

- **New specifications**: Create both `.md` (English) and `.ru.md` (Russian) versions
- **Updates to specifications**: Update both language versions
- **Issues and discussions**: Can be in Russian or English
- **Pull requests**: Can be in Russian or English

---

## How to Contribute

### 1. Reporting Issues

Found a typo, error, or have an idea for improvement?

- Check existing [issues](https://github.com/dapi/observability-reliability/issues) first
- Create a new issue with clear title and description
- Label appropriately: `bug`, `enhancement`, `question`

### 2. Suggesting New Specifications

Have an idea for a new specification?

- Open an issue with label `new-specification`
- Use the template: "Proposal: SRS-XXX Title"
- Describe the problem it solves
- Provide examples or references
- Wait for discussion and approval before creating the spec

### 3. Contributing Changes

**Small changes** (typos, minor improvements):
- Fork the repository
- Make changes
- Submit pull request

**Major changes** (new specifications, significant updates):
- Fork the repository
- Create an issue first for discussion
- Create a feature branch: `git checkout -b feature/new-spec-srs-XXX`
- Make changes following [Specification Format](#specification-format)
- Update both English and Russian versions
- Submit pull request with detailed description

---

## Specification Format

Every specification must follow this structure:

```markdown
# SRS-XXX Title (English)

Brief one-paragraph description of what this specification covers.

---

## What is [Concept]?

Clear explanation with:
- Definition
- Why it's important
- When to use it

---

## Anti-Patterns ❌

### ❌ Anti-Pattern Name
```
example of what NOT to do
```
**Why it's bad:** Explanation of risks

---

## Best Practices ✅

### 1. Practice Name
Detailed explanation with:
- Code examples (multiple languages if applicable)
- Configuration examples
- Real-world scenarios

---

## Common Implementations

### Language 1 (e.g., Python)
```python
# Code example
```

### Language 2 (e.g., Go)
```go
// Code example
```

---

## Metrics to Track

```python
SPECIFICATION_METRICS = {
    'metric_name': 'Description of what to measure'
}
```

---

## Tools and Platforms

| Tool | Use Case | Complexity | Cost |
|------|----------|------------|------|
| Tool Name | What it's for | Low/Medium/High | Free/$$/$$$ |

---

*Specification Name - brief tagline*
```

### Mandatory Sections

1. **Title and description** - Clear and concise
2. **What is...** section - Definition and importance
3. **Anti-Patterns** - Common mistakes to avoid (minimum 3)
4. **Best Practices** - Concrete recommendations (minimum 5)
5. **Examples** - Code/config examples (minimum 2 languages/tools)
6. **Metrics** - What to measure
7. **Tools** - Available solutions

### Optional Sections

- Architecture diagrams
- Decision trees
- Cost analysis
- Migration strategies
- Case studies

---

## Creating a New Specification

Follow these steps to create a new specification:

### Step 1: Proposal (GitHub Issue)

Create an issue using this template:

```markdown
Title: [Proposal] SRS-XXX Specification Title

## Summary
Brief description of the problem this specification solves.

## Use Cases
1. When would someone use this?
2. What problems does it address?

## Prior Art
- Links to existing specifications that relate to this
- Industry standards or frameworks that cover this

## Scope
What this specification WILL cover and what it WON'T cover.

## Success Criteria
How will we know this specification is complete and useful?

## Examples
Any existing implementations or references to include?
```

### Step 2: Research and Outline

Before writing:
- Study existing related specifications
- Research industry best practices
- Collect real-world examples
- Create outline following the format

### Step 3: Write English Version

Create `specs/SRS-XXX Title.md`:

```markdown
# SRS-XXX Title

Brief description...

---

## What is Title?

## Anti-Patterns ❌

### ❌ Anti-Pattern 1

---

## Best Practices ✅

### 1. Best Practice 1

---

## Examples

### Python Example

```python
# Code here
```

### Go Example

```go
// Code here
```

---

## Metrics

---

## Tools

---

*Specification Title - tagline*
```

### Step 4: Write Russian Version

Create `specs/SRS-XXX Title.ru.md`:

- Translate the entire specification
- Keep all code examples the same (only translate comments)
- Maintain the same structure and formatting
- Ensure technical accuracy in Russian terminology

**Tip**: Use professional Russian SRE/DevOps terminology.

### Step 5: Update README

Add the specification to the README.md table:

```markdown
| [SRS-XXX Title](specs/SRS-XXX%20Title.md) | P2 | Medium | Описание сложности |
```

### Step 6: Review and Submit

- Review both versions for consistency
- Check all links work
- Make sure all code examples are correct
- Submit pull request

---

## Review Process

### Before Submitting

- [ ] Both language versions created (.md and .ru.md)
- [ ] All mandatory sections included
- [ ] At least 3 anti-patterns documented
- [ ] At least 5 best practices documented
- [ ] At least 2 code examples from different languages/tools
- [ ] Metrics section completed
- [ ] Tools section completed
- [ ] README.md updated
- [ ] Links checked and working
- [ ] Code examples verified (syntax check if possible)

### Pull Request Checklist

Use this checklist in your PR description:

```markdown
## Checklist

- [ ] English version created (`SRS-XXX Title.md`)
- [ ] Russian version created (`SRS-XXX Title.ru.md`)
- [ ] All mandatory sections present
- [ ] At least 3 anti-patterns documented
- [ ] At least 5 best practices with examples
- [ ] Code examples from multiple languages/tools
- [ ] Metrics section completed
- [ ] Tools/platforms section completed
- [ ] README.md updated with new specification
- [ ] Links verified
- [ ] Technical terminology consistent with existing specs

## Reviewers

- [ ] Technical accuracy review
- [ ] Russian language review
- [ ] English language review
- [ ] Consistency check with existing specs
```

### Review Timeline

- **Acknowledgment**: Within 2 business days
- **Initial review**: Within 1 week
- **Approval**: Within 2 weeks (may require iterations)

---

## Standards and Conventions

### File Naming

- Pattern: `SRS-XXX Title.md`
- Use English titles even for Russian versions
- Replace spaces with `%20` in links
- Example: `SRS-032 SLI SLO SLA.md`

### Formatting

- Use markdown headings (`#`, `##`, `###`)
- Keep line length under 100 characters where possible
- Use code blocks with language identifiers:
  ```python
  # Python code
  ```
  ```go
  // Go code
  ```
  ```yaml
  # YAML config
  ```

- Use **bold** for key terms
- Use `inline code` for commands, file names, technical terms

### Diagrams

Use ASCII diagrams or mermaid syntax:

```
ASCII example:
┌─────────────┐
│  Component  │
└──────┬──────┘
       │
       ▼
┌─────────────┐
│  Service    │
└─────────────┘
```

### Code Examples

- Provide examples in at least 2 different languages or tools
- Include comments explaining the code
- Keep examples minimal but complete
- Use popular, well-maintained tools/frameworks

### Technical Terminology

Follow these conventions:

- **English**: Use standard SRE/DevOps terminology
- **Russian**: Use established Russian technical terms

Examples:
- Circuit breaker → Прерыватель цепи
- Graceful shutdown → Корректная остановка
- Idempotency → Идемпотентность
- Deadline propagation → Распространение дедлайнов

---

## Templates

### New Specification Template

Use this as your starting point:

**File: `specs/SRS-XXX Title.md`**

```markdown
# SRS-XXX Title

Brief one-paragraph description of what this specification covers and why it's important.

---

## What is [Concept]?

Clear definition in 2-3 paragraphs.

- What problem does it solve?
- When should you use it?
- What are the benefits?

---

## Anti-Patterns ❌

### ❌ Anti-Pattern 1: Bad Practice Name
```
Show what NOT to do with concrete example
```
**Why it's bad:** Explain the risks and consequences.

**Impact:** What can go wrong?

---

### ❌ Anti-Pattern 2: Another Bad Practice
```
Another example of what to avoid
```
**Why it's bad:** Clear explanation.

---

### ❌ Anti-Pattern 3: Yet Another Mistake
```
Third example of anti-pattern
```
**Why it's bad:** Impact on reliability/performance.

---

## Best Practices ✅

### 1. Best Practice Name
Detailed explanation of this practice.

**When to use:** Specific scenarios.

**Benefits:** What you gain.

#### Example Implementation

**Python:**
```python
# Python implementation
```

**Go:**
```go
// Go implementation
```

---

### 2. Another Best Practice
Explanation.

**Implementation details:**
- Detail 1
- Detail 2

#### Configuration Example
```yaml
# YAML configuration
```

---

### 3. Third Best Practice
Explanation.

**Monitoring:** What to watch for.

---

### 4. Fourth Best Practice
Explanation.

**Testing:** How to verify.

---

### 5. Fifth Best Practice
Explanation.

**Scaling considerations:**

---

## Implementation Examples

### Example 1: Scenario Name
```python
# Complete example for specific use case
```

### Example 2: Another Scenario
```yaml
# Configuration example
```

---

## Metrics to Track

```python
SPECIFICATION_METRICS = {
    'metric_1_name': 'Description of what to measure and why',
    'metric_2_name': 'Another important metric',
    'metric_3_name': 'Third key metric',
}
```

**Dashboard panels:**
- Panel 1: What it shows
- Panel 2: What it shows
- Panel 3: What it shows

---

## Tools and Platforms

| Tool/Platform | Use Case | Complexity | Cost | Notes |
|---------------|----------|------------|------|-------|
| Tool Name 1 | When to use it | Low/Medium/High | Free/Paid | Key features |
| Tool Name 2 | Different use case | Low/Medium/High | Free/Paid | Key features |
| Tool Name 3 | Another scenario | Low/Medium/High | Free/Paid | Key features |

**Recommendation:** Which tool to choose for which scenario.

---

## Additional Resources

- [Link to related specification](SRS-YYY Related Spec.md)
- [Link to another related spec](SRS-ZZZ Another Spec.md)
- External resource: [Name](https://example.com)

---

*[Specification Title] - brief tagline explaining core value*
```

### Issue Templates

#### Bug Report Template

```markdown
**Title:** [BUG] Brief description

**Affected Specification:** SRS-XXX Title

**Description:**
Clear description of the bug or error.

**Expected Behavior:**
What should happen.

**Actual Behavior:**
What actually happens.

**Suggested Fix:**
Your recommendations for fixing it.
```

#### Enhancement Template

```markdown
**Title:** [ENHANCEMENT] Brief description

**Affected Specification:** SRS-XXX Title

**Current State:**
What's missing or could be improved.

**Proposed Enhancement:**
What you suggest adding.

**Benefits:**
Why this enhancement would be valuable.

**Implementation Ideas:**
How this could be implemented.
```

---

## Questions?

If you have questions about contributing:

1. Check existing [GitHub Issues](https://github.com/dapi/observability-reliability/issues)
2. Open a new issue with label `question`
3. Or contact the maintainers

---

## Recognition

Contributors will be recognized in:
- GitHub contributors list
- Specification changelog (future)
- Project acknowledgments (future)

---

## License

By contributing, you agree that your contributions will be licensed under the project's license.

---

**Thank you for contributing to Site Reliability Specifications!**
