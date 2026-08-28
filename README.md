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
* `cp arquivo /nome/do/diretório` : copia o "arquivo" para a pasta "diretório".
* `mv arquivo diretório/` : move o "arquivo" para a pasta "diretório".
* `rm arquivo` : apaga um arquivo.
* `mv arquivo/ arq/` : renomeia o arquivo "arquvio" para "arq".

O comando **aptitude** é uma interface de linha de comando para o gerenciador de pacotes APT (Advanced Package Tool) usado em sistemas operacionais baseados em Debian, como Ubuntu e Debian. (s/n/q). Ao contrario do **apt install**, o aptitude lhe dará algumas opções quando há pacotes faltantes na instalação desejada por exemplo; **s** concordará com essa escolha (o que não é bom, pois instalará com os pacotes faltantes), **q** apenas sairá, e **n** procurará uma solução alternativa.para instalar pacotes faltantes.
:
* `sudo aptitude update`: Antes de instalar qualquer pacote, é uma boa prática garantir que o índice de pacotes esteja atualizado
* sudo aptitude install nome_pacote: Instala um pacote desejado.
  
O comando **apt** é uma ferramenta de gerenciamento de pacotes usada em sistemas operacionais baseados em Debian:
* `apt search “nome do pacote”`: mostra uma lista com pacotes disponíveis para instalação pelo apt.
* `apt install “nome do pacote”`: instala pacotes.
* `apt update`: atualiza pacote
* `apt remove “nome do pacote”`: remove pacotes.
* `apt clean`: Remove todos os arquivos de cache de pacotes, independentemente de serem necessários ou não
* `sudo apt autoclean`: Remove apenas os pacotes do cache que não podem mais ser baixados (ou seja, pacotes antigos que não estão mais disponíveis nos repositórios).
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
   * .bin : Aplicações de base para o sistema. Armazena todos os comandos usado pelo terminal.
   * .boot: Armazena o kernel, contém arquivos necessários para a inicialização do sistema.
   * .dev : Arquivos de acesso aos dispositivos físicos e conexões de rede. Armazenas as unidades (usb, serial, hd...)
   * .lib : Bibliotecas compartilhadas pelos programas do sistema e módulos do kernel.
   * .etc : contém arquivos de configuração para o sistema operacional, seus serviços e aplicativos.
   * .home : onde fica armazenado os arquivos e diretórios dos usuários.
   * .usr : onde os programas são instalados. Aplicações voltadas aos usuários
   * .root: onde fica armazenado os arquivos e diretórios do usuário root.
   * .sbin : arquivos executáveis de uso exclusivo do root.
   * .media : requentemente utilizada para montagem automática de dispositivos de armazenamento removíveis, como unidades USB, CDs, DVDs e outros dispositivos de mídia.
   * .mnt : é frequentemente utilizada para montagem manual de sistemas de arquivos temporários ou compartilhados.
   * .opt : é uma pasta comum em sistemas Linux e geralmente é usada para instalar aplicativos e pacotes de software adicionais que não são fornecidos pelos repositórios oficiais da distribuição.
   *  .proc : é um diretório especial no sistema de arquivos Linux que contém informações sobre processos em execução e informações do kernel.
   *  .run : é possível que os usuários ou aplicativos criem essa pasta para armazenar arquivos executáveis ou scripts específicos
   * .usr : é uma das pastas mais importantes no sistema de arquivos Linux e geralmente contém dados e programas de uso compartilhado por todos os usuários do sistema. Ela é uma abreviação de "Unix System Resources" (Recursos do Sistema Unix).
   *  .var é uma das pastas fundamentais no sistema de arquivos Linux e é utilizada para armazenar dados variáveis que podem ser modificados durante a operação normal do sistema. (arquivos diversos, áreas de spool, arquivos de log...)   
   *  ./mnt: montagem de diretórios compartilhados temporários.

Comando **dpkg**:
* `sudo dpkg --install “nome do pacote”`: instala um pacote através do gerenciador de pacotes (dpkg).
* `sudo dpkg --remove “nome do pacote”`: remove um pacote através do gerenciador de pacotes (dpkg).

O comando **mkdir** é utilizado para criar diretórios.
* `mkdir “nome do riretorio”`: cria um diretório.
* `mkdir "diretorio1" "diretorio2" "diretorio3"`: cria vários diretórios de uma só vez.
* `mkdir -p diretorio1/diretorio2/sub\ diretório`: criará tanto diretorio1, diretorio2 e sub diretório, mesmo que diretorio1 não exista previamente.
* `mkdir "pasta1/pasta2/ sub diretório"` : criará tanto pasta1, pasta2 e sub diretório, sem precisar da contra barra bara inserir o espaço.
* `mkdir -m 755 nome-do-diretorio`: Permite especificar as permissões (modo) dos diretórios criados. Criará um diretório com permissões de leitura, escrita e execução para o proprietário, e apenas permissões de leitura e execução para os outros.
* `mkdir -m 755 -p "this/is/my/linux/exam"`
  
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

* A primeira letra se refere ao tipo do objeto que está sendo manipulado.
  *  d (diretório)
  *  -(programa)
  *  l (link) 
  *  b (arquivo de bloco)
  *  c (arquivo especial de caractere)
  *  p (canal)
  *  s (socket)
* As 2°, 3° e 4° letras são as permissões do usuário (u de user), em relação ao tipo do objeto que está sendo manipulado. 
* As 5°, 6° e 7° letras são as permissões que o grupo (g de group), em relação ao tipo do objeto que está sendo manipulado.
* As 8°, 9° e 10° letras são as permissões dos demais grupos ou usuários (o de others),em relação ao tipo do objeto que está sendo manipulado.

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

### 📁 **4. Permissões em Diretórios**

