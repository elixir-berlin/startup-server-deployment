# Startup Server Deployment

Configuration to deploy the [extreame_startup](https://github.com/rchatley/extreme_startup) server.

Docker Imgae used `elixirberlin/extreme_startup:latest`


## Deploying

1) Configure kubectl
2) Cehckout this repo
3) run `kubectl apply --recursive -f k8s/`

## Remove deployment

`kubetl delete namespace extreme-startup`

## Checking logs of the running server

`kubectl logs -f deployment/extreme-server -n extreme-server`
