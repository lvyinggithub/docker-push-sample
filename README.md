# docker-push-sample
Sample repo on how to use GitHub Actions to push a docker image using the official Docker actions.

# Setup

You need to configure two secrets on your GitHub repo for this sample to work.

Navigate to the Docker Hub and generate a new access token. The access token is your password.

https://hub.docker.com/settings/security

The username is your normal user name, but it is also displayed when you generate a new access token.

Navigate to your Settings and Secrets and add two keys, one with your username and another with the access token:

https://github.com/sondreb/docker-push-sample/settings/secrets

The names should be:

DOCKER_USERNAME

DOCKER_PASSWORD

Finally you need to edit the build.yml, with your own custom tags, and of course change this to your own organization and docker image: 

```
repository: sondreb/dockerpushsample
```