As permissões funcionam um pouco diferente:

| Permissão | Significado em diretórios           |
| --------- | ----------------------------------- |
| `r`       | Listar conteúdo do diretório        |
| `w`       | Criar, renomear ou excluir arquivos |
| `x`       | Entrar no diretório (acesso)        |

### ⭐ **5. Permissões Especiais**

Além das permissões básicas, há **3 bits especiais**:

| Bit          | Nome                                                                         | Função                                                                         |
| ------------ | ---------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| `SUID`       | Set User ID                                                                  | Arquivo executa com o UID do dono                                              |
| `SGID`       | Set Group ID                                                                 | Arquivo executa com o GID do grupo; em diretórios, novos arquivos herdam o GID |
| `Sticky Bit` | Somente o dono pode apagar ou renomear arquivos em diretórios compartilhados |                                                                                |

Dados as características das permissões especiais mencionadas, é necessário ter certo cuidado ao definir as permissões. Em particular existe os ID de usuário que possui privilégios de "superusuário", comumente denominado nas distribuições Linux como usuário de "root". O usuário com privilégios de root está isento das restrições designadas pelo mecanismo de controle de acesso, este usuário tem amplo acesso a sistema e arquivos. Neste sentido, qualquer arquivo que pertença ao usuário de "root" e seja concedido permissão de SUID, consequentemente ele fornecerá acesso irrestrito ao sistema a qualquer usuário que execute tal arquivo. Portanto, é necessária muita cautela ao definir tais permissões.

Outro aspecto que deve ser avaliado no esquema tradicional de controle de acesso a arquivos no Linux é que por padrão ele propõe uma estrutura simples de domínios de proteção. O domínio está associado aos usuários, alterar o domínio reflete em substituir o ID do usuário temporariamente. Por exemplo, um usuário comum solicitar privilégios de superusuário para instalar um pacote no sistema ou efetuar uma configuração nos arquivos de sistema.

### **“Listas de Controle de Acesso no Linux” (ACLs)**
As **ACLs** (Access Control Lists) são um **recurso avançado** do Linux que permite definir **permissões individuais** para **vários usuários e grupos**, além do modelo tradicional (usuário / grupo / outros).

####  **Por que usar ACLs?**
O modelo tradicional no Linux só permite definir permissões para:

* O **proprietário** do arquivo;
* Um **único grupo**;
* E **todos os outros usuários**.

E se você quiser dar acesso de leitura apenas para um usuário específico que não é o dono e não está no grupo?
A Solução é usar **ACLs estendidas** para definir permissões mais granulares.

#### `setfacl`

Usado para **definir** permissões ACL.

Exemplo:

```bash
setfacl -m u:joana:rw arquivo.txt
```

→ Dá permissão de **leitura e escrita** para a usuária `joana` no arquivo `arquivo.txt`.

####  `getfacl`

Usado para **visualizar** as permissões ACL de um arquivo.

Exemplo:

```bash
getfacl arquivo.txt
```

Exemplo de saída do comando `getfacl`:

```
# file: arquivo.txt
# owner: aluno
# group: equipe1
user::rw-
user:joana:rw-
group::r--
mask::rw-
other::r--
```

Explicação:

* `user::rw-`: permissões do dono do arquivo.
* `user:joana:rw-`: permissões para a usuária específica `joana`.
* `group::r--`: permissões do grupo padrão.
* `mask::rw-`: **limita** as permissões efetivas de `joana` e do grupo.
* `other::r--`: permissões para todos os outros usuários.

#### **Como saber se um arquivo tem ACL?**

* O comando `ls -l` mostrará um **sinal de “+”** ao lado das permissões:

  ```
  -rw-r--r--+ 1 aluno equipe1 1024 arquivo.txt
  ```

O `+` indica que o arquivo tem **ACLs estendidas configuradas**.

#### Remover todas as ACLs:

```bash
setfacl -b arquivo.txt
```

#### Remover permissão específica:

```bash
setfacl -x u:joana arquivo.txt
```


### ⚠️ **Pontos de Atenção**

* Nem todos os sistemas de arquivos suportam ACLs (ex: precisa ativar no `ext4`, `xfs` etc.).
* ACLs podem gerar **conflitos de permissões**, se não forem bem planejadas.
* Requer **administração cuidadosa**, especialmente em ambientes multiusuários.

## Configurar o sudo para não pedir senha para o comando shutdown
Para permitir que o comando shutdown seja executado sem pedir senha, você pode configurar o sudo para não pedir senha ao executar o comando shutdown.

1. Verificar o caminho do comando shutdown: Verifique se o caminho do comando shutdown. Você pode fazer isso usando o comando:
```bash
which shutdown
```
Certifique-se de que o caminho retornado é /usr/sbin/shutdown.

2. Abra o terminal e edite o arquivo sudoers usando o comando visudo:
```bash
sudo visudo
```

3. Adicione a seguinte linha no final do arquivo sudoers:
```bash:
ubuntu ALL=(ALL) NOPASSWD: /usr/sbin/shutdown
```
nesse exemplo, ubuntu, é o usuário do sistema. Para saber o nome do usuário use o comando `whoami` no terminal.

4. Salve e feche o arquivo sudoers: CRTL+x, yes, ENTER.
      
5. Verifique se a configuração está correta para o usuário: 
```sh
sudo -u ubuntu sudo -l	
```
Isso listará todos os comandos que os usuários  pode executar sem senha. Certifique-se de que 
`/usr/sbin/shutdown` está listado corretamente com a opção **NOPASSWD**.

## Manter a Porta USB Conectada ao Dispositivo Sempre a Mesma (link simbólico)
No Linux, as portas USB podem ser dinâmicas, mudando de /dev/ttyUSB0 para /dev/ttyUSB1 ou outros dispositivos. Para fixar a porta USB de um dispositivo específico, você pode usar regras udev.

