# UMS-CPL: University of Muenster – Compilers & Programming Languages

This GitHub organization hosts research, teaching, and administrative artifacts in the area of **Compilers & Programming Languages (CPL)** developed at the University of Münster.

The organization follows a **flat repository structure** with **strict naming conventions** and a **controlled GitHub topic vocabulary**.

There is intentionally **no hierarchy via folders**. Structure is expressed **exclusively via repository names and topics**.

---

## 1. Repository Naming Conventions & Required Topics


| Category    | Repository Naming Convention              | Required Topics                                                   | Example                              |
|-------------|-------------------------------------------|-------------------------------------------------------------------|--------------------------------------|
| `paper`     | `paper-<venue><year>-<slug>`              | `paper`, `<venue>`, `<year>`, `<mdh/atf/hca>`                     | `paper-cgo26-mdh-schedules`          |
| `benchmark` | `benchmark-<venue><year>-<slug>`          | `benchmark`, `<venue>`, `<year>`, `<mdh/atf/hca>`                 | `benchmark-cgo26-mdh-schedules`      |
| `artifact`  | `artifact-<venue><year>-<slug>`           | `artifact`, `<venue>`, `<year>`, `<mdh/atf/hca>`                  | `artifact-cgo26-mdh-schedules`       |
| `talk`      | `talk-<event><year>-<slug>`               | `talk`, `<event>`, `<year>`, `<mdh/atf/hca>`                      | `talk-cgo26-mdh-overview`            |
| `proposal`  | `proposal-<funding-org><year>-<slug>`     | `proposal`, `<funding-org>`, `<year>`, `<mdh/atf/hca>`            | `proposal-dfg25-ai-codegen`          |
| `grant`     | `grant-<name><year>-<slug>`               | `grant`, `<name>`, `<year>`, `<mdh/atf/hca>`                      | `grant-en26-goe`                     |
| `review`    | `review-<venue><year>-<paper-id>`         | `review`, `<venue>`, `<year>`, `<mdh/atf/hca>`                    | `review-pldi26-1234`                 |
| `teaching`  | `teaching-<course>-<semester>-<slug>`     | `teaching`, `<course>`, `<semester>`, `<mdh/atf/hca>`             | `teaching-pjs-ss26-codegen-dl`       |
| `teaching`  | `teaching-<ba/ma/diss>-<year>-<name>`     | `teaching`, `<ba/ma/diss>`, `<year>`, `<name>`, `<mdh/atf/hca>`   | `teaching-ba-2026-john-doe`          |
| `protocol`  | `protocol-<date>-<slug>`                  | `protocol`, `<date>`, `<mdh/atf/hca>`                             | `protocol-2026-12-01-tensor-cores`   |
| `cv`        | `cv-<name>`                               | `cv`                                                              | `cv-john-doe`                        |
| `travel`    | `travel-<year>-<destination>-<slug>`      | `travel`, `<year>`, `<destination>`                               | `travel-2026-sydney-cgo`             |
| `misc`      | `misc-<slug>`                             | optional                                                          | `misc-headshots`                     |

---

## 3. GitHub Topics (Controlled Vocabulary)

Topics are **mandatory** and serve as the **only hierarchical mechanism**.

### 3.1 Primary Type (exactly one)

```
paper | benchmark | artifact | talk | proposal | grant | teaching | protocol | cv | travel | misc
```

---

### 3.2 Venue / Context

**Conferences / Journals** (lowercase, short):
```
cgo, pldi, cc, sc, eurollvm, hpca, ppoppp, toplas, taco
```

**Funding Organizations**:
```
dfg, bmbf
```

**Teaching Formats**:
```
pjs, sem, mgpp, ps, diss, ma, ba
```

---

### 3.3 Year

Always four digits:
```
2024, 2025, 2026
```

---

### 3.4 Research Themes (controlled)

Use **only from this list**:
```
mdh    # Code Generation
atf    # Code Optimization
hca    # Code Execution
misc   # else
```

Multiple themes are allowed.

---

## 4. Topic Rules (Strict)

- Use **lowercase only**
- No free-form invention of topics
- Prefer **short, stable identifiers**
- Topics must remain meaningful over **5+ years**

---

## 5. Privacy Rules

Repositories default to private

---

## 6. The `.github` Repository

The `.github` repository contains organization-wide defaults:

- Organization README (this document)
- Issue templates
- Pull request templates
- Contribution guidelines (if applicable)

---

## 7. Philosophy

This structure is designed to:

- Scale over long academic careers
- Survive personnel turnover
- Be understandable to reviewers, students, and funding agencies
- Avoid implicit knowledge and ad-hoc naming

**If a repository does not fit the scheme, the scheme is wrong – not the repository.**
