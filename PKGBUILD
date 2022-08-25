# Maintainer: Leonid Pilyugin  <l.pilyugin04@gmail.com>

pkgname=kawaii-config
pkgver=1.0
pkgrel=1
pkgdesc='Kawaii config files for MenheraOS'
arch=('x86_64')
license=('GPL3')
groups=('kawaii')
source=("${pkgname}-${pkgver}.tar.gz::https://github.com/LeonidPilyugin/$pkgname/releases/download/v$pkgver/files.tar.gz")
sha256sums=('e1d0e0625903ae09d06614520a726f8d504f48c489192a3958109acda34b661d')

package() {
    srcdir=$srcdir/files
    dir=$pkgdir/etc/skel
    install -dm755 $dir
    cp -r $srcdir/{.config,.kde4} $dir
}

