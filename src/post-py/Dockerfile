FROM python:3.6.0-alpine

WORKDIR /app
COPY . /app

RUN apk add --no-cache gcc && apk add --no-cache musl-dev \
 && rm -rf /var/cache/apk/*
RUN pip install --upgrade pip -r /app/requirements.txt

ENV POST_DATABASE_HOST post_db
ENV POST_DATABASE posts

ENTRYPOINT ["python3", "post_app.py"]
