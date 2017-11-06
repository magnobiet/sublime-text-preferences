# [Sublime Text 3](http://www.sublimetext.com/3)

> The text editor you'll fall in love with

> Sublime Text is a sophisticated text editor for code, markup and prose. You'll love the slick user interface, extraordinary features and amazing performance.

![Sublime Text](https://c758482.ssl.cf2.rackcdn.com/new_theme_large.png)

## Install

### Sublime Text

#### Windows

Download [`.exe` installer](https://www.sublimetext.com/3) and run (check **Add to explorer context menu**).

#### Linux Ubuntu (and Derivatives)

```bash
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
sudo apt-get install apt-transport-https
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt-get update
sudo apt-get install sublime-text
```

### [Package Control](https://packagecontrol.io/)

Follow [this](https://packagecontrol.io/installation#Simple) instructions and close Sublime Text after installation.

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

See [Package Control.sublime-settings#L6](Package%20Control.sublime-settings#L6)

## Licence

This project is licensed under the [MIT License](https://magno.mit-license.org/2014). Copyright © Magno Biét
