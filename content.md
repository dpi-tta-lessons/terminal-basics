# Terminal Basics

## Goal

By the end of this lesson, you’ll be able to open a terminal, move between folders, list files, and use handy shortcuts to work faster. Try each step in your own terminal as you go.

## 1. Open the Terminal

You can use the terminal in your codespace or on your computer.

- Mac: Press ⌘ + Space, type Terminal, hit Enter.
- Windows: Press Win + R, type cmd or powershell, hit Enter.
- Linux: Press Ctrl + Alt + T or find "Terminal" in your applications menu.

## 2. Where Am I?
 
Use `pwd` to print your current working directory.

```bash
pwd
```

### Expected Output (Mac/Linux):

```bash
/Users/yourname
```

### Expected Output (Windows):

```makefile
C:\Users\yourname
```

<aside class="why">
  <strong>Why this works:</strong> <code>pwd</code> stands for "print working directory". It tells you where you are in the file system.
</aside>

## 3. List Files and Folders

Use `ls` (or `dir` on Windows) to see what’s in your current folder.

```bash
ls
```

Expected Output:

```nginx
Desktop  Documents  Downloads  Music  Pictures
```

<aside class="tip">
  <strong>Windows users:</strong> Use <code>dir</code> instead of <code>ls</code> for now.
</aside>

## 4. Change Directory

Use `cd` followed by a folder name to move into it:

```bash
cd Documents
```

Then use `pwd` again to confirm where you are.

```bash
pwd
```

Expected Output:

```bash
/Users/yourname/Documents
```

## 5. Go Up One Folder

Use `cd ..` to move back to the parent directory:

```bash
cd ..
```

Then check your location again:

```bash
pwd
```

## 6. Make a Folder

Create a new folder with `mkdir`:

```bash
mkdir my-first-folder
```

Then check it’s there:

```bash
ls
```

## 7. Go Into the New Folder

```bash
cd my-first-folder
```

You’re now inside your new folder!

## 8. Handy Terminal Shortcuts

These shortcuts will save you time as you use the terminal more:

| Shortcut       | What It Does                             |
| -------------- | ---------------------------------------- |
| ↑ (Up Arrow)   | Scroll through previous commands         |
| ↓ (Down Arrow) | Scroll forward through command history   |
| Ctrl + C       | Cancel the current command               |
| Tab            | Autocomplete a file or folder name       |
| ⌘ + K          | Clear the terminal screen (like clear)   |
| !!             | Re-run the last command                  |
| touch          | Create (or update timestamp) of a file   |

<aside class="tip">
  Try pressing <code>Up Arrow</code> a few times to see your command history. Then press `Enter` to run one again. 
</aside>

<aside class="warning">
  <code>Ctrl + C</code> is your emergency stop button. Use it if a command freezes or runs too long. 
</aside>

## Practice Challenge

Try This:

- Go back to your home directory.
- Create a folder called `practice-terminal`.
- Inside it, create another folder called `subfolder`.
- Navigate into subfolder and use `pwd` to verify your path.
- Try using the `Up Arrow` to repeat the `mkdir` and `cd` commands.
- Use `⌘ + K` to clear your screen.

## Wrap-Up

You’ve learned how to:

- Open the terminal
- Find out where you are with `pwd`
- List files using `ls` or `dir`
- Move between folders with `cd`
- Create folders with `mkdir`
- Use shortcuts like `Up Arrow`, `Tab`, and `Ctrl + C`

<aside class="tip">
  <strong>Next step:</strong> Learn how to create and edit files from the terminal!
</aside>

## Quiz

- What command shows your current location in the terminal?
- pwd
  - Correct! `pwd` shows your current working directory.
- cd
  - Not quite. `cd` changes the directory.
- mkdir
  - Nope! That one creates directories.
{: .choose_best #current_directory title="Current Directory Command" answer="1"}

- Which of the following are valid terminal commands?
- cd
  - Correct! `cd` changes your location.
- ls
  - Correct! `ls` lists files in the current directory.
- start
  - Not usually. This works on some systems to open apps, but isn’t universal for navigation.
- make
  - Not correct. `make` is an advanced tool, not for basic file/folder tasks.
{: .choose_all #valid_commands title="Basic Terminal Commands" answer="[1,2]"}

- What does `Ctrl + C` do in the terminal?
- Runs the last command
  - Not quite. That’s what `!!` does.
- Clears the screen
  - Close! That's `Ctrl + L`.
- Stops a running command
  - Correct! `Ctrl + C` is your go-to for quitting a stuck or long-running process.
{: .choose_best #ctrl_c title="Interrupting Commands" answer="3"}
