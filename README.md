# konfig

This is **K**yle's c**onfig** setup... konfig :D

# bash_profile

Add parts of this that you want to your `.bash_profile`

```bash
# UPDATE THESE
export KONFIG_ROOT=path/to/konfig

source "$KONFIG_ROOT/bash/prompt"         # minimalistic prompt
source "$KONFIG_ROOT/bash/aliases"        # aliases for general productivity
alias touch="$KONFIG_ROOT/bash/mytouch"   # better touch command

# UPDATE THESE
export DEVSERVER=kad.sb.facebook.com
export DEVSERVER_FBSOURCE="/data/users/kad/fbsource"
export LOCAL_FBSOURCE="~/fbsource"

source "$KONFIG_ROOT/bash/nuclide"        # aliases specific to nuclide
```

### Usage

1. `con` (short for connect) will attempt to connect using `mosh -6 dev`
  1. `con2` for `dev2`, `con3` for `dev3`
2. `tt` attach to an existing tmux session or create a new one

# tmux

Link to the tmux conf in this repository.


```bash
ln -s path/to/konfig/tmux.conf ~/.tmux.conf
```

**TODO:** Would be nice if I could just import my tmux settings somehow, similar to
the sources above. Maybe one day I will look into this a bit more.

### Usage

1. `ctrl+a` allows you to run "tmux" commands
2. `ctrl+a, %` to split horizontally
3. `ctrl+a, "` to split vertically
4. `ctrl+a, x, y/n` to close something
5. `ctrl+a, <number>` to go to a window by number
6. `ctrl+a, c` create a new window
7. Can use the mouse to scroll
  1. For iTerm2: iTerm -> preferences -> profiles -> terminal -> enable
  "Enable xterm mouse reporting"
8. Hold `option` to highlight and copy text in the terminal
