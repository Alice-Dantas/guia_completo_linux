# Validação de CPF no Bash com Regex

## Código de exemplo

```bash
CPF="123.456.789-09"

if echo "$CPF" | grep -Eq '^[0-9]{3}\.[0-9]{3}\.[0-9]{3}\-[0-9]{2}$'; then
  echo "CPF válido no formato: $CPF"
else
  echo "CPF inválido: $CPF"
fi

CPF_INVALIDO="12345678909"

if echo "$CPF_INVALIDO" | grep -Eq '^[0-9]{3}\.[0-9]{3}\.[0-9]{3}\-[0-9]{2}$'; then
  echo "CPF válido no formato: $CPF_INVALIDO"
else
  echo "CPF inválido: $CPF_INVALIDO"
fi
```

## Entendendo o Regex
^[0-9]{3}\\.[0-9]{3}\\.[0-9]{3}\\-[0-9]{2}$

Quebra da expressão:

| Parte                   | Significado                                                   |
|-------------------------|---------------------------------------------------------------|
| `^`                     | Início da linha                                               |
| `[0-9]{3}`              | Três dígitos                                                  |
| `\.`                    | Ponto literal                                                 |
| `[0-9]{3}`              | Três dígitos                                                  |
| `\.`                    | Ponto literal                                                 |
| `[0-9]{3}`              | Três dígitos                                                  |
| `\-`                    | Hífen literal                                                 |
| `[0-9]{2}`              | Dois dígitos                                                  |
| `$`                     | Fim da linha                                                  |
