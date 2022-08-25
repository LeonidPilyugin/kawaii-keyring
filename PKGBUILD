# Maintainer: Leonid Pilyugin  <l.pilyugin04@gmail.com>

pkgname=kawaii-keyring
pkgver=1.1
pkgrel=1
pkgdesc='Kawaii PGP keyring'
arch=('x86_64')
license=('GPL3')
source=("${pkgname}-${pkgver}.tar.gz::https://github.com/LeonidPilyugin/$pkgname/releases/download/v$pkgver/files.tar.gz")
sha256sums=('9059603034d91e119401c947611ed0b35129a0d652154e376461790df997db04')
install="${pkgname}.install"

package() {
    srcdir=$srcdir/files
    dir=$pkgdir/usr/sharepacman/keyrings
    install -dm755 $dir
	install -m0755 $srcdir/kawaii{.gpg,-trusted} $dir/
}
