# Maintainer: Leonid Pilyugin  <l.pilyugin04@gmail.com>

pkgname=kawaii-config
pkgver=1.1
pkgrel=1
pkgdesc='Kawaii config files for MenheraOS'
arch=('x86_64')
url="https://github.com/LeonidPilyugin/kawaii-config"
license=('GPL3')
groups=('kawaii')
source=("$pkgname-$pkgver.tar.gz::https://github.com/LeonidPilyugin/$pkgname/releases/download/v$pkgver/files.tar.gz")
sha256sums=('bdd6ee468a18d723e2289c7fd662210c8219dbb356b86a2fb04dc9f6c3922d85')

package() {
    srcdir=$srcdir/files
    dir=$pkgdir/etc/skel
    install -dm755 $dir
    cp -r $srcdir/{.config,.kde4} $dir/
    cp $srcdir/.zshrc $dir/
}

