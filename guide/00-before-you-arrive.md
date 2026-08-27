# 0. Before You Arrive

Three things to do ahead of the session so we don't spend the first 20 minutes
waiting on downloads.

## Create a GitHub account

1. Go to [github.com](https://github.com) and click **Sign up**.
2. Use whatever email address you're comfortable using for this — personal or
   work, either is fine.
3. Pick a username. It's public and hard to change later, so avoid anything
   too tied to a current employer if you'd rather keep this account portable.

## Install Visual Studio Code

We'll use [Visual Studio Code](https://code.visualstudio.com/) (VS Code) as our
editor. It has a built-in Terminal and a built-in Git tool, so it's the only
thing you need to install.

1. Go to [code.visualstudio.com](https://code.visualstudio.com/) and download
   the Mac version.
2. Open the downloaded file and drag **Visual Studio Code** into your
   **Applications** folder.
3. Open it once from Applications to confirm it launches.

## Install the Xcode Command Line Tools

This is what actually puts the `git` program on your Mac. It's a few hundred
megabytes and can take 10+ minutes on slower connections, so please do this
before the session rather than during it.

1. Open **Terminal** (press `Cmd + Space`, type `Terminal`, hit Enter).
2. Type the following and press Enter:

   ```
   git --version
   ```

3. If Git isn't installed yet, a dialog will pop up offering to install the
   "Command Line Developer Tools." Click **Install** and accept the license.
4. Once it finishes, run `git --version` again — you should see something like
   `git version 2.39.3`.

If you get stuck on any of this, don't worry — we'll have time at the start of
the session to help everyone get set up. See [guide/02-setup.md](02-setup.md).
