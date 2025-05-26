# Comandos Úteis no Linux

Esta é uma lista de comandos gerais no Linux que não se encaixam diretamente em categorias como manipulação de arquivos, redes, processos ou permissões, mas que são extremamente úteis no dia a dia no terminal.

---

## Comandos e Atalhos

- `clear` – Limpa a tela do terminal.
- `reset` – Restaura o terminal ao estado padrão, útil quando ele “trava” visualmente.
- `history` – Mostra todos os comandos digitados até agora.
- `!!` – Repete o último comando executado.
- `!n` – Executa o comando número `n` da lista do histórico (ex.: `!45` executa o 45º comando).
- `watch` – Executa um comando repetidamente em intervalos (padrão: 2 segundos). Ex.: `watch df -h`.
- `alias` – Cria um atalho para comandos. Ex.: `alias cls='clear'`.
- `unalias` – Remove um alias criado.
- `echo` – Imprime texto na tela. Muito útil em scripts e testes.
- `yes` – Repete indefinidamente uma string (ex.: `yes y`). ⚠️ Pode travar o terminal se não for interrompido.
- `sleep` – Aguarda por um tempo definido. Ex.: `sleep 5` (espera 5 segundos).
- `time` – Mede quanto tempo um comando leva para ser executado. Ex.: `time ls`.
- `date` – Mostra a data e hora atuais.
- `cal` – Exibe o calendário do mês atual (ou outro, se especificado).
- `uptime` – Mostra há quanto tempo o sistema está ligado, além da carga média.
- `whoami` – Exibe o nome do usuário atual.
- `id` – Mostra UID, GID e grupos aos quais o usuário atual pertence.
- `uname` – Exibe informações sobre o sistema. Use `uname -a` para informações completas (kernel, arquitetura, etc.).
- `hostname` – Mostra ou define o nome do host (nome do computador na rede).
- `tput reset` – Uma alternativa ao `reset`. Restaura o terminal com menos impacto.
- `Ctrl + L` – Atalho de teclado que limpa a tela (equivalente ao `clear`).
- `Ctrl + C` – Interrompe um comando em execução.
- `Ctrl + D` – Encerra a sessão atual do terminal (logout).
- `Ctrl + Z` – Suspende um processo em primeiro plano.
- `fg` – Traz de volta ao primeiro plano um processo que foi suspenso com `Ctrl + Z`.
- `bg` – Coloca um processo suspenso para continuar rodando em segundo plano.
- `jobs` – Lista os processos que estão em segundo plano ou suspensos.

---

## Observações
- Comandos como `alias` podem ser adicionados ao arquivo `.bashrc` (ou `.zshrc` se você usa zsh) para se tornarem permanentes.
- Atalhos de teclado (`Ctrl + C`, `Ctrl + Z`, `Ctrl + L`, etc.) são extremamente poderosos no uso diário do terminal.
- Tenha cuidado ao usar `yes`, especialmente sem combinar com outros comandos, pois ele pode gerar uma quantidade infinita de saídas e travar o terminal.

---
