# 5. When Things Go Wrong

Common hiccups and how to fix them. If none of these match what you're
seeing, wave down the facilitator.

## "Please tell me who you are" when committing

Git doesn't know your name/email yet. Run in Terminal:

```
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Then try the commit again.

## VS Code shows red `<<<<<<<` and `>>>>>>>` markers in a file

This is a **merge conflict** — it happens when two people changed the same
lines and Git can't automatically combine them. It's not broken; it just
needs a decision from you.

1. Open the file. You'll see something like:

   ```
   <<<<<<< HEAD
   your version of the line
   =======
   their version of the line
   >>>>>>> their-branch-name
   ```

2. Edit the file by hand to keep whichever version (or a combination) you
   want, and delete the `<<<<<<<`, `=======`, and `>>>>>>>` marker lines
   entirely.
3. Save, then stage and commit the file as usual — this records your
   resolution.

## "Updates were rejected because the remote contains work that you do not have"

Someone else pushed changes since you last pulled. Click **Sync Changes**
(or **Pull**) in VS Code first to bring those changes down, resolve any
conflicts as above, then push again.

## I committed to `main` but meant to make a branch first

No harm done for this workshop — but going forward: create your branch
*before* editing, using the branch selector in the bottom-left of VS Code.
If you want to move an already-made commit onto a new branch, ask the
facilitator — it's a quick fix but easy to get wrong solo.

## "Permission denied" or "403" when pushing

You're likely trying to push directly to someone else's repository instead
of your fork of it. Double check the remote — in VS Code's Source Control
panel, the repository name shown should be *your* fork
(`your-username/their-repo`), not theirs directly. If it's not, re-clone
using the fork URL from your own GitHub account.

## I don't see my partner's Pull Request

Make sure you're looking at the **original** repository's Pull Requests tab
(the one you own), not your partner's fork. PRs opened against your repo
show up there even though the branch lives on their fork.
