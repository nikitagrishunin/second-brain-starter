# Setup instructions (for the AI)

You are setting up a "second brain" for the person you're talking to: a folder that makes you remember them, their
projects and their decisions between sessions. Follow these steps in order. Talk to them in the language they write in.
Keep every message short: they may be new to this.
Create and edit files with your file tools (edit/write), not with shell scripts: shell edits get blocked by permissions.

## Step 1. Get the files into this folder

- If AGENTS.md, CLAUDE.md and sessions.md are already here, skip to step 2.
- Otherwise download https://github.com/nikitagrishunin/second-brain-starter into **this** folder. Easiest:
  `git clone --depth 1 https://github.com/nikitagrishunin/second-brain-starter .sbs-tmp` (inside this folder), copy
  everything from `.sbs-tmp` here (hidden folders `.claude` and `.agents` too), then delete `.sbs-tmp`.
  No git? Download https://github.com/nikitagrishunin/second-brain-starter/archive/refs/heads/main.zip and unzip it here.
- Before you start, tell them in one plain sentence: "I'll ask a few times to download and copy files - press Allow."
- **If you can't download it, stop.** Never make up the folder structure yourself. Tell them: "I can't download it.
  Download the ZIP from github.com/nikitagrishunin/second-brain-starter (green Code button → Download ZIP), unzip it
  into this folder and tell me 'done'."
- Never overwrite a file of theirs that already exists. If one has the same name, ask first.
- Don't leave a `.git` folder from the starter: this is their folder, not a copy of the repository.

## Step 2. Tidy up

- Move README.md and this SETUP.md into `archive/starter/`. They're about the starter, not about the person.
- Keep PROMPTS.md: it's their cheat sheet.

## Step 3. Interview

Fill in the "About me" section of AGENTS.md. Ask **one short, simple question per message** (not three in one), wait for the answer, then the next.
At most 12 questions, each one simple. In this order, one line = one question:
1. What's your name?
2. What do you do for work?
3. What city do you live in?
4. What are the 1-3 biggest things you're working on right now?
5. Who matters most in your day-to-day? (only what helps you help them)
6. How do you make big decisions?
7. What do you never compromise on?
8. What are your goals for the next few months? Numbers, if you have them.
9. How do you like my answers: short or detailed?
10. What should I never do when I help you?

Rules for the interview:
- One question = one thing. No "and", no "and why" inside a question.
- When an answer is a rule ("never...", "always...", "short"), ask "Why?" as the next, separate question.
  A rule with a reason works in cases they never listed. After "skip", don't ask why.
- They may answer by voice and ramble. Pull out the facts; don't make them repeat themselves.
- "Skip" or "I don't know" is a fine answer. Move on and don't ask about that topic again.
- Don't ask about the memory rules in AGENTS.md (wrap up, decisions, safety): they're already set.
- Write their rules in their words. Don't make a rule wider than they said it ("no paid courses" stays about courses).
- Never ask for passwords, card numbers, ID or bank details.

## Step 4. Save

1. Show them the "About me" section you're about to write, as a short list, in the first person ("I'm...").
   Their rules ("never/always ..., because ...") go there as "My rules" lines. Numbers that change (debts, balances,
   dates) don't go there - they go to `memory/`. Never invent a "because": if they gave none, ask once or leave it out.
   Save after their "yes". Keep AGENTS.md under about 60 lines: it loads every session.
2. Details that don't need to load every time go into `memory/`, one fact per file with a clear name
   (`kids.md`, `career-switch.md`, `debt.md`), each with today's date.
3. For each big thing they're working on, create `projects/<short-name>/STATE.md` from `projects/_template/`.
   No amounts or balances in STATE.md: point to the memory file instead ("see memory/debt.md").
4. Choices they made go into decisions.md: date, decision in their words, why. Rules are not decisions: they stay in AGENTS.md.
5. Add the first entry at the top of sessions.md: today's date, "Done: set up the second brain", "Next: ...".

## Step 5. Permissions (explain in 2-3 lines, don't lecture)

- Claude Code: `.claude/settings.json` turns on "Accept edits": it edits files in this folder without asking, and still
  asks before most commands and before going online.
- Codex: if it asks whether to trust this folder, say yes. Keep the default "Ask for approval" mode.
- Don't turn on full access / bypass permissions.

## Step 6. Finish

Tell them, in at most 5 lines:
- Say "wrap up" at the end of every session; you'll save what was done, decided and what's next.
- Start a new chat at least once a day; the memory carries over, the clutter doesn't.
- Next: try one prompt from PROMPTS.md (importing old chats, a weekly check-in, or teaching you a task).

Last, delete the line "Not set up yet ... Follow SETUP.md" from the top of AGENTS.md. From now on, follow AGENTS.md.
