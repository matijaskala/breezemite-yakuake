# Breezemite themes for Yakuake

![](https://raw.githubusercontent.com/matijaskala/breezemite-yakuake/master/breezemite/icon.png)

To install a theme:
- get yakuake source code (https://download.kde.org/stable/yakuake or https://github.com/KDE/yakuake)
- `cd` into yakuake source code
- run `sed -i 's/\(Button->move(\)\(width() - \)\(m_skin->titleBar.*ButtonPosition().x()\)\(, m_skin->titleBar\)/\1(\3 <= 0) ? (- \3) : (\2\3)\4/' app/titlebar.cpp`
- compile and install: `mkdir build ; cd build ; cmake .. ; make ; sudo make install`
- place the theme in ~/.local/share/yakuake/kns_skins

note: you don't have to recompile yakuake to use the rhs theme