1. Conecte o DIspositivo e encontre os detalhes do dispositivo com o comando `lsusb`.
Você verá algo como:
```bash
Bus 002 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub
Bus 001 Device 006: ID 8087:0a2a Intel Corp. 
Bus 001 Device 004: ID 067b:2303 Prolific Technology, Inc. PL2303 Serial Port
Bus 001 Device 007: ID 0d8c:000c C-Media Electronics, Inc. Audio Adapter
Bus 001 Device 005: ID 1a86:7523 QinHeng Electronics HL-340 USB-Serial adapter
Bus 001 Device 003: ID 05e3:0608 Genesys Logic, Inc. Hub
```
2. Veja qual é o **idVendor** e **idProduct** do dispositivo, para este exemplo vamos usar o dispositivo **Bus 001 Device 005**.
O  idVendor é  1a86, e o idProduct é 7523.

4. Crie uma regra udev para o Arduino:
```bash
sudo nano /etc/udev/rules.d/99-usb-serial.rules
```

6. Adicione a regra baseada no ID do dispositivo encontrado:
```bash
SUBSYSTEM=="tty", ATTRS{idVendor}=="1a86", ATTRS{idProduct}=="7523", MODE="0666", GROUP="dialout", SYMLINK+="Arduino"
```
Substitua idVendor e idProduct pelos valores encontrados e ajuste SYMLINK para o nome desejado (por exemplo, arduino).

7. Salve e feche o arquivo. Use CRTL+x, y, e ENTER.

8. Reinicie as regras udev:
```bash
sudo udevadm control --reload-rules
sudo udevadm trigger
```
Agora, seu Arduino sempre estará acessível através do link simbólico /dev/arduino, independentemente de qual porta USB ele estiver conectado.
Listar portas seriais USB: `ls /dev/ttyUSB*` ou `ls /dev`

### A opção `MODE` em uma regra `udev`
A opção `MODE` em uma regra `udev` define as permissões de acesso para o arquivo de dispositivo que é criado no diretório `/dev`. Ela funciona exatamente da mesma forma que as permissões de arquivo padrão do Linux, que você pode ver ao usar o comando `ls -l`.

As permissões são definidas usando uma notação numérica octal (base 8).

#### Entendendo a Notação Octal

Um número de permissão de 3 ou 4 dígitos é usado, onde cada dígito representa um conjunto diferente de permissões:

*   **Primeiro dígito (opcional):** Bits especiais (SetUID, SetGID, Sticky bit). Geralmente é omitido (ou definido como 0), a menos que você precise de um comportamento muito específico.
*   **Segundo dígito:** Permissões para o **usuário proprietário** do arquivo.
*   **Terceiro dígito:** Permissões para o **grupo proprietário** do arquivo.
*   **Quarto dígito:** Permissões para **todos os outros usuários**.

Cada um desses dígitos é a soma dos seguintes valores:
*   **4** (Leitura - **r**ead)
*   **2** (Escrita - **w**rite)
*   **1** (Execução - e**x**ecute)

#### Exemplos Comuns de `MODE`

Vamos ver como isso se traduz em valores práticos para a opção `MODE`:

| `MODE` | Notação (rwx) | Significado |
| :--- | :--- | :--- |
| **`0666`** | `rw-rw-rw-` | **Leitura e escrita** para todos (proprietário, grupo e outros). É uma permissão muito aberta e comum para dispositivos que precisam ser acessíveis por qualquer usuário, como portas seriais. |
| **`0660`** | `rw-rw----` | **Leitura e escrita** para o proprietário e para os membros do grupo. Outros usuários não têm acesso. Esta é uma opção segura e muito usada, como no exemplo da sua pergunta anterior (`GROUP="dialout"`). |
| **`0600`** | `rw-------` | **Leitura e escrita** apenas para o usuário proprietário. Ninguém mais pode acessar o dispositivo. |
| **`0777`** | `rwxrwxrwx` | **Leitura, escrita e execução** para todos. A permissão de "execução" não faz muito sentido para a maioria dos arquivos de dispositivo, mas é tecnicamente possível. |
| **`0444`** | `r--r--r--` | **Apenas leitura** para todos. Útil se você quer garantir que nenhum processo possa escrever no dispositivo. |

### A opção `GROUP` em uma regra `udev`
A opção `GROUP` em uma regra `udev` é usada para definir qual **grupo de usuários** será o proprietário do arquivo de dispositivo criado no diretório `/dev`.

Isso é fundamental para gerenciar permissões de acesso de uma forma organizada, sem precisar dar acesso a todos os usuários do sistema ou forçar o uso do `sudo` para cada operação.

#### Como `GROUP` Funciona em Conjunto com `MODE`

As opções `GROUP` e `MODE` trabalham juntas para controlar o acesso a um dispositivo:

1.  **`GROUP="<nome_do_grupo>"`**: Esta parte atribui a propriedade do arquivo de dispositivo a um grupo específico. No seu exemplo original, era `GROUP="dialout"`.
2.  **`MODE="<permissões>"`**: Esta parte define *o que* o proprietário, o grupo e os outros podem fazer. Por exemplo, `MODE="0660"` concede permissões de leitura e escrita ao usuário proprietário e ao **grupo proprietário**.

Vamos usar o exemplo da sua primeira pergunta:
`SUBSYSTEM=="tty", ..., MODE="0660", GROUP="dialout", ...`

*   **`GROUP="dialout"`**: Diz ao sistema: "O grupo 'dialout' é o dono deste dispositivo".
*   **`MODE="0660"`**: Diz ao sistema: "O usuário dono pode ler/escrever (`6`), o grupo 'dialout' pode ler/escrever (`6`), e mais ninguém pode fazer nada (`0`)".

