FROM python:3.8-slim-buster

ENV PYTHONUNBUFFERED 1
ENV PYTHONDONTWRITEBYTECODE 1

WORKDIR /app/

RUN pip install --upgrade pip
RUN pip install uvicorn
RUN pip install fastapi
RUN pip install pydantic
#RUN pip install poetry

COPY . /app/
#RUN poetry install

EXPOSE 8000

CMD ["python", "main.py"]
