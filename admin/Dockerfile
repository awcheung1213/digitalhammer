# start base image from latest python version
# add env variable for log tracking
# create working directory /app
# copy requirements to /app/requirements.txt
# run install for everything in requirements
# copy all files to /app
# run the app on server 0.0.0.0:8000 *required to run on localhost*

FROM python:3.9
ENV PYTHONUNBUFFERED 1
WORKDIR /app
COPY requirements.txt /app/requirements.txt
RUN pip install -r requirements.txt
COPY . /app

CMD python manage.py runserver 0.0.0.0:8000