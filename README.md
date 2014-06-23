# Sublime Text 3

* [Download](http://www.sublimetext.com/3)
* [Packages](https://sublime.wbond.net/)

## Install on Windows

![Windows](https://bytebucket.org/maqinainternet/sublime-text/raw/9c95a9a26783c224b5b388506e6803c05c71b69d/Images/install-windows.gif?token=7f2a6d3e530fe0782050ae0687cffc4bd91d93b4)

Open PowerShell by right-clicking and selecting Run as administrator

```
cd "$env:appdata\Sublime Text 3\Packages\"
mkdir "C:\Program Files\Sublime Text 3\Data"
mv User "C:\Program Files\Sublime Text 3\Data"
cmd /c mklink /D User "C:\Program Files\Sublime Text 3\Data"
cd "C:\Program Files\Sublime Text 3\"
git clone https://<username>@bitbucket.org/maqinainternet/sublime-text.git Data
```
