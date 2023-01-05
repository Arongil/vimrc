# vimrc

## fd for fuzzy search

Run `brew install fzf`. Add to `~/.zshrc` the line `alias fd="cd \$(find * -type d | fzf)"`.

Now `fd` in the terminal will perform fuzzy directory change. Also `**<TAB>` anywhere in the terminal will pull up fuzzy search.

Note: `brew install fd` will download a package called `fd` which is an improvement on `find`. However, if you use it you can't alias `fd` to automatically change directory.

## vim keybinds in terminal

Add `bindkey -v` to `~/.zshrc` to enable vi keybinds in terminal commands. Use *esc* to enter normal mode. Note: disables `reverse-i-search`. For similar functionality use `/` for reverse search and `n` to find the next match, as in standard Vim.

## VimPlug

You'll want to install `VimPlug` to make color schemes like `gruvbox` work.

```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

To source `~/.vimrc`, run `:so %` from inside the `~/.vimrc` file.

To enable true color on `gruvbox` (rather than the 256 palette), add `source ~/.vim/plugged/gruvbox/gruvbox_256palette.sh` to `~/.zshrc`.
