
![example workflow](https://github.com/petermchale/docker-ci/actions/workflows/docker_hub.yml/badge.svg)
![example workflow](https://github.com/petermchale/docker-ci/actions/workflows/github_registry.yml/badge.svg)


# CI to Docker Hub and Github Registry

GitHub Actions that build the image defined by the Dockerfile 
and push them to Docker Hub and Github Registry
may be found in the `.github/workflows` directory. 

The logs associated with running the workflows may be found under the "Actions" tab in the GitHub repo. 

The Github Registry workflow is triggered by, e.g., 
```
git tag -a v1.0.8; git push origin v1.0.8
```

Once the workflows have executed successfully, one may then run the docker-hub image in a Docker Container via `docker run -p80:80 petermchale/docker-ci` and pull the Github Registry image via `docker pull ghcr.io/petermchale/docker-ci:latest`. 


