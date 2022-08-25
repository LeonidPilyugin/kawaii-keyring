# Maintainer: Leonid Pilyugin  <l.pilyugin04@gmail.com>

pkgname=kawaii-keyring
pkgver=1.1
pkgrel=1
pkgdesc='Kawaii PGP keyring'
arch=('x86_64')
license=('GPL3')
source=("${pkgname}-${pkgver}.tar.gz::https://github.com/LeonidPilyugin/$pkgname/releases/download/v$pkgver/files.tar.gz")
sha256sums=('1de778ff976f5dd5a9822a6ad7bd35078897bddb01af5028f5a965c78e3983c5')

package() {
    export install="src/files/${pkgname}.install"
    make DESTDIR="${pkgdir}" install
}