O resultado prático é que **qualquer usuário que seja membro do grupo `dialout` poderá acessar (ler e escrever) o dispositivo sem precisar de privilégios de administrador (sudo)**.

#### Grupos Comuns Usados em Regras `udev`

Diferentes grupos são usados para diferentes tipos de hardware, seguindo convenções do sistema Linux:

| Grupo | Finalidade Comum |
| :--- | :--- |
| **`dialout`** | Acesso a portas seriais, modems e dispositivos de comunicação serial (como Arduinos, ESP32, etc.). Este é o grupo do seu exemplo. |
| **`plugdev`** | Acesso a dispositivos removíveis que não são montados automaticamente, como câmeras ou celulares conectados via MTP/PTP. |
| **`video`** | Acesso direto a dispositivos de vídeo, como webcams ou placas de captura, para processamento de imagem. |
| **`audio`** | Acesso a dispositivos de áudio para aplicações de baixo nível. |
| **`input`** | Acesso a dispositivos de entrada brutos, como joysticks, gamepads e teclados especiais. |
| **`disk`** | Acesso direto a discos rígidos inteiros (ex: `/dev/sda`). É um grupo poderoso e geralmente não se dá acesso a usuários comuns. |
| **`lp`** | Acesso a impressoras (Line Printer). |

#### Por que Usar `GROUP`?

A principal vantagem é a **segurança e a conveniência**.

*   **Sem `GROUP`**: Por padrão, o dispositivo pertenceria ao `root`. Para acessá-lo, um usuário comum precisaria usar `sudo` para cada comando (ex: `sudo screen /dev/ttyUSB0`) ou o administrador teria que mudar as permissões manualmente com `chmod` toda vez que o dispositivo fosse conectado.
*   **Com `GROUP`**: O administrador só precisa adicionar os usuários autorizados ao grupo apropriado (ex: `dialout`) uma única vez. A partir daí, o `udev` cuida de tudo automaticamente. O usuário pode simplesmente usar o dispositivo diretamente, tornando o fluxo de trabalho muito mais simples e seguro.

Em resumo, a opção `GROUP` é a maneira correta e elegante no Linux de conceder acesso a hardware específico para um conjunto de usuários não-root.

### E quando mais de um dispositivo tem o mesmo **idVendor** e **idProduct** 

#### Pelo número de śeire (`serial`) 
O melhor atributo para isso é o **número de série** (`serial`) do dispositivo. A maioria dos dispositivos USB de qualidade, como os da Silicon Labs, possui um número de série único gravado em seu firmware.

Vamos seguir um processo semelhante, mas usando o número de série como nosso diferenciador.

##### Passo 1: Encontrar o Número de Série de Cada Dispositivo

Primeiro, precisamos descobrir o número de série de cada um dos seus dois dispositivos.

* Use o comando `ls -l /dev/serial/by-id/` para descobrir qual porta usb foi atribuida ao dispositivo.
* Outra opção é executar o comando `sudo dmesg -w` e conectar o dispositivo, mostrará algo como **usb 1-2: cp210x converter now attached to ttyUSB2**.

1.  Execute o comando `udevadm` para inspecionar os atributos do dispositivo. Substitua `/dev/ttyUSB0` pelo nome que o sistema atribuiu a ele.

    ```bash
    udevadm info -a -n /dev/ttyUSB0 | grep '{serial}'
    ```

2.  Procure pela linha que contém `ATTRS{serial}`. A saída será algo como:

    ```
    ATTRS{serial}=="00A1B2C3"
    ```
    Anote esse número de série (por exemplo, `00A1B2C3`).

3.  **Agora, desconecte o primeiro dispositivo e conecte o segundo.**
4.  Execute o mesmo comando novamente (ele provavelmente será mapeado para `/dev/ttyUSB0` também, já que é o único conectado).

    ```bash
    udevadm info -a -n /dev/ttyUSB0 | grep '{serial}'
    ```

5.  Anote o número de série do segundo dispositivo. Será um valor diferente, por exemplo:

    ```
    ATTRS{serial}=="00D4E5F6"
    ```

Agora você tem os identificadores únicos para cada dispositivo físico: `00A1B2C3` e `00D4E5F6`.

##### Passo 2: Criar ou Editar o Arquivo de Regras do udev

Assim como antes, vamos criar (ou editar) um arquivo de regras `udev`.

```bash
sudo nano /etc/udev/rules.d/99-usb-serial.rules
```

##### Passo 3: Adicionar as Novas Regras Baseadas no Número de Série

Adicione as seguintes regras ao arquivo, substituindo os números de série pelos que você encontrou e escolhendo os nomes para os links simbólicos (`SYMLINK`).

```
# Regra para o primeiro dispositivo (identificado pelo seu número de série)
SUBSYSTEM=="tty", ATTRS{idVendor}=="10c4", ATTRS{idProduct}=="ea60", ATTRS{serial}=="00A1B2C3", SYMLINK+="meu_dispositivo_A"

# Regra para o segundo dispositivo (identificado pelo seu número de série)
SUBSYSTEM=="tty", ATTRS{idVendor}=="10c4", ATTRS{idProduct}=="ea60", ATTRS{serial}=="00D4E5F6", SYMLINK+="meu_dispositivo_B"
```
##### Passo 4: Recarregar as Regras e Testar

Para aplicar as novas regras, execute:

```bash
# Recarregar as definições de regras
sudo udevadm control --reload-rules

# Reavaliar os dispositivos atualmente conectados
sudo udevadm trigger
```

Agora, com os dois dispositivos conectados (em quaisquer portas USB), verifique se os links simbólicos foram criados corretamente:

