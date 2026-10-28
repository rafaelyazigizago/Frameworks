---
name: antes-de-construir
description: Os dois passos obrigatórios antes de construir qualquer projeto pessoal de Rafael Yazigi — GUT para escolher O QUE construir primeiro, SIPOC para desenhar COMO o projeto funciona e de quem ele depende. USE SEMPRE que a conversa for começar um projeto novo, reconstruir um sistema que parou, ou escolher entre dois ou mais projetos/funções para construir. Dispare mesmo sem citar "GUT" ou "SIPOC".
---

# Antes de construir: GUT + SIPOC

## De onde vem esta regra

Decidida por Rafael Yazigi em 28/10/2026, entre 4 frameworks de gestão
(SWOT, GUT, SIPOC, Balanced Scorecard). Ficaram só GUT e SIPOC porque:

- **GUT** ataca o gargalo real: os projetos pessoais esperam decisão de
  qual vem primeiro mais do que esperam construção.
- **SIPOC** ataca a causa real das quebras: sistemas que dependiam de
  algo que parou sem ninguém ver (ex.: em 15/10/2026 um servidor alugado
  caiu e levou 8 projetos junto; em 22/10/2026 um login vencido fez um
  robô falhar 395 vezes e ainda marcar a tarefa como concluída).

SWOT e Balanced Scorecard **não** são regra. Use só se Rafael pedir.

## Quando usar

| Situação | Passo |
|---|---|
| Há 2 ou mais projetos, funções ou consertos disputando a vez | **GUT** |
| Vai começar um projeto novo | **SIPOC** antes de escrever código |
| Vai reconstruir um sistema que parou | **SIPOC** antes de reinstalar |
| Vai acrescentar uma função grande a um sistema existente | **SIPOC** só da parte nova |

**Não usar** em: conserto pequeno, pergunta, ajuste de texto, uma tarefa só.

## Passo 1 — GUT (o que vem primeiro)

1. Liste os candidatos (no máximo 10 por rodada).
2. Dê nota de 1 a 5 em cada eixo:

| Nota | Gravidade (o estrago) | Urgência (o prazo) | Tendência (se nada for feito) |
|---|---|---|---|
| 5 | extremamente grave | ação imediata | piora rápido |
| 4 | muito grave | urgente | piora em pouco tempo |
| 3 | grave | o quanto antes | piora a médio prazo |
| 2 | pouco grave | pouco urgente | piora a longo prazo |
| 1 | sem gravidade | pode esperar | não piora |

3. **Multiplique** G × U × T (resultado de 1 a 125). Não some.
4. Ordene do maior para o menor. Em empate, ganha a maior Gravidade.
5. **As notas são proposta do Claude; Rafael corrige.** Mostre a tabela com
   uma linha de "por quê" em cada nota e espere o OK antes de construir.

## Passo 2 — SIPOC (como o projeto funciona)

Preencha a tabela antes de escrever código:

| Letra | Pergunta | Exemplos do que entra |
|---|---|---|
| **S** — Fornecedores | De quem ou do que o projeto depende? | servidor, conta, chave de API, login, celular, chip, outro sistema, pessoa |
| **I** — Entradas | O que chega para ele trabalhar? | arquivo, mensagem, link, tarefa, dado |
| **P** — Processo | Quais são os passos? (de 4 a 7) | recebe → confere → transforma → grava → avisa |
| **O** — Saídas | O que ele entrega? | página, arquivo, mensagem, registro |
| **C** — Clientes | Quem usa a saída? | Rafael, família, outro sistema |

Depois da tabela, responda para **cada fornecedor**:

1. **Se ele parar, como Rafael fica sabendo?** Se não há aviso, o aviso
   entra no projeto.
2. **É o único?** Fornecedor único sem plano B é marcado como risco.
3. **Vence?** (login, chave, plano grátis que pausa, assinatura) — anote a
   data ou marque `[LACUNA]`.

Regra dura: **o sistema nunca marca "concluído" se a entrada falhou.**

## Formato da entrega

1. Tabela GUT (se houve disputa) → espera o OK.
2. Tabela SIPOC + as 3 perguntas por fornecedor → espera o OK.
3. Só então começa a construção.

Linguagem leiga, siglas explicadas na mesma frase, no máximo 5 itens por
lista.
