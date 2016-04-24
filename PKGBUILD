#Maintainer: Alex Gajewski <agajews@gmail.com>

_pkgname='Apricity Themes'
pkgname=apricity-themes-cinnamon
pkgver=1.0.3
pkgrel=1
pkgdesc='Cinnamon Assets for Apricity OS'
arch=(any)
license=(GPL)
url="https://github.com/Apricity-OS/apricity-themes-cinnamon"
depends=()
replaces=(apricity-themes)
conflicts=(apricity-themes, apricity-themes-gnome)
provides=(apricity-themes)
source=("apricity-themes-cinnamon.tar.gz")
sha256sums=('2bb308fa94f24579623f7a43027616a673bdb7affcb5f4367644b9516d17217e')
install="apricity-themes-cinnamon.install"

package() {
	rm -rf "${pkgdir}/usr/share/themes/Arctic Apricity"
	mkdir -p "${pkgdir}/usr/share/themes"
	mkdir -p "${pkgdir}/etc/skel/.config/autostart"
	cp -rf "${srcdir}/apricity-themes-cinnamon/Arctic Apricity" "${pkgdir}/usr/share/themes"
	cp -f "${srcdir}/apricity-themes-cinnamon/firstrun-desktop.sh" "${pkgdir}/etc/skel/.config/autostart"
}
