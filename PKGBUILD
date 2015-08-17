# Maintainer: Emmanuel Gil Peyrot <linkmauve@linkmauve.fr>

pkgbase='python-epub-hg'
pkgname=('python-epub-hg' 'python2-epub-hg')
pkgver=70
pkgrel=1
pkgdesc="Library to open and read files in the epub version 2."
arch=('any')
url="http://pypi.python.org/pypi/epub"
license=('LGPL3')
source=("$pkgbase::hg+https://bitbucket.org/exirel/epub")
md5sums=('SKIP')

package_python-epub-hg() {
  depends=('python')
  provides=('python-epub=0.5.0')
  conflicts=('python-epub')

  cd "$srcdir/$pkgbase"
  python setup.py install --root="$pkgdir/" --optimize=1
}

package_python2-epub-hg() {
  depends=('python2')
  provides=('python2-epub=0.5.0')
  conflicts=('python2-epub')

  cd "$srcdir/$pkgbase"
  python2 setup.py install --root="$pkgdir/" --optimize=1
}

# vim:set ts=2 sts=2 sw=2 et:
