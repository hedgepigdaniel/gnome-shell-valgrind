# Maintainer: Daniel Playfair Cal <daniel.playfair.cal@gmail.com>

pkgname=gnome-valgrind
pkgver=1.0
pkgrel=1
pkgdesc="Run GNOME with valgrind from display managers"
arch=('any')
depends=(gnome-session valgrind)
source=(
    gnome-shell-valgrind
    gnome-shell-gdb
    gnome-shell-valgrind.desktop
    gnome-shell-gdb.desktop
    gnome-valgrind.session
    gnome-gdb.session
    gnome-valgrind.desktop
    gnome-gdb.desktop
)
md5sums=('a0ee7338ed0a6211e04ba6e3f4820ce7'
         '46b5cca2865590e180e1a208678caa89'
         '10dc5bb0474a96cc80bd5c836ff19860'
         '3a44a49f68b2fc6394f70507235a7264'
         '7c3ca03e53231593830fbc934672b379'
         'c6bfe24eb6e5f190e83e7b7cae9c753f'
         '808a7fd3ffb9a714c899733c7ac41026'
         'c17c3be55264c18d36920cf5b90b3ed2')

package() {
    install -D -m755 gnome-shell-valgrind "$pkgdir/usr/bin/gnome-shell-valgrind"
    install -D -m755 gnome-shell-gdb "$pkgdir/usr/bin/gnome-shell-gdb"

    install -D -m644 gnome-shell-valgrind.desktop "$pkgdir/usr/share/applications/org.gnome.Shell-valgrind.desktop"
    install -D -m644 gnome-shell-gdb.desktop "$pkgdir/usr/share/applications/org.gnome.Shell-gdb.desktop"

    install -D -m644 gnome-valgrind.session "$pkgdir/usr/share/gnome-session/sessions/gnome-valgrind.session"
    install -D -m644 gnome-gdb.session "$pkgdir/usr/share/gnome-session/sessions/gnome-gdb.session"

    install -D -m644 gnome-valgrind.desktop "$pkgdir/usr/share/wayland-sessions/gnome-valgrind.desktop"
    install -D -m644 gnome-gdb.desktop "$pkgdir/usr/share/wayland-sessions/gnome-gdb.desktop"

    install -D -m644 gnome-valgrind.desktop "$pkgdir/usr/share/xsessions/gnome-valgrind.desktop"
    install -D -m644 gnome-gdb.desktop "$pkgdir/usr/share/xsessions/gnome-gdb.desktop"
}
