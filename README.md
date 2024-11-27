# outline-install-wrt-for-ra
# оригинальный автор - https://github.com/1andrevich/outline-install-wrt

Скрипт OpenWRT /bin/sh для установки Outline (Shadowsocks) с помощью [xjasonlyu/tun2socks](https://github.com/xjasonlyu/tun2socks)

## Как использовать:

Проверьте, установлены ли у вас kmod-tun и ip-full, если нет, запустите:

    opkg update
    opkg install kmod-tun ip-full

Скачаейте скрипт в ОЗУ сделайем его исполняемым:

    cd /tmp
    wget https://raw.githubusercontent.com/ZephyrFL/outline-install-wrt-for-ra/main/install_outline.sh -O install_outline.sh
    chmod +x install_outline.sh

Вам потребуется не менее **9 MiB свободного места** /

Запустите скрипт:    

    ./install_outline.sh

Вас попросят ввести:

 - IP-адрес вашего Outline-сервера
 - Конфиг Outline (Shadowsocks) в формате «ss://base64coded@HOST:PORT».

Если у вас возникли проблемы с доступом к raw.githubusercontent.com, попробуйте использовать зеркало этого проекта **(https://sourceforge.net/projects/outline-install-wrt/)**.
