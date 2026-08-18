---
name: triagem-15484
description: "Triagem do corte sob a Lei 15.484: data do acórdão × 3.9.2026, via REsp/RE, presunção I-V, Súmulas 7/283/126. Use depois do warning e antes de qualquer tópico ou peça; também quando o operador disser o tópico é exigível?, presunção, 500 salários, súmula 126."
---

# TRIAGEM-15484

## Anexos

- `context/lei-15484.md` (arts. 4º e 7º)
- `context/ec-125-art105.md`
- `context/cpc-1035-1035a.md`

## Saída obrigatória (tabela)

| Campo | Valor |
|---|---|
| Via | REsp / RE / os dois |
| Data de publicação do acórdão | AAAA-MM-DD |
| Tópico de relevância | exigível (≥ 3.9.2026) / prudencial (< 3.9.2026) |
| Presunção | não / I / II / III / IV / V — nunca VI |
| Súmula 7 | risco sim/não (reexame de prova) |
| Súmula 283 | risco sim/não (fundamento autônomo não impugnado) |
| Súmula 126 | risco sim/não (par RE+REsp) |
| Prequestionamento | sim / não → ED antes |

## Regras

- Sem data do acórdão, a triagem não fecha. Volta ao warning.
- Valor da causa ≥ 500 SM → presunção III. Conferir o salário mínimo do ano do ajuizamento/atualização; se o número não estiver nos autos, marcar “III possível — falta prova do valor”.
- Acórdão contra linha dominante do STJ → presunção V. Exige paradigma no anexo ou declaração de que o paradigma será buscado fora (não inventar REsp).
- Prequestionamento negativo → indicar `embargos-de-declaracao` da vertical. Este plugin não redige ED de origem.

## Guard

Não classificar “exigível” sem a data. Não criar presunção VI.
