# Vault Directory Semantics

This document defines the **semantic purpose** of each top-level directory in this vault.  
It is normative: structure changes should be reflected here.

The vault is designed for **long-term intellectual work**, with gradual convergence from raw notes toward coherent, publishable material.

---
## Design principles

1. **Local-first, text-first**
   - Markdown files are the canonical source of truth.
1. **Separation of concerns**
   - Thinking, structuring, arguing, and publishing are distinct activities.
3. **Refactorability**
   - Files may move or be renamed; meaning is preserved through links.
4. **Longevity**
   - The structure should remain viable for 5–10+ years.
5. **Book-readiness**
   - Long-form output should emerge naturally from the system.
---
## Directory overview

00-meta/ System rules and documentation
01-notes/ Raw, exploratory notes
02-concepts/ Stabilized concepts and definitions
03-arguments/ Explicit claims and reasoning
04-structures/ Maps, outlines, and frameworks
05-drafts/ Long-form working texts
06-public/ Publication-ready material
07-references/ Source notes and bibliographic material
08-data/ Small datasets
09-code/ Scripts and reusable code
10-notebooks/ Executable notebooks
assets/ Images and other binary media

---
## Directory semantics

### 00-meta/  system rules and documentation
**Purpose:**  
Documentation *about the vault itself*.

Contains:
- structural rules
- naming conventions
- lifecycle definitions
- tagging and status semantics
- export and migration strategy

This folder is small but authoritative.

Examples:
- `linking-rules.md`
- `note-lifecycle.md`
- `tags-and-statuses.md`
- `export-strategy.md`
---
### 01-notes/  raw, exploratory notes

**Purpose:**  
Capture ideas quickly and without premature formalization.

Characteristics:
- provisional
- exploratory
- may contain contradictions
- may later be split, merged, or promoted

**Recommended naming:** `YYYYMMDD-short-slug.md`

These notes form an **intellectual lab notebook**.

---
### 02-concepts/  stabilized concepts and definitions

**Purpose:**  
Canonical definitions of concepts used throughout the vault.

Rules:
- one concept per file
- careful, neutral language
- changes are deliberate

Concept notes should be link targets for arguments and drafts.

---
### 03-arguments/  explicit claims and reasoning

**Purpose:**  
Make reasoning explicit and inspectable.

Typically includes:
- a claim
- premises
- reasoning
- objections
- open questions

Arguments may reference multiple concepts.

---
### 04-structures/  maps, outlines, and frameworks

**Purpose:**  
Represent structure *about* the content.

Includes:
- outlines
- conceptual maps
- taxonomies
- dependency graphs
- candidate book structures

These notes often change and guide refactoring.

---
### 05-drafts/  long-form working texts

**Purpose:**  
Narrative writing aiming at coherence and readability.

Characteristics:
- prose-oriented
- integrates concepts and arguments
- may later be split into chapters or essays

Drafts are not yet considered stable.

---
### 06-public/  publication-ready material

**Purpose:**  
Curated, stable output intended for readers.

Rules:
- minimal TODOs
- stable structure
- suitable for static publication

Only this folder is assumed to be publicly exposed by default.

---
### 07-references/  source notes and bibliographic material

**Purpose:**  
Track external intellectual inputs.

Contains:
- bibliographic notes
- summaries
- quotations
- links to external reference managers

Avoid duplicating large source files; prefer links.

---
### 08-data/  small datasets

**Purpose:**  
Store empirical or illustrative data used in notes or notebooks.

Examples:
- CSV
- JSON
- small structured datasets

Always referenced from other notes.

---
### 09-code/  scripts and reusable code

**Purpose:**  
Non-interactive code artifacts.

Examples:
- scripts
- libraries
- helpers
- proof sketches

Code should be documented and stable.

---
### 10-notebooks/  executable notebooks

**Purpose:**  
Interactive computation, simulation, or proof exploration.

Rules:
- one notebook per question
- markdown cells explain intent and interpretation

This directory may remain empty until needed.

---
### assets/  images and other binary media

**Purpose:**  
Centralized storage for non-text artifacts.

Typical subfolders:
- `diagrams/`
- `figures/`
- `scans/`

Assets should be referenced, not orphaned.

---
## Note lifecycle (informal)

An idea may evolve through these stages:
`01-notes → 02-concepts → 03-arguments → 05-drafts → 06-public`

Most notes will not traverse all stages—and should not.

---
## Final note

This structure is a **tool for thinking**, not a constraint.  
Deviations are allowed, but should be intentional and documented here.