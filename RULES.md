# Dev-Centr product rules (handoff)

These rules apply when **Dev-Centr** (the application) is acting **on behalf of the user**: applying templates, syncing workspaces, init-repo flows, or other automation driven by the product.

They do **not** replace end-user agent rules. For portable personal rules, see [agent-rules](https://github.com/dev-centr/agent-rules) or a user fork such as [AMDphreak/agent-rules](https://github.com/AMDphreak/agent-rules).

## Product behavior

- Prefer the [Standard Project Templates](https://github.com/dev-centr/templates) repository (`dev-centr/templates`) for workspace and scaffolding content. Do not treat that repository as the home for **personal** agent rules; those live in the **agent-rules** family.
- When implementing or documenting Dev-Centr behavior, align with published Dev-Centr specifications and the [templates repository schema](https://docs.devcentr.org) in the Dev-Centr documentation.
- When the product needs to pass context to an embedded or integrated agent, load **this** repository’s rules for product-driven actions; load the user’s **agent-rules** clone for user-owned editing and project work.

## Read order (product integration)

1. This file (`RULES.md`) for product scope.
2. Relevant specs in the `devcentr` documentation repository as needed for the task.
