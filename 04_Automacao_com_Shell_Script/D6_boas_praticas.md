# Boas Práticas em Scripting Bash

## 1. Sempre comece com o Shebang
O **shebang** define qual interpretador será usado para rodar seu script.

```bash
#!/bin/bash
```
## 2. Use nomes de variáveis descritivos
Evite nomes curtos e sem sentido.

**Ruim:**
```bash
n="Alice"
```

**Bom:**
```bash
nome_usuario="Alice"
```
## 3. Cuidado com espaços e aspas
Sempre use aspas duplas em variáveis para evitar erros com espaços ou caracteres especiais.
```bash
echo "$nome_usuario"
```

## 4. Use funções para modularizar
Evita repetição e organiza melhor.

## 5. Documente seu script
Inclua um cabeçalho no início do arquivo com:
```bash
#!/bin/bash
# Descrição: Script que faz backup de arquivos.
# Autor: Alice Dantas
# Data: 29/05/2025
# Versão: 1.0
```
