# Repositories

В этом документе зафиксирован состав репозиториев проекта `Sol.app`.

Документ хранит переносимую структуру проекта без machine-specific абсолютных
путей.

## Репозитории проекта

- `sol_app`
- `sol_app_docs`
- `sol_backend`
- `sol_bruno`
- `sol_invite`
- `sol_site`

## Локальное расположение

Machine-specific пути задаются локально через
`ai-context/workspace/parameters/local-machine/local-machine.yaml`.

В git хранится только baseline-шаблон:
[`local-machine.example.yaml`](../../ai-context/baseline/templates/local-machine.example.yaml).

Для локальной структуры используются такие ключи:

- `repositories.sol_project_root` -> корень локальной группы проекта `sol_project/`
- `repositories.sol_app` -> репозиторий `sol_app`
- `repositories.sol_app_docs` -> репозиторий `sol_app_docs`
- `repositories.sol_backend` -> репозиторий `sol_backend`
- `repositories.sol_bruno` -> репозиторий `sol_bruno`
- `repositories.sol_invite` -> репозиторий `sol_invite`
- `repositories.sol_site` -> репозиторий `sol_site`

## Роль текущего репозитория

`sol_app_docs` используется как общий контур документации, проектного контекста
и постановки задач по `Sol.app`.

Реализация задач выполняется в профильных репозиториях проекта в зависимости от
области изменений.
