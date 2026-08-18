---
name: warning-entrada-corte
description: "Warning de entrada do resp-re-os. Substitui onboarding. Dispara antes de qualquer peça de REsp/RE/relevância/repercussão geral. Coleta 5 fatos e barra redação se faltar um. Use quando o operador disser REsp, recurso especial, RE, recurso extraordinário, relevância, repercussão geral, 15.484, 1.035-A, filtro do STJ, filtro do STF."
---

# WARNING-ENTRADA-CORTE

> Sem onboarding. Sem `/start`. Este bloco é a porta.

## Anexos

- `context/metodologia-topico.md` — ler primeiro.

## Texto (devolver inteiro, uma vez por sessão ou quando a via mudar)

```
Este plugin só opera corte superior (REsp Lei 15.484 + RE com repercussão geral).
Não substitui o cível. Não instrui o feito. Não promete afetação nem conhecimento.

Antes de redigir, preciso de 5 fatos:
1. Via: REsp / RE / os dois
2. Data de PUBLICAÇÃO do acórdão recorrido
3. Valor da causa (presunção III — 500 SM?) e se o acórdão contraria STJ (presunção V)
4. Questão federal / constitucional em uma frase
5. O acórdão enfrentou essa questão? (prequestionamento)

Se a matéria for conhecimento, tutela ou apelação, saia e use o plugin da vertical.
```

## Metodologia

1. Emitir o bloco.
2. Não redigir peça enquanto faltar qualquer um dos 5.
3. Com os 5 em mão, passar a `resp-re-master` (não pular a orquestradora).
4. Se o operador insistir em “só escreve o REsp”, repetir o item que falta. Não inventar data, valor ou prequestionamento.

## Guard

Sem data de publicação do acórdão → não classifica exigência do art. 4º. Sem questão em uma frase → não há tópico. Sem prequestionamento declarado → avisar ED prévio; não fingir que o acórdão enfrentou.
