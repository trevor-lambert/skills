# Writing rules for tickets

Use these while drafting, then check the draft against each one.

## Write for someone who wasn't there

1. The reader never saw the conversation. Don't write "as discussed", "option B", "the second approach", or names coined during the chat.
2. Name real things: files, services, endpoints, tables, flags, error messages. Put code identifiers in `backticks`.
3. Define an acronym or internal term the first time if a teammate on another team might not know it.

## Be specific

4. Each acceptance criterion names one result someone can observe or test. "Works as expected", "is well tested", "handles errors gracefully", and "is performant" don't count. Replace them with the actual behavior or number.
5. Why names who is affected and what it costs: failed requests, manual work, support tickets, minutes lost, a blocked feature.
6. Replace vague verbs with what happens. "Improve", "enhance", "streamline", "optimize", and "ensure" usually hide the real change.
7. Use numbers when the conversation has them: limits, timeouts, counts, versions.

## Don't repeat

8. What doesn't restate the title. How doesn't restate What. Acceptance criteria don't restate How.
9. Leave out discussion history, rejected options, and reasoning the implementer doesn't need.

## Remove AI tells

10. No em dashes. Use a period or a comma.
11. Plain words: "use" not "leverage" or "utilize", "is" not "serves as", "help" not "facilitate", "to" not "in order to".
12. Cut inflated words: robust, seamless, comprehensive, crucial, pivotal, critical (unless it is a real severity), delve, landscape, holistic.
13. No tacked-on -ing clauses: "..., ensuring consistency", "..., improving reliability". State the effect as its own fact or cut it.
14. One hedge at most. "May", not "could potentially".
15. Active voice. Name the actor: "the export job retries", not "retries are performed".
16. No filler openers or closers: "This ticket aims to", "It is important to note", "Overall, this will".

## Format

17. Bullets and checkboxes can be short statements. They don't need to be full sentences, but they need a verb.
18. Keep the template's labels, headings, and checkboxes exactly as written.
