
| ![alt text](https://raw.githubusercontent.com/sixsixfive/ivy/master/xfcesettings.png) | ![alt text](https://raw.githubusercontent.com/sixsixfive/ivy/master/matecontrol.png)|
| ------------- |:-------------:|

A very minimalistic but colorful png icon theme for X11 Desktops such as: [Xfce](http://xfce.org/), [LXQt](http://lxqt.org/), [MATE](http://mate-desktop.org/) or [Enlightenment](https://www.enlightenment.org/) heavily inspired by the [FatCow](http://www.fatcow.com/free-icons) & [Tango!](http://en.wikipedia.org/wiki/Tango_Desktop_Project) icons under [CC-BY-SA](http://creativecommons.org/licenses/by-sa/4.0/deed.en)

* Prebuilt set for Download: [Ivy@deviantart](http://sixsixfive.deviantart.com/art/Ivy-371216510)

#####Goals:

- try to create a generic icon theme from scratch
- no reflections (glossy highlights) or big fat icon shadows (the main difference to tango)
- legal, no trademarks-->only free logos
- no monochrome osx-like or blocky iphone-like icons

#####Howto create a png icon theme:

**Note:** *We make a png theme because it's faster and pixel perfect*

* **`cd ~`**
* **`git clone https://github.com/sixsixfive/ivy.git`** or
**`svn co https://github.com/sixsixfive/ivy/trunk/ivy-dev ivy`**
* **`cd ivy`**
* **`bash createpngset`**

####Notes:

Since the theme is still missing various small icons it's recommend to
use some fixes:

###### Disable Menu icons:

* GTK2 

[(xsettings)](http://www.freedesktop.org/wiki/Specifications/XSettingsRegistry/), Xfce uses xfconf, MATE uses gconf/mateconf)

**`Gtk/MenuImages "0"`**

* Qt4/KDE4

KDE-Systemsettings>App. Appearance>Style>Fine Tuning

* GTK3

disabled by default(will inherit xsettings)

###### or make them bigger (eg. 22px):

* GTK2 

[(xsettings)](http://www.freedesktop.org/wiki/Specifications/XSettingsRegistry/), Xfce uses xfconf, MATE uses gconf/mateconf)

**`Gtk/IconSizes "panel-menu=22,22:gtk-dialog=48,48:gtk-small-toolbar=22,22:gtk-large-toolbar=22,22:gtk-menu=22,22:gtk-button=22,22:panel-applications-menu=22,22:panel-directory-menu=22,22"`**

* Qt4/KDE4

KDE-Systemsettings>App. Appearance>Icons>Advanced

* GTK3

this useful setting has been removed by the gnome devs

* You could also make them bigger(eg. 22px): 

####Limitations/Bugs:

* some smaller icons are fuzzy cause they are scaled down from other sizes(sry, but I don't have plenty of time but someday they will be complete I guess ;)
* some icons are still missing(that's just a matter of time ;) 
* Due Xfce bug [10126](https://bugzilla.xfce.org/show_bug.cgi?id=10126) it's impossible to select any icons in the built-in *.desktop editor

