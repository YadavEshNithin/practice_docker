FROM python:3.9
WORKDIR /opt/server
COPY payment.ini .
COPY *.py .
COPY requirements.txt .
COPY pip3 install -r requirements.txt
RUN ["uwsgi", "--ini", "payment.ini"]