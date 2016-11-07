FROM python:latest

RUN pip install --upgrade pip \
        && pip install Flask \
        && pip install gunicorn

WORKDIR app

COPY server.py app/

EXPOSE 8000

ENTRYPOINT gunicorn --workers=4 --bind 0.0.0.0:8000 app.server:app
