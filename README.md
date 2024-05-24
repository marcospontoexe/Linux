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

* Nome do **comando** é o próprio comando que você deseja executar. Por exemplo, "ls" é o comando para listar arquivos e diretórios, "cd" é o comando para mudar de diretório e "mkdir" é o comando para criar um novo diretório.
    * Sempre é escrito com letras minúsculas.
      
* Os **parâmetros** modificam o comportamento padrão do comando.
    *  Geralmente são precedidas por um hífen ("-") quando o parâmetro é abreviado com uma letra (`ls -a`, exibe os todos os arquivos e diretórios),
    *  ou dois hifens ("--") quando o parâmetro é escrito por extenso (`ls --all`).
    *  Para alguns comandos não é necessário usar parâmetro na linaha de comando (`cd /diretório pai/diretório filho`).
    *  É possível usar mais de um parâmetro na mesma linha de comando (`ls -ah` ou `ls -a -h`, exibe todos os arquivos do diretório de forma humanizada).
    *  Os parâmetro são case sensitive.
    *  Em alguns comandos, o parâmetro "-h" lista todos os parâmetros disponíveis para aquele comando.
      
* **Argumentos**: É o nome de um arquivo ou path de um diretorio.

* A tecla **TAB** pressionada uma vez pode ser usada para completar o comando.
* A tecla **TAB** pressionada duas vezes mostra os possíveis complementos para o comando.
* A palavra **sudo** precedida do comando, executa o comando com permissão de administrador.

### Alguns comando úteis
* `pwd` : mostra o caminho absoluto (caminho atual).
* `man` : mostra o manual de um comando (man ls, mostra o manual do ls).
* `history` : mostra o histórico de comando digitados. Para acessar o comando digitar "!" e o número do histórico.
* `cat` : imprimi o conteúdo do arquivo na tela.
* `cp arquivo diretório/` : copia o "arquivo" para a pasta "diretório".
* `mv arquivo diretório/` : move o "arquivo" para a pasta "diretório".
* `rm arquivo` : apaga um arquivo.
* `mv arquivo/ arq/` : renomeia o arquivo "arquvio" para "arq".

O comando **aptitude** é uma interface de linha de comando para o gerenciador de pacotes APT (Advanced Package Tool) usado em sistemas operacionais baseados em Debian, como Ubuntu e Debian:
* `sudo aptitude update`: Antes de instalar qualquer pacote, é uma boa prática garantir que o índice de pacotes esteja atualizado
* sudo aptitude install nome_pacote: Instala um pacote desejado.
  
O comando **apt** é uma ferramenta de gerenciamento de pacotes usada em sistemas operacionais baseados em Debian:
* `apt search “nome do pacote”`: mostra uma lista com pacotes disponíveis para instalação pelo apt.
* `apt install “nome do pacote”`: instala pacotes.
* `apt update`: atualiza pacote
* `apt remove “nome do pacote”`: remove pacotes.
* `apt cleam`: limpa o cache.
* `apt autoremove`: apaga pacotes de programas removidos.
  
Comando **ls** (list):
* `ls`: lista os diretorios filhos e arquivos do diretorio atual.
* `ls -l`: listagem longa.
* `ls -a`: mostra todos os diretorios e arquivos, incluisve os arquivos ocultos (para deixar o arquivos oculto, colocar um “.” antes do nome do arquivos).

Comando **cd** (change directory):
* `cd /diretorio/diretorio`: troca de diretório.
* `cd ..`: retorna um diretorio.
* `cd .`: diretorio atual.
* `cd ~`: muda para o diretorio do usuário.
* `cd /`: muda para o diretorio raiz.
   * .bin : Armazena todos os comandos usado pelo terminal.
   * .boot: Armazena o kernel, contém arquivos necessários para a inicialização do sistema.
   * .dev : Armazenas as unidades (usb, serial, hd...).
   * .lib : Bibliotecas compartilhadas pelos programas do sistema e módulos do kernel.
   * .etc : contém arquivos de configuração para o sistema operacional, seus serviços e aplicativos.
   * .home : onde fica armazenado os arquivos e diretórios dos usuários.
   * .usr : onde os programas são instalados.
   * .root: onde fica armazenado os arquivos e diretórios do usuário root.
   * .sbin : arquivos executáveis de uso exclusivo do root.
   * .media : requentemente utilizada para montagem automática de dispositivos de armazenamento removíveis, como unidades USB, CDs, DVDs e outros dispositivos de mídia.
   * .mnt : é frequentemente utilizada para montagem manual de sistemas de arquivos temporários ou compartilhados.
   * .opt : é uma pasta comum em sistemas Linux e geralmente é usada para instalar aplicativos e pacotes de software adicionais que não são fornecidos pelos repositórios oficiais da distribuição.
   *  .proc : é um diretório especial no sistema de arquivos Linux que contém informações sobre processos em execução e informações do kernel.
   *  .run : é possível que os usuários ou aplicativos criem essa pasta para armazenar arquivos executáveis ou scripts específicos
   * .usr : é uma das pastas mais importantes no sistema de arquivos Linux e geralmente contém dados e programas de uso compartilhado por todos os usuários do sistema. Ela é uma abreviação de "Unix System Resources" (Recursos do Sistema Unix).
   *  .var é uma das pastas fundamentais no sistema de arquivos Linux e é utilizada para armazenar dados variáveis que podem ser modificados durante a operação normal do sistema.     

