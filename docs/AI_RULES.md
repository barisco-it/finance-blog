# AI Development Rules

AI acts as the implementation engineer.
The human (Product Owner) defines scope and approves changes.

These rules are mandatory.

---

## 1. Scope Discipline

- Only implement what is defined in the issue.
- Do not introduce additional features.
- Do not refactor unrelated files.
- Do not change architecture without explicit approval.

---

## 2. Dependency Control

- Do NOT add new npm packages without justification.
- Prefer built-in Next.js and React solutions.
- Keep dependencies minimal.

If a new package is required:
- Explain why
- Provide alternatives considered

---

## 3. File Change Transparency

Before implementation, AI must:

- List files to be changed
- Provide short implementation plan
- Explain why each file is touched

All changes must be small and reviewable.

---

## 4. Code Quality Standards

- Follow Next.js conventions
- Use TypeScript properly
- Avoid unnecessary abstractions
- Keep code readable and simple
- No unused variables or imports

---

## 5. Build Safety

Every implementation must:

- Pass lint
- Pass build
- Produce no console errors

If errors occur:
- Fix them before finalizing task

---

## 6. Architecture Stability

Do NOT:

- Change folder structure without approval
- Introduce state libraries
- Introduce backend/database without roadmap approval
- Add authentication system
- Add CMS

This is a static blog-first architecture.

---

## 7. Security Rules

- Never commit secrets
- Never expose environment variables
- Sanitize user inputs (if forms added later)

---

## 8. Output Format for Implementation

For every feature:

1. Plan
2. Files to modify
3. Code changes (diff style preferred)
4. How to test

No direct uncontrolled large rewrites.
