# Validação de E-mail no Bash com Regex

## Código de exemplo

```bash
EMAIL="usuario@dominio.com"

if echo "$EMAIL" | grep -Eq '^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'; then
  echo "E-mail válido: $EMAIL"
else
  echo "E-mail inválido: $EMAIL"
fi

EMAIL_INVALIDO="usuario@dominio"

if echo "$EMAIL_INVALIDO" | grep -Eq '^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'; then
  echo "E-mail válido: $EMAIL_INVALIDO"
else
  echo "E-mail inválido: $EMAIL_INVALIDO"
fi
```

## Entendendo o Regex

^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\\.[a-zA-Z]{2,}$

 Quebra da expressão:

| Parte                  | Significado                                                  |
|------------------------|--------------------------------------------------------------|
| `^`                    | Início da linha                                              |
| `[a-zA-Z0-9._%+-]+`    | Parte antes do `@` (nome do usuário). <br> Letras, números, ponto, sublinhado, %, +, - (um ou mais) |
| `@`                    | Símbolo arroba separador                                     |
| `[a-zA-Z0-9.-]+`       | Domínio (antes do ponto final). <br> Letras, números, ponto e hífen (um ou mais) |
| `\.`                   | Ponto literal entre domínio e extensão                       |
| `[a-zA-Z]{2,}`         | Extensão do domínio (ex.: com, br, org). <br> Pelo menos 2 letras |
| `$`                    | Fim da linha                                                |