```bash
ls -l /dev/meu_dispositivo_*
```

A saída mostrará os links apontando para os `ttyUSB*` correspondentes, não importando a ordem em que foram conectados.

```
lrwxrwxrwx 1 root root 7 Jan 14 20:55 /dev/meu_dispositivo_A -> ttyUSB1
lrwxrwxrwx 1 root root 7 Jan 14 20:55 /dev/meu_dispositivo_B -> ttyUSB0
```
(Note que `meu_dispositivo_A` pode apontar para `ttyUSB1` e `B` para `ttyUSB0`, ou vice-versa. O importante é que o link simbólico correto está sempre associado ao dispositivo físico correto).

Esta abordagem usando o número de série é a prática recomendada para criar identificadores persistentes para dispositivos USB que podem ser movidos entre diferentes portas.

#### Pelo KERNELS
No `udev`, existem diferentes atributos para identificar dispositivos. `KERNELS` verifica o **nome do dispositivo atribuído pelo kernel em algum nível da árvore de dispositivos (device tree)**.

No caso:

```udev
KERNELS=="3-1"
```

significa:

> "Aplique esta regra somente se, na hierarquia de dispositivos USB, existir um dispositivo cujo nome no kernel seja `3-1`."

Por exemplo, imagine:

```text
USB controller
└── 3-1
    └── 3-1:1.0
        └── ttyUSB0
```

O `3-1` normalmente representa algo como:

```text
USB bus 3
└── porta 1
```

Ou seja, **a porta física/topologia USB**.

procura esse nome **na árvore de dispositivos, incluindo dispositivos ancestrais**.

Por isso `KERNELS` é muito útil para identificar **a porta USB física**.


##### Como descobrir o `KERNELS` correto?

1. Descubra o dispositivo serial

```bash
ls /dev/ttyUSB*
```

Supondo:

```text
/dev/ttyUSB0
```

2. Obtenha o caminho do dispositivo

```bash
udevadm info --query=path --name=/dev/ttyUSB0
```

Você poderá obter algo parecido com:

```text
/devices/pci0000:00/0000:00:14.0/usb3/3-1/3-1:1.0/ttyUSB0/tty/ttyUSB0
```

O trecho:

```text
usb3/3-1/3-1:1.0
```

é o que nos interessa.

Nesse exemplo:

```text
KERNELS=="3-1"
```

corresponde ao dispositivo USB conectado ao **bus 3, porta 1**.

---

3. Crie a regra

Crie o arquivo:

```bash
sudo nano /etc/udev/rules.d/99-usb-serial.rules
```

E coloque:

```udev
SUBSYSTEM=="tty", KERNELS=="3-1", SYMLINK+="ESP", MODE="0666", GROUP="dialout"
```

Se quiser garantir que somente seu conversor específico seja selecionado, use também Vendor/Product:

```udev
SUBSYSTEM=="tty", KERNELS=="3-1", ATTRS{idVendor}=="10c4", ATTRS{idProduct}=="ea60", SYMLINK+="ESP", MODE="0666", GROUP="dialout"
```

---

4. Recarregue as regras

```bash
sudo udevadm control --reload-rules
sudo udevadm trigger
```

Ou simplesmente desconecte e conecte novamente o dispositivo USB.

---

5. Verifique

```bash
ls -l /dev/ESP
```

Deve aparecer algo como:

```text
/dev/ESP -> ttyUSB0
```

Você também pode verificar:

```bash
readlink -f /dev/ESP
```

Resultado:

```text
/dev/ttyUSB0
```

---

##### Um detalhe importante

O comando:

```bash
udevadm info --query=path --name=/dev/ttyUSB0
```

**não mostra explicitamente `KERNELS=="3-1"`**.

Ele mostra o caminho:

```text
.../usb3/3-1/3-1:1.0/...
```

Você identifica o `KERNELS` olhando para os componentes desse caminho.

Por exemplo:

```text
/devices/.../usb3/3-1/3-1:1.0/ttyUSB0/...
                   ↑
                KERNELS
                  3-1
```

Então, o fluxo fica:

```text
/dev/ttyUSB0
     ↓
udevadm info --query=path --name=/dev/ttyUSB0
     ↓
/devices/.../usb3/3-1/3-1:1.0/...
                   ↓
              KERNELS=="3-1"
                   ↓
              /dev/ESP
```

Se você tiver **2 ou 4 ESP32 idênticos conectados ao robô**, esse método é particularmente útil para criar `/dev/ESP1`, `/dev/ESP2`, `/dev/ESP3` e `/dev/ESP4` com base nas portas USB físicas.

