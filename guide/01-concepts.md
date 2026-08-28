# 1. Key Concepts

A few terms before we touch anything. It's fine if these don't fully click
yet — they'll make more sense once you've done them.

## Git vs. GitHub 

- **Git** is a program that runs on your computer and keeps a history of
  changes to a folder of files. It works entirely offline.
- **GitHub** is a website that hosts copies of those folders online, so you
  can back them up, share them, and collaborate with other people. 
  There are many others like gitlab.com, codeberg.org; sometimes companies host their own instances.

You could use Git without ever touching GitHub. But GitHub is what makes it
easy to publish your work and collaborate with others, so that's our focus
today.

## What is plain text, why does it matter?

Git is built to track changes *line by line* in plain text files — Markdown
(`.md`), plain text (`.txt`), CSV, code, and so on; i.e., files that show straightforward text when opened with something like TextEdit. 
Files that require special programs to read (e.g., PDFs, Excel files, images) are binary file types, which aren't supported natively by Git.
That's why everything in this tutorial is a `.md` file (i.e., plain text): Git can show you exactly which lines changed,
and can usually combine two people's edits automatically. While you **technically** can store binary file types, 
Git won't be able to track changes to these files properly - no edit tracking or merging. 
If you **really** need to store binary files, it's best to use Git Large File Storage (LFS), but that's outside the scope of today's lesson. 

## Vocabulary

- **Repository ("repo")** — a folder that Git is keeping a history of. Can
  live on your computer, on GitHub, or both.
- **Commit** — a saved snapshot of your changes, with a short message
  describing what you did. Think of it like a labeled checkpoint you can always refer to in the future.
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
