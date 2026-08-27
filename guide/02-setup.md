# 2. Setup Check

Quick round of checks before we start building. If you did
[Before You Arrive](00-before-you-arrive.md) already, this should take two
minutes. If not, follow along here.

## 1. Confirm Git is installed

Open **Terminal** (`Cmd + Space`, type `Terminal`, Enter) and run:

```
git --version
```

If you see a version number, you're set. If a dialog pops up offering to
install the Command Line Developer Tools, click **Install** — this can take a
few minutes.

## 2. Tell Git who you are

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

## 3. Sign in to GitHub inside VS Code

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
