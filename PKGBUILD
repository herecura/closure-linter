# $Id: PKGBUILD 78820 2012-10-25 06:47:28Z foutrelis $
# Maintainer: BlackEagle < ike DOT devolder AT gmail DOT com >
pkgname=closure-linter
pkgver=2.3.11
pkgrel=1
pkgdesc="A JavaScript style checker and style fixer"
arch=('any')
url="http://code.google.com/closure"
license=('APACHE')
depends=('python2' 'python2-gflags' 'python2-distribute')
source=("http://$pkgname.googlecode.com/files/${pkgname/-/_}-$pkgver.tar.gz")

build() {
	cd ${pkgname/-/_}-$pkgver
	python2 setup.py build
}

package() {
	cd ${pkgname/-/_}-$pkgver
	python2 setup.py install --root="$pkgdir"
}
sha256sums=('a17790366c8cf07c932aafc8f1945e550b3f381178e1a8aad0f6cc75d41510f6')
