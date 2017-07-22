# Maintainer: Daniel Playfair Cal <daniel.playfair.cal@gmail.com>

pkgname=gnome-valgrind
pkgver=1.0
pkgrel=1
pkgdesc="Run GNOME with valgrind from display managers"
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

install() {
    install -m755 ../gnome-valgrind-errors /usr/bin/gnome-valgrind-errors
    install -m755 ../gnome-valgrind-leaks /usr/bin/gnome-valgrind-leaks
    install -m644 ../gnome-valgrind-errors.desktop /usr/share/wayland-sessions/gnome-valgrind-errors.desktop
    install -m644 ../gnome-valgrind-leaks.desktop /usr/share/wayland-sessions/gnome-valgrind-leaks.desktop
    install -m644 ../gnome-valgrind-errors.desktop /usr/share/xsessions/gnome-valgrind-errors.desktop
    install -m644 ../gnome-valgrind-leaks.desktop /usr/share/xsessions/gnome-valgrind-leaks.desktop
}
