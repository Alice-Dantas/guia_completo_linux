# Estrutura de Diretórios do Linux (Filesystem Hierarchy Standard - FHS)

Diferente de sistemas como Windows, onde você tem letras de drive (C:, D:), o Linux organiza tudo em uma única hierarquia a partir do diretório raiz, representado por `/`. Essa estrutura é padronizada pelo **Filesystem Hierarchy Standard (FHS)**, o que facilita muito a vida de quem trabalha com diferentes distribuições.

Vamos explorar os diretórios mais importantes:

## O Diretório Raiz: `/`

Tudo no Linux começa a partir do diretório raiz (`/`). Ele é o topo da árvore de diretórios.

## Diretórios Comuns e Seus Propósitos:

* **`/bin` (binaries):** Contém comandos essenciais do sistema, disponíveis para todos os usuários (ex: `ls`, `cp`, `mv`).
* **`/sbin` (system binaries):** Contém comandos essenciais para a administração do sistema, geralmente executados pelo usuário `root` (ex: `fdisk`, `reboot`, `ip`).
* **`/etc` (et cetera):** Armazena arquivos de configuração do sistema e de programas (ex: `passwd`, `fstab`, arquivos de configuração do Apache).
* **`/home`:** Onde ficam os diretórios pessoais dos usuários comuns. Cada usuário tem seu próprio diretório aqui (ex: `/home/seunomeusuario`).
* **`/root`:** É o diretório pessoal do usuário `root` (administrador do sistema).
* **`/usr` (Unix System Resources):** Contém a maioria dos programas e bibliotecas compartilhadas pelos usuários. É um dos maiores diretórios.
    * **`/usr/bin`:** Mais executáveis de comandos para usuários.
    * **`/usr/sbin`:** Mais executáveis de comandos de sistema.
    * **`/usr/local`:** Para programas instalados manualmente ou compilados.
* **`/var` (variable):** Contém arquivos cujos conteúdos variam (logs, caches, spool files).
    * **`/var/log`:** Arquivos de log do sistema e de aplicativos.
    * **`/var/www`:** Conteúdo padrão para servidores web (se instalado).
* **`/tmp` (temporary):** Para arquivos temporários criados por programas. O conteúdo geralmente é apagado a cada reinício do sistema.
* **`/dev` (devices):** Contém arquivos especiais que representam dispositivos de hardware (ex: `/dev/sda` para o primeiro disco rígido).
* **`/proc` (processes):** Um sistema de arquivos virtual que fornece informações sobre processos em execução e sobre o kernel.
* **`/mnt` (mount):** Diretório usado para montar sistemas de arquivos temporariamente (pen drives, CDs, partições).
* **`/media`:** Usado para montar mídias removíveis automaticamente (pen drives, CDs/DVDs, cartões de memória).
* **`/opt` (optional):** Para pacotes de software opcionais, geralmente de terceiros, que não seguem a estrutura padrão do FHS.
* **`/boot`:** Contém os arquivos necessários para a inicialização do sistema, incluindo o kernel Linux.

## Entendendo a Hierarquia

Compreender essa estrutura é crucial para:

* **Navegar pelo sistema:** Saber onde encontrar arquivos e programas.
* **Resolver problemas:** Identificar onde logs de erro podem estar.
* **Administrar o sistema:** Configurar serviços e gerenciar permissões.

À medida que você avança nos estudos, a localização de cada diretório fará mais sentido em relação às tarefas que você estará realizando!
