# illich

Mataroa Collection list of blogs.

## Development

This is a standard [Django](https://docs.djangoproject.com/) application with
[uv](https://github.com/astral-sh/uv).

1. Create database tables with:

```sh
uv run manage.py migrate
```

2. Run development server with:

```sh
uv run manage.py runserver
```

## Format and lint

Run Python formatting with:

```sh
uv run ruff format
```

Run Python linting with:

```sh
uv run ruff check --fix
```

## Deploy

Every commit on branch `main` auto-deploys using GitHub Actions. To deploy manually:

```sh
cd ansible/
cp .envrc.example .envrc
uv run ansible-playbook playbook.yaml -v
```

## License

This software is licensed under the MIT license.
For more information, read the [LICENSE](LICENSE) file.
