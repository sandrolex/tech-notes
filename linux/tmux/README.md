## TMUX
* [Cheat Sheet](https://tmuxcheatsheet.com/)
* [tpm](https://github.com/tmux-plugins/tpm) plugin manager

list sessions

    tmux ls

detach session

    C-b d

attach session

    tmux a -t [session-name]

* [tmux nord theme](https://www.nordtheme.com/docs/ports/tmux/installation)
 

### config file (~/.tmux.conf)
    set -g @plugin 'tmux-plugins/tpm'
    set -g @plugin 'tmux-plugins/tmux-sensible'

    #set -g @plugin "arcticicestudio/nord-tmux"

    # Other examples:
    # set -g @plugin 'github_username/plugin_name'
    # set -g @plugin 'git@github.com:user/plugin'
    # set -g @plugin 'git@bitbucket.com:user/plugin'

    # Initialize TMUX plugin manager (keep this line at the very bottom of tmux.conf)
    run '~/.tmux/plugins/tpm/tpm'
