# Maintainer: liammmcauliffe <https://github.com/liammmcauliffe>
pkgname=hyprworm
pkgver=1.0.0
pkgrel=1
pkgdesc="A fast and lightweight window switcher for Hyprland built in C"
arch=('x86_64' 'aarch64')
url="https://github.com/liammmcauliffe/hyprworm"
license=('MIT')
depends=('cjson')
makedepends=('git' 'make' 'gcc')
source=("$pkgname-$pkgver.tar.gz::https://github.com/liammmcauliffe/hyprworm/archive/v$pkgver.tar.gz")
sha256sums=('c6f3e699632d5759558e96210790aac437cc3b5bce2d4e48ba26acc56f96aebc')

build() {
    cd "$pkgname-$pkgver"
    make
}

package() {
    cd "$pkgname-$pkgver"
    make DESTDIR="$pkgdir" install
}
