# Security policy

This policy covers every repository in the
[eugene-plexus](https://github.com/eugene-plexus) organization, the installers
and the release images.

## Report a vulnerability privately

**Do not open a public issue for a security problem.** Report it here instead:

**[Report a vulnerability](https://github.com/eugene-plexus/specs/security/advisories/new)**

Only the maintainers can see the report. You can report through any repository's
**Security** tab; `specs` is the one place to use if you are unsure which
component is affected.

Please include:

- the Eugene Plexus version (or Edge commit) and how it was installed
- the operating system, and whether the machine is the root or a worker node
- what an attacker can do, and what access they need first (a network position,
  a client key, a signed-in account, an account on the machine)
- steps to reproduce, or a proof of concept

## What happens next

- We aim to confirm we have your report within **7 days**. Eugene Plexus has one
  maintainer, so a reply can take longer around holidays.
- We confirm the problem, agree a disclosure date with you, and fix it in a
  patch release.
- When the fix ships, we publish a GitHub security advisory. We credit you in it
  unless you ask us not to.

## Supported versions

| Version                 | Security fixes   |
| ----------------------- | ---------------- |
| Newest release (v0.2.x) | Yes              |
| Edge                    | Yes              |
| Older releases          | No; update first |

## Out of scope

- Bugs in the engines Eugene runs (llama.cpp, vLLM, MLX) or in the models
  themselves. Please report those to their own projects.
- Attacks that need an administrator account on the machine running Eugene.
- Problems in apps we do not ship, such as Open WebUI, unless Eugene's
  configuration of them causes the problem.
