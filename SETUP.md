# Setup script (for the AI)

You are setting up this workspace for a law firm. The person in front of you is
probably a lawyer or office manager with no technical background. Your job is to make
this feel like a friendly 15-minute intake conversation, not software installation.

## Step 0: Get the files in place

If this folder doesn't already contain `AGENTS.md`, `firm/`, `matters/`, and `skills/`,
download the workspace from the GitHub link you were given into this folder. Try, in
order: `git clone <link> .`, or downloading the ZIP archive and unzipping it here. If
neither works, ask the person to click **Code → Download ZIP** on the GitHub page and
unzip it into this folder, then continue.

Once the files are here, read `AGENTS.md` so you know the rules you're setting up.

## Step 1: Explain what's about to happen (keep it short)

Tell them, in your own words:

- You'll ask about a dozen questions in four short rounds. Any can be skipped.
- Their answers become files in `firm/` that you read at the start of every session.
- **Don't share any client information during setup.** Firm-level answers only.

## Step 2: Interview, one round at a time

Ask one round, wait for answers, then move on. Accept short or partial answers. If an
answer is vague, write down what they said rather than pushing for more.

**Round 1: The firm**
1. Firm name, and your name and role?
2. Practice areas, and which one takes most of your time?
3. Which state(s) or jurisdictions do you practice in?
4. Who else works with you? (Names and roles; this helps with delegation and drafting.)

**Round 2: How you write**
5. How should letters to clients sound? (For example: warm and plain, or formal.)
6. How do you sign client letters and emails?
7. Any words, phrases, or habits you love or hate? (Paste a short sample letter you
   like, with client details removed, if you have one handy.)

**Round 3: Your positions**
8. What are a few standing positions or preferences your firm takes? Examples: "We
   prefer revocable trusts over wills for clients with real estate," "We never name the
   drafting attorney as fiduciary," "Engagement letters always include a scope limit."
9. Anything the AI should *never* do or say? (For example: never quote fees, never
   promise timing.)

**Round 4: Your week**
10. What recurring tasks eat the most of your week?
11. Which one would you most like help with first?

## Step 3: Write the firm files

Fill in, replacing every `[placeholder]`:

- `firm/profile.md` from Round 1. Set `Setup status: complete` and today's date.
- `firm/team.md` from question 4.
- `firm/voice.md` from Round 2. If they gave a sample, describe its traits (sentence
  length, tone, greetings, sign-off). Don't paste client details into it.
- `firm/positions.md` from Round 3. Keep their wording where you can.
- Leave `firm/lessons.md` as is. It fills up with use.

Anything skipped stays as `[not yet provided]` so it's easy to fill in later.

## Step 4: Tailor the skills

- Look at `skills/README.md`. The starter skills lean toward estate planning. If their
  practice is different, say so, and offer to set aside the ones that don't fit by
  moving them to `skills/_unused/`.
- For the task they named in question 11, create one new skill with
  `skills/make-a-skill`. Draft it from what they told you, show it to them, and adjust.
  Add it to `skills/README.md`.

## Step 5: Show them how to use it

Walk them through the fictional sample matter in `matters/_example-hartwell-trust/`:
open `matter.md`, point out **Where we left off**, and show how "Start my day" and
"Wrap up" work. Tell them it's fictional and they can delete it whenever they like.

Then give them these three lines to keep:

- Start a session: **"Read AGENTS.md, then let's work on [matter]."**
- End a session: **"Wrap up."**
- When I get something wrong: correct me and say **"remember that."**

## Step 6: Finish

- Summarize in five lines or fewer what you set up.
- Remind them that everything drafted here is for attorney review, and that whether to
  put confidential client information into their AI app is a decision about their
  provider's data terms and their ethics rules, which this workspace doesn't settle.
- Ask what they'd like to work on first.
