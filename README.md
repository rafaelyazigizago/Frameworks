> Cópia-mestra dos frameworks de construção de Rafael Yazigi. Ela existe em dois lugares iguais: o GitHub `rafaelyazigizago/Frameworks` (privado) e o OneDrive pessoal, na pasta `Frameworks`. Se os dois divergirem, o GitHub vence. O conteúdo oficial começa no primeiro título.

# Frameworks

## O que é

São as regras que o Claude Code e o OpenCode seguem **antes de construir** qualquer projeto pessoal. Foram decididas em 28/10/2026:

1. **GUT:** escolhe **o que vem primeiro** quando há 2 ou mais projetos ou funções disputando a vez.
2. **SIPOC:** desenha **de quem o projeto depende** antes de escrever código.

O detalhe completo (quando usar, como pontuar, o modelo da tabela) está em `antes-de-construir/SKILL.md`.

## Como instalar numa bancada nova (~5 min)

A conta do Claude conectada não importa: o Claude Code lê as regras do disco.

1. Copiar a habilidade para a pasta do Claude Code:
   `~/.claude/skills/antes-de-construir/SKILL.md`
2. Acrescentar ao `~/.claude/CLAUDE.md`:

   ```markdown
   ## Antes de construir — desde 28/10/2026

   Antes de começar, reconstruir ou escolher entre projetos, siga a habilidade
   `antes-de-construir` (`~/.claude/skills/antes-de-construir/SKILL.md`):
   GUT para escolher o que vem primeiro, SIPOC para desenhar de quem o projeto depende.
   ```

3. Acrescentar ao `~/.config/opencode/AGENTS.md` (OpenCode):

   ```markdown
   ## Antes de construir — desde 28/10/2026

   Antes de começar, reconstruir ou escolher entre projetos, leia e siga
   `~/.claude/skills/antes-de-construir/SKILL.md` (GUT + SIPOC).
   ```

4. Prova: abrir uma sessão nova e pedir "vou começar um projeto novo". O Claude deve propor a tabela SIPOC antes de qualquer código.

## Histórico

| Data | O quê |
|---|---|
| 28/10/2026 | Criação. Entre SWOT, GUT, SIPOC e Balanced Scorecard, Rafael escolheu GUT + SIPOC, gravados na habilidade e nos arquivos de regras |
