## Description:

Strategic Compact helps agents and users choose manual context compaction at logical workflow boundaries, especially after exploration phases, before major task switches, or when context approaches limits.

This skill is ready for commercial/non-commercial use.

## Publisher:

[djc00p](https://clawhub.ai/user/djc00p)

### License/Terms of Use:

MIT-0

## Use Case:

Developers and agent users use this skill to decide when to compact conversation context, preserve important work in files, and resume long multi-phase tasks with less irrelevant history.

### Deployment Geography for Use:

Global

## Known Risks and Mitigations:

Risk: The optional helper script uses unsafe temporary-file handling when enabled as a hook or scheduled job.

Mitigation: Use the written guidance manually by default; harden the temporary-file path, ownership checks, and integer validation before enabling the script in hooks or cron.

## Reference(s):

- [Strategic Compaction Guide](references/compaction-guide.md)
- [Tool Integration Guide](references/tool-integration.md)
- [ClawHub Skill Page](https://clawhub.ai/djc00p/skills/strategic-compact)

## Skill Output:

**Output Type(s):** [guidance, markdown, shell commands, configuration]

**Output Format:** [Markdown guidance with optional shell command examples and configuration snippets]

**Output Parameters:** [1D]

**Other Properties Related to Output:** [No API keys or environment variables are required by the skill metadata.]

## Skill Version(s):

1.0.1 (source: server release metadata)

## Ethical Considerations:

Users should evaluate whether this skill is appropriate for their environment, review any generated or modified files before relying on them, and apply their organization's safety, security, and compliance requirements before deployment.
