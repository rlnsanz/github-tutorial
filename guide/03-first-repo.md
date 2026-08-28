# 3. Your First Repository

We'll create a repository on GitHub, bring it down to your laptop, make a
change, and publish it back.

## Create the repository on GitHub

1. Go to [github.com](https://github.com) and click the **+** in the top
   right, then **New repository**.
2. Name it something like `firstname-lastname-notes`.
3. Leave it **Public** (so your partner can find it later).
4. Check **Add a README file**.
5. Click **Create repository**.

You now have a repository that exists only on GitHub's servers. Next we bring
it down to your computer.

## Clone it into VS Code

1. Open VS Code.
2. Press `Cmd + Shift + P` to open the Command Palette, type `Git: Clone`,
   and select it.
3. Choose **Clone from GitHub**. If prompted, sign in (see
   [Setup](02-setup.md#5-sign-in-to-github-inside-vs-code)).
4. Find and select the repository you just created.
5. Pick a folder on your computer to save it in — your Desktop or Documents
   folder is fine.
6. When VS Code asks if you'd like to open the cloned repository, click
   **Open**.

You now have a local copy, connected to the one on GitHub.

## Make a change

1. In the file explorer on the left, click `README.md` to open it.
2. Add a line about yourself — who you are, what you're working on, whatever
   feels natural. Save the file (`Cmd + S`). `.md` files have special formatting that you can use to create tables, headlines and much more. Check out https://www.markdownguide.org/basic-syntax/ for the syntax. 

Now we're going to make a labeled checkpoint (commit) and save it on github's servers (push).

## Commit and push

1. Click the **Source Control** icon in the left sidebar (looks like a branch
   with dots — or press `Ctrl + Shift + G`).
2. You'll see `README.md` listed under **Changes**. Hover over it and click
   the **+** to stage it.
3. In the message box at the top, write a short commit message, e.g.
   `Add intro to README`.
4. Click the checkmark (**Commit**) button.
5. Click **Sync Changes** (or **Publish Branch**, if this is your first
   commit) to push it up to GitHub.

## Confirm it worked

Go back to your repository's page on GitHub.com and refresh. You should see
your change in `README.md`, and a commit history showing your message.

> **Curious what VS Code just did for you?** Those same three steps are the
> commands `git add README.md`, `git commit -m "Add intro to README"`, and
> `git push` — typed into the Terminal instead of clicked. Same result,
> different interface. Feel free to try it in Terminal if you're curious.

---

Next: [4. Pair Exercise — Fork and Pull Request](04-pair-exercise.md).
