# Maintainer: Leonid Pilyugin  <l.pilyugin04@gmail.com>

pkgname=kawaii-keyring
pkgver=1.1
pkgrel=1
pkgdesc='Kawaii PGP keyring'
arch=('x86_64')
install="${pkgname}.install"
license=('GPL3')
source=("${pkgname}-${pkgver}.tar.gz::https://github.com/LeonidPilyugin/$pkgname/releases/download/v$pkgver/files.tar.gz")
sha256sums=('e7e7eb223e78c6d000b6a975bd37f19e073b68cbffb7628661cc4a1b988b1719')

package() {
	make DESTDIR="${pkgdir}" install
}

