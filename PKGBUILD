# shellcheck disable=SC2148
# Maintainer: juanvel400 <juanvel400@proton.me>
pkgname=unnfr
pkgver=0.2.0
pkgrel=1
pkgdesc="A simple RSS Reader"
arch=(any)
url="https://github.com/juanvel4000/ufr"
license=('GPL')
depends=('python' 'python-requests' 'python-xmltodict')
makedepends=('python-setuptools')
source=("https://files.pythonhosted.org/packages/2e/63/c4f27c3eeba65f0a288e28b0dca0b3be47353a2df4aa568ec88cbdcdf211/unnfr-0.2.0.tar.gz")
sha256sums=('e66a129c81ae54b2195087e7111027fd170f5b0008ac0d0fd95afb96eccb5407')

build() {
    cd "$pkgname-$pkgver"
    python setup.py build
}

package() {
    cd "$pkgname-$pkgver"
    python setup.py install --root="$pkgdir" --optimize=1
}
