# Maintainer: Daniel Playfair Cal <daniel.playfair.cal@gmail.com>

pkgname=gnome-valgrind
pkgver=1.0
pkgrel=1
pkgdesc="Run GNOME with valgrind from display managers"
arch=('any')
depends=(gnome-session valgrind)
source=(
    gnome-valgrind-errors
    gnome-valgrind-errors.desktop
    gnome-valgrind-leaks
    gnome-valgrind-leaks.desktop
)
md5sums=('e41ea6158d607f37f368509cd4d86b1e'
         'ee8c1bcd7c034c30674c6915bb6ab573'
         '7d9cdb2e7cb1a9fda9f7950ffff126a8'
         '90e9d304738080d48d25e134afd83109')

package() {
    install -D -m755 gnome-valgrind-errors "$pkgdir/usr/bin/gnome-valgrind-errors"
    install -D -m755 gnome-valgrind-leaks "$pkgdir/usr/bin/gnome-valgrind-leaks"
    install -D -m644 gnome-valgrind-errors.desktop "$pkgdir/usr/share/wayland-sessions/gnome-valgrind-errors.desktop"
    install -D -m644 gnome-valgrind-leaks.desktop "$pkgdir/usr/share/wayland-sessions/gnome-valgrind-leaks.desktop"
    install -D -m644 gnome-valgrind-errors.desktop "$pkgdir/usr/share/xsessions/gnome-valgrind-errors.desktop"
    install -D -m644 gnome-valgrind-leaks.desktop "$pkgdir/usr/share/xsessions/gnome-valgrind-leaks.desktop"
}
