# Docker+Flask Hello World
A simple Flask app running on Docker.

## Running the example

```shell
docker build -t flask:latest .
docker run -d -p 5000:5000 flask
docker run -d -p 5000:5000 -e APP_COLOR=pink flask
```

or, if you want to give your container a specific name:

```shell
docker build -t flask:latest .
docker run --name my-flask -d -p 5000:5000 flask
```