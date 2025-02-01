# shellcheck disable=SC2148
# Maintainer: juanvel400 <juanvel400@proton.me>
pkgname=unnfr
pkgver=0.2.4
pkgrel=1
pkgdesc="A simple RSS Reader written in python"
arch=(any)
url="https://github.com/juanvel4000/ufr"
license=('MIT')
depends=('python' 'python-requests' 'python-xmltodict' 'python-inscriptis')
makedepends=('python-setuptools')
source=("https://files.pythonhosted.org/packages/fc/a5/1b4140e3d55d7f2e1af3f3a314687d56013d7f0a58a19ffd53cf7ef93458/unnfr-0.2.4.tar.gz")
sha256sums=('5c4e0bdc7e20320e01604751ff593c177b6d2ca072d26510fce962fed6032b53')

build() {
    cd "$pkgname-$pkgver"
    python setup.py build
}

package() {
    cd "$pkgname-$pkgver"
    python setup.py install --root="$pkgdir" --optimize=1
}
