FROM python:3.9

WORKDIR /code

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . .

CMD gunicorn solien_web.wsgi:application --bind 0.0.0.0:8000
