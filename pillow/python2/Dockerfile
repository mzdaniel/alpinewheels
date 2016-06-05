FROM alpine
MAINTAINER Daniel Mizyrycki mzdaniel@glidelink.net

# Install alpine python3
RUN  apk update
RUN  apk add curl python
RUN  curl https://bootstrap.pypa.io/get-pip.py | python

# Build alpine python pillow wheel
RUN  apk add alpine-sdk python-dev libjpeg-turbo-dev zlib-dev
RUN  pip install wheel
RUN  LIBRARY_PATH=/lib:/usr/lib pip wheel pillow

RUN \
    echo -e '\nsha1 checksum for wheel verification:'  &&\
    sha1sum /Pillow*whl
