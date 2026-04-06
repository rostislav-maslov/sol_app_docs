# Repositories

В этом документе зафиксирован состав репозиториев проекта `Sol.app`.

Документ хранит переносимую структуру проекта без machine-specific абсолютных
путей.

## Репозитории проекта

Проект `sol_app` в этом контуре рассматривается как группа связанных
репозиториев, лежащих на одном уровне внутри `sol_project/`.

- `sol_app`
- `sol_app_docs`
- `sol_backend`
- `sol_bruno`
- `sol_invite`
- `sol_site`

## Как интерпретировать `sol_app_docs`

`sol_app_docs` - это не документация только для самого репозитория
`sol_app_docs`.

Это общий документационный и управленческий контур проекта `sol_app`, внутри
которого документация может относиться к любому из дочерних репозиториев
проекта или к их взаимодействию между собой.

Если документ не уточняет scope явно, его нужно читать в контексте общего
проекта `sol_app`, а не как контекст только одного репозитория.

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

Текущее состояние веток дочерних репозиториев хранится локально в
`ai-context/workspace/parameters/local-machine/local-machine.yaml` в секции
`repositories_state.branches`.

Это machine-local snapshot, поэтому его нужно держать в актуальном состоянии
локально и не фиксировать в versioned документации.

## Роль текущего репозитория

`sol_app_docs` используется как общий контур документации, проектного контекста
и постановки задач по `Sol.app`.

Реализация задач выполняется в профильных репозиториях проекта в зависимости от
области изменений.
