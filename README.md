WhiteSur snap port.
WhiteSur is a MacOS Big Sur like theme for GTK 3, GTK 2 and Gnome-Shell which supports GTK 3 and GTK 2 based desktop environments like Gnome, Pantheon, XFCE, Mate, etc. Created by  [vinceliuice](https://github.com/vinceliuice).

Git repos:\
[WhiteSur Gnome Theme](https://github.com/vinceliuice/WhiteSur-gtk-theme) \
[WhiteSur Icon Theme](https://github.com/vinceliuice/WhiteSur-icon-theme.git)

Port based on the theme ports from Genadi Naydenov (gantonayde).

The snap contains all flavours of the GTK themes. To connect the theme to other snap packages, please run:

` sudo snap connect [other snap]:gtk-3-themes whitesur-gtk-theme:gtk-3-themes `

` sudo snap connect [other snap]:icon-themes whitesur-gtk-theme:icon-themes `

To connect the theme to all apps which have available plugs to gtk-common-themes you can run:

` for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i whitesur-gtk-theme:gtk-3-themes; done `

` for i in $(snap connections | grep gtk-common-themes:icon-themes | awk '{print $2}'); do sudo snap connect $i whitesur-gtk-theme:icon-themes; done `


[Developer Website](https://github.com/vinceliuice)

<a href="https://snapcraft.io/whitesur-gtk-theme">
<img alt="Get it from the Snap Store" src="https://snapcraft.io/static/images/badges/en/snap-store-black.svg" />
</a>