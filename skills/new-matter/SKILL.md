---
name: new-matter
description: Open a new client matter folder from the template and fill in what's known. Use when the attorney starts a new client or engagement.
---

# New matter

1. Get the client's last name and a short description. Propose a folder name like
   `lastname-short-description` and confirm it.
2. Check `matters/` for an existing folder for the same client. If one exists, ask
   whether this is a new matter or a continuation.
3. Copy `matters/_template/` to the new folder.
4. If intake notes were provided, save them unchanged in `notes/` as
   `YYYY-MM-DD intake notes.md`, then follow `skills/intake-summary` to fill in
   `matter.md`.
5. Set **Opened** to today, **Status** to `intake`, and **Responsible attorney** from
   `firm/profile.md` unless told otherwise.
6. List every person and organization named. Say: "Please run these names through your
   conflicts check before we go further." You are not the conflicts check.
7. Write **Where we left off** and tell the attorney what you created.
