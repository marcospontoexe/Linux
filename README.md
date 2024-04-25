# Linux
O Linux é um sistema operacional de código aberto. Algumas das distribuições mais conhecidas incluem Ubuntu, Fedora, Debian e CentOS.

## Terminal do Linux
O terminal do Linux permite interagir com o sistema operacional por meio de comandos de texto. Existem vários terminais populares no Linux, cada um com suas próprias características e recursos. 
* GNOME Terminal: O GNOME Terminal é o terminal padrão do ambiente de desktop GNOME. Ele é conhecido por sua interface simples e fácil de usar, além de suportar várias abas e personalização.
* Konsole: O Konsole é o terminal padrão do ambiente de desktop KDE. Ele oferece uma ampla variedade de recursos avançados, como divisão de tela, suporte a cores e personalização extensiva.
* Terminator: O Terminator é um terminal de código aberto que oferece recursos avançados de divisão de tela e layout. Ele permite dividir a tela em várias janelas e trabalhar com várias sessões ao mesmo tempo.
* Xfce Terminal: O Xfce Terminal é o terminal padrão do ambiente de desktop Xfce. Ele é conhecido por sua leveza e simplicidade, oferecendo recursos essenciais para a maioria dos usuários.
* Tilix: Tilix é um terminal de código aberto que oferece recursos avançados, como divisão de tela, personalização de layout e suporte a várias abas. Ele é altamente personalizável e adequado para usuários avançados que precisam de funcionalidades avançadas.

## Comandos de texto
A linha de comando é composta sequêncialmente por: **nome do comando**,  **parâmetros** e **argumentos**.

* Nome do comando é o próprio comando que você deseja executar. Por exemplo, "ls" é o comando para listar arquivos e diretórios, "cd" é o comando para mudar de diretório e "mkdir" é o comando para criar um novo diretório.
    * Sempre é escrito com letras minúsculas.
      
* Os parâmetros modificam o comportamento padrão do comando.
    *  Geralmente são precedidas por um hífen ("-") quando o parâmetro é abreviado com uma letra (`ls -a`, exibe os todos os arquivos e diretórios),
    *  ou dois hifens ("--") quando o parâmetro é escrito por extenso (`ls --all`).
    *  Para alguns comandos não é necessário usar parâmetro na linaha de comando (`cd /diretório pai/diretório filho`).
    *  É possível usar mais de um parâmetro na mesma linha de comando (`ls -a -h`, exibe todos os arquivos do diretório de forma humanizada).
    *  Os parâmetro são case sensitive.
    *  Em alguns comandos, o parâmetro "-h" lista todos os parâmetros disponíveis para aquele comando.
      
* Argumentos: São informações adicionais fornecidas ao comando para que ele possa executar sua função. Por exemplo, ao usar o comando "cd", você precisa especificar o diretório para o qual deseja mudar. Da mesma forma, ao usar o comando "mkdir", você precisa fornecer o nome do novo diretório que deseja criar.

* A tecla **TAB** pressionada uma vez pode ser usada para completar o comando.
* A tecla **TAB** pressionada duas vezes mostra os possíveis complementos para o comando.
* A palavra **sudo** precedida do comando, executa o comando com permissão de administrador.

### Alguns comando úteis
O comando apt é uma ferramenta de gerenciamento de pacotes usada em sistemas operacionais baseados em Debian:
* `apt search “nome do pacote”`: mostra uma lista com pacotes disponíveis para instalação pelo apt.
* `apt install “nome do pacote”`: instala pacotes.
* `apt update`: atualiza pacote
* `apt remove “nome do pacote”`: remove pacotes.
* `apt autoremove`: apaga pacotes de programas removidos.
  
Comando list:
* `ls`: lista os diretorios filhos e arquivos do diretorio atual.
* `ls -l`: listagem longa.
* `ls -a`: mostra todos os diretorios e arquivos, incluisve os arquivos ocultos (para deixar o arquivos oculto, colocar um “.” antes do nome do arquivos).

Comando change directory:
* `cd /diretorio/diretorio`: troca de diretório.
* `cd ~`: muda para o diretorio do usuário.
* `cd /`: muda para o diretorio raiz.
* `cd ..`: retorna um diretorio.

Comando dpkg:
* `sudo dpkg --install “nome do pacote”`: instala um pacote através do gerenciador de pacotes (dpkg).
* `sudo dpkg --remove “nome do pacote”`: remove um pacote através do gerenciador de pacotes (dpkg).

O comando mkdir é utilizado para criar diretórios.
* `mkdir “nome do riretorio”`: cria um diretório.
* `mkdir "diretorio1" "diretorio2" "diretorio3"`: cria vários diretórios de uma só vez.
  
