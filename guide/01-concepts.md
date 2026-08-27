# 1. Key Concepts

A few terms before we touch anything. It's fine if these don't fully click
yet — they'll make more sense once you've done them.

## Git vs. GitHub

- **Git** is a program that runs on your computer and keeps a history of
  changes to a folder of files. It works entirely offline.
- **GitHub** is a website that hosts copies of those folders online, so you
  can back them up, share them, and collaborate with other people.

You could use Git without ever touching GitHub. But GitHub is what makes it
easy to publish your work and collaborate with others, so that's our focus
today.

## Why plain text?

Git is built to track changes *line by line* in plain text files — Markdown
(`.md`), plain text (`.txt`), CSV, code, and so on. That's why everything in
this tutorial is a `.md` file: Git can show you exactly which lines changed,
and can usually combine two people's edits automatically. It can technically
store a Word doc or a PDF too, but it can only tell you "this binary file
changed" — not what changed inside it, and it can't merge two people's edits
to one. Right tool for the job.

## Vocabulary

- **Repository ("repo")** — a folder that Git is keeping a history of. Can
  live on your computer, on GitHub, or both.
- **Commit** — a saved snapshot of your changes, with a short message
  describing what you did. Think of it like a labeled save point.
- **Push / Pull** — sending your commits up to GitHub (*push*), or bringing
  down commits someone else made (*pull*).
- **Clone** — making a local copy of a GitHub repository on your own
  computer, connected so you can push and pull from it.
- **Fork** — making your *own* copy of *someone else's* GitHub repository,
  under your account, so you can propose changes without needing permission
  to edit the original.
- **Branch** — a parallel version of the repo where you can make changes
  without affecting the main version until you're ready.
- **Pull Request ("PR")** — a request to merge changes from a branch (often
  on a fork) into another branch (often someone else's repo). It's the
  mechanism for proposing, discussing, and reviewing a change before it
  becomes official.

## The shape of today

You'll do this sequence twice: once alone with your own repository, then once
with a partner across two repositories.

```
create repo → clone it → edit a file → commit → push
                                                    │
                                                    ▼
                          fork a partner's repo → clone → branch →
                          edit → commit → push → open a Pull Request →
                          partner reviews and merges it
```
