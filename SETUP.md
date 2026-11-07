# Enable live tracking

1. Create or sign in to your account at https://wakatime.com/.
2. The Neovim and Codex CLI plugins are installed on this computer. Restart Neovim, run `:WakaTimeApiKey`, and enter your key. This saves the shared `~/.wakatime.cfg` used by both plugins. Start a new Codex session to load its plugin. Setup references: https://wakatime.com/neovim and https://wakatime.com/codex-cli.
3. Copy your API key from https://wakatime.com/settings/api-key and save it as the repository Actions secret `WAKATIME_API_KEY`: https://github.com/0utsights/0utsights/settings/secrets/actions/new. Do not commit it or paste it into chat.
4. Record some coding activity and verify it in your WakaTime dashboard.
5. Run **Update coding stats** from https://github.com/0utsights/0utsights/actions. It also runs daily at 06:23 UTC.

The workflow uses the built-in GitHub token; no personal GitHub token is configured. Without the WakaTime secret, it leaves the setup placeholder intact. A successful setup check alone does not mean activity tracking is connected.

The generated section includes AI time, AI versus human line counts, and, when provided by WakaTime, tokens, estimated costs, models, sessions, and prompts. Project names are hidden. Automated “insights” in the upstream action are heuristics, not assessments of skill or review quality.

Only activity recorded by connected integrations is represented. Missing tracking must not be interpreted as zero AI use. The public profile should not be treated as a precise timesheet or proof of code authorship.
