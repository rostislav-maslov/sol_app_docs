# Перевод `ai-context` на split `baseline/workspace`

- Время: `2026-04-06 06:06:54 +0300`
- Файлы: `ai-context/.gitignore`, `ai-context/README.md`, `ai-context/baseline/**/*`, `ai-context/workspace/**/*`, `docs/about/repositories.md`, `docs/about/sol-app.md`
- Что сделано: синхронизирован новый baseline из `https://github.com/foodtechlab/ai_context_rules` c физическим разделением на `ai-context/baseline/` и `ai-context/workspace/`.
- Что сделано: project-local данные перенесены из старой плоской структуры в `workspace`, включая changelog, AI task files, local-machine параметры и backlog эпиков.
- Что сделано: удалены устаревшие директории старой mixed-схемы и обновлены живые ссылки в документации на новые пути `workspace`.
- Что сделано: структура проверена через `ai-context/baseline/scripts/verify-ai-context.py` в режиме `project-manager`.
