# .Vimrc and plugins confing #

first of all start with this in vim terminal
``:smile``
- - -
## some vim plugins and sources that may helpful##
* learn vim in game:) https://vim-adventures.com/
* general and useful plugins: https://vimawesome.com/
* django plugins, here is good document(UsingVimWithDjango): https://code.djangoproject.com/wiki/UsingVimWithDjango
* another repos for make vimrc good for python and django and html https://github.com/tpope/vim-surround
* https://github.com/nvie/vim-flake8
* https://www.reddit.com/r/vim/comments/8c54ru/django_web_development_using_vim/
* https://github.com/tpope/vim-commentary
* cssPretty.vim: https://www.vim.org/scripts/script.php?script_id=2137
* https://github.com/matagus/vim_files
* https://github.com/mjbrownie/vim-htmldjango_omnicomplete
* htmlDjango(template) plugin autocomple for vim: https://www.vim.org/scripts/script.php?script_id=4027

- - -
### Need typing "Farsi"? ###
if you are a persian developer, that seems ``spacemacs`` editor is also compose of vim and emacs, AND Luckily supported ``Farsi`` language 
but if you still vim and like me need none-english language support use another console such as ``Konsole`` instead of default Ubuntu terminal
in Konsole ltr is Ok but for concatinate persian char is use this ``:set arabicshape!``
it'll be ok to concatinate chars


- - -
### Quick install vim plugins ###
copy repos address to `.vimrc` if use `Plug 'repos'` (if you use vim-plug) then run follow command in vim termital to install:  
`:PlugInstall`  
`source %` (reload without restart .vimrc)  
`:PlugClean` remove plugins.  
`:PlugUpdate` check if plugins updated?  (if you've got 'Permission Denied', sure you've ran `$sudo vim .vimrc` before.
- - -
### Vim-Terminal ###
`:term` and `:![terminal command you want]`  
somthing cool I've forgot:) all the terminal under you fingers with ':term'(divide window pane horizontally so you have terminal) OR if you wanna single command just :![command]

- - -
### Problem with copy to clipboard ###

copy vim blocks to clipboard for use out of vim: install `vim-gnome` or `vim-gtk` further more:
Checking for X11-clipboard support in terminal in http://vim.wikia.com/wiki/Accessing_the_system_clipboard
- - -
use markdown viewer in mozilla firefox:  
add this addon to browser: https://addons.mozilla.org/en-US/firefox/addon/markdown-viewer-webext/  
if it doesn't work(specially in ubuntu):  
    make this file in direction:
       `~/.local/share/mime/packages/text-markdown.xml`  
	with this content:  
```
        <?xml version="1.0"?>
        <mime-info xmlns='http://www.freedesktop.org/standards/shared-mime-info'>
          <mime-type type="text/plain">
            <glob pattern="*.md"/>
            <glob pattern="*.mkd"/>
            <glob pattern="*.markdown"/>
          </mime-type>
        </mime-info>
```
then run `$update-mime-database ~/.local/share/mime`
