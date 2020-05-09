# Setup básico ou post-install do Ubuntu 20.04
O que não está aqui:
  - Browser: [Vivaldi](https://vivaldi.com/pt-br/)
  - [Insync](https://www.insynchq.com)
  - [Ulauncher](https://ulauncher.io)

## Primeiro, excluir
    sudo apt purge thunderbird* rhythmbox firefox* hexchat
    sudo apt remove vim-tiny


## Atualizar
    sudo apt update
    sudo apt upgrade


## Instalar alguns softwares de uso corrente
    sudo apt install ubuntu-restricted-extras
    sudo apt install gnome-sushi flameshot
    sudo apt install mc htop ncdu neofetch curl

    sudo apt install speedtest-cli speedometer
    sudo apt install p7zip-full rar
    sudo apt install ntfs-3g exfat-fuse exfat-utils
    sudo apt install fonts-liberation fonts-inconsolata ttf-mscorefonts-installer
    sudo apt install git vim ctags
    sudo apt install build-essential apt-transport-https ca-certificates software-properties-common

    sudo apt install audacity gimp inkscape pdfshuffler
    sudo snap install bing-wall

    sudo apt install obs-studio obs-plugins
    sudo snap install kdenlive

## Instalar os pacotes do Latex
_Mudar isso para o docker??_

    sudo apt install texlive-extra-utils texlive-base texlive-lang-portuguese texlive-pictures texlive-fonts-extra texlive-fonts-recommended


## Instalacão do youtube-dl
    sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
    sudo chmod a+rx /usr/local/bin/youtube-dl


## Docker
Para instalar:

    sudo apt install docker.io docker-compose

Depois:

    sudo systemctl enable --now docker
    sudo usermod -aG docker seu_usuario

Depois só checar:

    docker --version

## Hardware
O único hardware que precisa de atenção é meu teclado.
Uso um Logitech G413 (layout americano).
Os acentos funcionam normalmente como layout do teclado após a escolha do idioma português do brasil para todo o sistema, mas o cedilha nada...


![Teclado - Seleção do idioma](imagens/teclado_1.png)


![Teclado - Seleção do modelo](imagens/teclado_2.png)

Para configurá-lo no Ubuntu, é preciso escolher o layout:


E adicionar no arquivo /etc/environment a seguinte linha:

    export GTK_IM_MODULE=cedilla

Depois de um reboot funciona tranquilo o cedilha.

