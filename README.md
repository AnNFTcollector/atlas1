# atlas1 — Claude skills

159 Claude skills, one folder per skill, in `skills/`.

## Install on another computer / Claude account (Claude Code)

1. On GitHub, click **Code → Download ZIP** and unzip it.
2. Open the unzipped folder, then open `skills/`.
3. Select **all folders** inside `skills/` and copy them into your personal skills folder:
   - **Windows:** `C:\Users\<your-name>\.claude\skills\`
   - **macOS / Linux:** `~/.claude/skills/`

   Create the `skills` folder if it doesn't exist. (`.claude` is hidden: on Windows, type the path into the Explorer address bar; on macOS, press `Cmd+Shift+.` in Finder.)
4. Restart Claude Code. Type `/` or ask "what skills do you have?" to confirm they're loaded.

The result should look like:

```
.claude/
└── skills/
    ├── accessibility-audit/
    │   └── SKILL.md
    ├── brainstorming/
    │   └── SKILL.md
    └── ...
```

Each skill folder must sit directly inside `skills/` (not nested one level deeper), with its `SKILL.md` at the top of the folder.

## Notes

- **claude.ai / Claude desktop app:** these don't read a folder on disk. Upload skills one at a time under **Settings → Capabilities → Skills**, each as a `.zip` of a single skill folder.
- **Adspirer skills** (`adspirer-*`) need the Adspirer connector set up on the new account to do anything.
- **Not included:** `docx`, `pdf`, `pptx`, `xlsx`, `computer-use`, `chrome-browser` and `built-in-browser`. Their license forbids copying them outside Claude, and Anthropic provides them to every account anyway. Skills built into Claude Code itself (e.g. `code-review`, `simplify`) aren't included either, since every install already has them.
