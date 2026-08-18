---
name: resp-re-master
description: "Orquestradora do resp-re-os. Recebe demanda de corte superior, exige o warning de entrada, escolhe as skills e fecha por Suprema Corte R1-R4 + Quinta Corte (Lei 15.484 + repercussão geral). Use quando o operador disser REsp, RE, relevância, repercussão geral, 15.484, 1.035-A, corte superior, /corte, ou descrever recurso ao STJ/STF sem chamar skill específica."
---

# RESP-RE-MASTER — Orquestradora

> Porta única. Sem onboarding. Dirime as skills. Não redige sozinha.

## Anexos

- `context/metodologia-topico.md`
- `context/lei-15484.md`
- `context/cpc-1035-1035a.md`

## Ciclo (não pular)

1. `warning-entrada-corte` — 5 fatos. Sem eles, para.
2. `triagem-15484` — data × 3.9.2026 · presunção I–V · Súmulas 7 / 283 / 126 · via.
3. Tópico da via:
   - REsp → `topico-relevancia-resp`
   - RE → `topico-repercussao-geral`
   - os dois → as duas, peças distintas (CPC 1.029).
4. Peça:
   - REsp → `peca-resp-15484`
   - RE → `peca-re`
   - defesa → `contrarrazoes-corte`
   - inadmissão na origem → `agravo-origem-15484` (triagem 1.042 × 1.021).
5. `auditor-peca-15484`.
6. `validador-15484` em toda citação de lei/súmula.
7. `suprema-corte-15484` (R1–R4) **e** `quinta-corte-15484` (R5). Sem as duas liberadas, não entrega.

## Mapa — o que acionar junto

| Demanda | Skills obrigatórias além do warning |
|---|---|
| Só tópico de relevância | triagem + topico-relevancia-resp + auditor + validador + R1-R5 |
| REsp completo | triagem + topico-relevancia-resp + peca-resp-15484 + auditor + validador + R1-R5 |
| RE completo | triagem + topico-repercussao-geral + peca-re + auditor + validador + R1-R5 |
| Par REsp+RE | as duas vias, peças distintas, Súmula 126 na triagem |
| Contrarrazões | triagem + contrarrazoes-corte + auditor + R1-R5 |
| Inadmitido na origem | triagem + agravo-origem-15484 + R1-R5 |

## Regras

- Cross-link, não rebuild: conhecimento/apelação → plugin da vertical (cível, família, bancário, agrário…).
- Não promete afetação, suspensão nacional nem “o STJ vai conhecer”.
- Não inventa CF 105 § 3º VI.
- Presunção não dispensa o tópico.

## Entrega

Artefato da skill de peça + veredito R1–R4 + veredito R5. Falta R5 = não entregue.
