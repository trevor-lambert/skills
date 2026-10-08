---
name: jira-ticket
description: Turn the current conversation into a concise Jira ticket with a title, story points, What, Why, Acceptance criteria, and How. Use when the user asks to write, draft, or create a Jira ticket, story, or task from the discussion, usually before starting implementation.
license: MIT
metadata:
  author: trevor-lambert
  version: "1.1.0"
---

# Jira ticket

Write a Jira ticket from the current conversation. A teammate who never saw the conversation should be able to read it and start work.

What and Why carry the ticket. Put most of the effort there. Acceptance criteria and How are short supporting sections.

## Process

1. **Prepare.** Read [the writing rules](references/writing.md).
2. **Gather.** Read the whole conversation. Use the decisions the user and agent settled on. Drop options that were rejected or abandoned. If the problem or scope is unclear, ask at most 2 questions before drafting. Don't invent requirements.
3. **Draft.** Fill in [the template](assets/ticket-template.md), following the writing rules as you write.
4. **Point.** Pick one Fibonacci value:
   - 1: trivial change or config
   - 2: small change in one area
   - 3: a few files, clear path
   - 5: several components, or one real unknown
   - 8: cross-cutting, or several unknowns
   - 13: too big. Recommend a split and name the pieces.
5. **Check.** Go through the writing rules one by one against the draft and fix every violation. Then reread it as the teammate who wasn't there: rewrite anything they would have to ask about.
6. **Output.** Print the ticket in one fenced markdown block. After it, add at most one line listing open questions or assumptions. Nothing else.
