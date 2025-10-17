# Solució: T03: Seguretat Lògica: recuperant accés a sistemes
![Portada](img/PorT03.png)

👤 Autor: Jhon Justiniano
🏫 Curs: SMX-B
🔒 Mòdul: Seguretat Informàtica

## 🗂️ Índex

- Introducció

- Procediment individual

- Vulnereu l’accés al GRUB del Linux

- Identifiqueu l’usuari del sistema

- Modifiqueu la contrasenya de l’usuari i verifiqueu que ara ja té accés

- Investigueu com es pot fortificar l’accés al GRUB. És molt important que indiquis les fonts d’informació que usis

- Configura la màquina virtual per tal de fortificar l’accés al GRUB

## 📄 Introducció
Després de la primera feina exitosa, us arriba un encàrrec urgent que obliga a que us hi poseu per donar-li solució.

Com a fase prèvia rebreu una formació sobre la seguretat lògica que us permetrà tenir els coneixements necessaris per afrontar la tasca.

Han arribat a la consultora un equip provinent d’un client que demana que els hi solucionem el problema.

Tenen un portàtil amb Zorin OS (un Linux amb entorn gràfic) que usava habitualment un directiu. El problema és que ha oblidat la contrasenya i és necessari poder recuperar l’accés perquè hi ha documentació molt important que cal recuperar. Per evitar que una acció catastròfica pugui danyar l’equip original, ens han clonat el disc en un disc virtual perquè hi treballeu.

Per tant, el primer pas serà crear una màquina virtual al que connectareu aquest disc. A continuació, cal que entreu a la màquina virtual, trobeu el nom de l’usuari existent i assigneu-li una contrasenya nova.

Quan el client és informat del senzill que és accedir a l’equip, demana si n’hi ha alguna manera de fortificar el sistema, ja que té por que si algú roba el portàtil hi pugui accedir a la informació que hi conté. Per tant, ara ens demanen que cerquem solucions per tal d’evitar que es pugui reiniciar la contrasenya amb el procediment anterior.

Investigueu el procediment per tal que l’accés al GRUB quedi protegit per contrasenya per evitar canvis de configuració.

## 💻 Procediment individual
Primer abans de tot hem de crear la màquina, per això ens anem a virtualbox i li donem a nova, posem al nom, on la volem guardar i per últim posar l’ISO que ens van donar en la comuna.

![foto1](img/1.png)

Desprès ens anem a hardware y posem de memòria base 4096 MB i de processadors hi posem 4.

![foro2](img/2.png)

Seguidament ens dirigim a configuracions i a l’apartat de emmagatzematge hem de posar el discs que tambè ens la donan en la comuna, el disc ho hem de posar com a sata. Desprès guardem i li donem a iniciar la màquina.

![foto3](img/3.png)

## 🔒 Vulnereu l’accés al GRUB del Linux
Una vegada li donem a iniciar la máquina hem de presionar shift + qualsevol lletra, això ho hem de fer per poder estar com a root sense que iniciem sessió. Ens surtirà un menú el cual en d’entrar a “Advanced options for Zorin”

![foto4](img/4.png) 

Una vegada entrem ens sortirà un altre menù el cual hen d’entrar a la segona opció “Zorin, with Linux 6.8.0-85-generic (recovery mode)”

![foto5](img/5.png)
