# Proof First

Proof First is a compact coding-agent skill for reliable implementation without heavyweight process. It asks the agent to understand the real problem, make the smallest sensible change, verify the behavior that matters, and report evidence instead of confidence.

It includes focused workflows for bug fixes, features and refactors, skeptical review, and autonomous runs. It deliberately excludes transcript mining, model-specific routing, automatic messaging, deployment, and auto-merge behavior.

## Install in Codex

Ask Codex:

```text
Install the proof-first skill from https://github.com/stephiesworld/proof-first
```

The repository is private initially, so installation requires GitHub access to the `stephiesworld` account. You can also copy this repository to `~/.codex/skills/proof-first/`.

## Use

Invoke it explicitly when rigor matters:

```text
$proof-first Fix the duplicate invoice bug. Reproduce it first and verify the real checkout flow.
```

Codex may also select it automatically for substantial coding work.

## Cursor

The instruction format is also readable by Cursor. Copy the repository into `.cursor/skills/proof-first/` in a project and invoke it as `/proof-first`. Tool names and agent behavior still depend on the host product.

## Acknowledgment

This skill is an independent, compact implementation inspired in part by the workflow ideas in Lauren Tan's MIT-licensed [pstack](https://github.com/cursor/plugins/tree/main/pstack). It does not include pstack's source code, branding, automation pack, or full playbook system.

## License

MIT
