## Step 1: Launch 'db' and 'api' containers for [Menu app](https://github.com/Acemore/YLab_University_python_intensive_project)

```
docker compose -f menu_app/docker-compose.yml up -d
```

Wait several seconds.

Open http://127.0.0.1:8000/api/v1/menus

## Step 2: Launch 'api-tests' container for [Menu app CRUD tests](https://github.com/Acemore/YLab_University_python_intensive_project_tests)

*IMPORTANT: Depends on Step 1*

```
docker compose -f menu_app_tests/docker-compose.yml up
```

## Remove containers

```
docker compose -f menu_app/docker-compose.yml rm -sf
docker compose -f menu_app_tests/docker-compose.yml rm -sf
```
