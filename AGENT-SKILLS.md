# agent-skills adaptations

This branch is pinned by flexi767/agent-skills. Only `council` is installed.
Rebase it onto upstream `main` to re-pin.

- `council`: delegates must not run test suites, builds, typecheck, type-aware
  lint or local models; the parent runs checks and passes results in the brief.
  Reason: the host resource policy allows one heavy command at a time, and three
  parallel reviewers each running the suite would exhaust memory.

Not installed, with reasons: `agent-skills/DECISIONS.md`.
