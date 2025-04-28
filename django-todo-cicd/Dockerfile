FROM python:3

WORKDIR /data

RUN sudo apt -y update
RUN pip install django==5.2
RUN pip install setuptools

COPY . .

RUN python manage.py migrate

EXPOSE 8000

CMD ["python","manage.py","runserver","0.0.0.0:8000"]


