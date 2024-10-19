# Maintainer: Leonid Pilyugin  <l.pilyugin04@gmail.com>

pkgname=kawaii-keyring
pkgver=1.3
pkgrel=1
pkgdesc='Kawaii PGP keyring'
url='https://github.com/LeonidPilyugin/kawaii-keyring'
arch=('x86_64')
license=('GPL3')
source=("$pkgname-$pkgver.tar.gz::https://github.com/LeonidPilyugin/$pkgname/releases/download/v$pkgver/files.tar.gz")
sha256sums=('4835e6b42622466352c8ba90d92e7e07d3c42b01988340227e2a614ce394d527')
install="$pkgname.install"

package() {
    srcdir=$srcdir/files
    dir=$pkgdir/usr/share/pacman/keyrings
    install -dm755 $dir
	install -Dm644 $srcdir/kawaii{.gpg,-trusted} $dir/
}
