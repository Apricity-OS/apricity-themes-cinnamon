#Maintainer: Alex Gajewski <agajews@gmail.com>

_pkgname='Apricity Themes'
pkgname=apricity-themes-cinnamon
pkgver=1.0.2
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
sha256sums=('42772cd6fd57a06ca0b4eb742c8453e52190d8df88b476d4a4c1524cc906bb87')
install="apricity-themes-cinnamon.install"

package() {
	rm -rf "${pkgdir}/usr/share/themes/Arctic Apricity"
	mkdir -p "${pkgdir}/usr/share/themes"
	mkdir -p "${pkgdir}/etc/skel/.config/autostart"
	cp -rf "${srcdir}/apricity-themes-cinnamon/Arctic Apricity" "${pkgdir}/usr/share/themes"
	cp -f "${srcdir}/apricity-themes-cinnamon/firstrun-desktop.sh" "${pkgdir}/etc/skel/.config/autostart"
}
