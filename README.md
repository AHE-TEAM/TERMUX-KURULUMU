# Termux Kurulumu ve Yapılandırması

Termux, Android üzerinde güçlü bir Linux terminal ortamı sağlar.

## Termux İndirme

Termux artık Google Play Store'dan desteklenmiyor. Bunun yerine şu adresten yükleyebilirsiniz:

- **F-Droid'**[den indirin](https://f-droid.org/packages/com.termux/)
- **Github'** [dan indirin](https://github.com/termux/termux-app/releases/)
- **Diğer Termux Uygulamaları:** [F-Droid Arama](https://search.f-droid.org/?q=termux&lang=en)

## Temel Komutlar

- **Paketleri Güncelleyin:**

    ```bash
    pkg update
    pkg upgrade
    ```

- **Paketleri Temizleyin:**

    ```bash
    pkg autoclean
    pkg clean
    ```

- **Depo Yansımalarını Güncelleyin:**

    ```sh
    termux-change-repo
    ```

## Yaygın Paketler

- **cURL:**

    ```bash
    pkg install curl
    ```

- **Git:**

    ```bash
    pkg install git
    ```

- **wget:**

    ```bash
    pkg install wget
    ```

- **Zip ve Unzip:**

    ```bash
    pkg install zip unzip
    ```

- **Python 2 ve 3:**

    ```bash
    pkg install python2
    pkg install python
    ```

- **Node.js (LTS sürümü):**

    ```bash
    pkg install nodejs
    pkg install nodejs-lts
    ```

- **jq (JSON Formatlama):**

    ```bash
    pkg install jq
    ```

- **libxml2-utils:**

    ```bash
    pkg install libxml2-utils
    ```

- **grep:**

    ```bash
    pkg install grep
    ```

- **bc (Hassas Hesaplama):**

    ```bash
    pkg install bc
    ```

- **htop (Sistem Yöneticisi):**

    ```bash
    pkg install htop
    ```

- **figlet:**

    ```bash
    pkg install figlet
    ```

- **httping (HTTP Pinger):**

    ```bash
    pkg install httping
    ```

- **dnsutils (IP Adresi Bulma):**

    ```bash
    pkg install dnsutils
    ```

- **openssh (SSH ve SFTP Yönetimi):**

    ```bash
    pkg install openssh
    ```

- **FFmpeg (Multimedya İşleme):**

    ```bash
    pkg install ffmpeg
    ```

- **youtube-dl:**

    ```bash
    curl -sL https://gist.githubusercontent.com/santhoshkumar/48dad71342f8dc68029b5d5f33504302/raw/13d40d51dd45597f2b74b30361c642f3e56ed187/package.sh | bash
    ```

- **PHP ve Composer:**

    ```bash
    pkg install php
    curl -sS https://getcomposer.org/installer | php -- --install-dir=/data/data/com.termux/files/usr/bin --filename=composer
    ```

- **nano (Düzenleyici):**

    ```bash
    pkg install nano
    ```

- **Zsh (Ohmyzsh ile birlikte):**

    ```bash
    pkg install zsh
    ```

- **HTTPie (cURL Alternatifi):**

    ```bash
    pip install --upgrade pip setuptools
    pip install --upgrade httpie
    pip install -U requests[socks]
    pip install requests
    ```

- **Python Geliştirme Paketleri:**

    ```bash
    pkg install clang libffi openssl
    ```

- **DuckDuckGo:**

    ```bash
    pip install ddgr
    ```

- **screenfetch (Sistem Bilgisi):**

    ```bash
    pkg install screenfetch
    ```

- **w3m (Metin Tabanlı Tarayıcı):**

    ```bash
    pkg install w3m
    ```

- **cowsay:**

    ```bash
    pkg install cowsay
    ```

- **perl:**

    ```bash
    pkg install perl
    ```

- **Ruby:**

    ```bash
    pkg install ruby
    ```

- **Rust:**

    ```bash
    pkg install rust
    ```

- **Cloudflared:**

    ```bash
    pkg install cloudflared
    ```

- **sqlite:**

    ```bash
    pkg install sqlite
    ```

- **fakeroot:**

    ```bash
    pkg install fakeroot
    ```

- **sshpass:**

    ```bash
    pkg install sshpass
    ```

- **Golang:**

    ```bash
    pkg install golang
    ```

- **PRoot:**

    ```bash
    pkg install proot
    ```

## Özelleştirme ve Ekstra Araçlar

- **Ekstra Tuş Satırlarını Etkinleştirin:**

    `.termux/termux.properties` dosyasına şu satırları ekleyin:

    ```bash
    extra-keys = [ \
    ['ESC','|','/','HOME','UP','END','PGUP','DEL'], \
    ['TAB','CTRL','ALT','LEFT','DOWN','RIGHT','PGDN','BKSP'] \
    ]
    ```

- **Termux-exec ve Termux API:**

    ```bash
    pkg install termux-exec
    pkg install termux-api
    ```

- **SD Kart Erişimi:**

    ```bash
    termux-setup-storage
    ```

- **Depo ve Paket Yönetimi:**

    ```bash
    pkg list-installed
    pkg uninstall <package-name>
    termux-upgrade-repo
    ```

- **Yardım:**

    ```bash
    pkg help
    ```

## Ek Kaynaklar

- [Termux Wiki](https://wiki.termux.com/wiki/Main_Page)
- [Termux-setup-storage hakkında daha fazla bilgi](https://wiki.termux.com/wiki/Termux-setup-storage)

Bu yapılandırmalar, Termux kullanımınızı daha verimli ve işlevsel hale getirecektir.

