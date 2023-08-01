FROM python:3.10-slim

RUN apt-get update && apt-get install -y git
RUN git clone --depth 1 -b 0.1.0 https://github.com/Acemore/YLab_University_python_intensive_project /app

WORKDIR /app

RUN pip install poetry
RUN poetry install

CMD ["poetry", "run", "uvicorn", "menu_app.main:app", "--host", "0.0.0.0"]
