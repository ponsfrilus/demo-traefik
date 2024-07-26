# Demo traefik

A few examples of [Traefik 3] configuration, using the *.localhost[^1] as
described in the RFC6761:
> Name resolution APIs and libraries SHOULD recognize localhost names as special
> and SHOULD always return the IP loopback address for address queries

The dashboard should be accessible at http://dashboard.localhost.

The demo app ([whoami]), should be accessible at http://demotraefik.localhost.

1) In [example_01](./example_01), the most basic configuration, all in HTTP.
1) In [example_02](./example_02) a middleware (`https_redirect`) is used to 
   redirect all HTTP to HTTPS, using the Traefik default certificat.


[Traefik 3]: https://github.com/traefik/traefik/releases/tag/v3.1.0
[^1]: https://datatracker.ietf.org/doc/html/rfc6761#section-6.3
[whoami]: https://github.com/traefik/whoami
