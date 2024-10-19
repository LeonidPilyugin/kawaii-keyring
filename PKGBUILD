# Maintainer: Leonid Pilyugin  <l.pilyugin04@gmail.com>

pkgname=kawaii-keyring
pkgver=1.2
pkgrel=1
pkgdesc='Kawaii PGP keyring'
url='https://github.com/LeonidPilyugin/kawaii-keyring'
arch=('x86_64')
license=('GPL3')
source=("$pkgname-$pkgver.tar.gz::https://github.com/LeonidPilyugin/$pkgname/releases/download/v$pkgver/files.tar.gz")
sha256sums=('dc125a0f8cd24d13395eba54d35c11849d70cd269d9c02483fb298517dfe013f')
install="$pkgname.install"

package() {
    srcdir=$srcdir/files
    dir=$pkgdir/usr/share/pacman/keyrings
    install -dm755 $dir
	install -Dm644 $srcdir/kawaii{.gpg,-trusted} $dir/
}
