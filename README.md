
# CI to Docker Hub and Github Registry

GitHub Actions that build the image defined by the Dockerfile 
and push them to Docker Hub and Github Registry
may be found in the `.github/workflows` directory. 

The logs associated with running the workflows may be found under the "Actions" tab in the GitHub repo. 

Once the workflow have executed successfully, one may then run the built images in a Docker Container via `docker run -p80:80 petermchale/docker-ci` and pull the Github Registry image via `docker pull ghcr.io/petermchale/docker-ci:latest`. 


