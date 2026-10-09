# Cola de referência: Git na prática · Git Cheatsheet

> 🌍 [中文](README.md) · [Español](README.es.md)

Uma **cola de uma página só** com comandos de Git para emergências reais: 30 comandos organizados por cenário — **configuração, dia a dia, desfazer, branches, rebase, stash, remoto, resgate e avançado**. Cada entrada diz três coisas: **o que faz, um comando pronto para copiar e etiquetas de uso**. Sem enrolação; todos os comandos são sintaxe real do git.

## Para quem é

Para desenvolvedores que vivem entre `git add`, `commit` e `push`, e para quem já tomou um susto com conflito de `rebase`, branch apagada ou commit perdido. Se você só conhece o básico, esta cola salva na hora crítica.

## Como usar

1. Vá direto ao **[CHEATSHEET.md](CHEATSHEET.md)** — o corpo da referência; os comandos em inglês funcionam igual em todo lugar.
2. Comece pelos três de "configuração": identidade, branch padrão `main` e aliases úteis. Configura uma vez e vale para sempre:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
   git config --global init.defaultBranch main
   ```
3. Se algo der errado, vá à seção "resgate": o `reflog` recupera quase qualquer commit "perdido".

## O que está incluído

| Categoria | Conteúdo |
|---|---|
| ⚙️ Configuração | Identidade, branch padrão, aliases |
| 📅 Dia a dia | Status, staging, commits, ver histórico |
| ↩️ Desfazer | Tirar do staging, descartar mudanças, reset (três modos), revert |
| 🌿 Branches | Criar branches, merge com `--no-ff`, apagar branches locais e remotas |
| 🔁 Rebase | Rebase, rebase interativo, `--continue/--abort`, a regra de ouro |
| 📦 Stash | Guardar e recuperar mudanças, listar, aplicar por nome |
| 🌐 Remoto | remote, fetch com prune, pull --rebase, publicar branches |
| 🆘 Resgate | reflog para recuperar commits, cherry-pick, bisect para caçar bugs |
| 🚀 Avançado | worktree, submódulos, clone raso |

Todos os comandos são sintaxe real do git (ver https://git-scm.com/doc); operações perigosas (`reset --hard`, `push --force`) trazem aviso explícito.

## Contribuições são bem-vindas

Comando errado, cenário faltando ou tradução a melhorar? *Pull requests* são bem-vindos. Mantenha o formato (título / uma frase / bloco de código / etiquetas) e **verifique se cada comando é real antes de enviar**.

## Licença

MIT © 2026 Guangyi Zhao. Veja [LICENSE](LICENSE).
