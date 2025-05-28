# Organizar Arquivos por Extensão  
Script que organiza arquivos de uma pasta, movendo-os para subpastas conforme a extensão.

**Arquivo:** organizar.sh

## Conteúdo do Script:
```bash
#!/bin/bash

echo "Digite o caminho da pasta:"
read pasta

cd "$pasta" || { echo "Pasta não encontrada!"; exit 1; }

for arquivo in *.*; do
    extensao="${arquivo##*.}"
    mkdir -p "$extensao"
    mv "$arquivo" "$extensao/"
done

echo "Arquivos organizados por extensão."
```

## Explicação do funcionamento
- Solicita o caminho da pasta onde estão os arquivos.
- Cria subpastas com os nomes das extensões dos arquivos.
- Move cada arquivo para sua respectiva pasta.
- Informa que a organização foi concluída.

## Execute os seguintes comandos no terminal
```bash
chmod +x organizar.sh
```
```bash
./organizar.sh
```

## Resultado esperado
Os arquivos da pasta serão movidos para subpastas nomeadas com suas extensões.
