# UMS-CPL: University of Muenster – Compilers & Programming Languages

This GitHub organization hosts research, teaching, and administrative artifacts of the  
**CPL (Compilers & Programming Languages)** group.

The organization follows a **flat repository structure** with **strict naming conventions**
and a **controlled GitHub topic vocabulary**.

There is intentionally **no hierarchy via folders**.  
Structure is expressed **exclusively via repository names and topics**.

---

## 1. Repository Naming Scheme

All repositories follow the pattern:

```
<category>-...
```

### Categories

| Category    | Purpose |
|------------|---------|
| `paper`     | Paper source (LaTeX, figures, scripts) |
| `benchmark` | Benchmark implementations & datasets |
| `artifact`  | Artifact Evaluation packages |
| `talk`      | Slides, posters, demo material |
| `proposal`  | Funding and project proposals |
| `grant`     | Grants (e.g., travel grants) |
| `teaching`  | Theses, seminars, etc |
| `protocol`  | Meeting notes |
| `cv`        | Academic CVs |
| `travel`    | Conference and research travel planning |
| `misc`      | Miscellaneous or non-classifiable material |

---

## 2. Examples

### Papers
```
paper-cgo26-mdh-schedules
paper-pldi25-atf-python-interface
```

### Artifacts
```
artifact-cgo26-mdh-schedules
```

### Proposals / Grants
```
proposal-dfg25-ppp-dl
grant-en26-goe
```

### Teaching
```
teaching-pjs26-codegen-dl
teaching-ma26-rs-mdh
```

### Protocols
```
protocol-2026-01-10-mdh-meeting
```

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
