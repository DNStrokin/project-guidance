# project-guidance

Навык для Codex, Cursor и Claude Code. Помогает подготовить инструкции агентам, требования, дорожную карту и руководство разработчика. В новом проекте описывает первый результат, который можно проверить. В существующем сверяет документацию с кодом и тестами и находит ближайший шаг. [Инструкции навыка](SKILL.md)

## Установка

Выберите личный каталог на машине, где работает агент. [Документация Codex](https://developers.openai.com/codex/skills/) · [Cursor](https://cursor.com/docs/skills) · [Claude Code](https://code.claude.com/docs/en/skills)

| Среда | Каталог навыка | Вызов в чате |
| --- | --- | --- |
| Codex | `~/.agents/skills/project-guidance` | `$project-guidance` |
| Cursor | `~/.agents/skills/project-guidance` или `~/.cursor/skills/project-guidance` | `/project-guidance` |
| Claude Code | `~/.claude/skills/project-guidance` | `/project-guidance` |

Для Codex и Cursor достаточно одного клона.

```sh
git clone https://github.com/DNStrokin/project-guidance.git "$HOME/.agents/skills/project-guidance"
```

Если используете все три среды на Linux или macOS, подключите этот же клон к Claude Code.

```sh
mkdir -p "$HOME/.claude/skills"
ln -s "$HOME/.agents/skills/project-guidance" "$HOME/.claude/skills/"
```

Для отдельной установки Claude Code можно сразу клонировать навык в его каталог.

```sh
git clone https://github.com/DNStrokin/project-guidance.git "$HOME/.claude/skills/project-guidance"
```

Чтобы обновить навык, выполните `git pull --ff-only` из каталога клона.

## Пример

Откройте чат в рабочем проекте, вызовите навык командой из таблицы и добавьте задачу.

> Актуализируй инструкции для агентов и дорожную карту. Сохрани правила для отдельных каталогов и укажи ближайший шаг, готовность которого можно проверить.
