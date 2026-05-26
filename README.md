# auto-ppt

A Codex skill for turning documents, notes, and raw text into presentation decks with slide structure, visual direction, and speaker notes.

## Repository Layout

```text
auto-PPT/
├── README.md
├── LICENSE
├── .gitignore
└── auto-ppt/
    ├── SKILL.md
    └── agents/
        └── openai.yaml
```

The installable Codex skill is the `auto-ppt/` directory.

## Install In Codex

### Option 1: Manual install

Copy the `auto-ppt/` directory into your local Codex skills folder:

- Windows: `%USERPROFILE%\.codex\skills\auto-ppt\`
- macOS/Linux: `~/.codex/skills/auto-ppt/`

Then restart Codex.

### Option 2: Install from GitHub

Install the `auto-ppt/` path from this repository with your Codex skill installer workflow, then restart Codex.

## Usage

Invoke the skill explicitly as `$auto-ppt`, or let Codex pick it when you ask for help building a deck.

Example prompts:

```text
Use $auto-ppt to turn this project summary into a 10-minute investor presentation.
```

```text
Use $auto-ppt to convert these research notes into an academic slide deck with speaker notes.
```

## What The Skill Does

1. Reads source content and extracts presentation structure.
2. Asks for duration, use case, language, and style constraints.
3. Proposes a slide-by-slide outline and waits for approval.
4. Confirms a visual direction before full deck generation.
5. Produces a presentation workflow that ends in a `.pptx` deck and `speaker_notes.md`.

## License

MIT. See `LICENSE`.
