# Backup Simples
Script que gera um backup compactado de uma pasta informada pelo usuário.

## Conteúdo do Script:
```bash
#!/bin/bash

DATA=$(date +%Y-%m-%d)

echo "Digite o caminho da pasta que deseja fazer backup:"
read pasta

echo "Digite o caminho onde salvar o backup:"
read destino

tar -czf "$destino/backup_$DATA.tar.gz" "$pasta"

echo "Backup criado em $destino/backup_$DATA.tar.gz"
```

## Explicação do funcionamento
- Solicita o caminho da pasta a ser salva.
- Solicita onde salvar o backup.
- Cria um arquivo .tar.gz com a data atual no nome.
- Imprime uma mensagem informando onde o backup foi criado.


## Execute os seguintes comandos no terminal
```bash
chmod +x backup.sh
```
```bash
./backup.sh
```

## Resultado Esperado
Será criado um arquivo *backup_YYYY-MM-DD.tar.gz* no diretório atual contendo os arquivos da pasta especificada.
