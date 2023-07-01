

pkgname=jmusicbot
pkgver=0.3.9
pkgrel=1
pkgdesc="JMusicBot"
arch=('any')
depends=()
source=("https://github.com/jagrosh/MusicBot/releases/download/${pkgver}/JMusicBot-${pkgver}.jar"
	"discordbot.conf"
	"jmusicbot.service")
noextract=("JMusicBot-${pkgver}.jar")
sha512sums=(SKIP SKIP SKIP)

_bot_root="/srv/discordbot"

package() {
	install -d "${pkgdir}${_bot_root}"
	install -Dm644 "JMusicBot-${pkgver}.jar" "${pkgdir}${_bot_root}/JMusicBot.jar"
	install -Dm644 "jmusicbot.service" "${pkgdir}/usr/lib/systemd/system/jmusicbot.service"
	install -Dm644 "discordbot.conf" "${pkgdir}/usr/lib/sysusers.d/discordbot.conf" 
}
