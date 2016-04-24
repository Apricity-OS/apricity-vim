#Maintainer: Alex Gajewski <agajews@gmail.com>

_pkgname='Apricity Vim'
pkgname=apricity-vim
pkgver=0.1.4
pkgrel=1
pkgdesc='Vim config for Apricity OS'
arch=(any)
license=(GPL)
install="apricity-vim.install"
url="https://github.com/ApricityOS"
source=("apricity-vim.tar.gz")
sha256sums=('1c4dae9bcf39742f001a8bc7c110a2f20d1cd3820b47ef53c220809dc07c2fd7')

package() {
	mkdir -p "${pkgdir}/etc/skel/"
	rm -rf "${pkgdir}/etc/skel/.vim"
	rm -f "${pkgdir}/etc/skel/.vimrc"
	cp -rf "${srcdir}/apricity-vim/.vim" "${pkgdir}/etc/skel"
	cp -f "${srcdir}/apricity-vim/.vimrc" "${pkgdir}/etc/skel"

	mkdir -p "${pkgdir}/root/"
	rm -rf "${pkgdir}/root/.vim"
	rm -f "${pkgdir}/root/.vimrc"
	cp -rf "${srcdir}/apricity-vim/.vim" "${pkgdir}/root"
	cp -f "${srcdir}/apricity-vim/.vimrc" "${pkgdir}/root"
}
