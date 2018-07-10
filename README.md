# .tmux

## Cheatsheets

* Ctrl+b "         # split pane horizontally.
* Ctrl+b %         # split pane vertically.
* Ctrl+b c         # (c)reate a new window.
* Ctrl+b n         # move to the (n)ext window.
* Ctrl+b p         # move to the (p)revious window.
* <C-b> I          # Install plugins
* <C-b> R          # reload tmux config
* <C-b> d          # detach current session
* <C-b> c          # create new session
* <C-b> ?          # help
* <C-b> $          # rename session
* <C-b> ,          # rename window
* <C-b> s          # list session
* <C-b> w          # list window
* <C-b> t          # show time
* Ctrl+b arrow key # switch pane.
* Hold Ctrl+b, don't release it and hold one of the arrow keys # resize pane.


- C-a left      # go to the next pane on the left
- C-a right     # (or one of these other directions)
- C-a up
- C-a down
- C-a o         # go to the next pane (cycle through all of them)
- C-a ;         # go to the ‘last’ (previously used) pane

- C-a x         # kill the current pane
- C-a q         # display pane numbers for a short while


## Build from source code

### prepare

```shell
$ sudo apt install build-essential automake pkg-config libevent-dev libncurses5-dev
```

```
$ git clone https://github.com/tmux/tmux.git
$ cd tmux
$ sh autogen.sh
$ ./configure && make

$ sudo cp tmux /usr/local/bin/
```

```
$ ln -s ~/.tmux/.tmux.conf ~/
```


## ref
- <https://lukaszwrobel.pl/blog/tmux-tutorial-split-terminal-windows-easily/>
- <https://unix.stackexchange.com/questions/12032/how-to-create-a-new-window-on-the-current-directory-in-tmux>
