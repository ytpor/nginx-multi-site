# Nginx Multi Site

Skeleton project to illustrate [Path-based Routing] in [nginx-proxy].

## Getting started

### Test domain

On Windows, add this to your `hosts` file.

    127.0.0.1 multi-site.local

### Create docker network

Check whether you have the `nginx-proxy` network.

    docker network ls

If not found, create the `nginx-proxy` network.

    docker network create nginx-proxy

### Start the container

Start the container

    docker compose up -d

You can then access the application through the following URLs:

    http://multi-site.local
    http://multi-site.local/bar/
    http://multi-site.local/bar/home/
    http://multi-site.local/foo/
    http://multi-site.local/foo/home/

## References

* [nginx-proxy][nginx-proxy]
* [Path-based Routing][Path-based Routing]

[nginx-proxy]: https://github.com/nginx-proxy/nginx-proxy
[Path-based Routing]: https://github.com/nginx-proxy/nginx-proxy/tree/main/docs#path-based-routing
