Containerisation
================

* [Container Training](https://container.training/)
    * Introduction to docker to Kubernetees deployments
* [[containerisation-WASM]]

* [The Docker, Kubernetes, Terraform, and AWS crash course series](https://blog.gruntwork.io/the-docker-kubernetes-terraform-and-aws-crash-course-series-dca343ba1274) [[kubernetes]]
    * Ramp up on DevOps tools in minutes via a series of lightning quick, hands-on crash courses where you learn by doing.

Docker
------

* [The Ultimate Docker Cheat Sheet](https://devopscycle.com/blog/the-ultimate-docker-cheat-sheet/)
* [BuildKit in depth: Docker's build engine explained](https://depot.dev/blog/buildkit-in-depth) Feb 2024

Dockerfile



data containers --volumes-from

lxc (docker)
lxd (aws lambda)
https://github.com/p8952/bocker


`--squash`

https://github.com/slimtoolkit/slim
brew install docker-slim

https://ubuntu.com/blog/we-reduced-our-docker-images-by-60-with-no-install-recommends

apt-get purge   --auto-remove && \
apt-get clean

* [Running Docker Containers as Current Host User](https://jtreminio.com/blog/running-docker-containers-as-current-host-user/) - Making local development less aggravating
* [Best Practices Around Production Ready Web Apps with Docker Compose](https://nickjanetakis.com/blog/best-practices-around-production-ready-web-apps-with-docker-compose)
* [Optimizing Docker image size and why it matters](https://contains.dev/blog/optimizing-docker-image-size)

https://www.fromlatest.io/#/

https://medium.com/sciforce/strategies-of-docker-images-optimization-2ca9cc5719b6

Sharing build cache

* Rubbish - manual and clumbsy
    * [Distributing Docker Cache across Hosts](https://runnable.com/blog/distributing-docker-cache-across-hosts)
        * Docker 1.10 changed layer cache
        * explicitly use `save` and `load` for tag.gz of layers
    * [Caching Docker layers on serverless build hosts with multi-stage builds, --target, and --cache-from](https://andrewlock.net/caching-docker-layers-on-serverless-build-hosts-with-multi-stage-builds---target,-and---cache-from/)
        * `--cache-from` for manually pushing build image. There must be a better way ...
* [Docker build cache sharing on multi-hosts with BuildKit and buildx](https://medium.com/titansoft-engineering/docker-build-cache-sharing-on-multi-hosts-with-buildkit-and-buildx-eb8f7005918e)
    * [docker/buildx](https://github.com/docker/buildx)
        * [Registry cache](https://docs.docker.com/build/cache/backends/registry/)
        * [GitHub Actions cache](https://docs.docker.com/build/cache/backends/gha/)
    * ```bash
        IMAGE_TAG=<IMAGE_REPO>:<CI_COMMIT_HASH>
        CACHE_TAG=<CACHE_REPO>:<CI_PROJECT_ID>-<CI_BRANCH_NAME>
        docker buildx build \
            -t $IMAGE_TAG \
            -f ./Dockerfile \
            --cache-from=type=registry,ref=$CACHE_TAG \
            --cache-to=type=registry,ref=$CACHE_TAG,mode=max \
            --push \
            --progress=plain \
            .
        ```

* [SubUser](https://subuser.org/)
    * Using docker containers to run applications with only dir level access
    * > Subuser turns a docker container into a normal program. But this program is not fully privileged. It can only access the directory from which it was called

* [The smallest Docker image to serve static websites](https://lipanski.com/posts/smallest-docker-image-static-website)
    * `thttpd` 187kb - built with alpine but uses the `scratch` image with no OS installed
* [Working on Multiple Web Projects with Docker Compose and Traefik](https://georgek.github.io/blog/posts/multiple-web-projects-traefik/)
    * Using a domain trafik that points to 127.0.0.1 and having name resolution - Kind of neat and simple docker-compose.override


### Docker Commandline Helpers

```bash
alias docker_clean='docker volume rm $(docker volume ls -qf dangling=true) ; docker rm $(docker ps -q -f status=exited) ; docker rmi $(docker images -q -f dangling=true)'
alias docker_nuke='docker_rm_all ; docker rmi --force $(docker images -q -a) ; docker volume rm $(docker volume ls -qf dangling=true) ; docker network rm $(docker network ls -q)'
alias docker_ps='docker ps -a --format "{{.ID}}\t{{.Names}}"'
alias docker_rm_all='docker_stop_all ; docker rm $(docker ps -a -q) --force'
alias docker_rm_exited='docker ps -a | grep Exit | cut -d " " -f 1 | xargs docker rm'
alias docker_stop_all='docker stop $(docker ps -a -q)'
```

Podman
------

* Secure by default
* No Root level daemon

* [Migrating from Docker to Podman](https://marcusnoble.co.uk/2021-09-01-migrating-from-docker-to-podman/)
* [Quadlets might make me finally stop using docker-compose](https://major.io/p/quadlets-replace-docker-compose/)

* [Will Nix Overtake Docker?](https://blog.replit.com/nix-vs-docker)
    * repl.it is moving from a single 30gb mega- container to a `nix` package pick and mix approach
* [On the joy of podman and auto-updates](https://feldspaten.org/2022/07/09/On-the-joy-of-podman-and-auto-updates/)
    * using podman for system services


---

* [The good things in the current age in tech](https://blog.kronis.dev/articles/the-good-things-in-the-current-age-in-tech)
    * [[containerisation]]
    * [[open-source]]


* [How we reduced 502 errors by caring about PID 1 in Kubernetes](https://about.gitlab.com/blog/2022/05/17/how-we-removed-all-502-errors-by-caring-about-pid-1-in-kubernetes/) #SIGTERM #SIGKILL

Orchestration
-------------

* [The container orchestrator landscape](https://lwn.net/SubscriberLink/905164/e1f4d4c1ce35f8b9/)
    * Systems quickly require many containers and they are difficult to deploy individually. We need orchestration. We keen [[kubernetes]]




[//begin]: # "Autogenerated link references for markdown compatibility"
[containerisation-WASM]: containerisation-WASM.md "Containerisation WASM"
[kubernetes]: kubernetes.md "Kubernetes"
[containerisation]: containerisation.md "Containerisation"
[open-source]: open-source.md "Open Source"
[//end]: # "Autogenerated link references"