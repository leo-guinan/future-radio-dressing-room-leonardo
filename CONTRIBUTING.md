# Changing Leonardo

Leonardo is a character in Future Radio, and you can help shape them. If something in an
episode didn't ring true — or rang so true it should become canon — propose it here.

## Three ways in

1. **Talk to Leonardo first.** Load them locally and see how they respond:

   ```bash
   git clone <this repo> && cd <this repo>
   npx github:leo-guinan/future-radio-character-bible chat .
   ```

   In the chat, `/propose <your note>` writes a viewer note file with the last few
   lines of your conversation attached. Commit it on a branch and open a pull request.

2. **Add a viewer note** — the usual route. Create
   `memory/viewer-notes/YYYY-MM-DD-short-title.md`:

   ```markdown
   ---
   from: your name or handle (or "anonymous")
   experience: what you watched or heard — the episode, the scene, the moment
   episode: E02
   ---
   What should be true about Leonardo from now on, in a sentence or two.
   ```

3. **Edit CHARACTER.md** — for changes to who Leonardo *is*: their job, constraints, or
   recurring conflict. These get the closest review.

No GitHub account? Open an issue with the "Viewer note" form instead.

## What can't change in a pull request

- `history/` and `history.jsonl` are the record of what Leonardo actually did in the
  writers' room. They're written by the room only.
- `memory/notes.md` is append-only. Respond to an old note with a new one.
- `bible/` is generated from everything else. Leave it out of your PR; it's rebuilt on merge.

A check runs on every pull request and explains anything it rejects. Merged notes become
canon: they appear in Leonardo's bible and in the next episode the showrunner projects them into.
