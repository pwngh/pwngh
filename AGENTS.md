# Council defaults

When a project calls for council, use these three full members at high reasoning
effort unless the user explicitly changes the roster:

- OpenAI GPT Sol. Resolve an available Sol version and record its exact model ID.
- Anthropic Claude Opus. Resolve an available Opus version and record its exact model ID.
- Google Gemini 3.8 Flash (High), model ID `gemini-3.8-flash-high` through Antigravity CLI.

Gemini 3.8 Flash is an explicitly chosen full member, not a flagship model or a
non-blocking reviewer. Do not describe it as a flagship. Give all three members
the same review scope and include each member's findings in the agreement gate.

Limit council to three complete review rounds total. If agreement is not reached
after round three, stop and show the user the open findings, disagreements, and
relevant evidence. Do not start a fourth round or imply approval.

Put the actual model names, reasoning effort, round numbers, and returned scores
in the council table in the pull-request description. Write `no score` if none
was returned. Never invent model identity, usage, scores, or consensus.

If a selected model cannot be reached, report the failure and stop at a local
branch. Do not silently substitute another model or provider.

For this profile and housekeeping project, council is skipped under Preston's
explicit housekeeping exception. A sol-loop review is separate from council.
Never merge a pull request on Preston's behalf.
