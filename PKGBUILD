# Maintainer: Willian <willianpts@gmail.com>
_pkgbase='shiftfs'
pkgname=${_pkgbase}-dkms
pkgver="c51f72e"
pkgrel=1
epoch=
pkgdesc="UID/GID shifting overlay filesystem for containers"
arch=('x86_64')
url="https://github.com/brauner/linux/tree/shiftfs"
license=("GPL2")
groups=()

depends=('dkms')
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()

options=()
install=
changelog=
source=('shiftfs.c' 'magic.h' 'Makefile' 'dkms.conf')

noextract=()
validpgpkeys=()

md5sums=('a2ea1280ff757230a69eca9402290f8b'
         '8de70097311e38ea7d2938d151e1d155'
         'SKIP' 'SKIP')

prepare() {
	/bin/true
}

package() {
    dest="${pkgdir}/usr/src/${_pkgbase}-$pkgver"
	install -d "$dest"

    # Copy sources (including Makefile)
    cp -rfv ${srcdir}/* "${dest}/"
}
