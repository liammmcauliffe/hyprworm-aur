# Maintainer: liammmcauliffe <https://github.com/liammmcauliffe>
pkgname=hyprworm
pkgver=1.1.0
pkgrel=1
pkgdesc="A fast and lightweight window switcher for Hyprland built in C"
arch=('x86_64' 'aarch64')
url="https://github.com/liammmcauliffe/hyprworm"
license=('MIT')
depends=('cjson')
makedepends=('git' 'make' 'gcc')
source=("$pkgname-$pkgver.tar.gz::https://github.com/liammmcauliffe/hyprworm/archive/v$pkgver.tar.gz")
sha256sums=('7af416f24823959bc162806d846782c98dc5616994a0bfa8bc3cbc15ff345d77')

build() {
    cd "$pkgname-$pkgver"
    make
}

package() {
    cd "$pkgname-$pkgver"
    make DESTDIR="$pkgdir" install
}
