# stmux

`stmux` is a script to create tmux session.

Session name is based on current directory.

Config file is a bash file named `.tmux_session` and placed inside your project directory.

## Run

add `stmux` to your `$PATH` for easier use.

```bash
$ cp .tmux_session.example my_project/.tmux_session
$ stmux
# window with three horizonal panes should be open
```

## Add .tmux_session to ignore file

You may want to add `.tmux_session` to your global ignore file for git or other scm.

## inside tmux session 

When you are in tmux session, it will create detached session and will run `switch-client`.

## Based on

- Brian P. Hogan - tmux 2 Productive Mouse-Free Development-Pragmatic Bookshelf (2017), chapter Creating a Custom Setup with tmux Commands
- Attach or create tmux session named the same as current directory.
  - https://github.com/thoughtbot/dotfiles/blob/master/bin/tat
  - https://thoughtbot.com/upcase/videos/tmux-navigation
- https://stackoverflow.com/questions/16398850/create-new-tmux-session-from-inside-a-tmux-session/34778112#34778112
