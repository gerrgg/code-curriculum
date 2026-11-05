# Open a project in Ubuntu

You'll use Bash, the shell in Ubuntu, for the command-line lessons. Windows Subsystem for Linux (WSL) lets you run Ubuntu on your Windows PC. Start with your saved repair-shop page and the Windows version of VS Code. For a new WSL installation you'll need administrator access, an internet connection, and time to restart.

## Check your PC

Open **PowerShell** from Start and run:

```powershell
wsl --list --verbose
```

If Ubuntu is listed with version **2**, skip to **Open Ubuntu**. On a fresh PC, follow the installation step below. If an existing Ubuntu installation shows version 1, follow Microsoft's [version guidance](https://learn.microsoft.com/windows/wsl/install#upgrade-version-from-wsl-1-to-wsl-2) before continuing.

## Install WSL

Save your work. From Start, right-click **PowerShell**, choose **Run as administrator**, then enter:

```powershell
wsl --install -d Ubuntu
```

Restart Windows when prompted. If the installation reports an error, use the exact message to find the matching step in [Microsoft's WSL troubleshooting guide](https://learn.microsoft.com/windows/wsl/troubleshooting).

## Open Ubuntu

Open **Ubuntu** from Start. On first launch, choose a Linux username and password when prompted. The password field stays blank while you type. Press **Enter** to submit it. Back in PowerShell, run `wsl --list --verbose` again and check that Ubuntu now shows version **2**.

Switch back to the **Ubuntu** window. Run these commands one line at a time:

```bash
mkdir -p ~/projects/repair-shop
cd ~/projects/repair-shop
pwd
explorer.exe .
```

The first line creates your project folder inside your Linux home directory. The second enters it. The third prints its location, ending in `/projects/repair-shop`. The last line opens that same folder in Windows File Explorer.

In a second File Explorer window, open the repair-shop folder in Documents. Copy your `index.html` into the Ubuntu folder. From here on, edit the copy in Ubuntu.

## Connect your editor

In Windows VS Code, open **Extensions** with **Ctrl + Shift + X**. Search for **WSL**, choose the extension published by Microsoft, and install it. Close VS Code. In the Ubuntu terminal you used above, run:

```bash
code .
```

The dot means “this folder.” The first connection can take a few minutes. Look for **WSL: Ubuntu** in the lower-left corner of the editor and `index.html` in its Explorer. If the command fails, use the [VS Code WSL setup guide](https://code.visualstudio.com/docs/remote/wsl).

## Check which copy you're editing

In the connected editor, change the Saturday opening time to 10 am and save. In the Ubuntu terminal, run `cat index.html` to print the file. Find the changed time. Open the HTML file from the Ubuntu File Explorer window in your browser and check the same time there.

Close the editor and terminal. Open Ubuntu again and return to the project folder. Open it in VS Code and use the terminal to show where the project lives. You can use the commands above as a reference.

---

[Edit on GitHub](https://github.com/gerrgg/code-curriculum/edit/main/lessons/windows/wsl-workspace.md) · [Report a broken link](https://github.com/gerrgg/code-curriculum/issues/new?title=Broken+link+%E2%80%94+Open+a+project+in+Ubuntu&body=Lesson%3A+lessons%2Fwindows%2Fwsl-workspace.md%0A%0AWhich+link+is+broken%2C+and+what+happened+when+you+opened+it%3F) · [Report an issue or suggestion](https://github.com/gerrgg/code-curriculum/issues/new?title=Lesson+feedback+%E2%80%94+Open+a+project+in+Ubuntu&body=Lesson%3A+lessons%2Fwindows%2Fwsl-workspace.md%0A%0AWhich+step+were+you+on%2C+and+what+would+you+change%3F) · [Lesson change log](https://github.com/gerrgg/code-curriculum/commits/main/lessons/windows/wsl-workspace.md)
