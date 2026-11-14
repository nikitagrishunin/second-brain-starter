# Second Brain Starter

A folder that makes your AI remember you, your projects and your decisions, and keep that memory up to date by itself.
Works with Claude Code (Anthropic) and Codex (OpenAI). From the video "How to make AI remember you" on Prompted.

## Quick start

Open an empty folder in Claude Code or Codex and paste:

> Set up my second brain from https://github.com/nikitagrishunin/second-brain-starter. Copy the folder structure here. Then interview me, one question at a time, to fill in CLAUDE.md: who I am, what I'm working on, how I make decisions, what matters most to me, and how I like my answers. Ask for the "because" behind every rule. Max 20 questions. Show me the file before you save it.

Prefer a file? Click the green **Code** button above, then **Download ZIP**.

## What you need

- Any computer from the last seven or eight years (Mac or Windows). The AI runs on the company's servers; your computer only keeps the folder.
- Claude Code (paid Claude plan) or Codex (works on a free ChatGPT account, with tight limits).
- No terminal, no code.

## Set it up in 3 steps

1. Make an empty folder and open it in Claude Code or Codex.
2. Paste the setup prompt from [PROMPTS.md](PROMPTS.md), section 1.
3. Answer the interview by voice. Give the "because" behind every rule.

Then work as usual and say "wrap up" at the end of every session.

## What's inside

| File | What it's for |
|---|---|
| CLAUDE.md | The main file. Loads every session. Who you are, the rules that keep memory alive, where everything lives. Keep it short. |
| AGENTS.md | Codex reads this one. It points to CLAUDE.md, so one folder works in both. |
| sessions.md | Where you stopped: Done, Decided, Next. |
| decisions.md | What you decided, and why. |
| memory/ | One fact per file, with clear names. |
| projects/ | One folder per project, with a short STATE.md. |
| skills/ | How you do your recurring tasks. |
| inbox/, archive/ | Things to sort. Things that are done. |
| .claude/settings.json, .codex/config.toml | Safe permission settings for Claude Code and Codex. |
| PROMPTS.md | Every prompt from the video. |

## Why it's built like this

- The AI starts every session blank and only knows what gets loaded. So the main file loads by itself.
- The more you load, the thinner its attention gets, and the middle of a long text gets lost. So the main file is a table of contents, and details live in separate files.
- The AI finds files by searching names and words. So one fact per file, with a clear name.
- Memory the AI writes for itself can make results worse. So it suggests, and you say yes.

## Permissions

- When Claude first opens the folder, it asks whether you trust it. It's your folder: yes.
- Claude Code: use the "Accept edits" mode. It changes files in this folder without asking every time, and still asks before it runs most commands or goes online. The folder sets this for you in `.claude/settings.json`.
- Codex: keep "Ask for approval" in the menu next to the input. Same idea: edits inside the folder, asks before going online or outside it. Set in `.codex/config.toml`.
- "Bypass permissions" (Claude Code) and "Full access" (Codex, shows up only after you turn it on in Settings) let the AI do anything without asking. Not on day one.
- During setup from a link, the AI asks once to go online and download the folder. Allow it.

## Safety

- Never put passwords, card numbers or ID numbers in this folder.
- The main file says: never send, pay, delete or post without asking. Keep that line.
- It's your folder. Back it up like any other folder.

## No computer, or free plan?

See [PROMPTS.md](PROMPTS.md), section 10: the light version for ChatGPT Projects. It works on your phone.
