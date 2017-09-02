# [Sublime Text 3](http://www.sublimetext.com/3)

> The text editor you'll fall in love with

> Sublime Text is a sophisticated text editor for code, markup and prose. You'll love the slick user interface, extraordinary features and amazing performance.

![Sublime Text](https://c758482.ssl.cf2.rackcdn.com/new_theme_large.png)

## Install

### Sublime Text

#### Windows

Download [installer](https://download.sublimetext.com/Sublime%20Text%20Build%203126%20x64%20Setup.exe) and run (check **Add to explorer context menu**)

#### Linux Ubuntu (and Derivatives)

```bash
wget -c https://download.sublimetext.com/sublime-text_build-3126_amd64.deb
sudo dpkg -i sublime-text*.deb
```

### [Package Control](https://packagecontrol.io/)

Follow [this](https://packagecontrol.io/installation#Simple) instructions and close Sublime Text after installation

### My Preferences

#### Windows

Open **Command Prompt** by right-clicking and selecting **Run as Administrator**

```powershell
cd "%appdata%/Sublime Text 3/Packages/"
move User User-BKP
git clone https://github.com/magnobiet/sublime-text-preferences.git User
cd User
npm run install
```

#### Linux Ubuntu (and Derivatives)

```bash
cd ~/.config/sublime-text-3/Packages/
mv User User-BKP
git clone https://github.com/magnobiet/sublime-text-preferences.git User

cd sublime-text-3
sudo npm run install
```

## Installed Packages

[Package Control.sublime-settings](https://github.com/magnobiet/sublime-text-preferences/blob/master/Package%20Control.sublime-settings#L6)

## Icon

![Sublime Text Icon](https://raw.githubusercontent.com/magnobiet/sublime-text/master/Icons/sublime-text.png)

by [Jon-Paul Lunney](https://dribbble.com/shots/382465-Sublime-Text-2-update-Replacement-Icon)

## Licence

This project is licensed under the [MIT License](https://magno.mit-license.org/2014). Copyright © Magno Biét