---

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
   WorkingDirectory=/caminho/para/  #diretório do arquivo python a ser executado 
   ExecStart=/usr/bin/python3 /caminho/para/seu_codigo.py  #nome e caminho do arquivo python a ser executado
   Restart=on-failure    # ou always
   
   [Install]
   WantedBy=multi-user.target   #ou default.target
   ```
3. No arquivode serviço altere as informações do usuário do sistema (User), diretório e nome do arquivo ".py" de acordo com as informações do seu arquivo python.
4. Salve e feche o arquivo de serviços.
5. Recarregue o daemon do systemd usando o comando `sudo systemctl daemon-reload` no terminal do Linux.
6. Se você quiser que o serviço seja iniciado automaticamente na inicialização do sistema, você pode ativá-lo com o comando: `sudo systemctl enable nome_do_arquivo`.
7. Inicie o serviço usando o comando `sudo systemctl start nome_do_arquivo`. O "nome_do_arquivo" é o nome dado ao arquivo de serviços criado.
8. Verifique o status do serviço usando o comando `sudo systemctl status nome_do_arquivo`, deve ser retornado algo como:
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

### A diretiva `Type=` 
A diretiva `Type=` é uma das mais importantes na seção `[Service]` de um arquivo `systemd`, pois ela informa ao `systemd` como gerenciar o ciclo de vida do processo do seu serviço. A escolha do tipo correto é crucial para que o `systemd` saiba quando o serviço foi iniciado com sucesso, como monitorá-lo e como lidar com ele.

#### 1. `Type=simple` (Padrão)
É o tipo mais comum e o padrão se você não especificar nenhum.

*   **Como funciona:** O `systemd` considera o serviço **iniciado imediatamente** após o processo principal (definido em `ExecStart=`) ser executado (fork/exec). O `systemd` não espera que o processo termine de carregar ou sinalize que está pronto.
*   **Quando usar:**
    *   Para scripts ou programas que rodam, fazem seu trabalho e terminam (embora `oneshot` seja melhor para isso).
    *   Para programas que rodam continuamente (daemons) e não precisam de uma longa inicialização antes de estarem operacionais.
    *   Quando o processo principal é o processo que realmente importa e ele não cria outros processos filhos que continuam rodando em segundo plano.
*   **Exemplo:** Um script que inicia um servidor web simples que fica escutando em uma porta.
    ```ini
    [Service]
    Type=simple
    ExecStart=/usr/bin/python3 /opt/meu_servidor_web.py
    Restart=on-failure
    ```

#### 2. `Type=forking`
Usado para daemons tradicionais que se "bifurcam" (fork) para o background.

*   **Como funciona:** O `systemd` considera o serviço iniciado **após o processo pai original terminar**. A expectativa é que este processo pai configure o ambiente e inicie um processo filho que continuará rodando como o verdadeiro daemon. O `systemd` então rastreia esse processo filho.
*   **Quando usar:**
    *   Para softwares mais antigos que foram projetados para se "daemonizar" sozinhos, ou seja, eles se colocam em segundo plano por conta própria.
    *   Quando o comando em `ExecStart` inicia um processo e sai imediatamente, deixando um filho para trás.
*   **Como o `systemd` sabe qual processo rastrear?** Geralmente, você precisa especificar um arquivo PID com a diretiva `PIDFile=`.
*   **Exemplo:** Um servidor de banco de dados antigo que se inicia em background.
    ```ini
    [Service]
    Type=forking
    ExecStart=/usr/sbin/meu-db-server --daemon --config /etc/meu-db.conf
    PIDFile=/var/run/meu-db-server.pid
    ```
    **Atenção:** Este tipo é considerado legado. O ideal é que os próprios aplicativos não se "daemonizem", deixando essa responsabilidade para o `systemd`.

#### 3. `Type=oneshot`
Para tarefas que executam uma ação única e depois terminam.

*   **Como funciona:** O `systemd` espera o processo terminar completamente antes de considerar o serviço "iniciado" (ou "ativo"). Outros serviços que dependem dele só começarão depois que ele for concluído com sucesso.
*   **Quando usar:**
    *   Scripts de configuração que precisam rodar uma única vez durante o boot (ex: configurar regras de firewall, carregar módulos do kernel, limpar arquivos temporários).
    *   Tarefas que precisam ser executadas antes ou depois de outros serviços.
*   **Comportamento especial:** Por padrão, um serviço `oneshot` só é executado uma vez. Se você tentar iniciá-lo novamente, o `systemd` verá que ele já foi concluído e não fará nada. Para permitir que ele seja executado sempre que for chamado, você precisa adicionar `RemainAfterExit=yes`.
*   **Exemplo:** Um script que limpa um diretório de cache na inicialização.
    ```ini
    [Unit]
    Description=Limpar cache na inicialização

    [Service]
    Type=oneshot
    ExecStart=/bin/rm -rf /var/cache/meu_app/*
    ```
*   **Exemplo com `RemainAfterExit`:** Um serviço que configura a rede, mas precisa permanecer "ativo" para que outros serviços possam depender dele.
    ```ini
    [Service]
    Type=oneshot
    ExecStart=/usr/local/bin/configurar-rede.sh
    RemainAfterExit=yes
    ```

#### 4. `Type=notify`
Para daemons modernos que sinalizam ativamente ao `systemd` quando estão prontos.

*   **Como funciona:** O serviço precisa notificar o `systemd` (usando a função `sd_notify()` ou um comando de shell) quando sua inicialização estiver completa e ele estiver pronto para receber trabalho. O `systemd` considera o serviço iniciado somente após receber essa notificação.
*   **Quando usar:**
    *   É o método **preferido e mais robusto** para serviços de longa duração.
    *   Ideal para aplicações com um tempo de inicialização significativo (ex: carregar um grande modelo de machine learning, conectar-se a um banco de dados remoto). Isso garante que os serviços dependentes só comecem quando este estiver *realmente* pronto.
*   **Exemplo:** Um servidor de aplicação moderno.
    ```ini
    [Service]
    Type=notify
    ExecStart=/opt/meu_app/server
    # O código do 'server' deve chamar sd_notify("READY=1") quando estiver pronto.
    ```

#### 5. `Type=dbus`
Um tipo especializado para serviços que são ativados via D-Bus.

*   **Como funciona:** O serviço deve adquirir um nome no barramento de mensagens D-Bus. O `systemd` considera o serviço iniciado assim que esse nome é adquirido.
*   **Quando usar:** Apenas se você estiver desenvolvendo um serviço que se integra profundamente com o D-Bus, o que é comum em ambientes de desktop Linux (GNOME, KDE).
*   **Exemplo:**
    ```ini
    [Service]
    Type=dbus
    BusName=org.meuprojeto.MeuServico
    ExecStart=/usr/lib/meu-servico-dbus
    ```

##### Tabela Resumo

| Tipo | Quando o `systemd` considera o serviço "iniciado"? | Caso de Uso Típico |
| :--- | :--- | :--- |
| **`simple`** | Imediatamente após `ExecStart` ser executado. | Scripts simples, daemons que não se bifurcam. **O mais comum.** |
| **`forking`** | Após o processo pai original de `ExecStart` terminar. | Daemons legados que se colocam em segundo plano. **Evite se possível.** |
| **`oneshot`** | Após o processo de `ExecStart` terminar com sucesso. | Scripts de tarefa única (configuração, limpeza). |
| **`notify`** | Após o serviço enviar uma mensagem de "pronto" para o `systemd`. | Daemons modernos e robustos com tempo de inicialização. **O ideal.** |
| **`dbus`** | Quando o serviço adquire um nome no barramento D-Bus. | Serviços que se integram com o D-Bus. |

### Exemplo

#### Seção `[Unit]`

Esta seção contém metadados sobre o serviço e define suas dependências e a ordem de inicialização.

| Linha | Explicação |
| :--- | :--- |
| `Description=servico_exemplo` | Fornece uma descrição curta e legível do que o serviço faz. Ela aparece em logs e status do sistema, facilitando a identificação. |
| `After=network-online.target outro_servico.service` | **Instrução de ordenação.** Garante que este serviço (`servico_exemplo`) só tentará iniciar **depois** que o serviço `network-online.target` (que indica que a rede está ativa) e o seu outro serviço customizado `outro_servico.service` tenham sido iniciados com sucesso. Isso é crucial para garantir que as dependências estejam prontas. |
| `Wants=network-online.target` | **Instrução de dependência (não-crítica).** Indica que este serviço "deseja" que o `network-online.target` seja iniciado junto com ele. Se o `network-online.target` falhar ao iniciar, o `servico_exemplo.service` ainda assim tentará iniciar. É uma dependência mais fraca do que `Requires=`. |

#### Seção `[Service]`

Esta é a seção principal, que define como o serviço será executado.

| Linha | Explicação |
| :--- | :--- |
| `Type=simple` | Define o tipo de inicialização do processo. `simple` significa que o `systemd` considera o serviço iniciado assim que o processo principal (especificado em `ExecStart`) é executado. É o tipo mais comum e padrão. |
| `User=ubuntu` | Especifica que o comando do serviço será executado pelo usuário `ubuntu`. |
| `Group=ubuntu` | Especifica que o processo será executado com o grupo primário `ubuntu`. |
| `WorkingDirectory=/home/ubuntu` | Define o diretório de trabalho para o processo executado. Ou seja, o script `/home/ubuntu/bringup_navigation.sh` será executado como se você tivesse primeiro navegado para o diretório `/home/ubuntu`. |
| `Environment="HOME=/home/ubuntu"` | Define a variável de ambiente `HOME` para o processo. Isso é importante para programas que procuram arquivos de configuração no diretório home do usuário (ex: `~/.bashrc`). |
| `Environment="USER=ubuntu"` | Define explicitamente a variável de ambiente `USER`. |
| `Environment="DISPLAY=:0"` | Define a variável de ambiente `DISPLAY`, indicando ao sistema qual tela gráfica usar. Isso é necessário se o seu script de navegação precisar iniciar alguma aplicação com interface gráfica (GUI)|
| `Environment="PYTHONUNBUFFERED=1"` | Força o Python a enviar os outputs (saídas) diretamente para o `stdout`/`stderr` sem usar um buffer. Isso é **muito útil** para depuração, pois garante que você veja os logs em tempo real no `journalctl`, em vez de esperar o buffer encher. |
| `Environment="TERM=xterm-256color"` | Define o tipo de terminal. Isso ajuda a garantir que as saídas coloridas (`colout`) sejam renderizadas corretamente nos logs. |
| `ExecStart=/bin/bash /home/ubuntu/script_bash.sh` | **O comando principal.** Esta é a linha que efetivamente inicia o seu serviço. Ela executa o script `script_bash.sh` usando o interpretador `/bin/bash`. |
| `Restart=on-failure` | **Política de reinicialização.** Instruí o `systemd` a reiniciar o serviço automaticamente se ele terminar com um código de saída diferente de zero (ou seja, se falhar). |
| `RestartSec=10` | Define um tempo de espera de 10 segundos antes de tentar reiniciar o serviço após uma falha. |
| `StandardOutput=journal+console` | Redireciona a saída padrão (`stdout`) do seu script para o log do sistema (`journal`) e também para o console do sistema (`/dev/console`). |
| `StandardError=journal+console` | Redireciona a saída de erro (`stderr`) para os mesmos locais da saída padrão. |
| `ProtectHome=no` | Desativa uma medida de segurança do `systemd` que, por padrão, torna os diretórios `/home` somente leitura para o serviço. Você precisa desativar isso (`no`) porque seu `WorkingDirectory` e scripts estão em `/home/ubuntu`. |
| `ProtectSystem=off` | Desativa outra medida de segurança que monta os diretórios `/usr` e `/boot` como somente leitura. Geralmente é seguro deixar como `strict`, mas pode ser desativado se o seu script precisar escrever em locais inesperados do sistema. |
| `ReadWritePaths=/home/ubuntu/Desktop/logs` | Concede permissão explícita de leitura e escrita para o serviço no diretório `/home/ubuntu/Desktop/logs`. Esta é uma forma mais segura de dar acesso a pastas específicas, em vez de desativar completamente a proteção com `ProtectHome`. |

#### Seção `[Install]`

Esta seção define o que acontece quando o serviço é "habilitado" ou "desabilitado" com `systemctl enable` ou `systemctl disable`.

| Linha | Explicação |
| :--- | :--- |
| `WantedBy=multi-user.target` | Quando você executa `systemctl enable servico_exemplo.service`, esta linha cria um link simbólico que faz com que o serviço seja iniciado automaticamente durante o boot do sistema, assim que o sistema atinge o nível de execução multiusuário (o estado padrão para um sistema sem interface gráfica iniciada). |

#### Usando **colout** para logs coloridos
Para versões antigas do ubuntu (18, 20) use o comando `pip install colout` ou `sudo apt install colout`.

Para versões modernas do ubuntu use o `pipx`:
**1. Instale o `pipx` (se ainda não tiver):**
O `pipx` pode ser instalado diretamente pelo `apt`.

```bash
sudo apt update
sudo apt install pipx
```

**2. Use o `pipx` para instalar o `colout`:**
Depois de instalar o `pipx`, você precisa garantir que os executáveis dele estejam no seu `PATH` (caminho de busca de comandos). O `pipx` faz isso para você com o seguinte comando:

```bash
pipx ensurepath
```
**Importante:** Após rodar `pipx ensurepath`, você **precisa fechar e reabrir seu terminal** ou carregar o arquivo de configuração do seu shell novamente (ex: `source ~/.bashrc`) para que a mudança tenha efeito.

Agora, finalmente, instale o `colout`:

```bash
pipx install colout
```

Depois de instalado execute o comando `journalctl -u servico_exemplo -f | colout INFO green | colout ERROR red bold | colout WARN yellow` para ver os logs coloridos.

---

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

## Coniguração Ethernet usando **nmcli**
Para sistemas que utilizam o **NetworkManager**, você pode configurar o IP estático usando a ferramenta **nmcli**.



### Cadastrar e conectar a uma rede nova

#### 1.1 Rede com senha (WPA2)
```bash
sudo nmcli connection add type wifi con-name "NOME_DO_PERFIL" ssid "NOME_DA_REDE" \
  wifi-sec.key-mgmt wpa-psk wifi-sec.psk 'SENHA_DA_REDE'

sudo nmcli connection modify "NOME_DO_PERFIL" \
  connection.autoconnect yes \
  connection.autoconnect-priority 10
```

> **Alternativa mais cautelosa** (não obrigatória, só para evitar a senha em texto puro no histórico do shell): criar o perfil com `connection.autoconnect no`, pedir a senha via `read -s -p "Senha: " WIFI_PASS`, aplicar com `wifi-sec.psk "$WIFI_PASS"` e depois `unset WIFI_PASS`. Funciona igual, é só mais uma etapa.

#### 1.2 Rede aberta (sem senha)

```bash
sudo nmcli connection add type wifi con-name "NOME_DO_PERFIL" ssid "NOME_DA_REDE"

sudo nmcli connection modify "NOME_DO_PERFIL" \
  connection.autoconnect yes \
  connection.autoconnect-priority 10
```

#### 1.3 Ativar a troca

**Não rode `nmcli connection up NOME_DO_PERFIL` enquanto estiver em SSH pelo hotspot** — a sessão cai no mesmo instante. Prefira derrubar o hotspot, deixando o NetworkManager escolher a rede nova sozinho:

```bash
sudo nmcli connection down rede_propria
```

### Conectar Automaticamente (DHCP):
Para conectar automaticamente usando DHCP, você pode simplesmente ativar a interface: `nmcli con up id "ssid"`.

### Configurar um IP Estático 
Se você precisar configurar um IP estático, use o comando abaixo, substituindo os valores conforme necessário:

1. Listar redes Wi-Fi disponíveis: `nmcli dev wifi list` ou `nmcli con show`.
   
Suponha que a saída inclua uma rede chamada "MinhaRedeWiFi";
   * Conectar à rede Wi-Fi: `nmcli dev wifi connect "MinhaRedeWiFi" password "senha1234"`
   * Verificar a conexão: `nmcli con show --active`

3. Verificar se o ip ja está em uso com o comando ping: `ping 192.168.1.100`

4. Definindo o ip estático:
   
* Definindo ip e máscara de rede: `nmcli con mod MinhaRedeWiFi ipv4.addresses 192.168.1.100/24`
* Definindo gateway: `nmcli con mod MinhaRedeWiFi ipv4.gateway 192.168.1.1`
* Definindo dns: `nmcli con mod MinhaRedeWiFi" ipv4.dns "8.8.8.8 8.8.4.4"`
* Definindo ip estático: `nmcli con mod MinhaRedeWiFi ipv4.method manual`
* Reinicie a conexão: `nmcli con down MinhaRedeWiFi` e também `nmcli con up MinhaRedeWiFi`

### Alterar a prioridade de conexão

O NetworkManager escolhe a rede com base na prioridade configurada.

#### 1. Liste as conexões salvas

```bash
nmcli connection show
```

Saída de exemplo:

```text
NAME             UUID                                  TYPE  DEVICE
MinhaCasa        xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx  wifi  wlan0
Empresa          xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx  wifi  --
Celular          xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx  wifi  --
```

---

#### 2. Veja a prioridade atual

```bash
nmcli connection show "MinhaCasa" | grep connection.autoconnect-priority
```

---

#### 3. Defina uma prioridade

Quanto **maior o número**, maior a prioridade.

Exemplo:

```bash
nmcli connection modify "Empresa" connection.autoconnect-priority 100
```

```bash
nmcli connection modify "MinhaCasa" connection.autoconnect-priority 50
```

```bash
nmcli connection modify "Celular" connection.autoconnect-priority 10
```

Assim, quando todas estiverem disponíveis, a ordem será:

1. Empresa
2. MinhaCasa
3. Celular

---

#### 4. Reinicie a conexão

```bash
sudo systemctl restart NetworkManager
```

---
