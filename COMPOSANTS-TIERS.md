# Composants tiers / Third-party components

WDCPi assemble des logiciels libres. Chacun garde **sa propre licence**. La licence de WDCPi ([LICENSE.md](LICENSE.md))
ne couvre que le code propre à WDCPi : la console, l'installateur et les scripts. Elle ne s'applique à aucun des
composants ci-dessous.

*WDCPi bundles free software. Each component keeps **its own licence**. The WDCPi licence ([LICENSE.md](LICENSE.md))
covers only WDCPi's own code (the console, the installer and the scripts), and none of the components below.*

## Dans l'image Raspberry Pi / In the Raspberry Pi image

| Composant / Component | Licence | Code source / Source code |
|---|---|---|
| Raspberry Pi OS (Debian 13 « trixie ») et ses paquets | licences propres à chaque paquet (surtout GPL, LGPL, BSD, MIT) | https://deb.debian.org/debian/pool/ · https://archive.raspberrypi.com/debian/pool/ |
| Noyau Linux / Linux kernel | GPL-2.0 | https://github.com/raspberrypi/linux |
| Firmware Raspberry Pi | licence propre (redistribuable) / own licence (redistributable) | https://github.com/raspberrypi/firmware |
| Docker Engine, containerd, runc | Apache-2.0 | https://github.com/moby/moby · https://github.com/containerd/containerd · https://github.com/opencontainers/runc |
| Fail2ban | GPL-2.0 | https://github.com/fail2ban/fail2ban |
| UFW | GPL-3.0 | https://launchpad.net/ufw |
| WireGuard tools | GPL-2.0 | https://git.zx2c4.com/wireguard-tools |
| OpenVPN | GPL-2.0 | https://github.com/OpenVPN/openvpn |
| needrestart, unattended-upgrades | GPL-2.0 / GPL | paquets Debian (voir ci-dessus) / Debian packages (see above) |
| Python et ses bibliothèques : FastAPI, Starlette, Uvicorn, Pydantic, psutil, dnspython, python-multipart, python-pam | licences propres (MIT, BSD, ISC, Apache-2.0) | paquets Debian `python3-*` / Debian `python3-*` packages |

## Téléchargés au premier démarrage / Downloaded at first boot (images Docker officielles / official Docker images)

| Composant / Component | Licence | Code source / Source code |
|---|---|---|
| Caddy (+ modules caddy-dns) | Apache-2.0 (modules : voir chaque dépôt / see each repository) | https://github.com/caddyserver/caddy · https://github.com/caddy-dns |
| MariaDB | GPL-2.0 | https://github.com/MariaDB/server |
| WordPress | GPL-2.0-or-later | https://github.com/WordPress/WordPress |
| PHP | licence PHP / PHP licence | https://github.com/php/php-src |
| Apache HTTP Server | Apache-2.0 | https://github.com/apache/httpd |
| Nginx | BSD-2-Clause | https://github.com/nginx/nginx |
| Adminer | Apache-2.0 ou GPL-2.0 / Apache-2.0 or GPL-2.0 | https://github.com/vrana/adminer |
| mlocati/php-extension-installer | MIT | https://github.com/mlocati/docker-php-extension-installer |

## Code source des composants GPL / Source code of GPL components

Les paquets de l'image sont ceux, non modifiés, des dépôts officiels de Debian et de Raspberry Pi. Leur code source
est disponible aux adresses ci-dessus. La version exacte de chaque paquet est listée dans le fichier
`wdcpi-AAAA-MM-JJ.paquets.txt` publié avec chaque image. Si une source manque, demandez-la par une
[issue](https://github.com/Trano89/WDCPi/issues) : nous la fournirons.

*The image's packages are the unmodified packages from the official Debian and Raspberry Pi repositories. Their
source code is available at the addresses above. The exact version of each package is listed in the
`wdcpi-YYYY-MM-DD.paquets.txt` file published with each image. If a source is missing, ask for it in an
[issue](https://github.com/Trano89/WDCPi/issues) and we will provide it.*
