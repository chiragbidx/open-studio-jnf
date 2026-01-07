# 🐼 Panda Template Manifest – New Agency Template

> **This document defines how AI must understand and operate on the New Agency template inside Panda.**
> It is the highest authority for AI-driven code suggestions.

---

## 1. Template Metadata (DO NOT MODIFY STRUCTURE)

```md
# Panda Template Manifest

template_name: "New Agency"
template_id: "panda-new-agency-001"
template_version: "1.0.0"
template_type: "marketing-landing"
layout_style: "modern-agency"
technology_stack: ["HTML5", "CSS3"]
responsive: true
dark_mode: false
rtl_supported: false

author: "Panda Templates"
last_updated: "2026-01-04"
```

---

## 2. Template Intent & Design Philosophy

```md
## Template Intent

This template is designed for:
- Digital agencies
- Consulting firms
- Creative studios

Primary goals:
- Clear service positioning
- Trust building
- Lead generation
```

### Design Rules

```md
- Professional, modern layout
- Clear visual hierarchy
- Conversion-focused CTAs
```

⚠️ **AI DESIGN RULE**
Do NOT introduce new design systems, animations, or layouts unless explicitly requested.

---

## 3. File & Folder Structure (SOURCE OF TRUTH)

```md
/
├── index.html
├── new-agency/
│   ├── standalone.html
│   └── css/
│       ├── style.css        # READ-ONLY
│       └── custom.css       # READ-ONLY
├── vendor/                  # READ-ONLY
├── assets/
```

---

## 4. Change Control Rules (CRITICAL)

### CSS

```md
- style.css and custom.css are READ-ONLY
- Vendor CSS must NEVER be edited
- CSS changes allowed ONLY on explicit request
```

### Images

```md
- Images are READ-ONLY by default
- Image changes allowed ONLY if:
  - A specific image is named, OR
  - A direct image URL is provided
```

### Sections

```md
- All sections are IMMUTABLE by default
- No add/remove/reorder unless explicitly requested
```

---

## 5. Default AI Assumptions

```md
- HTML unchanged
- CSS unchanged
- Images unchanged
- Sections unchanged
- Only TEXT CONTENT is editable
```

---

## 6. Sections Overview

```md
1. Header
2. Hero
3. About
4. Services
5. Portfolio
6. Process
7. Testimonials
8. Clients
9. CTA
10. Footer
```

---

## 7. Section-Level Contract (Example)

```md
## Section: Hero

Editable:
- Headline
- Subheadline
- CTA text

Non-editable:
- Layout
- Classes
- Structure
```

---

## 8. AI Code Suggestion Modes

### Full Code Suggestion
- Return full file content
- Use only for large changes

### Diff-Based Suggestion
- Return minimal diffs
- Default mode

---

## 9. Change Permission Matrix

```md
| Change Type | Default | Explicit |
|------------|---------|----------|
| Text       | ✅      | ❌       |
| CSS        | ❌      | ✅       |
| Images     | ❌      | ✅       |
| Sections   | ❌      | ✅       |
| Vendor     | ❌      | ❌       |
```

---

## 10. AI Hard Stop Conditions

```md
- CSS implied but not requested
- Image change without image reference or URL
- Section change without section name
- Vendor file targeting
```

---

## 11. AI FINAL DIRECTIVE

```md
This manifest is the highest authority.
If conflicts arise:
→ Follow this document
→ Ask for clarification
→ Do NOT assume
```
