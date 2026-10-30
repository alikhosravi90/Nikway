# NIKWAY Documentation and Living Book Standard

**ID:** NB-DOC-001  
**Version:** 1.0.0  
**Status:** Proposed, not approved  
**Document date:** 2026-10-31  
**Exact event time:** Not recorded  
**Time zone:** Asia/Tehran  
**Language:** English

## 1. Purpose
This standard defines how NIKWAY records its real journey of understanding, design, decisions, action, and change. The record should support a trustworthy history and future books, guides, reports, and learning materials.

It governs documentation, not product architecture or permission to carry out technical work.

## 2. Principles
1. **Clear source:** Give every important topic, decision, and event a stable ID and source.
2. **Separate claims:** Distinguish observations, interpretations, ideas, proposals, decisions, and verified results.
3. **Record time:** Keep event, writing, review, and publication times separate.
4. **Keep history:** Make corrections traceable. Do not present later knowledge as if it was known earlier.
5. **Grow step by step:** Improve documents as understanding grows.
6. **Separate languages:** Keep Persian and English in separate files with linked IDs and versions.
7. **Avoid duplication:** Link to the main record instead of making conflicting copies.
8. **Protect information:** Do not publish secrets, private records, or customer data.
9. **Keep content portable:** Use simple, reusable source files.
10. **Respect authority:** A document does not grant permission to merge code, deploy, or run operations.

## 3. Document Types
| ID prefix | Type |
|---|---|
| NB-DOC | Standard |
| NB-EVT | Event |
| NB-CON | Concept |
| NB-MOD | Model |
| NB-ADR | Decision record |
| NB-EVD | Evidence |
| NB-RPT | Report |
| NB-PLB | Practical guide |
| NB-CH | Book chapter |

Never reuse an assigned ID for a different subject.

## 4. Required Information
Each document should include a title, ID, version, status, author or owner, record date, scope, sources, links, and change history.

Record exact timestamps with a time-zone offset. If a time is unknown, say so. A Git commit time is not proof of when an event occurred.

## 5. Event Journal
For each important event, record when it happened, who was involved, its context, the opening question, observations, evidence, interpretation, and outcome.

Correct older entries through traceable changes, not silent deletion.

## 6. Decisions
Each important decision should state the context, problem, options, criteria, choice, reasons, possible effects, evidence, approver, and status.

Statuses: Proposed, Accepted, Rejected, Superseded, Withdrawn. Do not present a proposal as an approved decision.

## 7. Book Chapters
A chapter may include an opening question, story, background, concepts, real example, model or image, options, decisions, lessons, practical guidance, and sources.

The **journal** records what happened; the **book** tells the story; a **playbook** explains how to do the work; a **handbook** collects reference guidance.

## 8. Persian and English
Keep the two editions in separate files, with a shared content ID, version, and translation status.

Translation status: Not Started, Draft, In Review, Synchronized. Prefer clear everyday words while keeping official names and technical IDs accurate.

## 9. Versions
Use three-part versions, such as 1.0.0: major change, compatible addition, small fix.

Document, book, model, and software versions are separate. Published versions should link to a specific Git change and release date.

## 10. Sources and Evidence
Record source title, author or publisher, date, version, link, and access date when available. Separate original sources, third-party analysis, and internal records. Mark direct quotes and interpretations clearly.

## 11. Work Flow
Question or event → context and evidence → concept or model → review and decision → book and guides → review → versioned publication → feedback.

The flow can repeat and does not have to be strictly linear.

## 12. Local Work and Publishing
Writing and Git versioning can begin on a local computer. GitHub supports sharing and collaboration.

Simple text-based source files remain primary. Website, PDF, and e-book outputs require checks, especially for Persian text layout.

## 13. Quality Check
- [ ] ID and version are valid.
- [ ] Facts and assumptions are separate.
- [ ] Times are recorded without guessing.
- [ ] Sources and links are checked.
- [ ] No private information is exposed.
- [ ] Text is clear.
- [ ] Translation matches the source.
- [ ] Change history is traceable.
- [ ] Persian layout and print output are checked when needed.
- [ ] Required approval is recorded.

## 14. Translation Sync
Each bilingual document must record a shared content ID, Persian revision, English revision, translation source revision, and sync status.

**Change rule:** A meaning-changing edit to the Persian source marks the linked English edition as **Needs Review** until it is checked. Minor editorial changes only trigger review when they affect translation.

**Proposed automated check:** Compare the current Persian revision with the revision used for the English translation and warn if they differ. This check is **not yet implemented or run**.

**Style and terminology:** [Persian writing guide](NB-STYLE-FA-001.md), [Persian glossary](../glossary/terms.fa.md), [English glossary](../glossary/terms.en.md).

## 15. Status
This standard is still **proposed**. Older projects and assets must not be deleted, merged, or rewritten without separate permission. This document does not prove that running services have stopped.

**Next:** Review and approve the standard, then record the first journal event and book chapter.

---
**Persian edition:** [فارسی](NB-DOC-001.fa.md)
