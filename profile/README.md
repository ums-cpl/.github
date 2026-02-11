# UMS-CPL: University of Muenster – Compilers & Programming Languages

This GitHub organization hosts research, teaching, and administrative artifacts in the area of **Compilers & Programming Languages (CPL)** developed at the University of Münster.

The organization follows a **flat repository structure** with **strict naming conventions** and a **controlled GitHub topic vocabulary**.

There is intentionally **no hierarchy via folders**. Structure is expressed **exclusively via repository names and topics**.


## 1. Repository Naming Conventions & Required Topics

| Category    | Repository Naming Convention                  | Example                              | Required Topics                                                     |
|-------------|-----------------------------------------------|--------------------------------------|---------------------------------------------------------------------|
| `paper`     | `paper-<venue><year>-<slug>`                  | `paper-cgo26-mdh-schedules`          | `paper`, `<venue>`, `<year>`, `<research-area>`                     |
| `benchmark` | `benchmark-<venue><year>-<slug>`              | `benchmark-cgo26-mdh-schedules`      | `benchmark`, `<venue>`, `<year>`, `<research-area>`                 |
| `artifact`  | `artifact-<venue><year>-<slug>`               | `artifact-cgo26-mdh-schedules`       | `artifact`, `<venue>`, `<year>`, `<research-area>`                  |
| `talk`      | `talk-<event><year>-<slug>`                   | `talk-cgo26-mdh-overview`            | `talk`, `<event>`, `<year>`, `<research-area>`                      |
| `poster`    | `poster-<event><year>-<slug>`                 | `poster-cgo26-src-jane-doe`          | `poster`, `<event>`, `<year>`, `<research-area>`                    |
| `proposal`  | `proposal-<funding-org><year>-<slug>`         | `proposal-dfg25-ai-codegen`          | `proposal`, `<funding-org>`, `<year>`, `<research-area>`            |
| `grant`     | `grant-<year>-<slug>`                         | `grant-26-sc-ecp`                    | `grant`, `<year>`, `<research-area>`                                |
| `topic`     | `topic-<slug>`                                | `topic-tensor-core-eval`             | `topic`, `<research-area>`                                          |
| `teaching`  | `teaching-<course>-<semester>-<slug>`         | `teaching-pjs-ss26-ai-codegen`       | `teaching`, `<course>`, `<semester>`, `<research-area>`             |
| `teaching`  | `teaching-<thesis>-<year>-<name>`             | `teaching-ba-26-jane-doe`            | `teaching`, `<thesis>`, `<year>`, `<research-area>`                 |
| `protocol`  | `protocol-<date>-<slug>`                      | `protocol-2026-12-01-tensor-cores`   | `protocol`, `<date>`, `<research-area>`                             |
| `cv`        | `cv-<name>`                                   | `cv-jane-doe`                        | `cv`                                                                |
| `bio`       | `bio-<name>`                                  | `bio-jane-doe`                       | `bio`                                                               |
| `travel`    | `travel-<year>-<destination>-<slug>`          | `travel-26-sydney-cgo`               | `travel`, `<year>`, `<destination>`                                 |
| `misc`      | `misc-<slug>`                                 | `misc-headshots`                     | optional                                                            |


## 2. **Global Naming Rules**

All identifiers used within this organization — including repository names, topics, slugs, and other naming elements — follow a single, consistent convention:

- Use **lowercase characters only**
- Keep identifiers **short, descriptive, and stable**
- Use **hyphen-separated** words
- Do **not** use spaces or underscores

These rules apply uniformly across the entire organization and are intended to ensure consistency, longevity, and machine-friendliness.  
This scheme is intentionally designed to be machine-readable and suitable for automation, indexing, and long-term archival.

Topics are **mandatory** and serve as the **only hierarchical mechanism**.

---

### Categories

```
paper | benchmark | artifact | talk | poster | proposal | grant | topic | teaching | protocol | cv | travel | misc
```

### `<venue>`

Conference and journal acronyms.

Examples:
```
pldi, cgo, toplas, taco
```

### `<event>`

Event code (including conference and journal acronyms)

Examples:
```
pldi, cgo, toplas, taco, mlir-developer-meeting
```

### `<funding-org>`:

Funding organization acronym.

Examples:
```
dfg, bmbf, nsf
```

### `<course>`

Course acronym.

Examples:
```
pjs, sem, mgpp, ps
```

### `<semester>`

Semester acronym `ssYY` or `wsYY`, where `YY` denotes the year.

Examples:
```
ss25, ws26
```

### `<thesis>`

Thesis type.

Examples:
```
ba, ma, diss
```

### `<name>`

First and last name.

Examples:
```
jane-doe, john-doe
```


### `<year>` 

Two digits (YY).

Examples: 
```
24, 25, 26
```

### `<date>` 

ISO 8601 format (YYYY-MM-DD).

Examples: 
```
2024-01-15, 2025-06-30, 2026-12-01
```

### `<destination>`

Lowercase, hyphen-separated full city names. Avoid abbreviations unless they are globally unambiguous.

Examples:
```
berlin, washington-dc, new-york, san-francisco, hong-kong
```

### `<slug>`

Short, human-readable identifier describing the **specific content or focus** of the repository.

Examples:
```
mdh-schedules, ai-codegen
```

### `<research-area>`

One or more research areas describing the technical focus of the repository.

Allowed values:
`code-generation | code-optimization | code-execution`

Rules:
- One or more values MAY be used
- Prefer the minimal sufficient set
- If none of the above apply, contact the organization administrators before creating the repository


## 3. Topic Rules (Strict)

- Follow the Global Naming Rules
- No free-form invention of topics
- Prefer **short, stable identifiers**
- Topics must remain meaningful over **5+ years**


## 4. Privacy Rules

Repositories are private by default.  
Public visibility requires an explicit justification (e.g., published artifact, teaching material, or public benchmark).


## 5. The `.github` Repository

The `.github` repository contains organization-wide defaults:

- Organization README (this document)
- Issue templates
- Pull request templates
- Contribution guidelines (if applicable)


## 6. Philosophy

This structure is designed to:

- Scale over long academic careers
- Survive personnel turnover
- Be understandable to reviewers, students, and funding agencies
- Avoid implicit knowledge and ad-hoc naming

**If a repository does not fit the scheme, the scheme is wrong – not the repository.**


## 7. Repository Hygiene (General)

All repositories are expected to be **clean, intentional, and self-contained**.  
They represent **long-lived research records** and must remain understandable without implicit context.

**Examples of expected practice include:**

- **Paper repositories (`paper-*`)**
  - clean, incremental commits
  - explicit **Git tags** for submitted and accepted versions (including reviews)
  - the **current compiled PDF** is always committed to the repository
  - sources and rendered output are kept **consistent**

These examples are **illustrative, not exhaustive**.  
The general rule applies to all categories: **a repository is a record, not a scratch space**.


## 8. Meeting Log Template

Structured supervision and project meetings follow a standardized Markdown template to ensure consistency, traceability, and long-term archival quality.

The official meeting log template is maintained in:

https://github.com/ums-cpl/misc-meeting-log-template/blob/main/meeting-log-template.md

All supervision-related repositories (e.g., `paper-*`, `teaching-*`) are expected to use this template unless a justified deviation is documented.
