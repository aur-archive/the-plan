# Maintainer: Kamil Wisniewski (FORMOZA) <formoza@autistici.org>

pkgname=the-plan
pkgver=1.0
pkgrel=2
pkgdesc="A fly ascends to the skies, pondering the pointlessness of its brief existence. The Plan was developed as a side project by Krillbite Studio"
arch=(any)
url=http://www.krillbite.com/theplan/
license=(custom)
depends=('wget' 'xorg-server')
install=$pkgname.install
provides=($pkgname)
source=(http://www.krillbite.com/theplan/download/linux/ThePlan.zip)
md5sums=(57f382c4b01ee7b37418b15762559e57)

package()
{
  mkdir -p $pkgdir/opt/$pkgname/
  cp -dr --preserve=mode,timestamp "$srcdir/The Plan_Data/" $pkgdir/opt/$pkgname/
  install "$srcdir/The Plan" $pkgdir/opt/$pkgname/
  mkdir -p $pkgdir/usr/bin
  ln -s "/opt/$pkgname/The Plan" $pkgdir/usr/bin/$pkgname
}