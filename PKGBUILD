# Maintainer: Leonid Pilyugin  <l.pilyugin04@gmail.com>

pkgname=kawaii-keyring
pkgver=1.0
pkgrel=1
pkgdesc='Kawaii PGP keyring'
arch=('x86_64')
install="${pkgname}.install"
license=('GPL3')

package() {
	make DESTDIR="${pkgdir}" install
}

