# Pull base image
FROM python:3.9

# Set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PHYTHONUNBUFFERED 1

# Set work directory
WORKDIR /home/joonyi/PycharmProjects/django-prof

# Install dependencies
COPY Pipfile Pipfile.lock /home/joonyi/PycharmProjects/django-prof/
RUN pip install pipenv && pipenv install --system

# Copy project
COPY . /home/joonyi/PycharmProjects/django-prof/
