# shellcheck disable=SC2148
# Maintainer: juanvel400 <juanvel400@proton.me>
pkgname=unnfr
pkgver=0.2.3
pkgrel=1
pkgdesc="A simple RSS Reader written in python"
arch=(any)
url="https://github.com/juanvel4000/ufr"
license=('MIT')
depends=('python' 'python-requests' 'python-xmltodict' 'python-inscriptis')
makedepends=('python-setuptools')
source=("https://files.pythonhosted.org/packages/10/53/64bd6a8df0d327c70e9c6d04d1fa3c3ed8be846db7f351044862edf8beb3/unnfr-0.2.3.tar.gz")
sha256sums=('490985755568d547bb76dc513ecbe243472c9c7f9b87cf4c72bf3cc4fc57512e')

build() {
    cd "$pkgname-$pkgver"
    python setup.py build
}

package() {
    cd "$pkgname-$pkgver"
    python setup.py install --root="$pkgdir" --optimize=1
}
