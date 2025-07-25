# Learn the Terminal: Navigate Your Computer Like a Developer

The terminal gives you powerful control over your computer. Whether you're installing software, running programs, or managing files, learning the terminal helps you move faster and work like a developer.

## Goal

Goal
By the end of this lesson, you'll be able to open a terminal, move between folders, view files, create directories, and use keyboard shortcuts to work faster. You'll create and navigate a practice workspace on your computer using the terminal, no mouse needed.

## 1. Open the Terminal

Choose one:

- Codespace: Create a repo using the [static html template](https://github.com/dpi-tta-projects/static-html-template).
- Mac: Press ⌘ + Space, type `Terminal`, hit Enter.
- Windows: Press Win + R, type `cmd` or `powershell`, hit Enter.
- Linux: Press Ctrl + Alt + T or find "Terminal" in your applications menu.

## 2. Where Am I?

Use `pwd` to print your current working directory.

```bash
pwd
```

### Expected Output (Mac/Linux)

```bash
/Users/yourname
```

### Expected Output (Windows PowerShell)

```powershell
C:\Users\yourname
```

<aside class="why">
  <strong>Why this works:</strong> <code>pwd</code> stands for "print working directory". It tells you where you are in the file system.
</aside>

## 3. What's Inside This Folder?

Use `ls` to see what's in your current folder.

```bash
ls
```

Expected Output:

```nginx
Desktop  Documents  Downloads  Music  Pictures
```

### Extras

- `ls -l`: Show detailed info like size, owner, and permissions.
- `ls -a`: Show all files, including hidden ones like .git.

## 4. Move Into a Folder

To go into a folder use `cd`. For example:

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

Then check it's there:

```bash
ls
```

Go Into the New Folder

```bash
cd my-first-folder
```

You're now inside your new folder!

## 7. Create a File

To create an empty file:

```bash
touch hello.txt
```

Check it's there:

```bash
ls
```

<aside class="why">
  <strong>Why this works:</strong> <code>touch</code> creates a file if it doesn't exist or updates the timestamp if it does.
</aside>

## 8. View and Change Permissions

Let's see the file's permissions:

```bash
ls -l
```

To make it executable (example):

```bash
chmod +x hello.txt
```

<aside class="tip">
  <strong>Tip:</strong> Use this for shell scripts later on! For now, just try it out.
</aside>

## 9. View Help for Any Command

<!-- TODO: screenshot -->

You can read built-in help docs for any command. To see the 'manual' for `ls` type:

```bash
man ls
```

To exit the manual, press `q`.

## 10. Clear the Terminal

<!-- TODO: screenshot video -->

To clean up your screen:

```bash
clear
```

Or on Mac:

```bash
⌘ + K
```

<!-- 

## 11. Exiting vi or a Stuck Command



If you accidentally open a file in `vi`, here's how to escape:

- Press Esc
- Type `:q!`
- Hit Enter

<aside class="warning">
  <code>vi</code> is a powerful editor, but can be confusing at first. Don't worry, you'll learn it later.
</aside> 

-->

<!-- TODO

| Option + → / ← (Mac) | Jump one word at a time in the command line |
| Ctrl + → / ← (Linux/Win)	Same as above: move by word instead of letter

 -->

## 11. Terminal Shortcuts You'll Use Constantly

These shortcuts will save you time as you use the terminal more:

| Shortcut       | What It Does                             |
| -------------- | ---------------------------------------- |
| ↑ (Up Arrow)   | Scroll through previous commands         |
| ↓ (Down Arrow) | Scroll forward through command history   |
| Ctrl + C       | Cancel the current command               |
| Tab            | Autocomplete a file or folder name       |
| ⌘ + K          | Clear the terminal screen (like clear)   |
| !!             | Re-run the last command                  |


<!-- TODO: add demo video -->
<aside class="tip">
  Try pressing <code>Up Arrow</code> a few times to see your command history. Then press `Enter` to run one again.
</aside>


<!-- TODO: add demo video -->
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

You've learned how to:

- Open the terminal
- Find out where you are with `pwd`
- List files using `ls` or `dir`
- Move between folders with `cd`
- Create folders with `mkdir`
- Use shortcuts like `Up Arrow`, `Tab`, and `Ctrl + C`

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
  - Not usually. This works on some systems to open apps, but isn't universal for navigation.
- make
  - Not correct. `make` is an advanced tool, not for basic file/folder tasks.
{: .choose_all #valid_commands title="Basic Terminal Commands" answer="[1,2]"}

- What does `Ctrl + C` do in the terminal?
- Runs the last command
  - Not quite. That's what `!!` does.
- Clears the screen
  - Close! That's `Ctrl + L`.
- Stops a running command
  - Correct! `Ctrl + C` is your go-to for quitting a stuck or long-running process.
{: .choose_best #ctrl_c title="Interrupting Commands" answer="3"}

## References

- [Basic Unix Commands](https://mally.stanford.edu/~sr/computing/basic-unix.html)
