# Sublime Text 3

> The text editor you'll fall in love with

> Sublime Text is a sophisticated text editor for code, markup and prose.
You'll love the slick user interface, extraordinary features and amazing performance.

* [Official website](http://www.sublimetext.com/3)
* [Package Control](https://packagecontrol.io/)

[![Sublime Text 3][shield-sublime]][sublime]

## Install

### Windows

- Download [installer](https://download.sublimetext.com/Sublime%20Text%20Build%203114%20x64%20Setup.exe) and run (check **Add to explorer context menu**)
- Open **PowerShell** by right-clicking and selecting **Run as Administrator**

```powershell
cd "C:\Program Files\Sublime Text 3\"
git clone https://github.com/magnobiet/sublime-text.git Data
npm run install
```

### Linux Ubuntu (and Derivatives)

```bash
cd ~/Downloads
wget -c https://download.sublimetext.com/sublime-text_build-3114_amd64.deb # as super user
dpkg -i sublime-text*.deb

cd ~/.config/
mv sublime-text-3 sublime-text-3-BKP
git clone https://github.com/magnobiet/sublime-text.git sublime-text-3

cd sublime-text-3
npm run install # as super user
```

## Installed Packages

- AlignTab
- AngularJS
- AngularJS Snippets
- ApacheConf.tmLanguage
- ASCII Decorator
- AutoFileName
- Bootstrap 3 Snippets
- Bower
- BracketHighlighter
- BufferScroll
- cdnjs
- CodeIgniter Snippets
- Color Highlighter
- CSScomb
- DocBlockr
- Dotfiles Syntax Highlighting
- EditorConfig
- Emmet
- FileSystem Autocompletion
- Git
- GitGutter
- Grunt
- Handlebars
- Highlight
- HTML5
- JavaScript Console
- JavaScript Patterns
- JavaScript Snippets
- JsFormat
- Laravel 5 Artisan
- Laravel 5 Snippets
- Laravel Blade Highlighter
- ~~LESS~~
- Line Endings Unify
- LineEndings
- List stylesheet variables
- Markdown Preview
- nginx
- Package Control
- ~~PHP Companion~~
- PHP Getters and Setters
- phpfmt
- PlainTasks
- Reindent on save
- Sass
- SassBeautify
- SCSS
- SideBarEnhancements
- Silex Snippets
- SqlBeautifier
- StringEncode
- SublimeCodeIntel
- SublimeLinter
- SublimeLinter-contrib-scss-lint
- SublimeLinter-csslint
- SublimeLinter-jscs
- SublimeLinter-jshint
- SublimeLinter-json
- SublimeLinter-php
- SublimeLinter-phplint
- SublimeLinter-pylint
- SublimeLinter-xmllint
- TrailingSpaces
- Trimmer

## Icon

![Sublime Text Icon](https://raw.githubusercontent.com/magnobiet/sublime-text/master/Icons/sublime-text.png)

by [Jon-Paul Lunney](https://dribbble.com/shots/382465-Sublime-Text-2-update-Replacement-Icon)
