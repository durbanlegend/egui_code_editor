# terminal

ctrl + z = move to background, run 'fg' to bring it back in current terminal

ctrl + c = clear current line

ctrl + d = kill current terminal window (must have clear current line to work)

# custom scripts

~/kill-tmux.sh

~/start-tmux.sh

# tmux

leader = ctrl + space

## windows
leader - ? = view all shortcuts (arrow keys to navigate, ctrl+s to search, q to quit)

leader - w = search windows

leader - (n from 0-9) = jump to window n

leader - [ = scroll/read mode, q to exit

leader - n = next window

leader - p = previous window

leader - c = create new window

leader - & = kill current window (must confirm with y/n + enter)


## panes

leader - % = split pane horizontally

leader - " = split pane vertically

leader - x = kill pane (must confirm with y/n + enter)

leader - arrow keys = navigate between panels

leader - z = zoom in/out of selected pane

leader - o = cycle through panes on current window

leader - , = rename current window

leader - < window menu?

leader - > pane menu?

leader - : = command menu
    :resize-pane -R/L/U/D 15
        (Right/Left/Up/Down, pick one)

leader - alt + arrow = resize pane (has problems on mac terminals, use above command or modify startup script to set pane size rather)

# nvim

## normal

### to enter visual mode

v = visual mode

V = visual mode (full line)

x/y/d = cut/copy/cut selection

vi" = select everything inside "
vi' = select everything inside '
va' = select everything around '
yVaB = yank entire block enclosing or following cursor
dVaB = cut entire block enclosing of following cursor

### to enter insert mode

a = append after cursor

i = insert before cursor

o = start new line below cursor

O = start new line above cursor

### esc to return to normal mode

u = undo

ctrl + r = redo

:! + [bash command] = run command in terminal

$ = end of line

^ = start of line (equivalient to "0 - w")

gg = go to top of file

G = go to bottom of file

gv - repeat previous selection

[[ or ]] = previous/next function start

{ or } = jump to previous/next empty line

w = next word

e = end of word

b = previous word

r = replace character under cursor with character that follows

cw = change from current cursor position to end of word (will remove up to end of word and drop into insert mode)

y = yank

Y = yank rest of line

x = cut (character in normal mode, selection in visual mode)

dd = cut entire line

p = paste

. - repeat last command

/ = search

n = next matching search (remember to hit enter after search first)

N = previous matching search

* = find matching word under cursor

% = find matching square/curly/regular brace

K = show docs for symbol under cursor

ctrl + ] = jump to definition

ctrl + o = go back from jump to definition

:n + enter = go to line n

[ or ] - b = cycle left/right through open buffers

[ or ] - d = cycle through diagnostics

space - / = comment/uncomment current line/selection

space - ff = find file (ctrl + p/n to scroll back through search history, ctrl+j/k or tab/shift to navigate to next/previous result)

space - fw = find word in working dir

space - fb = find open buffer

space - ft = find theme/colour scheme

space - lD = view all diagnostics

ESCAPE TWICE TO EXIT ANY OF THE ABOVE

space - ld = show full detail on diagnostic

space - la = show available code actions (cursor must be at exact character where diagnostic tag starts)

space - o = toggle focus with explorer

space - e = open close explorer

space - tv = open vertical split terminal (th for horizontal, tf for floating)

space - gg = open lazygit, q to quit, p to pull, P to push, space to stage/unstage file, c to commit, ctrl + u/d to scroll up or down in current file

ctrl + hjkl = navigate selected pane within nvim

ctrl - [n] - [+/-/</>] = for current pane, expand/shrink(vertical), shrink/expand horizontally by n columns/rows

space - q = quit pane

space - \ = split pane horizontally

space - | = split pane vertically

space - w - write



## nvim terminal

ctrl+\ - ctrl+n = enter visual mode

i/a = go back into insert mode

## nvim explorer

e - auto-expand explorer to text

y - mark to copy

x - mark to cut

p - paste

a - add file/folder (folder must end with /)

d - delete

H - show/hide hidden files

/ - filter

? - view shortcuts for explorer
