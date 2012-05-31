# Better CSS Syntax for Vim

Highlights for full CSS2, most of HTML5 & CSS3 properties (include prefix like -moz-).

__Preview:__

Molokai sheme:

![Molokai](https://img.skitch.com/20120531-nt3x6qcgkjj7huarpfsh65cmph.jpg)

Slate scheme:

![Slate](https://img.skitch.com/20120531-ju922dsa9u68ib7cbwq27yaygj.jpg)

## Known issue:

- May not collaborate with some plugins, e.g. CSS Color, Sass
- Some properties can't highlighted well with prefix
- CSS3 animation properties highlighting

Because of this plugin is built for standard CSS and not compatible with original css.vim (see [this](https://github.com/ChrisYip/Better-CSS-Syntax-for-Vim/issues/9#issuecomment-6034606)), if you run into any error that related to CSS, you may need this:

__Sass:__

How to get rid of the error:

- edit `sass.vim`, go to line 16, delete `cssValue.*,`
- edit your `.vimrc`, add `au BufRead,BufNewFile *.sass set filetype=css`

Or, try [css3 syntax](http://www.vim.org/scripts/script.php?script_id=3042) or [vim-css3-syntax](https://github.com/hail2u/vim-css3-syntax).