pkgname=apricity-theme
pkgver=1.0
_pkgver=1.0
_pkgname=apricity-theme
pkgrel=1.1
pkgdesc='Setup Apricity for Reborn'
url='https://github.com/keeganmilsten/Reborn-Packages/tree/master/cosmic/apricity'
arch=('any')
license=('GPL3')
depends=('unzip' 'gnome-shell-extension-status-menu-buttons' 'gnome-shell-extension-topicons-plus' 'gnome-shell-extension-dash-to-dock' 'gnome-shell-extension-update' 'gnome-shell-extensions' 'arc-gtk-theme' 'gnome-tweaks')
source=("${pkgname}-${_pkgver}.tar.gz::https://codeload.github.com/RebornOS/${_pkgname}/tar.gz/1.1")
install=schema.install

package() {
    cd "${srcdir}/${_pkgname}-1.1"

    install -Dm644 98_gnome.gschema.override  \
        "${pkgdir}/usr/share/glib-2.0/schemas/98_gnome.gschema.override"

    install -D -m 777 elementary.jpg \
    	 "${pkgdir}/usr/share/backgrounds/elementary.jpg"

    install -D -m 777 ApricityGnome@anassboulmane.gmail.com.zip \
    	 "${pkgdir}/usr/share/gnome-shell/extensions/ApricityGnome@anassboulmane.gmail.com.zip"

    install -D -m 777 Move_Clock@rmy.pobox.com.v15.shell-extension.zip \
    	 "${pkgdir}/usr/share/gnome-shell/extensions/Move_Clock@rmy.pobox.com.v15.shell-extension.zip"

    install -D -m 777 Apricity-Icons.zip \
    	 "${pkgdir}/usr/share/icons/Apricity-Icons.zip"

    install -D -m 777 Arctic-Apricity.zip \
    	 "${pkgdir}/usr/share/icons/Arctic-Apricity.zip"

}
