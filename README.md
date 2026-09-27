# Law Firm AI Workspace

A starter workspace that gives an AI assistant a lasting memory of your firm: who you
are, how you write, what positions you take, and where every matter stands. It is just
folders and plain-text files. There is no software to install and no account to create
beyond the AI app you already use.

It works with the Claude desktop app, ChatGPT's Codex app, Claude Code, or any AI tool
that can read and write files in a folder on your computer.

## Why a folder instead of chats

Chats forget. Each new conversation starts from zero, so you re-explain your firm, your
client, and your preferences again and again. In this workspace the AI reads your firm's
files at the start of every session and updates the matter file at the end. The work
builds on itself instead of starting over.

## Start in five minutes

1. Make an empty folder on your computer, for example `Documents/Firm Workspace`.
2. Open the Claude desktop app (Cowork) or the Codex app and point it at that folder.
3. Paste this:

   > Set up my firm workspace using https://github.com/sagerock/law-firm-workspace.
   > Download it into this folder, then follow SETUP.md.

4. Answer the setup questions. It takes about 15 minutes. Skip anything you like; you
   can fill it in later.

If your app can't download from GitHub, click **Code → Download ZIP** on the GitHub
page, unzip it into your folder, and paste: *"Follow SETUP.md in this folder."*

## Using it day to day

Start each session with: **"Read AGENTS.md, then let's work on [matter]."**
(Claude Code and Codex read it automatically. Other apps may need the reminder.)

Some things to try:

- "Start my day." Shows open items and deadlines across your matters.
- "New matter: [paste intake notes]." Creates a matter folder and a summary.
- "Draft a letter to the client explaining the next steps."
- "Review this draft against our positions." Drop the file in `inbox/` first.
- "Wrap up." Saves where you left off so next time picks up there.
- "Make this a skill." Turns something you just did into a reusable routine.

When the AI gets something wrong, correct it and say "remember that." It records the
lesson in `firm/lessons.md` and follows it from then on.

## What's in the folder

| Folder | What it holds |
|---|---|
| `AGENTS.md` | The rules the AI follows in this workspace. `CLAUDE.md` points to it. |
| `firm/` | Firm profile, team, writing voice, practice positions, and lessons learned. |
| `matters/` | One folder per client matter, each with a `matter.md` that tracks status. |
| `skills/` | Step-by-step routines for recurring work. Add your own. |
| `inbox/` | Drop documents here for the AI to review or file. |

## Before you use it with client work

This workspace organizes *how* the AI works. It does not decide *whether* client data
may go to an AI provider, and it doesn't make any provider's retention or training
terms suitable for your practice. Check your AI plan's data terms, your jurisdiction's
ethics guidance (see ABA Formal Opinion 512 on generative AI), and your engagement
letters before putting confidential information in. Everything the AI drafts is a
draft; a lawyer reviews it before it goes anywhere.

Made by [SageRock](https://sagerock.com).
