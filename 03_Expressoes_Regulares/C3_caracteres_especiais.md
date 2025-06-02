## Tabela de Caracteres Especiais que precisam ser escapados

|  Caractere    |   Função na Regex                 |  Para buscar literalmente |
|---------------|-----------------------------------|-----------------------------|
| `.`           | Qualquer caractere                | `\.`                        |
| `*`           | Zero ou mais repetições           | `\*`                        |
| `+`           | Uma ou mais repetições            | `\+`                        |
| `?`           | Zero ou uma ocorrência            | `\?`                        |
| `^`           | Início da linha                   | `\^`                        |
| `$`           | Fim da linha                      | `\$`                        |
| `\|`           | Ou (alternância)                  | `\\|`                        |
| `(` e `)`     | Agrupamento                       | `\(` e `\)`                 |
| `[` e `]`     | Conjunto de caracteres            | `\[` e `\]`                 |
| `{` e `}`     | Quantificadores                   | `\{` e `\}`                 |
| `/`           | Barra (em alguns ambientes)       | `\/`                        |
| `\`           | Caractere de escape                | `\\`                        |

---

- Sempre que quiser que o caractere especial seja interpretado **literalmente**, use uma **barra invertida (`\`)** antes dele.
- Atenção: a própria barra invertida (`\`) também é um caractere especial e precisa ser escapada como `\\`.

---
