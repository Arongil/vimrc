# vimrc

## fd for fuzzy search

Run `brew install fzf`. Add to `~/.zshrc` the line `alias fd="cd \$(find * -type d | fzf)"`.

Now `fd` in the terminal will perform fuzzy directory change. Also `**<TAB>` anywhere in the terminal will pull up fuzzy search.

Note: `brew install fd` will download a package called `fd` which is an improvement on `find`. However, if you use it you can't alias `fd` to automatically change directory.
