# GitHub Self Hosted Runner for Organization


This repository contains **Dockerfile** of GitHub self-hosted Runner for Organization.
Originally taken from https://sanderknape.com/2020/03/self-hosted-github-actions-runner-kubernetes/

To run this docker image, you will need to supply two `ENV` variables
- `GITHUB_ORG`: Please supply your own GitHub Organization name
- `GITHUB_PAT`: This is GitHub Personal Access Token that has an `admin:org` scope.

Example of running it:

``` sh
$ docker run -it -e GITHUB_ORG=lifepal -e GITHUB_PAT=<personal access token> lifepal/github-runner-org:2.263.0
```

This image tag is following GitHub Runner's version
