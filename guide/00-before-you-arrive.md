# Before You Arrive

We'll cover this together at the start of the session (see [Setup](02-setup.md)).
If you'd like to save yourself a few minutes on the day, or already have a
GitHub account, feel free to do some or all of this ahead of time.

## Create a GitHub account

1. Go to [github.com](https://github.com) and click **Sign up**.
2. Use whatever email address you're comfortable using for this&mdash;personal or
   school, either is fine.
3. Pick a username you're comfortable sharing publicly and using beyond
   this workshop.

## Install and Launch VS Code

We'll use [Visual Studio Code](https://code.visualstudio.com/) (VS Code) as our
editor. It has a built-in Terminal and Git controls to make working with files
easier. You'll also need to install Git, as described below.

### macOS

1. Go to [code.visualstudio.com](https://code.visualstudio.com/) and download
   the Mac version.
2. Open the downloaded file and drag **Visual Studio Code** into your
   **Applications** folder.
3. Open it once from Applications to confirm it launches.

### Windows

Follow the Windows instructions in
[Setup: Install VS Code](02-setup.md#2-install-vs-code-skip-if-you-already-have-it),
including the installer options listed there. Open VS Code once to confirm it
launches.

## Install Git

### macOS: Install the Xcode Command Line Tools

This is what actually puts the `git` program on your Mac. It's a few hundred
megabytes and can take 10+ minutes on slower connections. Doing it in advance means less waiting during the session, but we've built time in either way.

1. Open **Terminal** (press `Cmd + Space`, type `Terminal`, hit Enter).
2. Type the following and press Enter:

   ```
   git --version
   ```

3. If Git isn't installed yet, a dialog will pop up offering to install the
   "Command Line Developer Tools." Click **Install** and accept the license.
4. Once it finishes, run `git --version` again — you should see something like
   `git version 2.39.3`.

### Windows

Follow the Windows instructions in [Setup: Install Git](02-setup.md#3-install-git),
including the editor and terminal choices shown in the screenshots. Then
[confirm Git is installed](02-setup.md#4-confirm-git-is-installed) using PowerShell.

We'll configure Git and sign in to GitHub in VS Code together during Setup.

If you get stuck on any of this, don't worry. We'll finish it together at the start of the session. 

## Next

See [guide/02-setup.md](02-setup.md).
