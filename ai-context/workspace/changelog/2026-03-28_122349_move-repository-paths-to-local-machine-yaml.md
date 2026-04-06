# Перенос путей репозиториев в `local-machine.yaml`

- Время: `2026-03-28 12:23:49`
- Файлы: `ai-context/parameters/local-machine/.gitignore`, `ai-context/parameters/local-machine/README.md`, `ai-context/parameters/local-machine/local-machine.example.yaml`, `docs/about/repositories.md`
- Что сделано: machine-specific пути репозиториев перенесены из отдельного env-формата в существующий `local-machine` YAML-формат.
- Что сделано: создан локальный файл `local-machine.yaml` с путями текущего ПК, а `local-machine.example.yaml` расширен секцией `repositories`.
- Что сделано: документация переведена с env-переменных на YAML-ключи `repositories.*`.
