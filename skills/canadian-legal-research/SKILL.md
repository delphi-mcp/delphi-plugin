---
name: canadian-legal-research
description: Research Canadian case law and legislation with Delphi. Use when the user asks what the law is in a Canadian jurisdiction, whether a case is still good law, how courts have applied a test or a statutory provision, or asks to check the citations in a draft.
---

# Canadian legal research with Delphi

Delphi holds English-language Canadian decisions and statutes from the federal courts, the Supreme Court of Canada and every province and territory outside Quebec. It gives you the law and the passage that supports it. You do the reasoning, and the user decides what to do with it. Delphi is a research tool and does not give legal advice.

## How to research

1. Start with `search`, in plain words. Use the court, jurisdiction and date filters when the user names them.
2. Treat a search result, a `principle` or an `analyze` figure as a lead. Open the pinpointed paragraph with `get_document` before you rely on it.
3. Cite only what Delphi returned. Copy the citation and the paragraph number from the response. Never cite from memory.
4. Note up every authority the answer rests on with `noteup`, and read the citing passages, not only the status. A clean status means no negative treatment was detected, not that none exists.
5. For a statute, use `legislation` for the text of the section and `noteup` for the cases that apply it. Delphi holds the current version only, so say so when the question is about the law on a past date.
6. When the user pastes a draft and asks for a citation check, use `check_document`, then report each problem with the corrected citation.
7. Use `analyze` for patterns across many decisions, such as award ranges or how often a review succeeds. Report the numbers with the sample they came from.
8. `screen` is experimental. Use it only when the user wants one question asked of many decisions, and present every answer as a pointer to read, not a finding.

## How to answer

- Lead with the answer, then the authority for it with a pinpoint.
- Italicize case names and the names of Acts.
- Say what you searched for and did not find, and anything you did not check.
- When the user describes their own situation, give the law and the leading authorities, and suggest that they speak with a lawyer licensed in their province before acting on it.
