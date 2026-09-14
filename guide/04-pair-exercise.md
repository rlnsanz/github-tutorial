# 4. Pair Exercise — Fork and Pull Request

Find a partner near you. Together, you'll propose, review, and merge **one pull
request** using the repositories you created in
[3. Your First Repository](03-first-repo.md).

## Choose your roles

Pick roles, or flip a coin:

- **Proposer:** fork the reviewer's repository, make a change, and open a pull request.
- **Reviewer:** share your repository, review the proposed change, merge it, and
  pull the result onto your laptop.

The proposer uses their laptop for steps 2–7 while the reviewer follows along.
For steps 8–9, the reviewer uses their laptop while the proposer follows along.
Talk through what you're doing and check in before moving to the next step.
Keep your chosen roles throughout the pair exercise and the optional contribution
below.

## 1. Share the reviewer's repo URL — together

The reviewer shares the URL of the repository they created in the last
section (e.g. `https://github.com/reviewer-username/their-notes`).

The proposer will make a copy under their own GitHub account, called a **fork**.
This lets them make changes without needing permission to edit the reviewer's
repository directly.

## 2. Fork it — proposer

1. Open the reviewer's repository page on GitHub.com.
2. Click **Fork** (top right), then **Create fork**.

You now have your own copy of their repo, under your account. This is
separate from their copy — changes here reach their repository only when your
pull request is merged.

## 3. Clone your fork into VS Code — proposer

Same as before, but this time pick **your fork** (it'll be under your
username, not theirs):

1. `Cmd + Shift + P` → `Git: Clone` → **Clone from GitHub**.
2. Select your fork of your partner's repo.
3. Choose a folder, then **Open** when prompted.

Next, create a branch in your fork. A branch lets you work on a change within a
repository; a fork is a separate repository under your account.

## 4. Create a branch — proposer

1. Click the branch name in the bottom-left corner of VS Code (it'll say
   `main`).
2. Choose **Create new branch**, and give it a name like `add-a-note`.

Working in a branch keeps your change separate until it's reviewed.

## 5. Make a change — proposer

Open `README.md` and add a short note, comment, or question addressed to your
partner — e.g. a line under a new `## Note from <your name>` heading. Save
the file.

## 6. Commit and push the branch — proposer

1. Open **Source Control**, stage the change, write a commit message, and
   commit — same as before.
2. Click **Publish Branch**. This pushes your new branch to *your fork* on
   GitHub (not your partner's repo — you don't have permission to push there
   directly, which is exactly why we're using a Pull Request).

## 7. Open a pull request — proposer

1. Go to GitHub.com — it will likely show a banner offering to
   **Compare & pull request**. Click it. (If not, go to your partner's
   original repository and click **Pull requests → New pull request →
   compare across forks**, then pick your fork and branch.)
2. Confirm the base repository is the **reviewer's** repo and the base branch is
   `main`. The head repository should be **your fork**, with `add-a-note` selected
   as the compare branch.
3. Add a title and description, then click **Create pull request**.
4. Share the pull request URL with the reviewer.

## 8. Review and merge — reviewer

On your laptop, open the link the proposer shared, or find the pull request in
your original repository's **Pull requests** tab.

1. Open the PR and click the **Files changed** tab to see exactly what
   changed, line by line.
2. Explain the change to your partner in your own words. Leave a comment if you
   like — click the `+` next to a line.
3. If it looks good, click **Merge pull request**, then **Confirm merge**.

## 9. Pull the merge down locally — reviewer

Back in VS Code, open your own repository from the previous exercise, switch to the
`main` branch (bottom-left branch selector) and click **Sync Changes** to
pull down the merged change. Open `README.md` and confirm together that the
proposer's note is there.

Together, you've completed a full collaboration loop: fork, branch, commit,
push, pull request, review, merge, pull.

## Finished early? Contribute to the workshop repository

Keep the same proposer and reviewer. Together, add a useful resource for
journalists, researchers, or social scientists to
[the workshop repository](https://github.com/rlnsanz/github-tutorial).

1. The proposer forks the workshop repository into their own GitHub account
   and clones that fork into VS Code, as in steps 2–3.
2. Create a branch named `add-resource`.
3. In VS Code's file explorer, open the `contributions` folder and create a file
   named `your-github-username.md`, replacing the placeholder with your username.
   If that file already exists, use `your-github-username-2.md` instead. Each pair
   uses its own file to avoid editing the same lines.
4. Add the resource's name, a link, and one sentence explaining why it's useful.
   See the [contribution example](../contributions/README.md).
5. Save, stage, commit, and publish the branch, as in step 6.
6. Open a pull request with `rlnsanz/github-tutorial` as the base repository and
   its default branch as the base branch. Select your fork and `add-resource` as
   the head repository and compare branch. Give the PR a title such as
   `Recommend a resource: <resource name>`.
7. Share the PR link with your partner. The reviewer opens **Files changed**,
   checks the recommendation and link, and leaves a comment with feedback.
8. Show the PR to a facilitator, who can review and merge it. You don't need to
   wait for the merge to finish this optional exercise.

Completing one pull request with your partner in steps 1–9 is the main goal.
This contribution is an optional way to practice on a shared project.

---

Hit an error somewhere in there? Check
[5. When Things Go Wrong](05-troubleshooting.md).
