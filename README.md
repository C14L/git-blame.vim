git-blame.vim
==========
```
 ███╗  ███╗ █████╗      ████╗ █╗     ███╗ █╗  █╗█████╗      █╗  █╗ ███╗ █╗  █╗
█╬══█╗ ╚█╔╝ ╚═█╔═╝      █╔══█╗█║    █╬══█╗██╗██║█╔═══╝      █║  █║ ╚█╔╝ ██╗██║
█║  ╚╝  █║    █║        █║  █║█║    █║  █║█╔█╬█║█║          █║  █║  █║  █╔█╬█║
█║      █║    █║  █████╗████╬╝█║    █║  █║█║╚╝█║████╗       █║  █║  █║  █║╚╝█║
█║ ██╗  █║    █║  ╚════╝█╔══█╗█║    █████║█║  █║█╔══╝  ██╗  █║  █║  █║  █║  █║
█║ ╚█║  █║    █║        █║  █║█║    █╔══█║█║  █║█║     ██║  ╚█╗█╬╝  █║  █║  █║
╚███╬╝ ███╗   █║        ████╬╝█████╗█║  █║█║  █║█████╗ ╚═╝   ╚█╬╝  ███╗ █║  █║
 ╚══╝  ╚══╝   ╚╝        ╚═══╝ ╚════╝╚╝  ╚╝╚╝  ╚╝╚════╝        ╚╝   ╚══╝ ╚╝  ╚╝
```

See Git Blame information in the status bar for the currently selected line.

![](https://wx3.sinaimg.cn/large/bceaad1fly1frwfmv58g4j21kw0ingph.jpg)

![](https://wx3.sinaimg.cn/large/bceaad1fly1frwfmv539mj21kw0inq7e.jpg)

![](https://wx2.sinaimg.cn/large/bceaad1fly1frwfmv50ytj21kw0in42a.jpg)

Installation
--------------

Simply Install

If you don't have a preferred installation method, I recommend
installing [pathogen.vim](https://github.com/tpope/vim-pathogen), and
then simply copy and paste:

```bash
    cd ~/.vim/bundle
    git clone git@github.com:zivyangll/git-blame.vim.git
```

Using [vim-plug](https://github.com/junegunn/vim-plug):

```vim
Plug 'zivyangll/git-blame.vim'
```

Using [Vundle](https://github.com/VundleVim/Vundle.vim)

```viml
Plugin 'zivyangll/git-blame.vim'
```


Show Git Blame info with a hotkey
---------------------------------

Add this line to your `.vimrc` settings file

```vim
nnoremap <Leader>s :<C-u>call gitblame#echo()<CR>
```

Press `<leader>s` to see the Git Blame info for the line the cursor is currently on.


Show Git Blame info always
--------------------------

Add this line to your `.vimrc` settings file

```vim
:autocmd CursorMoved * call gitblame#echo()
```

This will always show the Git Blame info for the currently active line in the status bar.


Self-Promotion
--------------

Like git-blame.vim? Follow the repository on
[GitHub](https://github.com/zivyangll/git-blame.vim) and vote for it on [vim.org](https://www.vim.org/scripts/script.php?script_id=5704). And if
you're feeling especially charitable, follow [GitHub](https://github.com/zivyangll).

Thanks
--------------

[git-messenger.vim](https://github.com/rhysd/git-messenger.vim)

License
-------

See [MIT License](https://github.com/zivyangll/git-blame.vim/blob/master/LICENSE).

