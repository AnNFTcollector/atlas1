# atlas1 — Claude skills

159 Claude skills in `skills/`, one **`.skill`** file per skill, ready for the Claude app's skill uploader.

## Install on another Claude account

1. On GitHub, click **Code → Download ZIP**, unzip it, and open the `skills` folder.
2. In the Claude app, open **Settings → Capabilities → Skills** and upload the `.skill` files from that folder.

Each `.skill` file holds one complete skill: its `SKILL.md` plus any reference docs, scripts, fonts or other assets it uses, all under 200 files. Every file passed `skill-creator`'s validator when it was packaged.

## Using them in Claude Code instead

A `.skill` file is a zip archive. To use one in Claude Code, unzip it into your personal skills folder (`C:\Users\<your-name>\.claude\skills\` on Windows, `~/.claude/skills/` on macOS/Linux). It extracts as a `<skill-name>/` folder containing `SKILL.md`. Restart Claude Code afterwards.

## Notes

- Some skills had extra header fields (`category`, `catalog_summary`, `display_order`) that the uploader doesn't accept. They were moved under `metadata:` in the `SKILL.md` header, so nothing was lost.
- **Adspirer skills** (`adspirer-*`) need the Adspirer connector set up on the new account to do anything.
- **Not included:** `docx`, `pdf`, `pptx`, `xlsx`, `computer-use`, `chrome-browser` and `built-in-browser`. Their license forbids copying them outside Claude, and Anthropic provides them to every account anyway.
