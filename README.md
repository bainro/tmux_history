## GOOD TMUX SETTINGS

### Put this into ~/.tmux.conf:
set -g mouse on

### avoid duplicates (~/.bashrc)
export HISTCONTROL=ignoredups:erasedups

### append history entries (~/.bashrc)
shopt -s histappend

### After each command, save and reload history (~/.bashrc)
export PROMPT_COMMAND="history -a; history -c; history -r; $PROMPT_COMMAND"
