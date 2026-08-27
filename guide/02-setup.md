# 2. Setup

We'll get everyone to the same starting point together — nothing needed in
advance. If you already did some of this in
[Before You Arrive](00-before-you-arrive.md) (or already had a GitHub account
or VS Code installed), skip straight to whichever step you still need.

## 1. Create a GitHub account (skip if you already have one)

1. Go to [github.com](https://github.com) and click **Sign up**.
2. Use whatever email address you're comfortable using for this — personal or
   work, either is fine.
3. Pick a username. It's public and hard to change later, so avoid anything
   too tied to a current employer if you'd rather keep this account portable.

## 2. Install VS Code (skip if you already have it)

We'll use [Visual Studio Code](https://code.visualstudio.com/) (VS Code) as
our editor. It has a built-in Terminal and a built-in Git tool, so it's the
only thing you need to install.

1. Go to [code.visualstudio.com](https://code.visualstudio.com/) and download
   the Mac version.
2. Open the downloaded file and drag **Visual Studio Code** into your
   **Applications** folder.
3. Open it once from Applications to confirm it launches.

## 3. Confirm Git is installed

Open **Terminal** (`Cmd + Space`, type `Terminal`, Enter) and run:

```
git --version
```

If you see a version number, you're set. If a dialog pops up offering to
install the Command Line Developer Tools, click **Install** — this puts the
actual `git` program on your Mac and can take a few minutes, longer on
slower connections. Once it finishes, run `git --version` again to confirm.

## 4. Tell Git who you are

Git attaches a name and email to every commit you make. Set that up now
(swap in your own name and the email you used for GitHub):

```
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

No output means it worked. You can check with:

```
git config --global user.name
git config --global user.email
```

## 5. Sign in to GitHub inside VS Code

1. Open **VS Code**.
2. Click the **Accounts** icon in the bottom-left corner of the window (looks
   like a small person).
3. Choose **Sign in with GitHub**.
4. Your browser will open and ask you to authorize VS Code — click
   **Authorize**.
5. Come back to VS Code — you should see your GitHub username in that same
   corner.

This lets VS Code push and pull on your behalf without you typing a password
every time.

---

Everyone caught up? On to [3. Your First Repository](03-first-repo.md).