Comando **dpkg**:
* `sudo dpkg --install “nome do pacote”`: instala um pacote através do gerenciador de pacotes (dpkg).
* `sudo dpkg --remove “nome do pacote”`: remove um pacote através do gerenciador de pacotes (dpkg).

O comando **mkdir** é utilizado para criar diretórios.
* `mkdir “nome do riretorio”`: cria um diretório.
* `mkdir "diretorio1" "diretorio2" "diretorio3"`: cria vários diretórios de uma só vez.
* `mkdir -p diretorio1/diretorio2/sub\ diretório`: criará tanto diretorio1, diretorio2 e sub diretório, mesmo que diretorio1 não exista previamente.
* `mkdir "pasta1/pasta2/ sub diretório"` : criará tanto pasta1, pasta2 e sub diretório, sem precisar da contra barra bara inserir o espaço.
* `mkdir -m 755 nome-do-diretorio`: Permite especificar as permissões (modo) dos diretórios criados. Criará um diretório com permissões de leitura, escrita e execução para o proprietário, e apenas permissões de leitura e execução para os outros.
  
O comando **touch** é usado para criar arquivos de qualquer tipo de extensão:
* `touch “arquivo.extenção”`: cria um arquivo no diretorio atual.

### Caracteres de referência global
Os caracteres de referência global são ultilizados nos parâmetros de comandos para realizar operações de busca e manipulação de texto com base em padrões definidos, por exempolo o regex.
* \* : Substitui uma ou mais letra do argumento do comando.
    * "cat*" corresponde a qualquer cadeia de caracteres que comece com "cat" e termie com qualquer caractere.
    * "*.conf" corresponde a todos arquivos de configuração.
* \? : usado para substituir apenas uma letra do argumento do comando.
    * "?sys" corresponde a qualquer cadeia de caracteres que tenha apenas uma letra antes de "sys".
* \[a-z] : substitui qualquer letra do argumento por uma faixa de caracteres (de a até z no exemplo).
    * "c[a-o]" corresponde a qualquer cadeia de caracteres que comece com a letra "c" seguido por um intervalor de "a" até "o". 
* \[a,z] : substitui qualquer letra do argumento por a ou z.
    *  "c[a,o]" corresponde a qualquer cadeia de caracteres que comece com a letra "c" seguido por "a" ou "o".
    *  "c[a,h-o]" corresponde a qualquer cadeia de caracteres que comece com a letra "c" seguido por "a" mais um intervalor de "h" até "o".
* \{ab,cd} : Usado para fazer referência a padrões de caractere.
    * "*.{conf, old}" : Retorna qualquer extensão .conf e .old.
 
## Gerenciamento de permissões
O gerenciamento de permissões no Linux é uma parte fundamental da segurança do sistema e permite controlar quem pode **acessar**, **modificar** ou **executar** arquivos, diretórios ou link no sistema de arquivos.

As permissões no Linux são atribuídas a cada arquivo, diretório ou link e são definidas para três tipos de usuários: o proprietário do arquivo, o grupo do arquivo e todos os outros usuários do sistema.

Ao usar o comando `ls -l` será retornado algo parecido com 

