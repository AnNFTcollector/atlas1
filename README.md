# atlas1 — Claude skills

159 Claude skills, one folder per skill, in `skills/`.

## Install as zip uploads (Claude desktop app / Cowork)

The skill uploader only accepts **one skill per zip**, so all skills are also packaged as **plugins**. A plugin can hold many skills. Uploads are limited to 200 files per zip, and the skills have 885 files, so there are five zips, each under 200:

| Zip | Skills | Files | Range |
|---|---|---|---|
| `zips/my-skills-part-1.zip` | 33 | 159 | accessibility-audit … calculator-design |
| `zips/my-skills-part-2.zip` | 18 | 195 | canvas-design … creative-brief-selector |
| `zips/my-skills-part-3.zip` | 43 | 194 | creative-direction … interactive-product-tour |
| `zips/my-skills-part-4.zip` | 38 | 195 | internationalization … seo-keyword-gap-audit |
| `zips/my-skills-part-5.zip` | 27 | 147 | seo-offpage … writing-skills |

Upload each zip as a **plugin**, not as a skill: open the **Plugins** section of the Claude app's customize settings, choose to upload a plugin, and pick the zip. Repeat for all five. The skills then show up prefixed with the plugin name, e.g. `my-skills-part-4:seo-keyword`.

## Install by copying folders (Claude Code)

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
