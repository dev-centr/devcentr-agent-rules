# Dev-Centr product rules (handoff)

> **Dev Configuration (Fill these in before passing to AI)**:
> `CODE_ROOT= # insert the path to your code hive`
> `DEVCENTR_RULES_PATH=$CODE_ROOT/github.com/dev-centr/devcentr-agent-rules`

These rules apply when **Dev-Centr** (the application) is acting **on behalf of the user**: applying templates, syncing workspaces, init-repo flows, or other automation driven by the product.

## Context Assembly (CRITICAL FIRST STEP)

You must read all foundational rules and specifications in a single step using your native file reading tools. All paths below are strictly relative to `$DEVCENTR_RULES_PATH`.

Read these files **simultaneously in parallel tool calls** to assemble your full context:

- `RULES.md` (this file)
- Relevant specs in the `devcentr` documentation repository as needed for the task.

*(Fallback)*: If you lack native file reading tools, use a terminal to read them in one command, but beware of truncation.

## Product behavior

- Prefer the [Standard Project Templates](https://github.com/dev-centr/templates) repository (`dev-centr/templates`) for workspace and scaffolding content. Do not treat that repository as the home for **personal** agent rules; those live in the **agent-rules** family.
- When implementing or documenting Dev-Centr behavior, align with published Dev-Centr specifications and the [templates repository schema](https://docs.devcentr.org) in the Dev-Centr documentation.
- When the product needs to pass context to an embedded or integrated agent, load **this** repository’s rules for product-driven actions; load the user’s **agent-rules** clone for user-owned editing and project work.

---
They do **not** replace end-user agent rules. For portable personal rules, see [agent-rules](https://github.com/dev-centr/agent-rules) or a user fork such as [AMDphreak/agent-rules](https://github.com/AMDphreak/agent-rules).
