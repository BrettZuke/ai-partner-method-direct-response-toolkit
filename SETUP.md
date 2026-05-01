# Setup

This is a documentation + templates repo — no Python, no compiler, no dependencies. The "tool" is Claude Code reading the SOP and templates on your behalf. You can also use this repo entirely by hand (read frameworks, copy templates, write yourself), no AI required.

---

## Required (to use anything)

### 1. Git

```bash
git --version
```

If missing: `brew install git` (Mac), `sudo apt install git` (Linux), or [Git for Windows](https://git-scm.com/download/win).

### 2. Clone the repo

```bash
git clone https://github.com/BrettZuke/ai-partner-method-direct-response-toolkit.git
cd ai-partner-method-direct-response-toolkit
```

That's it. You can now read every framework, swipe file, and template.

---

## Recommended (to use Claude Code)

[Claude Code](https://claude.com/claude-code) is an AI assistant that runs in your terminal. Drop it inside this repo and it reads `CLAUDE.md` automatically — meaning it knows the frameworks, the SOP, and how to use the templates.

### Install

```bash
npm install -g @anthropic-ai/claude-code
```

(Need npm? Install Node.js from [nodejs.org](https://nodejs.org/) — npm comes with it.)

### Verify

```bash
claude --version
```

### Start a session inside this repo

```bash
cd ai-partner-method-direct-response-toolkit
claude
```

Try:

> *"What can you help me write?"*

Claude will list the asset types and ask which one you need.

---

## Your daily workflow

### 1. Set up a brief for each client / offer

```bash
cp examples/brief.example.json clients/<client-slug>/brief.json
```

The brief is the single source of truth for that client's audience, awareness level, offer, voice, and proof points. Update it as you learn more.

> The example brief is for "Apex Performance" — a $4,800 fitness coaching offer. Use it as a model for the level of detail you want.

### 2. Generate the draft

In your Claude Code session:

> *"Using `clients/mike-fitness/brief.json`, write a long-form sales page."*
>
> *"Same brief — write a 3,500-word VSL script."*
>
> *"Same brief — give me 15 headline variants pulling from the swipe file."*

Claude follows the SOP, picks the right framework based on awareness level, and produces a draft.

### 3. Edit for voice

The 80% Claude writes is structurally correct. The last 20% is making it sound like your client — not generic AI prose. Read every line out loud. Cut anything that sounds robotic.

### 4. QA before delivery

Run through the checklist in `SOP.md` → "Quality Checklist". Especially:
- No banned phrases (full list in `voice-and-constraints.md`)
- Active voice throughout
- Single CTA
- Mobile-friendly paragraphs (max 4 lines)
- 6th-grade readability

### 5. Test on real traffic

Direct response is a measurement game. Two-variant test your headlines. Let the data tell you which version converts — not your opinion or your client's.

---

## Optional — the no-AI workflow

Don't have Claude Code? Don't want to use AI? This repo still works:

1. Open `frameworks.md`. Pick the framework that matches your audience.
2. Open the right template in `templates/`.
3. Open `swipe-headlines.md` for headline ideas.
4. Open `voice-and-constraints.md` to QA your draft.

The templates and swipe files are designed to be standalone. Claude just speeds up the process.

---

## Troubleshooting setup

| Problem                                          | Fix                                                                  |
|--------------------------------------------------|----------------------------------------------------------------------|
| `claude: command not found` after npm install    | npm's global bin isn't on your PATH. Run `npm config get prefix` and add `$(...)/bin` to your shell rc. |
| Claude doesn't seem to read CLAUDE.md            | Make sure you ran `claude` from inside the repo root.                |
| `git clone` says "permission denied"             | The repo URL is HTTPS, not SSH — re-copy from GitHub.                |

If you hit something not in this table, open an issue with the exact command and the full error.
