# BodyByData Showcase: Project Plan

## Product statement

The BodyByData showcase is a public engineering paper, not a marketing landing
page. Its job is to let a technical reviewer, product leader, recruiter, or
curious user understand what was built, why it was built that way, what failed,
how AI-assisted workflows were controlled, and what evidence supports the final
claims.

The page should demonstrate data science, product management, architecture,
frontend and backend engineering, security thinking, design, and prompt
engineering without explicitly presenting itself as a job-seeking page.

## Reference experience

The visual and editorial reference is the Triad showcase:

<https://github.com/jonathanascona/triad-showcase>

The BodyByData version preserves its core system:

- Source Serif 4 for prose
- JetBrains Mono for labels, numbers, code, and navigation
- Narrow paper-like reading column
- Numbered chronological sections
- Light and dark themes
- Fixed table of contents on large screens
- Real syntax highlighting
- Inline SVG architecture diagrams
- Actual screenshots and artifacts
- Honest callouts where a statement could otherwise mislead
- A closing sources and citations section

## Audiences

### Technical reviewer

Needs architecture boundaries, formulas, code, tests, security evidence, and
specific failure resolutions.

### Product or engineering leader

Needs scope control, sequencing, tradeoffs, iteration, and evidence that the
project continued through production problems.

### Recruiter or hiring manager

Needs a readable narrative that demonstrates cross-functional capability
without requiring a deep repository review.

### Prospective user

Needs a plain explanation of what the demo does, what its numbers mean, and
what it does not claim.

## Content architecture

1. Abstract
2. The Problem
3. Designing the Build
4. System Architecture
5. From Inputs to Signals
6. The Readiness Formula
7. Eight Sprints
8. Problems Encountered
9. Prompt Engineering and Review
10. Privacy and Security
11. The Working Demo
12. Where This Goes Next
13. Skills Exercised
14. Sources and Citations

The order follows the actual build chronology and reasoning. It does not move
the most impressive material to the front at the cost of accuracy.

## Source-of-truth hierarchy

When sources disagree, use this order:

1. Code and tests on application `main`
2. Merged commit and pull request history
3. `docs/STATUS.md`
4. `docs/logs/SECURITY_LOG.md`
5. `docs/logs/CODERABBIT_LOG.md`
6. `docs/logs/PROMPT_LOG.md`
7. `docs/PROJECT_PLAN.md`
8. Memory or conversational recollection

No claim based only on memory is published as fact.

## Core narrative

BodyByData began with a product question: can fragmented health data become one
useful daily decision without hiding the math? The build answered that question
through a strict architecture boundary:

- ingestion normalizes data but performs no scoring
- the intelligence layer performs pure calculations but no upload handling
- every score returns its components, inputs, and confidence
- the interface exposes the reasoning instead of only the result

The project also became an experiment in controlled AI-assisted development.
Large sprint prompts established invariants and acceptance criteria. Small
follow-up prompts corrected actual failures. GitHub Actions and CodeRabbit
provided independent checks. Living logs prevented the final story from being
rewritten into a clean but false retrospective.

## Evidence inventory

Already available:

- complete project plan and sprint prompts
- prompt, security, and CodeRabbit logs
- application commit and PR history
- production screenshots
- readiness, confidence, training-load, coaching, and lifecycle code
- test and audit results from sprint closeouts
- production CORS incident and resolution
- deferred items documented instead of presented as complete

Still requested from the owner:

- original notebook or sketch photographs, if they exist
- early UI mockups predating the React implementation
- a short first-person origin note
- any image showing the real phone, iPad, or laptop planning workflow

Missing artifacts remain labeled as missing. They are never recreated and
presented as originals.

## Delivery phases

### Phase 1: Foundation

- standalone repository
- full page structure and design system
- real application screenshots
- system diagram
- first factual narrative draft
- PM and sprint planning documents

### Phase 2: Evidence enrichment

- owner process artifacts
- verified PR and CodeRabbit counts
- selected code excerpts linked to permanent commit URLs
- citations for outside methodology
- visual comparison against the Triad page

### Phase 3: Editorial and accessibility QA

- fact check every number and causal claim
- keyboard and screen-reader pass
- 320px, 390px, 768px, and desktop visual pass
- contrast check in both themes
- link verification
- typography scan for prohibited dash characters

### Phase 4: Publish

- create `bodybydata-showcase` GitHub repository
- push through a focused pull request if branch protection is enabled
- enable GitHub Pages from `main`
- verify the public URL on desktop and mobile

## Definition of done

- The page is independently deployable from one static repository.
- Every technical claim traces to code, tests, logs, commits, or a cited source.
- The working demo and source repository are linked.
- Failures and deferred work are visible.
- The prompt-engineering section describes controls and iteration, not magic.
- The page names only technologies actually used.
- The site works without JavaScript except theme, chart, highlighting, and TOC
  enhancement.
- All links, themes, breakpoints, and keyboard paths are verified.
- The repository contains zero em dash and zero en dash characters.

