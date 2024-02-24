
# deploy-to-development
Workflow for build and deploy a Docker Image to registry

## Actions applied to this workflow

- [actions/checkout](https://github.com/actions/checkout)
- [docker/setup-buildx-action](https://github.com/docker/setup-buildx-action)
- [docker/login-action](https://github.com/docker/login-action)
- [docker/build-push-action](https://github.com/docker/build-push-action)

## Configuration Dependencies

#### Environments

```
  development
```

#### Environment Variables

| Name       | Default     | Description                                                   |
| :--------  | :---------- |:--------------------------------------------------------------|
| `REGISTRY` | `docker.io` | **Required**. Id of Registry that will host the Docker Image  |

#### Environment Secrets

| Name       | Defaul      | Description                                                   |
|:-----------|:------------|:--------------------------------------------------------------|
| `USER`     | `-`         | **Required**. Login of the Registry Account                   |
| `TOKEN`    | `-`         | **Required**. Unique access Token                             |
