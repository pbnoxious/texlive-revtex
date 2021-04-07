# Contributor: pbnoxious <pbnoxious@web.de>

pkgname=latex-revtex
pkgver=4.2e
pkgrel=1
pkgdesc="REVTeX package used by the American Physical Society, American Institute of Physics, and Optical Society of America"
arch=('any')
url='https://journals.aps.org/revtex'
license=('')
makedepends=('unzip')
depends=('texlive-latex3')
source=('http://mirrors.ctan.org/install/macros/latex/contrib/revtex.tds.zip')
md5sums=('0427e76dace754ed568968c5ff689909')

package() {
  for d in bibtex doc source tex; do
    install -m 0664 -d -D ${srcdir}/${d} /usr/share/texmf/${d}
  done
}
