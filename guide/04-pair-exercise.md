# 4. Pair Exercise — Fork and Pull Request

Find a partner near you. You'll each propose a change to the *other person's*
repository from [3. Your First Repository](03-first-repo.md), and merge each
other's changes in. Do the steps below at the same time, side by side — it'll
make more sense watching it happen from both ends.

## 1. Get your partner's repo URL

Ask your partner for the URL of the repository they created in the last
section (e.g. `https://github.com/their-username/their-notes`).

## 2. Fork it

1. Open your partner's repository page on GitHub.com.
2. Click **Fork** (top right), then **Create fork**.

You now have your own copy of their repo, under your account. This is
separate from their copy — changes here don't touch theirs until you open a
Pull Request.

## 3. Clone your fork into VS Code

Same as before, but this time pick **your fork** (it'll be under your
username, not theirs):

1. `Cmd + Shift + P` → `Git: Clone` → **Clone from GitHub**.
2. Select your fork of your partner's repo.
3. Choose a folder, then **Open** when prompted.

## 4. Create a branch

1. Click the branch name in the bottom-left corner of VS Code (it'll say
   `main`).
2. Choose **Create new branch**, and give it a name like `add-a-note`.

Working in a branch keeps your change separate until it's reviewed.

## 5. Make a change

Open `README.md` and add a short note, comment, or question addressed to your
partner — e.g. a line under a new `## Note from <your name>` heading. Save
the file.

## 6. Commit and push the branch

1. Open **Source Control**, stage the change, write a commit message, and
   commit — same as before.
2. Click **Publish Branch**. This pushes your new branch to *your fork* on
   GitHub (not your partner's repo — you don't have permission to push there
   directly, which is exactly why we're using a Pull Request).

## 7. Open a Pull Request

1. Go to GitHub.com — it will likely show a banner offering to
   **Compare & pull request**. Click it. (If not, go to your partner's
   original repository and click **Pull requests → New pull request →
   compare across forks**, then pick your fork and branch.)
2. Confirm the base repository is your **partner's** repo and the head is
   your fork's branch.
3. Add a title and description, then click **Create pull request**.

## 8. Swap roles — review and merge

Now find the Pull Request your partner opened against *your* repository
(check your repo's **Pull requests** tab, or the notification GitHub sent
you):

1. Open the PR and click the **Files changed** tab to see exactly what
   changed, line by line.
2. Leave a comment if you like — click the `+` next to a line.
3. If it looks good, click **Merge pull request**, then **Confirm merge**.

## 9. Pull the merge down locally

Back in VS Code, on your *original* repository (not the fork), switch to the
`main` branch (bottom-left branch selector) and click **Sync Changes** to
pull down your partner's merged change.

You've now completed a full collaboration loop: fork, branch, commit, push,
Pull Request, review, merge, pull.

---

Hit an error somewhere in there? Check
[5. When Things Go Wrong](05-troubleshooting.md).
