# skills

Personal agent skills, in the [Agent Skills](https://agentskills.io) format.

## jira-ticket

Turns a planning conversation into a Jira ticket with a title, story points, What, Why, Acceptance criteria, and How. It writes for a teammate who wasn't in the conversation and checks the draft against [ticket writing rules](skills/jira-ticket/references/writing.md).

```bash
npx skills add trevor-lambert/skills --skill jira-ticket -g
```

Run it with `/jira-ticket`, or ask "write a Jira ticket for this".

## commit-message

Writes a Conventional Commits message for the staged changes. The diff supplies what changed, and the conversation supplies why. It prints the message and doesn't commit.

```bash
npx skills add trevor-lambert/skills --skill commit-message -g
```

Run it with `/commit-message`, or ask "write a commit message".
