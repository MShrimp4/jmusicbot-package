pkgname=jmusicbot
pkgver=0.3.9
pkgrel=1
pkgdesc="JMusicBot"
arch="noarch"
depends=""
license="Apache-2.0"
url="https://github.com/jagrosh/MusicBot"
source="https://github.com/jagrosh/MusicBot/releases/download/${pkgver}/JMusicBot-${pkgver}.jar
	jmusicbot.openrc"
noextract="JMusicBot-${pkgver}.jar"
builddir="$srcdir"

install="$pkgname.pre-install"

_bot_root="/var/www/discordbot"

package() {
	install -dm755 -o discordbot -g discordbot "${pkgdir}${_bot_root}"
	install -Dm755 "JMusicBot-${pkgver}.jar" "${pkgdir}${_bot_root}/JMusicBot.jar"
	install -Dm755 "jmusicbot.openrc" "${pkgdir}/etc/init.d/jmusicbot"
}
sha512sums="
ea14f241653e0412d955c32e18a7d63b5513cd5d4bbb3f953d32cdfc749450e5a65e00f59e0fbd138ecefbce1839b6232bd30b8703fd8f0f4173486966a98130  JMusicBot-0.3.9.jar
d195de4cec5ebc8e56542b9a7624159a14008ab2ff64063cc5b72b1785b2b67c79eb7a9fd1fe6b9de3019a76cfd8772d85b89e56bb15240fff443dc2665d430e  jmusicbot.openrc
"
