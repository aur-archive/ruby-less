# Generated by gem2arch (https://github.com/anatol/gem2arch)
# Maintainer: Anatol Pomozov <anatol.pomozov@gmail.com>
# Contributor: Guilherme "nirev" Nogueira <guilherme@nirev.org>
# Contributor: Chris Darnell <cedeel@gmail.com>

_gemname=less
pkgname=ruby-$_gemname
pkgver=2.6.0
pkgrel=1
pkgdesc='Leaner CSS, in your browser or Ruby (via less.js)'
arch=(any)
url='http://lesscss.org'
license=(MIT)
depends=(ruby ruby-commonjs)
options=(!emptydirs)
source=(https://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
sha1sums=('41457c8d01833ae12bb5e15e0f9d276fd6e2417c')

package() {
  local _gemdir="$(ruby -e'puts Gem.default_dir')"
  gem install --ignore-dependencies --no-user-install -i "$pkgdir/$_gemdir" -n "$pkgdir/usr/bin" $_gemname-$pkgver.gem
  rm "$pkgdir/$_gemdir/cache/$_gemname-$pkgver.gem"
}
