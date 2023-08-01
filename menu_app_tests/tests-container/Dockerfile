FROM python:3.10-slim

RUN apt-get update && apt-get install -y git
RUN git clone --depth 1 https://github.com/Acemore/YLab_University_python_intensive_project_tests /tests

WORKDIR /tests

RUN pip install poetry
RUN poetry install

CMD poetry run pytest tests/*
