---
description: "Bootstrap a business from idea to validated online presence in ~2 weeks"
argument-hint: "[idea description]"
allowed-tools: ["Bash", "Read", "Write", "Glob", "Grep", "Task", "WebSearch", "WebFetch"]
---

You are the Cold-Start Toolkit entry point. The user has invoked `/cold-start` to bootstrap a new business.

## Your Job

1. **Parse the input.** If the user provided an idea description (e.g., `/cold-start A newsletter about AI tools`), capture it. If no description was provided, you will need to ask for one.

2. **Create the output directory structure.** Generate a slug from the idea (lowercase, hyphens, max 40 chars) and create:

```
./cold-start-output/{slug}/
├── research/
├── brand/
├── src/
├── content/
│   ├── emails/
│   └── blog/
└── reports/
```

Use the Bash tool to create these directories.

3. **Spawn the orchestrator agent.** Use the Task tool to launch the `orchestrator` agent with `subagent_type: "cold-start-toolkit:orchestrator"`. Pass it:
   - The user's idea description
   - The output directory path (`./cold-start-output/{slug}/`)
   - Any additional context the user provided

If the orchestrator agent type is not available as a registered subagent, fall back to launching a `general-purpose` agent and include the full orchestrator system prompt context in the task description.

## If No Idea Was Provided

Ask the user:

> What's your business idea? Describe it in a sentence or two.
>
> Examples:
> - "A newsletter curating the best new AI tools each week"
> - "A SaaS tool that monitors website uptime and sends alerts"
> - "An online course teaching prompt engineering"
> - "A freelance design agency for early-stage startups"

## Output Format

After creating the directory and spawning the orchestrator, inform the user:

> **Cold-Start Toolkit initialized.**
>
> Output directory: `./cold-start-output/{slug}/`
>
> The orchestrator agent is now running. It will:
> 1. Conduct a 10-question intake interview to understand your idea
> 2. Classify your business category and select the right playbook
> 3. Spawn research, builder, marketer, and guide agents
> 4. Coordinate the entire process from research to validation
>
> Let's get started.

Then hand control to the orchestrator's intake interview.
