# docker-slanger

  docker run --name some-redis -d redis

> Start the redis container

  docker build -t slanger .

> Build the slanger image

  docker run -p 8080:8080 -p 4567:4567 -it --link redis:redis --rm poll-slanger slanger --app_key your-key --secret your-secret -r "redis://172.17.0.32:6379/0"

> Run the image linking it to redis
