# Blueprint plugins

Community plugins for [Blueprint](https://github.com/bobosneefdev/blueprint).

## Submit a plugin

1. Ask your bot to build it, then copy `plugins/<name>.json` from your workspace
   (`%LOCALAPPDATA%\blueprint\workspace\plugins`).
2. Open a PR adding it to `plugins/`. CI runs `bot validate` on it: the schema, CEL type checks,
   real event payloads, and the plugin's own fixture tests must all pass.
3. Plugins that approximate data Rust+ doesn't expose must say so in `heuristic`.

Import in your portal: Settings → Import from gallery → paste the file's raw GitHub URL.
