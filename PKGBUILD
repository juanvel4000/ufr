# shellcheck disable=SC2148
# Maintainer: juanvel400 <juanvel400@proton.me>
pkgname=unnfr
pkgver=0.2.2
pkgrel=1
pkgdesc="A simple RSS Reader"
arch=(any)
url="https://github.com/juanvel4000/ufr"
license=('GPL')
depends=('python' 'python-requests' 'python-xmltodict' 'python-inscriptis')
makedepends=('python-setuptools')
source=("https://files.pythonhosted.org/packages/9f/b2/0714619aca4a3213b930a1453be5dfa6bc39c1cbeb81a4f24873caceb472/unnfr-0.2.2.tar.gz")
sha256sums=('ddf697fdba56d364d9f3ab37d45c6ea031859971d9ebc85c970a165cf099c083')

build() {
    cd "$pkgname-$pkgver"
    python setup.py build
}

package() {
    cd "$pkgname-$pkgver"
    python setup.py install --root="$pkgdir" --optimize=1
}
