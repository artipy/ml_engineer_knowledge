# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Что это за репозиторий

Obsidian vault для изучения Machine Learning. Содержит сырые заметки из курса и обработанные заметки, отформатированные для Obsidian.

## Структура

```
raw_notes/         # Сырые заметки — черновики, конспекты, изображения
notes/             # Обработанные заметки для Obsidian (читаемый финальный вид)
raw_notes/processed_log.md   # Какие raw_notes уже превращены в notes/
notes/reading_log.md         # Какие notes/ прочитаны пользователем
```

## Workflow: превращение сырых заметок в Obsidian-заметки

1. Прочитать файл из `raw_notes/`
2. Создать обработанную заметку в `notes/` — тот же номер и название, но с форматированием Obsidian
3. Обновить оба лога: `raw_notes/processed_log.md` и `notes/reading_log.md`

## Формат заметок в `notes/`

Каждая заметка начинается с YAML frontmatter:

```yaml
---
tags:
  - ml
  - <топик>
aliases:
  - <русское название>
created: YYYY-MM-DD
source: raw_notes/<исходный файл>
---
```

Использовать Obsidian callout-блоки: `[!example]`, `[!tip]`, `[!warning]`, `[!important]`, `[!summary]`.

Завершать заметку секцией `## Связанные заметки` со ссылками `[[...]]`.

## Логи

**`raw_notes/processed_log.md`** — добавлять запись при создании каждой новой заметки:

| Файл | Статус | Создана заметка | Дата |
|---|---|---|---|
| имя файла | ✅ использован | notes/имя заметки | дата |

**`notes/reading_log.md`** — добавлять запись со статусом `📋 не прочитано` при создании каждой новой заметки.
