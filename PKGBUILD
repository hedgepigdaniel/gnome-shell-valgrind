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
md5sums=('a0ee7338ed0a6211e04ba6e3f4820ce7'
         '08e983491f0e9621a3bf6d07861bbaaf'
         'b80f8ac6e603369ba70a1db709a968cd'
         '9054476686470f0bf45aab63ba61d22d')

package() {
    install -D -m755 gnome-shell-valgrind-errors "$pkgdir/usr/bin/gnome-shell-valgrind-errors"
    install -D -m644 gnome-shell-valgrind-errors.desktop "$pkgdir/usr/share/applications/org.gnome.Shell-valgrind-errors.desktop"
    install -D -m644 gnome-valgrind.session "$pkgdir/usr/share/gnome-session/sessions/gnome-valgrind-errors.session"
    install -D -m644 gnome-valgrind-errors.desktop "$pkgdir/usr/share/wayland-sessions/gnome-valgrind-errors.desktop"
    install -D -m644 gnome-valgrind-errors.desktop "$pkgdir/usr/share/xsessions/gnome-valgrind-errors.desktop"
}
