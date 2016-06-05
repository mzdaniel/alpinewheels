Alpine linux python wheels
==========================

Temporary support for Alpine wheels based on musl libc.

`Alpine Linux`_ is a wonderful lightweight Linux distro featuring python3
support. `Many projects`_ are targetting it as it streamlines developer
processes. In our Python community, the standard packaging is pypi, and although
it recently started featuring `glibc support`_ with the awesome job of the Pypa
team, it still `lacks support`_ for musl based libc as needed in Alpine.

This repo, and related docker images tries to fill this void until a better
solution is found. The artifacts and images are gratiously built in the
`dockerhub`_, and the actual wheels hosted on `github`_.

For now, packages supported are:

  - pillow


.. _Alpine Linux: https://github.com/gliderlabs/docker-alpine
.. _Many projects: https://github.com/gliderlabs/docker-alpine/issues/57
.. _glibc support: https://github.com/pypa/manylinux
.. _lacks support: https://github.com/pypa/manylinux/issues/37

