# Catch Up, Explore, and Ask Questions

Take these five minutes at your own pace. Finish a step, try something new,
or talk through a question with your partner or a facilitator. Choose what
helps you most; you don't need to complete everything on this page.

- [Still working? Pick up where you left off.](#catch-up)
- [Finished early? Choose something to explore.](#explore-a-little-more)
- [Something isn't working? Check the common pitfalls.](#common-pitfalls)

## Catch up

Use this time to finish the exercise you’re on. If you’re stuck, wave down
Rolando or Rosty.

## Explore a little more

Pick one activity, on your own or with your partner:

- **Read your history.** Open your `workshop-notes` repository's commit
  history on GitHub and select your earlier commit. Find the line you added.
  How does the commit message help explain the change?
- **Experiment on a branch.** A branch lets you develop changes separately.
  A team might use `main` for accepted work, `prod` for the version in use,
  and `dev` for development; those roles are team conventions. Try keeping
  an experiment separate from `main`:

  1. Open your own `workshop-notes` folder in VS Code with no uncommitted
     changes. Open **Terminal → New Terminal** and run:

     ```sh
     git switch -c dev main
     ```

     This creates and switches to `dev`, starting from `main`.
  2. Add `This line was a mistake.` to `README.md`. Save, stage, and commit
     just this change. Keep this experiment local: skip publishing or syncing.
  3. Start again from the good version on `main`:

     ```sh
     git switch -c dev2 main
     ```

     Look at `README.md`: the mistaken line is gone. `dev2` starts from
     `main`, which never received the experimental commit.
  4. Delete the abandoned local branch:

     ```sh
     git branch -D dev
     ```

     `-D` deletes the branch even though its work wasn't merged. Use it here
     because `dev` contains only the experiment you're choosing to discard.

  You can now try a different change on `dev2`. Deleting a branch doesn't
  undo changes already merged into `main` or `prod`.
- **Try a longer extension.** Start the optional “Finished early?” activity
  at the end of the [Pair Exercise](04-pair-exercise.md): recommend a
  resource by opening a pull request to the workshop repository. You can
  continue this after the workshop.

This is also time for questions about your own work: what might you track in
a repository, and who might you collaborate with? For more to try later,
see [Resources](06-resources.md).

## Common pitfalls

Wave down Rolando or Rosty anytime. These fixes are here as a handy reference.

### "Please tell me who you are" when committing

Git doesn't know your name/email yet. Run in Terminal:

```
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

Then try the commit again.

### VS Code shows red `<<<<<<<` and `>>>>>>>` markers in a file

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
3. Save, then stage and commit the file as usual. This records your
   resolution.

### "Updates were rejected because the remote contains work that you do not have"

Someone else pushed changes since you last pulled. Click **Sync Changes**
(or **Pull**) in VS Code first to bring those changes down, resolve any
conflicts as above, then push again.

### "Permission denied" or "403" when pushing

You may be trying to push to someone else's repository, or be signed in
with a different GitHub account.

### I don't see my partner's Pull Request

Make sure you're looking at the **original** repository's Pull Requests tab
(`workshop-notes`), not your partner's fork. 

---

Wrap up with [Resources](06-resources.md).
