# minimal vimrc for dein

* https://github.com/Shougo/dein.vim/issues/20

```sh
mv ~/.vim{,.orig}

# for dein
rm -fr /tmp/.cache && git clone https://github.com/Shougo/dein.vim /tmp/.cache/dein/repos/github.com/Shougo/dein.vim
vim -N -u ./minimal-vimrc -U NONE -i NONE
```

```vim
" redir
redir > ./scriptnames-dein.txt | silent! scriptnames | redir END
```

```sh
# for neobundle
rm -fr /tmp/.cache && git clone https://github.com/Shougo/neobundle.vim /tmp/.cache/bundle/neobundle.vim
vim -N -u ./neobundle-vimrc -U NONE -i NONE
```

```vim
" redir
redir > ./scriptnames-neobundle.txt | silent! scriptnames | redir END
```

```sh
mv ~/.vim{.orig,}
```
