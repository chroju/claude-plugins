# claude-plugins

Personal [Claude Code](https://claude.com/claude-code) plugins.

## Install

```
/plugin marketplace add chroju/claude-plugins
/plugin install hrns@chroju
```

## Plugins

| Plugin | Description |
|--------|-------------|
| [hrns](./plugins/hrns/) | Workflow harnesses that drive a task through explicit phases with subagents |

### hrns

Harnesses that keep the main context as an orchestrator and delegate the
context-heavy work to subagents.

- `/hrns:dev` — runs a development task as requirements agreement → design
  fix → verification-first implementation → independent review → PR and CI,
  with an explicit approval gate after requirements and after design.

## Local development

```
claude --plugin-dir ./plugins/hrns
claude plugin validate ./plugins/hrns
claude plugin validate .
```

## License

[MIT](LICENSE)
