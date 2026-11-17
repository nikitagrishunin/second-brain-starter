# Second Brain Starter

A folder that makes your AI remember you, your projects and your decisions, and keep that memory up to date by itself.
Works with Claude Code (Anthropic) and Codex (OpenAI). From the video "How to make AI remember you" on Prompted.

## Quick start (one sentence)

1. Make an empty folder and open it in Claude Code or Codex.
2. Type this and send:

```
Set up my second brain from https://github.com/nikitagrishunin/second-brain-starter. If you can't open the link, stop and tell me.
```

The AI downloads the folder - it asks a few times to go online and copy files: press Allow each time.
Then it interviews you, one question at a time.
Answer by voice if you like, and give the "because" behind every rule.

**No internet access for the AI, or prefer a file?** Click the green **Code** button above → **Download ZIP** and unzip it:
you get a folder. Open that folder in Claude Code or Codex and type: `Set up my second brain`.

After setup: say **"wrap up"** at the end of every session. That's the whole habit.

## What you need

- Any computer from the last seven or eight years (Mac or Windows). The AI runs on the company's servers; your computer
  only keeps the folder.
- Claude Code (paid Claude plan) or Codex (works on a free ChatGPT account, with tight limits).
- No terminal, no code.

## What's inside

| File | What it's for |
|---|---|
| AGENTS.md | The main file. Loads every session. Who you are, the rules that keep memory alive, where everything lives. Codex reads it directly. |
| CLAUDE.md | One line that loads AGENTS.md into Claude Code, so one folder works in both. |
| SETUP.md | Step-by-step setup instructions for the AI. Moves to `archive/` after setup. |
| sessions.md | Where you stopped: Done, Decided, Next. |
| decisions.md | What you decided, and why. |
| memory/ | One fact per file, with clear names. |
| projects/ | One folder per project, with a short STATE.md. |
| skills/ | How you do your recurring tasks. |
| inbox/, archive/ | Things to sort. Things that are done. |
| .claude/, .agents/ | Safe permission settings for Claude Code, and the setup skill for Claude Code and Codex. |
| PROMPTS.md | Every prompt from the video. |

## Why it's built like this

- The AI starts every session blank and only knows what gets loaded. So the main file loads by itself.
- The more you load, the thinner its attention gets, and the middle of a long text gets lost. So the main file is a
  table of contents, and details live in separate files.
- The AI finds files by searching names and words. So one fact per file, with a clear name.
- Memory the AI writes for itself can make results worse. So it suggests, and you say yes.

## Permissions

- When Claude first opens the folder, it asks whether you trust it. It's your folder: yes.
- Claude Code: the folder turns on "Accept edits" (`.claude/settings.json`): it changes files in this folder without
  asking every time, and still asks before most commands and before going online.
- Codex: if it asks whether you trust the folder, say yes. Keep the default "Ask for approval" mode: edits in this
  folder, asks before going online. To let it download the starter, allow the request when it asks.
- "Bypass permissions" (Claude Code) and "Full access" (Codex) let the AI do anything without asking. Not on day one.

## Safety

- Never put passwords, card numbers or ID numbers in this folder.
- The main file says: never send, pay, delete or post without asking. Keep that line.
- It's your folder. Back it up like any other folder.

## No computer, or free plan?

See [PROMPTS.md](PROMPTS.md), section 10: the light version for ChatGPT Projects. It works on your phone.
