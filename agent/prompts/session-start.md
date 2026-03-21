# TRPG Session Start Checklist

Use this quick checklist when starting a new dedicated TRPG run.

1. Verify plugin load path includes `~/.openclaw/extensions/trpg-runtime`.
2. Verify plugin entry `trpg-runtime` is enabled.
3. Verify dedicated mode overlay sets:
   - `agents.list[].id = "trpg"`
   - `agents.list[].agentDir = "~/.openclaw/extensions/trpg-runtime/agent"`
4. Run:
   - `openclaw config validate --json`
   - `openclaw plugins info trpg-runtime`
   - `openclaw agents bindings --agent trpg --json`
5. Do an initial read probe with `trpg_store_get` before story progression.