![arquivo](https://github.com/marcospontoexe/Linux/blob/main/imagens/ls%20para%20arquivo.png)
para um arquivo.

![diretório](https://github.com/marcospontoexe/Linux/blob/main/imagens/ls%20para%20diret%C3%B3rio.png)
para um diretório.

* A primeira letra se refere ao tipo de arquivo.
  *  d(diretório)
  *  -(programa)
  *  l(link) 
* As 2°, 3° e 4° letras são as permissões do usuário (u de user), dono do diretorio ou programa ou link. 
* As 5°, 6° e 7° letras são as permissões do grupo (g de group) 
* As 8°, 9° e 10° letras são as permissões dos demais grupos ou usuários (o de others) 

Os seguinte tipos de permissões no Linux são:
* Leitura (r): Permite visualizar o conteúdo de um arquivo ou listar o conteúdo de um diretório.
* Escrita (w): Permite modificar ou adicionar conteúdo a um arquivo ou criar, renomear ou excluir arquivos em um diretório.
* Execução (x): Permite executar um arquivo como um programa ou script ou acessar um diretório e seus subdiretórios.
* Permissão negada (-).
  
exemplo: **drwxr-xrw-**
* é um diretório
* USER tem permissão rwx
* GROUP tem apenas permissão rx
* OTHERS tem apenas permissão rw

O comando **chmod** gerencia as permissões dos arquivos, diretórios ou link, que são os argumentos do comando:
* `chmod +x “argumento”` : adiciona permissão de execussão para todos usuários.
* `chmod u-w “argumento”` : remove permissão de escrita para o usuário (u).
* `chmod g+r “argumento”` : adiciona permissão de leitura para o grupo (g).
* `chmod o-x “argumento”` : remove permissão de execussão para o outros (o).

## Script Bash
Basicamente, um script bash é um arquivo de texto comum que contém uma série de comandos. Esses comandos são uma mistura de comandos que você normalmente digitaria na linha de comando do terminal (cd, ls, cp...). Um ponto importante a lembrar, no entanto, é:
* Qualquer coisa que você possa executar normalmente na linha de comando do terminal pode ser colocada em um script e fará exatamente a mesma coisa. Da mesma forma, qualquer coisa que você possa colocar em um script também pode ser executada normalmente na linha de comando e fará exatamente a mesma coisa.

A extensão do arquivo é **`.sh`**. Normalmente, esta é a extensão que você sempre usará ao criar um novo script bash. O script deve começar com a linha `#!/bin/bash`. Todos os scripts bash começarão com esta linha especial. Basicamente, ela permite ao sistema Linux saber que este arquivo é um script bash. A imagem a baixo mostra o conteudo de um script bash para imprimir "Hello there, Developers!"

![Script bash](https://github.com/marcospontoexe/Linux/blob/main/imagens/script%20bash.png)

Para executar um scrip bash pelo terminal, digite `./nome_do_script.sh`.

### Passando um parâmetro para um script bash
É possível passar parâmetros para um script bash. Isso é útil quando você deseja que seu script execute de maneira diferente, dependendo dos valores dos parâmetros de entrada (também chamados de argumentos). Veja a baixo um script que recebe um parâmetro e imprime na tela uma menssagem de acordo com o parâmetro recebido.

![passando parâmetro para o script](https://github.com/marcospontoexe/Linux/blob/main/imagens/script%20bash%20parametros.png)

Para executar o script com o parâmetro, digite no terminal de comando: `./nome_do_script.sh valor_do_parâmetro`.

## Iniciando um serviço automaticamente
Os arquivos de serviço são usados para definir como os serviços devem ser iniciados, parados e gerenciados pelo systemd. Esses arquivos, geralmente são encontrados em "/etc/systemd/system/", possuem extensão .service e contêm configurações como o comando a ser executado, as dependências do serviço, entre outras opções de configuração.

### Inicando uma aplicação python
Para iniciar uma aplicação python, deve-se criar um arquivo de serviço (.service) no diretório "/etc/systemd/system/" e indicar nesse aqurquivo o nome do arquivo python, o path do diretório onde o arquivo python está, e o nome do usuário do sistema. Após ter criado o arquivo de serviço, recarregue o daemon do systemclt.

O systemctl é uma ferramenta poderosa e central para o gerenciamento de serviços e unidades do sistema em distribuições Linux que usam o systemd como sistema de inicialização padrão. Ele fornece uma interface consistente e eficiente para administradores de sistema controlarem e monitorarem o funcionamento do sistema e dos serviços.

Veja um passo a passo:
1. Crie um novo arquivo de serviço no diretório "/etc/systemd/system/" usando o comando `sudo touch /etc/systemd/system/nome_do_arquivo.service` no terminal do linux, ou usando a interface gráfica do sistema operacional para navegar até o diretório.
2. Adicione o seguinte conteúdo ao arquivo de serviço:
   ```
   [Unit]
   Description=Descrição do arquivo .py   #descrição sobre o serviço
   After=network.target
   
   [Service]
   User=usuário  #usuário do sistema
   WorkingDirectory=/diretório/do/arquivo  #diretório do arquivo python a ser executado 
   ExecStart=/usr/bin/python nome_do_arquivo.py  #nome do arquivo python a ser executado
   Restart=on-failure
   
   [Install]
   WantedBy=multi-user.target   #ou default.target
   ```
3. No arquivode serviço altere as informações do usuário do sistema (User), diretório e nome do arquivo ".py" de acordo com as informações do seu arquivo python.
4. Salve e feche o arquivo de serviços.
5. Recarregue o daemon do systemd usando o comando `sudo systemctl daemon-reload` no terminal do Linux.
6. Inicie o serviço usando o comando `sudo systemctl start nome_do_arquivo`. O "nome_do_arquivo" é o nome dado ao arquivo de serviços criado.
7. Verifique o status do serviço usando o comando `sudo systemctl status nome_do_arquivo`, deve ser retornado algo como:
```
   nome_do_arquivo.service - Descrição do serviço
   Loaded: loaded (/etc/systemd/system/nome_do_arquivo.service; enabled; vendor preset: enabled)
   Active: active (running) since [data e hora]
     Docs: link_para_documentação
 Main PID: [PID]
    Tasks: [número de tarefas]
   Memory: [uso de memória]
      CPU: [uso da CPU]
   CGroup: /system.slice/nome_do_arquivo.service
           └─[PID] /caminho/para/executável
```
8. Ative o serviço na inicialização do sistema usando o comando `sudo systemctl enable nome_do_arquivo`.

## Criando um alias
Cria o arquivo: `touch .bash_aliases`.
Abre o arquivo: `nano .bash_aliases`.

Exemplo de comando dentro do arquivo: `alias pharmy="ssh -X -C ubuntu@pharmy.local"`

Ativando o alias: `source .bash_aliases`.

## Matando um processo
Para ver os processos ativos em seu sistema digite `ps faux`. Para filtrar um processo use o comando **`| grep`**: `ps faux | grep nome_do_processo`.

Usando o comando **`kill`** é possível encerrar um processo. Para isso é preciso saber o **número PID** do porcesso: `kill número_PID`.

Caso o processo estaja rodando em segundo plano, o camando kill será ignorado pelo processo. Para isso, o comando bg é muito útil. O comando bg é usado para retomar a execução de um processo suspenso em segundo plano, execute agora o seguinte comando `bg`. Então, agora que a execução do processo foi retomada, o sinal de kill que enviamos antes foi recebido corretamente, então o processo que esva em segundo plano será encerrado.

## Protocolo SSH
Secure Shell, mais comumente conhecido como ssh, é um protocolo que permite aos usuários conectar-se a uma máquina remota de forma segura. Ele é baseado em uma arquitetura Cliente-Servidor. Assim, a partir da sua máquina local (Cliente), você pode fazer login na máquina remota (Servidor) para transferir arquivos entre as duas máquinas, executar comandos na máquina remota, etc.

A estrutura do comando ssh é a seguinte: `ssh [opções] user@host comando`.
* opções: São as opções específicas do comando ssh, como definir a porta ou especificar um arquivo de chave privada.
* user: Faz referência à conta com a qual você deseja fazer login na máquina remota. Se você não especificar um usuário, será usado o nome de usuário da sua conta local.
* host: Faz referência à máquina remota à qual você deseja acessar (onde o servidor SSH está em execução), pode usar o nome ou endereço ip.
* comando: Opcionalmente, você pode fornecer um comando para ser executado na máquina remota após a conexão ser estabelecida. Se não for fornecido, você será conectado ao shell da máquina remota.

A seguir algumas opções que podere ser usadas com o comando ssh:
* **p porta**: Especifica a porta para conectar-se ao servidor SSH.
* **i arquivo-chave**: Especifica o arquivo de chave privada a ser usado para autenticação.
* **l usuário**: Especifica o nome de usuário para fazer login no servidor remoto.
* **C**: Habilita compressão durante a transmissão de dados.
* **X**: Habilita o encaminhamento de X11 para suportar aplicativos gráficos remotos.
* **v**: Aumenta o nível de verbosidade, exibindo mais informações de depuração durante a conexão.
* **o opção**: Permite especificar opções adicionais de configuração, como *UserKnownHostsFile*, *StrictHostKeyChecking*, entre outras.

Para fechar uma sessão ssh e voltar para sua máquina local, execute o comando `exit`.
