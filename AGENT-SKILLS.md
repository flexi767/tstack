# agent-skills adaptations

This branch is pinned by flexi767/agent-skills. Only `council` is installed.
Rebase it onto upstream `main` to re-pin.

- `council`: delegates must not run test suites, builds, typecheck, type-aware
  lint or local models; the parent runs checks and passes results in the brief.
  Reason: the host resource policy allows one heavy command at a time, and three
  parallel reviewers each running the suite would exhaust memory.
- `council`: delegates run at medium reasoning effort, not high, unless the user
  names a level. Reason: owner, 2026-11-04, to save tokens.
- `council`: default members are Claude Opus, GPT Sol and GPT Astra (owner,
  2026-11-04), replacing "one flagship per provider".

Not installed, with reasons: `agent-skills/DECISIONS.md`.
