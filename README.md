# Feynman Why

Sometimes you ask “why?” because you want one specific answer.

Feynman Why encourages assistants to answer that question using available
evidence, then stop and let the conversation continue naturally. A short,
sufficient answer can be the whole task.

Consider a hypothetical task whose timings are already available in the logs.

**Without the skill, an answer can turn into an unrequested project:**

> **User:** Why did this task take ten minutes?
>
> **Assistant:** The log shows one minute of work and nine minutes waiting in
> the queue. I'll compare previous runs, investigate worker capacity, adjust
> the configuration, and rerun the task to verify a fix.

**With the skill, the answer can be enough:**

> **User:** Why did this task take ten minutes?
>
> **Assistant:** The log shows one minute of work and nine minutes waiting in
> the queue.

That can be the whole exchange. Another question might follow. An investigation
or fix might be requested. Each request gets its own scope.

You can explicitly request deeper investigation or more autonomous work:
“Investigate the delay, make the appropriate fixes, and verify the result.”
Those requests keep their full scope, including broader work already requested
in the conversation.

In his [interview on why questions](https://fs.blog/richard-feynman-on-why-questions/),
Richard Feynman explores how an explanation depends on what the questioner
already understands and what would satisfy their question. This skill applies
that insight one question at a time. The full interview is included in the
skill instructions.

To use, load [the skill instructions](skills/feynmanwhy/SKILL.md) into your
assistant, or install the `skills/feynmanwhy/` folder through its supported
skill mechanism.

The skill applies to direct questions such as “Why does this happen?” and
“How come?”
