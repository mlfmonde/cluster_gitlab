# cluster_gitlab
GitLab service provided by a GitLab Docker image, in context of the [cluster](https://github.com/mlfmonde/cluster) project

> Then, the indications below are for the [cluster](https://github.com/mlfmonde/cluster) context

## Deployment
This service is deployed via Consul like other services in the cluster.

## Configuration
For the first launch, an initial configuration and database were generated. This configuration can be customized in editing the `gitlab.rb` file in `/etc/gitlab/` (this directory is mapped with a Docker volume named `containername_config`).

Clone by SSH is dependent of the Cluster HAProxy configuration, specificly the port used for it (see [the Cluster HAProxy configuration file template](https://github.com/mlfmonde/cluster/blob/master/haproxy/conf/haproxy.cfg.ctmpl)).
