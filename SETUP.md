# Setup script (for the AI)

You are setting up this workspace for a law firm. The person in front of you is
probably a lawyer or office manager with no technical background. Your job is to make
this feel like a friendly 15-minute intake conversation, not software installation.

## Step 0: Get the files in place (do this quietly)

**Choose the folder without making the person decide.** If a folder is already open and
it's empty or already holds this workspace, use it. Otherwise create a folder called
`Firm Workspace` in their Documents folder, work there, and tell them in one line where
it is. If your app requires the person to pick or approve a folder, suggest the new
`Documents/Firm Workspace` folder rather than listing options.

If this folder doesn't already contain `AGENTS.md`, `firm/`, `matters/`, and `skills/`,
get them from the GitHub link you were given:

1. Download into a temporary folder *outside* this one, using `git clone` or the ZIP
   archive, whichever works.
2. Copy the contents into this folder so `AGENTS.md` sits directly inside it, not in a
   nested `law-firm-workspace-main/` subfolder.
3. **Do not copy the `.git` folder.** This workspace will hold client files and must
   never stay connected to the public repository. If a `.git` folder ended up here
   anyway, delete it.
4. Delete the temporary folder.

If you can't download at all, ask the person to click **Code → Download ZIP** on the
GitHub page and unzip it anywhere. Then you do the copying in steps 2–4 yourself.

If the files were already here, check for a `.git` folder that points to the public
repository and remove it after telling the person why.

Then read `AGENTS.md` so you know the rules you're setting up.

## Step 1: Explain what's about to happen (keep it short)

Tell them, in your own words:

- You'll ask about a dozen questions in four short rounds. Any can be skipped.
- Their answers become files in `firm/` that you read at the start of every session.
- **Don't share any client information during setup.** Firm-level answers only.

## Step 2: Interview, one round at a time

Ask one round, wait for answers, then move on. Accept short or partial answers and
write down what they said. Ask a follow-up only when an answer could be read two ways
that would change how you'd draft, for example "separate trusts" (per spouse or per
child?).

**Round 1: The firm**
1. Firm name, and your name and role?
2. Practice areas, and which one takes most of your time?
3. Which state(s) or jurisdictions do you practice in?
4. Who else works with you? (Names and roles.)
5. For letters: office address, phone, email, website, and signature block?

**Round 2: How you write**
6. Who are your typical clients? (For example: retirees, young families, business
   owners.) This shapes how everything is explained.
7. How should letters to clients sound? How do you sign them?
8. Any words, phrases, or habits you love or hate? A short sample letter you like,
   with client details removed, helps a lot.

**Round 3: Your positions**
9. What are a few standing positions or preferences your firm takes on how matters
   are handled? Answer in your own words; there are no wrong answers. (If they're
   stuck, offer a neutral shape: "We always…" / "We never…" / "We prefer X over Y
   when…")
10. Anything the AI should *never* do or say, in any document?

**Round 4: Your week**
11. What recurring tasks eat the most of your week?
12. Which one would you most like help with first?

## Step 3: Write the firm files

Fill in only the files in `firm/`. Leave `matters/` alone, including the sample.

- `firm/profile.md` from Rounds 1 and 4. Set `Setup status: complete` and today's date.
  Set `Client data check` to `not yet confirmed` unless they say they've checked.
- `firm/team.md` from question 4.
- `firm/voice.md` from Round 2. If they gave a sample, describe its traits (sentence
  length, tone, greetings, sign-off). Don't copy client details into it.
- `firm/positions.md` from Round 3, including question 10 under **Never**. Keep their
  wording where you can.
- Leave `firm/lessons.md` as is. It fills up with use.

Anything skipped becomes `[not yet provided]` so it's easy to fill in later.

## Step 4: Tailor the skills

1. Read `skills/README.md`. The starter skills lean toward estate planning. If their
   practice is different, offer to move the ones that don't fit to `skills/_unused/`.
2. For the task they named in question 12, check whether an existing skill already
   covers it. If one does, tell them which one and what to say to use it, and skip
   to Step 5.
3. Otherwise, ask one or two quick questions to learn what a good result looks like
   (what goes in it, when it happens, who does which part). Build on existing skills
   rather than repeating them. Follow `skills/make-a-skill`, show them the draft,
   and adjust.

## Step 5: Show them how to use it

Offer a two-minute tour of the fictional sample matter; skip it if they'd rather not.
If they want it: open `matters/_example-hartwell-trust/matter.md`, point out **Where we
left off**, and describe (don't run) what "Start my day" and "Wrap up" would do. It's
fictional and they can delete it whenever they like.

Either way, give them these three lines to keep:

- Start a session: **"Let's work on [matter]."** If I ever seem to have forgotten
  your firm, say **"Read AGENTS.md first."**
- End a session: **"Wrap up."**
- When I get something wrong: correct me and say **"remember that."**

## Step 6: Finish

In ten lines or fewer:

- What you set up.
- What was skipped or left as `[not yet provided]`.
- A suggestion for the next skill, based on their other answers to question 11.
- A reminder that everything drafted here is for attorney review.
- Ask directly: "Have you confirmed that your AI plan's data terms and your ethics
  rules allow putting client information in here?" Record the answer in the
  `Client data check` line of `firm/profile.md`. If not yet, suggest using initials
  instead of client names until they have.

Then ask what they'd like to work on first.
