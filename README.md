#### Dockerizing a Svelte app

Login to Docker Hub

```zsh
$ docker login
```

create a Svelte container

```zsh
$ docker build -t {yourDockerUsername}/svelte-app:1.0.0 .
```

Test the Svelte container by running it. It should be visible at localhost:8080

```zsh
$ docker run -p 8080:5000 {yourDockerUsername}/svelte-app:1.0.0
```

Push the container to your Docker Hub account repository

```zsh
$ docker push {yourDockerUsername}/svelte-app:1.0.0
```
