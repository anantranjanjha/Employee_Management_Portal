FROM python:3.7-alpine
RUN mkdir /app
WORKDIR /app

ADD requirements.txt /app

ADD app.py /app

RUN pip install -r requirements.txt

CMD ["gunicorn","--bind","0.0.0.0:8000","app:app"]