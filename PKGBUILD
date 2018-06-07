# Based on the file created for Arch Linux by:
# Pierre Schmitz <pierre@archlinux.de>

# Maintainer : Philip Müller <philm@manjaro.org>
# Maintainer : Guillaume Benoit <guillaume@manjaro.org>

pkgname=manjaro-keyring
pkgver=20180607
pkgrel=1
pkgdesc='Manjaro PGP keyring'
arch=('any')
url='http:/manjaro.org'
license=('GPL')
install="${pkgname}.install"
source=('Makefile'
        'manjaro.gpg'
        'manjaro-revoked'
        'manjaro-trusted')
sha256sums=('ac8fed4c8dbb910bb4fb3c01cb63de00d6b25ac79734ea5c933706aff6f9c950'
            '17174efdc7a1daaa92d986c8982abd9dd306923f4bc42babe623e6414dfb211d'
            'ce3dce1721eb380d2ba6c5c668c7e466d391eff7ee1285f88b90e01023324b72'
            '418565a5434748e9853e54761e1d13a02660c0cc9ac4eb1d17e6d290b979ab7c')

package() {
	cd "${srcdir}"
	make PREFIX=/usr DESTDIR=${pkgdir} install
}
