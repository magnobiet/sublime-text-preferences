# Sublime Text 3

* [Download](http://www.sublimetext.com/3)
* [Packages](https://sublime.wbond.net/)

## Install on Windows

![Windows](https://bytebucket.org/maqinainternet/sublime-text/raw/9c95a9a26783c224b5b388506e6803c05c71b69d/Images/install-windows.gif?token=7f2a6d3e530fe0782050ae0687cffc4bd91d93b4)

Open PowerShell by right-clicking and selecting Run as administrator.

```
cd "C:\Program Files\Sublime Text 3\"
git clone https://<username>@bitbucket.org/maqinainternet/sublime-text.git Data
cd "$env:appdata\Sublime Text 3\Packages\"
cmd /c mklink /D User "C:\Program Files\Sublime Text 3\Data"
```

## Install on Ubuntu

```
cd $HOME/Downloads
#wget http://c758482.r82.cf2.rackcdn.com/sublime-text_build-3065_i386.deb
wget http://c758482.r82.cf2.rackcdn.com/sublime-text_build-3065_amd64.deb
sudo dpkg -i sublime-text_build-*.deb
cd $HOME/.config/
git clone https://<username>@bitbucket.org/maqinainternet/sublime-text.git
```