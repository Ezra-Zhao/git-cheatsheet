# Hoja de referencia: Git en la práctica · Git Cheatsheet

> 🌍 [中文](README.md) · [Português](README.pt.md)

Una **hoja de referencia de una página** con comandos de Git para emergencias reales: 30 comandos organizados por escenario — **configuración, uso diario, deshacer, ramas, rebase, stash, remoto, rescate y avanzado**. Cada entrada dice tres cosas: **qué hace, un comando listo para copiar y etiquetas de uso**. Sin relleno; todos los comandos son sintaxis real de git.

## Para quién es

Para desarrolladores que viven entre `git add`, `commit` y `push`, y para cualquiera a quien un conflicto de `rebase`, una rama borrada o un commit perdido le haya dado un susto. Si solo conoces lo básico, esta hoja te salva en el momento crítico.

## Cómo usarla

1. Ve directo a **[CHEATSHEET.md](CHEATSHEET.md)** — el cuerpo de la referencia; los comandos en inglés funcionan igual en todas partes.
2. Empieza con los tres de "configuración": identidad, rama por defecto `main` y alias útiles. Se configuran una vez y sirven para siempre:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
   git config --global init.defaultBranch main
   ```
3. Si algo sale mal, ve a la sección "rescate": `reflog` recupera casi cualquier commit "perdido".

## Qué incluye

| Categoría | Contenido |
|---|---|
| ⚙️ Configuración | Identidad, rama por defecto, alias |
| 📅 Uso diario | Estado, staging, commits, ver historial |
| ↩️ Deshacer | Quitar del staging, descartar cambios, reset (tres modos), revert |
| 🌿 Ramas | Crear ramas, merge con `--no-ff`, borrar ramas locales y remotas |
| 🔁 Rebase | Rebase, rebase interactivo, `--continue/--abort`, la regla de oro |
| 📦 Stash | Guardar y recuperar cambios, listar, aplicar por nombre |
| 🌐 Remoto | remote, fetch con prune, pull --rebase, publicar ramas |
| 🆘 Rescate | reflog para recuperar commits, cherry-pick, bisect para cazar bugs |
| 🚀 Avanzado | worktree, submódulos, clon superficial |

Todos los comandos son sintaxis real de git (ver https://git-scm.com/doc); las operaciones peligrosas (`reset --hard`, `push --force`) llevan advertencia explícita.

## Contribuciones bienvenidas

¿Un comando incorrecto, un escenario que falta o una traducción mejorable? Los *pull requests* son bienvenidos. Mantén el formato (título / una frase / bloque de código / etiquetas) y **verifica que cada comando sea real antes de enviarlo**.

## Licencia

MIT © 2026 Guangyi Zhao. Ver [LICENSE](LICENSE).
