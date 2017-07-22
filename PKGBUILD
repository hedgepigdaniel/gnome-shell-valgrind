# Maintainer: Daniel Playfair Cal <daniel.playfair.cal@gmail.com>

pkgname=gnome-valgrind
pkgver=1.0
pkgrel=1
pkgdesc="Run GNOME with valgrind from display managers"
arch=('any')
depends=(gnome-session valgrind)
source=(
    gnome-shell-valgrind-errors
    gnome-shell-valgrind-errors.desktop
    gnome-valgrind.session
    gnome-valgrind-errors.desktop
)
md5sums=('128ca0e44694745319a6a7f23ffbf3e9'
         'f58f87d46682376a943706f56883e7a3'
         'f9c53c458b72061dab1fb32d85b27ee3'
         '9054476686470f0bf45aab63ba61d22d')

package() {
    install -D -m755 gnome-shell-valgrind-errors "$pkgdir/usr/bin/gnome-shell-valgrind-errors"
    install -D -m644 gnome-shell-valgrind-errors.desktop "$pkgdir/usr/share/applications/org.gnome.Shell-valgrind-errors.desktop"
    install -D -m644 gnome-valgrind.session "$pkgdir/usr/share/gnome-session/sessions/gnome-valgrind-errors.session"
    install -D -m644 gnome-valgrind-errors.desktop "$pkgdir/usr/share/wayland-sessions/gnome-valgrind-errors.desktop"
    install -D -m644 gnome-valgrind-errors.desktop "$pkgdir/usr/share/xsessions/gnome-valgrind-errors.desktop"
}
