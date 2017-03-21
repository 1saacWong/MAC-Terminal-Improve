# Cheatsheet to improve the Mac Terminal colour for readibility

Open **Terminal** and type `nano .bash_profile`

**Paste**:

```
export PS1="\[\033[36m\]\u\[\033[m\]@\[\033[32m\]\h:\[\033[33;1m\]\w\[\033[m\]\$ "
export CLICOLOR=1
export LSCOLORS=ExFxBxDxCxegedabagacad
alias ls='ls -GFh'
```

`Control+O` to **save**, then `Control+X` to **exit**.

- [x] Explanation:
> The first line changes the bash prompt to be colourised, and the prompt to be `username@hostname:cwd $`

> **alias ls** includes flags by default. **-G** colourises output, **-h** adjusts to human readable size, and **-F** displays @ after a symlink,  / after a directory and * after an executable.

## Extra

Click **Terminal** menu and choose **Preferences** then **Settings**.
Go to ** profile/theme** then **Text**. Activate **Use bold fonts** and **Use bright colours for bold text**.

Adjust **Color & Effects** for background colour. Set opacity at 80% and blur at 100%.

