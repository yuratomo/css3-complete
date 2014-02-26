css3-complete
=================
Vim omnifunc for css3.

Install
-------
Set your .vimrc as follows.

    " Vundle
    Bundle 'yuratomo/css3-complete'

Settings
--------
Set your .vimrc as follows.
### autoload java-api-complete
    au BufNewFile,BufRead *.css    setl omnifunc=css3#complete
    
### show status refarence
    au CompleteDone *.css          call css3#showRef()
    au BufNewFile,BufRead *.css    inoremap <expr> <c-down> css3#nextRef()
    au BufNewFile,BufRead *.css    inoremap <expr> <c-up>   css3#prevRef()

ScreenShots
----------
