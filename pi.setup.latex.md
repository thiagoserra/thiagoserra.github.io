# RaspberryPi como máquina de escrever

![equipamento 01](imagens/pi_kit_00.png | width=350)
![equipamento 02](imagens/pi_kit_01.png | width=350)

![equipamento 03](imagens/pi_kit_02.png | width=350)


Este brevíssimo artigo mostra meu projeto com Raspberry Pi (3b), utilizando-o como
uma máquina de escrever moderna :-)

Explicando... como um compilador portátil para produzir documentos em Latex.

## Passo 1 - Instalar o Raspbian
Hoje existem mais de 20 flavours de Linux para ARM, mas, pela facilidade de adaptação ao hardware,
indico sempre o [Raspbian](https://www.raspberrypi.org/downloads/raspbian/).

A instalação é muito simples, existem criadores de SD para Window, Linux e Mac. Procure
por [Raspberry Pi Imager](https://www.raspberrypi.org/downloads/) e baixo o específico para seu S.O.

Ao executar, a  instalação é intuitiva, sendo necessário indicar o S.O. (Raspbian), o destino (SD)
 e, mandar baixar e instalar.

## Passo 2 - Após o boot
Primeira coisa, mudar a senha do usuário pi e partir para as instalações dos pacotes e apps:
Antes, dê um apt update e apt upgrade...

Coisas que não uso:

```
sudo apt purge thonny
sudo apt purge vim-tiny
```

Pacotes para Latex:

```
sudo apt install texlive-base texlive-lang-portuguese
sudo apt install texlive-extra-utils 
sudo apt install texlive-fonts-recommended
sudo apt install texlive-lang-greek
sudo apt install texlive-latex-extra texlive-lang-other
sudo apt install texlive-latex-recommended
sudo apt install texlive-xetex 
sudo apt install abntex2 texlive-publishers
```

Alguns sw úteis (pelo menos eu uso):

```
sudo apt install mc
sudo apt install vim
sudo apt install htop
sudo apt install ncdu
sudo apt install openssh-client
sudo apt install fonts-firacode
sudo apt install evince
```

Para meu teclado e mouse:

```
sudo apt install solaar
```


O editor de texto e pacote de correção de texto:

```
sudo apt install geany geany-plugin-latex
sudo apt install geany-plugin-spellcheck geany-plugin-ctags geany-plugin-git-changebar
sudo apt install myspell-pt-br
```

## Passo 3: configurar o Geany
O geany é um editor de texto simples e leve, rodando bem no Pi.
Ele possui diversos plugins para melhorar a experiência e, um específico para documentos Tex.

Abaixo os que deixo habilitado:

![geany plugins](imagens/pi_ed_1.png | width=350)


## O Resultado
A experiência é bastante tranquila.

Como meu notebook permanece em casa e, editar Tex no iPad Pro é uma aventura complicada,
basta colocar o Pi na mochila.

Levo um teclado Logitech K230 e um mouse M280 (ambos em fio, conectados pelo mesmo receptor), um Adaptor HDMI para VGA e,
uma fonte 5V.

A comodidade do F9 (gerar PDF a partir do Latex) e depois F5 (mostrar o arquivo PDF gerado).

Fora que você poderá andar com sua "máquina de escrever" onde for, bastando ter um monitor a sua disposição.

No meu caso, todos os meus trabalhos estão no github, o que torna ainda mais fácil e portável a experiência!



![geany tela inicial - digitando](imagens/pi_ed_2.png | width=250)
![geany menu construir - gerar pdf e dvi](imagens/pi_ed_3.png | width=250)
![geany atalhos para comandos](imagens/pi_ed_4.png | width=250)

![geany definir comandos de compilação](imagens/pi_ed_5.png | width=250)





Esse e outros artigos estão compartilhados no GitHub!

Acesse: https://thiagoserra.github.io

