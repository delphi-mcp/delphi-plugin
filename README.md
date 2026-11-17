# Delphi for Claude

Delphi gives Claude direct access to Canadian law: about 1.7 million English-language court and tribunal decisions and statutes from the Supreme Court of Canada, the federal courts, and every province and territory outside Quebec. Claude can find the leading cases on a question, read the paragraph that supports each point, check whether a case is still good law, and verify every citation in a draft.

This plugin connects Claude to the Delphi server and adds a research skill that sets out how to use it well: search first, read the pinpointed paragraph before relying on it, note up every authority the answer rests on, and cite only what Delphi returned.

## Install

In Claude, open the plugin directory, find Delphi and install it. Claude asks you to sign in to your Delphi account the first time it uses a Delphi tool. A Delphi subscription is required.

In Claude Code: `/plugin install delphi` from the directory, or add the server yourself with `claude mcp add --transport http delphi https://delphi-mcp.com/mcp`.

## What it includes

- `.mcp.json`: the Delphi server at `https://delphi-mcp.com/mcp`.
- `skills/canadian-legal-research`: the research method.

## What it sends

When Claude uses a Delphi tool, it sends the tool's inputs to the Delphi server at https://delphi-mcp.com over HTTPS: your search terms and questions, the case or statute requested, and the text of any draft you ask it to check. Delphi does not store a draft it checks. Usage records are kept as the privacy policy describes.

## Limits

Delphi is a research tool and does not give legal advice. Treatment labels, outcomes, statistics and screening answers are produced by software, and each points to the passage it rests on. Screening is experimental. Quebec decisions and French-only decisions are not covered.

Documentation: https://delphi-mcp.com/docs. Privacy: https://delphi-mcp.com/privacy. Support: https://delphi-mcp.com/support.
