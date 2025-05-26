# Introdução à Automação com Shell Script

A automação de tarefas no Linux é uma das maiores vantagens de se usar esse sistema operacional. Com os **shell scripts**, é possível criar programas simples que executam uma sequência de comandos automaticamente.

## O que é um Shell Script?

Um **shell script** é um arquivo de texto que contém uma série de comandos que podem ser executados pelo interpretador de comandos (shell), como o Bash. Esses scripts são usados para automatizar tarefas repetitivas, como backups, atualizações, renomeação de arquivos, entre outros.

## Por que automatizar?

Automatizar tarefas traz diversos benefícios:

- Economia de tempo
- Redução de erros humanos
- Padronização de processos
- Eficiência em tarefas administrativas e de manutenção

## Como criar um Shell Script?

1. Crie um arquivo com a extensão `.sh` (no terminal):
   ```bash
   touch meu_script.sh
   ```

2. Comece com a "shebang" na primeira linha para indicar qual shell será usado (dentro do arquivo):
   ```bash
   #!/bin/bash
   ```

    🔸 **O que é `#!/bin/bash`?**  
      - Essa linha é chamada de **shebang** e serve para informar ao sistema qual interpretador deve ser usado para executar o script. No caso, `#!/bin/bash` indica que o script será executado pelo Bash, que é um dos shells mais comuns no Linux.

    🔸 Se desejar, é possível usar outros interpretadores, como:
      - `#!/usr/bin/python3` → para scripts em Python  
      - `#!/usr/bin/env bash` → busca o Bash no PATH do sistema, tornando o script mais portável


3. Escreva os comandos desejados no arquivo. Por exemplo:
   ```bash
   echo "Olá, este é meu primeiro script!"
   ```

4. Torne o script executável (no terminal):
   ```bash
   chmod +x meu_script.sh
   ```

5. Execute (no terminal):
   ```bash
   ./meu_script.sh
   ```
