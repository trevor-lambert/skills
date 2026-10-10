# Writing rules for commit messages

Use these while writing, then check the message against each one.

## Say why, not what

1. The diff already shows what changed. The body explains why, and what a reviewer can't see in the diff.
2. Don't list files, functions, or line changes. Don't narrate the diff ("updated X, then changed Y").
3. The reader wasn't in the conversation. Don't write "as discussed", "per the plan", or names coined during the chat.

## Be specific

4. The subject names the actual change. "update code", "fix bug", "improvements", and "misc changes" don't count.
5. Replace vague verbs with what happens. "Improve", "enhance", "streamline", "optimize", and "ensure" usually hide the real change.
6. Name real things: services, endpoints, config keys, error messages. Put code identifiers in `backticks` in the body.
7. Use numbers when you have them: limits, timeouts, versions, measured speedups.

## Remove AI tells

8. No em dashes. Use a period or a comma.
9. Plain words: "use" not "leverage" or "utilize", "is" not "serves as", "help" not "facilitate", "to" not "in order to".
10. Cut inflated words: robust, seamless, comprehensive, crucial, pivotal, holistic.
11. No tacked-on -ing clauses: "..., ensuring consistency", "..., improving reliability". State the effect as its own fact or cut it.
12. One hedge at most. "May", not "could potentially".
13. Active voice in the body. Name the actor.
14. No filler: "This commit", "This change", "Overall,".

## Format

15. Subject in imperative mood: "add", not "added" or "adds".
16. Short commits get a subject only. Don't pad a body to have one.
