# Tmux simple git status

Prints current pane git branch and uncommitted changes (if available). Forked from
[kristijanhusak/tmux-simple-git-status](https://github.com/kristijanhusak/tmux-simple-git-status).
Includes the number of untracked files in addition to all original stats.

Outputs:

* active branch
* number of changed files
* number of inserted lines
* number of deleted lines
* number of untracked files

## Installation
### Installation with [Tmux Plugin Manager](https://github.com/tmux-plugins/tpm) (recommended)

Add plugin to the list of TPM plugins in `.tmux.conf`:

    set -g @plugin 'iacsa/tmux-simple-git-status'

Add `#{simple_git_status}` to your `status-left` or `status-right` tmux option:

```
set -g status-left "#{simple_git_status}"
```

Hit `prefix + I` to fetch the plugin and source it.

