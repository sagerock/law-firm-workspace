---
name: make-a-skill
description: Turn a recurring task into a reusable skill in this workspace. Use when the attorney says "make this a skill" or a task has repeated.
---

# Make a skill

1. Ask, or infer from the session: what's the task, when does it come up, and what
   does a good result look like? If you just did the task, use what worked and every
   correction the attorney made.
2. Pick a short lowercase name with hyphens, like `engagement-letter`.
3. Create `skills/<name>/SKILL.md` in this format:

   ```
   ---
   name: <name>
   description: <what it does>. Use when <the phrases or situations that trigger it>.
   ---

   # <Title>

   1. Numbered steps, written as instructions to the AI.
   ```

4. Rules for good skills:
   - Steps the AI can follow without asking what was meant.
   - Point to `firm/` files instead of copying their content.
   - No client names or facts. Use placeholders.
   - Say what gets saved and where.
   - Mark law-dependent steps `[verify]`.
5. Show the draft to the attorney and adjust it.
6. Add a row to the table in `skills/README.md`.
