# STS2 Mod Builder

A Codex skill for creating and maintaining Slay the Spire 2 mods. It covers local game API inspection, Harmony patching, DLL/PCK projects, build and load validation, local installation, and Steam Workshop packaging and publishing.

The installed game assemblies are treated as the API source of truth. RitsuLib guidance is optional; the skill does not add a framework dependency by default.

## Install

Clone this repository into your Codex skills directory:

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
git clone https://github.com/iiimur/sts2-mod-builder.git "${CODEX_HOME:-$HOME/.codex}/skills/sts2-mod-builder"
```

Restart or reload Codex so it discovers the skill. To update an existing clone, run `git pull` from that directory.

## Contents

- `SKILL.md` — lifecycle workflow and operating rules.
- `references/api-inspection.md` — local assembly reflection and Harmony compatibility notes.
- `references/ritsulib.md` — optional RitsuLib integration patterns.
- `references/workshop.md` — Steam Workshop publishing guidance.
- `scripts/stage_workshop.py` — stages runtime files into an uploader workspace.
