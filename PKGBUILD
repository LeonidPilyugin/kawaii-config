# Maintainer: Leonid Pilyugin  <l.pilyugin04@gmail.com>

pkgname=kawaii-config
pkgver=2.0
pkgrel=1
pkgdesc='Kawaii config files for MenheraOS'
groups=('kawaii')
url='https://github.com/LeonidPilyugin/kawaii-config'
arch=('x86_64')
license=('GPL3')
source=("$pkgname-$pkgver.tar.gz::https://github.com/LeonidPilyugin/$pkgname/releases/download/v$pkgver/files.tar.gz")
sha256sums=('372b68a2170b9e2fa0399ecc75dad17e4d83c087d17a19b57cbc37cfc97bebef')

package() {
    srcdir=$srcdir/files
    dir=$pkgdir/etc/skel
    install -dm755 $dir
    cp -r $srcdir/{.config,.kde4} $dir/
    cp $srcdir/.zshrc $dir/
}

