# Python template

Создайте репозиторий из шаблона и клонируйте его:

```sh
gh repo create my-project --template zerokqx/devenv-python --private --clone
cd my-project
```

Замените `--private` на `--public` для публичного репозитория. Измените имя проекта в `pyproject.toml`, затем разрешите direnv и добавляйте зависимости:

```sh
direnv allow
uv add <пакет>
uv run python main.py
```

Окружение можно также запустить командой `devenv shell`. При входе зависимости синхронизируются автоматически.
