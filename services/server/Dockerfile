FROM python:3.8-slim-buster

ENV PYTHONUNBUFFERED 1
ENV PYTHONDONTWRITEBYTECODE 1

WORKDIR /code/

RUN pip install --upgrade pip
RUN pip install poetry
COPY . /code/
RUN poetry install

EXPOSE 8000

CMD ["python", "main.py"]
