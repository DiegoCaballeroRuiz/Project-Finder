# Project-Finder (pf)
pf is a small shell script that stores your project directories in a plain text database and opens them in tmux sessions using fzf

## Instalation
Grab the pf file and add the route to its parent directory to your $PATH variable in your shell's rc file, the following is an example for .bashrc:

```bash
export PATH="$HOME/.scripts/pf/:$PATH"
```

Now try running pf or pf help and follow the instructions!

## Features
- Add important projects to a database
- Travel at lightning speed between stored projects
- Create custom and persistent tmux sessions
- Remove old or outdated projects from the database

The following video is a short demonstration of pf alongside tmux popups
![](./assets/Pf-demonstration.mp4)

## Important notes
- pf has no dependencies outside fzf and tmux
- I recommend using pf alongside tmux popups like so:
    ```conf
    bind f display-popup -E "pf"
    ```
