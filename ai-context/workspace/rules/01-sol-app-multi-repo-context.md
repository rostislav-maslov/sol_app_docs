# Контекст multi-repo проекта `sol_app`

## Статус

Действует.

## Цель

Убрать неоднозначность, в которой `sol_app_docs` ошибочно воспринимается как
документация только для самого себя, а не как общий контур документации для
всей группы репозиториев проекта `sol_app`.

## Область применения

- документация в `sol_app_docs`;
- task-постановки и project context в этом репозитории;
- любые AI-задачи, где нужно понять, к какому дочернему репозиторию относится
  описание, решение или изменение;
- любые cross-repo действия, зависящие от текущих локальных веток.

## Правило

- считать `sol_app_docs` общим документационным и управленческим репозиторием
  проекта `sol_app`;
- считать дочерними репозиториями проекта `sol_app`, `sol_app_docs`,
  `sol_backend`, `sol_bruno`, `sol_invite` и `sol_site`;
- при работе с документацией по умолчанию учитывать, что она может описывать
  любой дочерний репозиторий проекта или их взаимодействие;
- перед выводами и действиями, зависящими от текущего состояния кода в
  дочерних репозиториях, сначала проверять их текущие ветки;
- использовать локальный snapshot веток из
  `ai-context/workspace/parameters/local-machine/local-machine.yaml` как
  быстрый источник контекста и обновлять его при изменениях.

## Что запрещено

- трактовать `sol_app_docs` как изолированный репозиторий без связи с остальной
  группой `sol_app`;
- писать документацию так, будто она по умолчанию относится только к одному
  репозиторию, если scope не уточнен;
- принимать branch-sensitive решения по памяти без проверки актуальных веток
  дочерних репозиториев.

## Чеклист применения

- определить, к какому дочернему репозиторию или набору репозиториев относится
  текущий документ или задача;
- проверить локальный branch snapshot в
  `ai-context/workspace/parameters/local-machine/local-machine.yaml` или
  обновить его через `git -C <repo-path> rev-parse --abbrev-ref HEAD`;
- в ответах и документации явно указывать целевые репозитории, если это важно
  для понимания scope;
- не смешивать versioned проектный контекст и machine-local branch state.

## Связанные файлы

- `/Users/rostislavmaslov/workspace/projects/sol_project/sol_app_docs/docs/about/repositories.md`
- `/Users/rostislavmaslov/workspace/projects/sol_project/sol_app_docs/ai-context/workspace/parameters/repository-parameters.yaml`
- `/Users/rostislavmaslov/workspace/projects/sol_project/sol_app_docs/ai-context/workspace/parameters/local-machine/local-machine.yaml`
