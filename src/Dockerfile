FROM python:3.8

ENV PYTHONUNBUFFERED 1

WORKDIR /usr/src/app

RUN pip install pillow django-crispy-forms matplotlib seaborn pandas xhtml2pdf

COPY requirements.txt ./
RUN pip install -r requirements.txt


COPY . . 
CMD python manage.py runserver 0.0.0.0:80
