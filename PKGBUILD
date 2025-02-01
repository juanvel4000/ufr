# shellcheck disable=SC2148
# shellcheck disable=SC2034
# shellcheck disable=SC2164
# shellcheck disable=SC2154
# Maintainer: juanvel400 <juanvel400@proton.me>
pkgname=unnfr
pkgver=0.2.5
pkgrel=1
pkgdesc="A simple RSS Reader written in python"
arch=(any)
url="https://github.com/juanvel4000/ufr"
license=('MIT')
depends=('python' 'python-requests' 'python-xmltodict' 'python-inscriptis')
makedepends=('python-setuptools')
source=("https://files.pythonhosted.org/packages/85/c0/a8bbd80b9aa6a988ce6523f91dd112f4d37002de3a9e039b8b241ebb184c/unnfr-0.2.5.tar.gz")
sha256sums=('a6422499d0a84fe0be06e1d9f5298e0b4fe76748595bc861d46089e0743eaa98')

build() {
    cd "$pkgname-$pkgver"
    python setup.py build
}

package() {
    cd "$pkgname-$pkgver"
    python setup.py install --root="$pkgdir" --optimize=1
}
