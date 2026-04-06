# Зафиксирован multi-repo контекст проекта `sol_app`

- Время: `2026-04-06 06:16:39 +0300`
- Файлы: `ai-context/workspace/parameters/repository-parameters.yaml`, `ai-context/workspace/rules/01-sol-app-multi-repo-context.md`, `docs/about/repositories.md`
- Что сделано: в repository-level параметрах зафиксировано, что `sol_app_docs` является общим документационным и управленческим контуром проекта `sol_app` для группы дочерних репозиториев.
- Что сделано: добавлено project-specific правило, обязывающее учитывать multi-repo scope и проверять актуальные ветки дочерних репозиториев перед branch-sensitive действиями.
- Что сделано: документация по репозиториям уточнена так, чтобы `sol_app_docs` интерпретировался как общий контур документации проекта, а текущие ветки дочерних репозиториев хранились в machine-local snapshot.
