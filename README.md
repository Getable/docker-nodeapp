# docker nodeapp [![The official docker image](http://dockeri.co/image/getable/nodeapp)](https://registry.hub.docker.com/u/getable/nodeapp/)

A generic container for spinning up node apps.

## Usage
1. Add a Dockerfile to your repo.

    ```ini
    FROM getable/nodeapp
    ```

2. Build: `docker build -t myNodeApp .`
3. Run: `docker run -d --restart=always -P myNodeApp`

## Notes
* `NODE_ENV` defaults to production. You can override by passing an env var to the run script with: `-e "NODE_ENV=staging"`
* The docker file exposes port 80.

## Developing
Pushing to this repo pushes to [the official docker image](https://registry.hub.docker.com/u/getable/nodeapp/).
