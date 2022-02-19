
# DevOps

## Kubernetes:

I love the power of orchestration, it gives super powers the developer.

???+ danger "My Kubernetes learning path"

    - [X] Setup my own hardware cluster with Kubernetes from scratch
    - [X] Configured and used GKE (Google Kubernetes Engine)
    - [X] CNIs and storage backends
    - [X] Configured deployments of Ingresses, ReplicaSet, StatefulSets...
    - [X] RBAC
    - [X] Oauth2 setup for web exposed services, integrating them with frontends and backends
    - [X] **Creating deployments** and **HELM charts** for projects I build.
    - [X] Rancher

## Other cool tools:

???+ warning "Traefik"
    ![](https://traefik.io/static/traefik-proxy-logo--white-82153be41e0ce620a921b4bce974f6d8.svg)

    I just love using Traefik, I always use this expose my containers on the web, and it manages my https certificates automatically. <br/>
    <br/>
    If you read this on the web, this is the docker-compose serving this site:
    ```yaml
    ---
    version: '3'
    services:
      resume:
        build: .
        networks:
          - reverse-proxy
        labels:
          - "traefik.http.routers.docs.rule=Host(`resume.${DOMAIN}`)"
          - "traefik.http.routers.docs.entrypoints=web,websecure"
          - "traefik.enable=true"
          - "traefik.http.routers.docs.tls=true"
          - "traefik.http.services.docs.loadbalancer.server.port=80"
          - "traefik.http.routers.docs.tls.certresolver=myresolver"

    networks: 
      reverse-proxy:
        external: true
    ```

???- abstract "Docker Expert"

    - [X] Creating optimized DockerFiles
    ```docker
    # Stage 1 - the build process
    FROM node:14 as build-deps
    WORKDIR /usr/src/app
    COPY package.json .
    COPY package-lock.json .
    RUN npm i
    ADD . /usr/src/app
    COPY .env-prod ./src/.env
    RUN npm run build

    # Stage 2 - the production environment
    FROM nginx:alpine
    COPY --from=build-deps /usr/src/app/build /usr/share/nginx/html
    ADD ./nginx/default.conf /etc/nginx/conf.d/default.conf
    EXPOSE 80
    CMD ["nginx", "-g", "daemon off;"]

    ```

    - Setting up containers to use GPU resources

    - Docker desktop, docker-compose and docker swarm
    <div class="termy">
    ```console
    // start up all services
    $ docker-compose up -d --build
    // wait for all services to be running

    [+] Running 4/4
    - Container autodoc_classifier-1                  Running                                                                                                                                                                                                          0.0s
    - Container autodoc_api-1                         Running                                                                                                                                                                                                          0.0s
    - Container traefik                               Running                                                                                                                                                                                                          0.0s
    - Container autodoc-postgres                      Running                                                                                                                                                                                                          0.0s
    ```
    </div>


???- abstract "![](https://docs.gitlab.com/assets/images/gitlab-logo.svg)  Gitlab Ci"
    
    This is my preferential open source CI system yet. <BR/>
    Integrated with Docker and Kubernetes, If I have a choice, I'm running Gitlab-CI <BR/>
    My AI platform was built completely by gitlab CI, and IT was just great to work with.



???- abstract "Jenkins"
    - [X] Wrote pipelines in groovy

???- abstract "Ansible"
    - [X] Tower :heart:
    - [X] Deploying roles
    - [X] Creating new roles
    

