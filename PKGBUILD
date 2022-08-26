# Maintainer: Leonid Pilyugin  <l.pilyugin04@gmail.com>

pkgname=kawaii-keyring
pkgver=1.1
pkgrel=1
pkgdesc='Kawaii PGP keyring'
url='https://github.com/LeonidPilyugin/kawaii-keyring'
arch=('x86_64')
license=('GPL3')
source=("$pkgname-$pkgver.tar.gz::https://github.com/LeonidPilyugin/$pkgname/releases/download/v$pkgver/files.tar.gz")
sha256sums=('2a0c658d6762fba93292b328c245024e5caae72a3578fd5a7c58dea11c15ddd3')
install="$pkgname.install"

package() {
    srcdir=$srcdir/files
    dir=$pkgdir/usr/share/pacman/keyrings
    install -dm755 $dir
	install -m0755 $srcdir/kawaii{.gpg,-trusted} $dir/
}
