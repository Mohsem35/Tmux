## TMUX Documentation


### Introduction

This documentation provides a guide for using TMUX, a **terminal multiplexer**, on Linux systems. TMUX allows users to create and manage multiple terminal sessions, windows, and panes within a single terminal window or SSH session.
Installation

To install TMUX on your system, use the following command:
```shell
sudo dnf install tmux
```
### Getting Started

#### Starting TMUX

To start TMUX, simply type **`tmux`** in your terminal.

#### Detaching from TMUX

To detach from a TMUX session, press **`Ctrl + b`**, then **`d`**

### TMUX Layers

TMUX operates with three primary layers: **Session**, **Window**, and **Panes**

#### 1. Session

```shell
# create a new session with a specified name
tmux new -s <session_name>

# list all TMUX sessions
tmux ls

# attach to the most recent TMUX session
tmux a

# attach to a specific TMUX session by index number
tmux a -t <index_number>

# kill a TMUX session
tmux kill-session -t <session_name>
```


#### 2. Window

Within a TMUX session, you can create multiple windows, each containing its own shell environment.

```shell
# create a new window
Ctrl + b, then C

# switch between windows
Ctrl + b, then N

# rename a window
Ctrl + b, then ,

# view window details
Ctrl + b, then w

# close a window
Ctrl + b, then &
```

#### 3. Panes

Panes allow you to divide the terminal window into multiple sections, each running its own command or shell.

```shell
# divide the screen vertically
Ctrl + b, then %

# divide the screen horizontally
Ctrl + b, then "

# navigate between panes
Ctrl + b, then arrow(right, left, up, down) keys

# increase/decrease pane size
Ctrl + b, then continuous keypress on arrow keys

# equalize pane sizes vertically
Ctrl + b, then Alt + 1

# equalize pane sizes horizontally
Ctrl + b, then Alt + 2

# close a pane
Ctrl + b, then X
```
### Conclusion

TMUX is a powerful tool for managing terminal sessions, windows, and panes efficiently. With the commands provided in this documentation, you can make the most out of TMUX's capabilities. Experiment with different layouts and configurations to suit your workflow preferences.

TMUX is a powerful tool for managing terminal sessions, windows, and panes efficiently. With the commands provided in this documentation, you can make the most out of TMUX's capabilities. Experiment with different layouts and configurations to suit your workflow preferences.
