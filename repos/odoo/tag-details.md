<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `odoo`

-	[`odoo:14`](#odoo14)
-	[`odoo:14.0`](#odoo140)
-	[`odoo:15`](#odoo15)
-	[`odoo:15.0`](#odoo150)
-	[`odoo:16`](#odoo16)
-	[`odoo:16.0`](#odoo160)
-	[`odoo:latest`](#odoolatest)

## `odoo:14`

```console
$ docker pull odoo@sha256:725ddd95720fcd1ef948185ca6e50936664f6642ca4aebd08376d57fc4333f3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:56d6b90cb5a467439fafceb0f1389c152747379365d20b9bacb491168174923d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.8 MB (532768024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:850f712d90dc26e7acb7f0e76d10fe193798125a92f7a26ed75e53e77a601077`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:47 GMT
ADD file:ca4076bfffab8d09636384070ca253570590554cff76a132afaae5cd89b363b5 in / 
# Tue, 04 Jul 2023 01:20:48 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:54:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:54:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:54:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:23 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:56:34 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:56:37 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:56:37 GMT
ENV ODOO_VERSION=14.0
# Tue, 04 Jul 2023 16:56:37 GMT
ARG ODOO_RELEASE=20230629
# Tue, 04 Jul 2023 16:56:37 GMT
ARG ODOO_SHA=621799a3ab09aacdf4139b3dbea6af48a2fb0df0
# Tue, 04 Jul 2023 16:58:03 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=621799a3ab09aacdf4139b3dbea6af48a2fb0df0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 04 Jul 2023 16:58:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 04 Jul 2023 16:58:07 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 04 Jul 2023 16:58:07 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=621799a3ab09aacdf4139b3dbea6af48a2fb0df0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 04 Jul 2023 16:58:08 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 04 Jul 2023 16:58:08 GMT
EXPOSE 8069 8071 8072
# Tue, 04 Jul 2023 16:58:08 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 04 Jul 2023 16:58:08 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 04 Jul 2023 16:58:08 GMT
USER odoo
# Tue, 04 Jul 2023 16:58:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 16:58:08 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:90ac1ecaf92c8ae0cb37d29d8cc01b5802612c12edb933c369ad4c586ea94c6c`  
		Last Modified: Tue, 04 Jul 2023 01:26:21 GMT  
		Size: 27.1 MB (27138502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00e825012af0c5f20095b1f8902b3341da662edb2331f4bc160e8291a8d2ff8`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 213.2 MB (213180476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab84fcf971d80a1b3e08f8415ad0ba35cbedb84cb7594ec24c79ad3dab44e84`  
		Last Modified: Tue, 04 Jul 2023 16:59:56 GMT  
		Size: 13.5 MB (13520290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc728f9cb60a83b4ab60b063840b0f84f5855805efe3fee682ef70cb18bb5`  
		Last Modified: Tue, 04 Jul 2023 16:59:54 GMT  
		Size: 458.3 KB (458274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a42d222d146900666c054ac1c165e03457150b661f1c20eb9a986adf4d2678`  
		Last Modified: Tue, 04 Jul 2023 17:00:23 GMT  
		Size: 278.5 MB (278468023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5156c18e6590cd36a4e4f59b32b52ef418667a3135e813115765772a34adf1a`  
		Last Modified: Tue, 04 Jul 2023 16:59:52 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506b322f0c562cb9aebf20161af21d5616174cc29a2966e2a2d9a1db65dbb722`  
		Last Modified: Tue, 04 Jul 2023 16:59:52 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de50af5eecc3c9b985c696efb3004d9afd15abc265fe45b109811e2cb805035d`  
		Last Modified: Tue, 04 Jul 2023 16:59:52 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c9ef420f6d91442c5d866fd4d642a88523a1fede003a97fea4d238c47fdf60`  
		Last Modified: Tue, 04 Jul 2023 16:59:52 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:725ddd95720fcd1ef948185ca6e50936664f6642ca4aebd08376d57fc4333f3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:56d6b90cb5a467439fafceb0f1389c152747379365d20b9bacb491168174923d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.8 MB (532768024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:850f712d90dc26e7acb7f0e76d10fe193798125a92f7a26ed75e53e77a601077`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:47 GMT
ADD file:ca4076bfffab8d09636384070ca253570590554cff76a132afaae5cd89b363b5 in / 
# Tue, 04 Jul 2023 01:20:48 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:54:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:54:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:54:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:23 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:56:34 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:56:37 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:56:37 GMT
ENV ODOO_VERSION=14.0
# Tue, 04 Jul 2023 16:56:37 GMT
ARG ODOO_RELEASE=20230629
# Tue, 04 Jul 2023 16:56:37 GMT
ARG ODOO_SHA=621799a3ab09aacdf4139b3dbea6af48a2fb0df0
# Tue, 04 Jul 2023 16:58:03 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=621799a3ab09aacdf4139b3dbea6af48a2fb0df0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 04 Jul 2023 16:58:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 04 Jul 2023 16:58:07 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 04 Jul 2023 16:58:07 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=621799a3ab09aacdf4139b3dbea6af48a2fb0df0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 04 Jul 2023 16:58:08 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 04 Jul 2023 16:58:08 GMT
EXPOSE 8069 8071 8072
# Tue, 04 Jul 2023 16:58:08 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 04 Jul 2023 16:58:08 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 04 Jul 2023 16:58:08 GMT
USER odoo
# Tue, 04 Jul 2023 16:58:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 16:58:08 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:90ac1ecaf92c8ae0cb37d29d8cc01b5802612c12edb933c369ad4c586ea94c6c`  
		Last Modified: Tue, 04 Jul 2023 01:26:21 GMT  
		Size: 27.1 MB (27138502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00e825012af0c5f20095b1f8902b3341da662edb2331f4bc160e8291a8d2ff8`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 213.2 MB (213180476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab84fcf971d80a1b3e08f8415ad0ba35cbedb84cb7594ec24c79ad3dab44e84`  
		Last Modified: Tue, 04 Jul 2023 16:59:56 GMT  
		Size: 13.5 MB (13520290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc728f9cb60a83b4ab60b063840b0f84f5855805efe3fee682ef70cb18bb5`  
		Last Modified: Tue, 04 Jul 2023 16:59:54 GMT  
		Size: 458.3 KB (458274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a42d222d146900666c054ac1c165e03457150b661f1c20eb9a986adf4d2678`  
		Last Modified: Tue, 04 Jul 2023 17:00:23 GMT  
		Size: 278.5 MB (278468023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5156c18e6590cd36a4e4f59b32b52ef418667a3135e813115765772a34adf1a`  
		Last Modified: Tue, 04 Jul 2023 16:59:52 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506b322f0c562cb9aebf20161af21d5616174cc29a2966e2a2d9a1db65dbb722`  
		Last Modified: Tue, 04 Jul 2023 16:59:52 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de50af5eecc3c9b985c696efb3004d9afd15abc265fe45b109811e2cb805035d`  
		Last Modified: Tue, 04 Jul 2023 16:59:52 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c9ef420f6d91442c5d866fd4d642a88523a1fede003a97fea4d238c47fdf60`  
		Last Modified: Tue, 04 Jul 2023 16:59:52 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:381f35ec281791453fd64d7071724382b78714e2e942f773586dee03b677b7f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:96d93e66b824ede9752f189da16e13ed160409362cbf8c1d3203ff6843e4830a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.6 MB (561602709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea005d900fc2684f2227c023ff31c6fed616e3718f18f5ce44a712a573bc3ec8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:48:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:52:59 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:53:05 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:53:06 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:53:06 GMT
ENV ODOO_VERSION=15.0
# Tue, 04 Jul 2023 16:53:06 GMT
ARG ODOO_RELEASE=20230629
# Tue, 04 Jul 2023 16:53:06 GMT
ARG ODOO_SHA=0d61fc77caa30bb4687fe3418606581f29bbb6ae
# Tue, 04 Jul 2023 16:54:19 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=0d61fc77caa30bb4687fe3418606581f29bbb6ae
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 04 Jul 2023 16:54:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 04 Jul 2023 16:54:22 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 04 Jul 2023 16:54:22 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=0d61fc77caa30bb4687fe3418606581f29bbb6ae
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 04 Jul 2023 16:54:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 04 Jul 2023 16:54:23 GMT
EXPOSE 8069 8071 8072
# Tue, 04 Jul 2023 16:54:23 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 04 Jul 2023 16:54:23 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 04 Jul 2023 16:54:23 GMT
USER odoo
# Tue, 04 Jul 2023 16:54:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 16:54:23 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecec17eceb6c3674130e046a294357d03d0a4328163573bf205d3e3313a92b3`  
		Last Modified: Tue, 04 Jul 2023 16:59:33 GMT  
		Size: 220.3 MB (220302668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a3ff92d45f28abea1907822b9422b22044c4d8c3ea79cbbd890eedec7d2a2b`  
		Last Modified: Tue, 04 Jul 2023 16:59:09 GMT  
		Size: 2.6 MB (2576221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae451cd3af67981acb0b0f325d282607dfb4442750de0e5ef333d984e2ecae`  
		Last Modified: Tue, 04 Jul 2023 16:59:08 GMT  
		Size: 453.8 KB (453828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804d45ee74a68d0d6ec8bf9c6c4707fa975620fa6e8e86671ba12b90da86befc`  
		Last Modified: Tue, 04 Jul 2023 16:59:41 GMT  
		Size: 306.9 MB (306850143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20053c8659db7748f6f8a27341a65c322ff448e62805311b6f4e3b72c41d114f`  
		Last Modified: Tue, 04 Jul 2023 16:59:06 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ec76ea4a84c1df622a13a25651e40d81f91fc1041af661ba4d59d23127e1c2`  
		Last Modified: Tue, 04 Jul 2023 16:59:06 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86847c16cb8cb32d5f5503c9f547d469a38d21cc488237bdcd378caa94d1896f`  
		Last Modified: Tue, 04 Jul 2023 16:59:06 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f938d1ed8c42b3a30f5456df35bfdb8577cbbe8cff04a4effbbef18a95c1d918`  
		Last Modified: Tue, 04 Jul 2023 16:59:06 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:381f35ec281791453fd64d7071724382b78714e2e942f773586dee03b677b7f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:96d93e66b824ede9752f189da16e13ed160409362cbf8c1d3203ff6843e4830a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.6 MB (561602709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea005d900fc2684f2227c023ff31c6fed616e3718f18f5ce44a712a573bc3ec8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:48:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:52:59 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:53:05 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:53:06 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:53:06 GMT
ENV ODOO_VERSION=15.0
# Tue, 04 Jul 2023 16:53:06 GMT
ARG ODOO_RELEASE=20230629
# Tue, 04 Jul 2023 16:53:06 GMT
ARG ODOO_SHA=0d61fc77caa30bb4687fe3418606581f29bbb6ae
# Tue, 04 Jul 2023 16:54:19 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=0d61fc77caa30bb4687fe3418606581f29bbb6ae
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 04 Jul 2023 16:54:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 04 Jul 2023 16:54:22 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 04 Jul 2023 16:54:22 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=0d61fc77caa30bb4687fe3418606581f29bbb6ae
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 04 Jul 2023 16:54:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 04 Jul 2023 16:54:23 GMT
EXPOSE 8069 8071 8072
# Tue, 04 Jul 2023 16:54:23 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 04 Jul 2023 16:54:23 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 04 Jul 2023 16:54:23 GMT
USER odoo
# Tue, 04 Jul 2023 16:54:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 16:54:23 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecec17eceb6c3674130e046a294357d03d0a4328163573bf205d3e3313a92b3`  
		Last Modified: Tue, 04 Jul 2023 16:59:33 GMT  
		Size: 220.3 MB (220302668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a3ff92d45f28abea1907822b9422b22044c4d8c3ea79cbbd890eedec7d2a2b`  
		Last Modified: Tue, 04 Jul 2023 16:59:09 GMT  
		Size: 2.6 MB (2576221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae451cd3af67981acb0b0f325d282607dfb4442750de0e5ef333d984e2ecae`  
		Last Modified: Tue, 04 Jul 2023 16:59:08 GMT  
		Size: 453.8 KB (453828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804d45ee74a68d0d6ec8bf9c6c4707fa975620fa6e8e86671ba12b90da86befc`  
		Last Modified: Tue, 04 Jul 2023 16:59:41 GMT  
		Size: 306.9 MB (306850143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20053c8659db7748f6f8a27341a65c322ff448e62805311b6f4e3b72c41d114f`  
		Last Modified: Tue, 04 Jul 2023 16:59:06 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ec76ea4a84c1df622a13a25651e40d81f91fc1041af661ba4d59d23127e1c2`  
		Last Modified: Tue, 04 Jul 2023 16:59:06 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86847c16cb8cb32d5f5503c9f547d469a38d21cc488237bdcd378caa94d1896f`  
		Last Modified: Tue, 04 Jul 2023 16:59:06 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f938d1ed8c42b3a30f5456df35bfdb8577cbbe8cff04a4effbbef18a95c1d918`  
		Last Modified: Tue, 04 Jul 2023 16:59:06 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:3aa97f01110e533fab6580c1a987046c98a10e4b798b2baf6cb848a526f53fc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:8e8df096eb391f96fd3b1e51fa00a7720532ae8811c2aaff442bb0d609a8264f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.0 MB (573033394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40718f7a7eee51656289a628eb9d59f54bcf96033d6962351b34b17bdeaf80cd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:48:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:50:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:50:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:50:14 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:50:14 GMT
ENV ODOO_VERSION=16.0
# Tue, 04 Jul 2023 16:50:14 GMT
ARG ODOO_RELEASE=20230629
# Tue, 04 Jul 2023 16:50:14 GMT
ARG ODOO_SHA=ef1a7436be87a897efa0d0b4a50a159d2ee3e1e3
# Tue, 04 Jul 2023 16:51:46 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=ef1a7436be87a897efa0d0b4a50a159d2ee3e1e3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 04 Jul 2023 16:51:51 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 04 Jul 2023 16:51:51 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 04 Jul 2023 16:51:52 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=ef1a7436be87a897efa0d0b4a50a159d2ee3e1e3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 04 Jul 2023 16:51:52 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 04 Jul 2023 16:51:52 GMT
EXPOSE 8069 8071 8072
# Tue, 04 Jul 2023 16:51:52 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 04 Jul 2023 16:51:52 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 04 Jul 2023 16:51:52 GMT
USER odoo
# Tue, 04 Jul 2023 16:51:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 16:51:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c7d3da2fbd2d726a8fe59c3992de7895dd89fadab551a495625fa48e8c5e7`  
		Last Modified: Tue, 04 Jul 2023 16:58:45 GMT  
		Size: 221.0 MB (220991764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd6f861e7cdc6a59484c202dc889a03e05ccea95d4463d5151d5d4d453f418b`  
		Last Modified: Tue, 04 Jul 2023 16:58:21 GMT  
		Size: 2.6 MB (2579607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9919e5999fecf8a9ca11971e06d8a9e2cd6d34b66814734d1133fa1a15c18974`  
		Last Modified: Tue, 04 Jul 2023 16:58:20 GMT  
		Size: 453.8 KB (453840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72b80784b1819dcb26ff4ac23fd0e981e5b59daeb96bc2eb173ef7a97521e47`  
		Last Modified: Tue, 04 Jul 2023 16:58:54 GMT  
		Size: 317.6 MB (317588331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0918cc5e4fe4444ba313877471573928ff73d6eb08c566e4bf1a64b5fe9d5c5c`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890d52ab2feccdb1b6a5a157fc44b5b8dc6c10da6a4d773e0852f44dbe00858d`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdf0cb1de4095f820f4c8c8efceb14c92129cdbe45aa9cdd593dca9fd07a7b8`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37189b96bd4dc00a49598b397f12db3b2b04922f15cafe76bbfda6c47a53d211`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:3aa97f01110e533fab6580c1a987046c98a10e4b798b2baf6cb848a526f53fc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:8e8df096eb391f96fd3b1e51fa00a7720532ae8811c2aaff442bb0d609a8264f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.0 MB (573033394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40718f7a7eee51656289a628eb9d59f54bcf96033d6962351b34b17bdeaf80cd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:48:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:50:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:50:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:50:14 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:50:14 GMT
ENV ODOO_VERSION=16.0
# Tue, 04 Jul 2023 16:50:14 GMT
ARG ODOO_RELEASE=20230629
# Tue, 04 Jul 2023 16:50:14 GMT
ARG ODOO_SHA=ef1a7436be87a897efa0d0b4a50a159d2ee3e1e3
# Tue, 04 Jul 2023 16:51:46 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=ef1a7436be87a897efa0d0b4a50a159d2ee3e1e3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 04 Jul 2023 16:51:51 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 04 Jul 2023 16:51:51 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 04 Jul 2023 16:51:52 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=ef1a7436be87a897efa0d0b4a50a159d2ee3e1e3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 04 Jul 2023 16:51:52 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 04 Jul 2023 16:51:52 GMT
EXPOSE 8069 8071 8072
# Tue, 04 Jul 2023 16:51:52 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 04 Jul 2023 16:51:52 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 04 Jul 2023 16:51:52 GMT
USER odoo
# Tue, 04 Jul 2023 16:51:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 16:51:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c7d3da2fbd2d726a8fe59c3992de7895dd89fadab551a495625fa48e8c5e7`  
		Last Modified: Tue, 04 Jul 2023 16:58:45 GMT  
		Size: 221.0 MB (220991764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd6f861e7cdc6a59484c202dc889a03e05ccea95d4463d5151d5d4d453f418b`  
		Last Modified: Tue, 04 Jul 2023 16:58:21 GMT  
		Size: 2.6 MB (2579607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9919e5999fecf8a9ca11971e06d8a9e2cd6d34b66814734d1133fa1a15c18974`  
		Last Modified: Tue, 04 Jul 2023 16:58:20 GMT  
		Size: 453.8 KB (453840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72b80784b1819dcb26ff4ac23fd0e981e5b59daeb96bc2eb173ef7a97521e47`  
		Last Modified: Tue, 04 Jul 2023 16:58:54 GMT  
		Size: 317.6 MB (317588331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0918cc5e4fe4444ba313877471573928ff73d6eb08c566e4bf1a64b5fe9d5c5c`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890d52ab2feccdb1b6a5a157fc44b5b8dc6c10da6a4d773e0852f44dbe00858d`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdf0cb1de4095f820f4c8c8efceb14c92129cdbe45aa9cdd593dca9fd07a7b8`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37189b96bd4dc00a49598b397f12db3b2b04922f15cafe76bbfda6c47a53d211`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:3aa97f01110e533fab6580c1a987046c98a10e4b798b2baf6cb848a526f53fc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:8e8df096eb391f96fd3b1e51fa00a7720532ae8811c2aaff442bb0d609a8264f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.0 MB (573033394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40718f7a7eee51656289a628eb9d59f54bcf96033d6962351b34b17bdeaf80cd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:48:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:50:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:50:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:50:14 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:50:14 GMT
ENV ODOO_VERSION=16.0
# Tue, 04 Jul 2023 16:50:14 GMT
ARG ODOO_RELEASE=20230629
# Tue, 04 Jul 2023 16:50:14 GMT
ARG ODOO_SHA=ef1a7436be87a897efa0d0b4a50a159d2ee3e1e3
# Tue, 04 Jul 2023 16:51:46 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=ef1a7436be87a897efa0d0b4a50a159d2ee3e1e3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 04 Jul 2023 16:51:51 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 04 Jul 2023 16:51:51 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 04 Jul 2023 16:51:52 GMT
# ARGS: ODOO_RELEASE=20230629 ODOO_SHA=ef1a7436be87a897efa0d0b4a50a159d2ee3e1e3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 04 Jul 2023 16:51:52 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 04 Jul 2023 16:51:52 GMT
EXPOSE 8069 8071 8072
# Tue, 04 Jul 2023 16:51:52 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 04 Jul 2023 16:51:52 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 04 Jul 2023 16:51:52 GMT
USER odoo
# Tue, 04 Jul 2023 16:51:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 16:51:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c7d3da2fbd2d726a8fe59c3992de7895dd89fadab551a495625fa48e8c5e7`  
		Last Modified: Tue, 04 Jul 2023 16:58:45 GMT  
		Size: 221.0 MB (220991764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd6f861e7cdc6a59484c202dc889a03e05ccea95d4463d5151d5d4d453f418b`  
		Last Modified: Tue, 04 Jul 2023 16:58:21 GMT  
		Size: 2.6 MB (2579607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9919e5999fecf8a9ca11971e06d8a9e2cd6d34b66814734d1133fa1a15c18974`  
		Last Modified: Tue, 04 Jul 2023 16:58:20 GMT  
		Size: 453.8 KB (453840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72b80784b1819dcb26ff4ac23fd0e981e5b59daeb96bc2eb173ef7a97521e47`  
		Last Modified: Tue, 04 Jul 2023 16:58:54 GMT  
		Size: 317.6 MB (317588331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0918cc5e4fe4444ba313877471573928ff73d6eb08c566e4bf1a64b5fe9d5c5c`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890d52ab2feccdb1b6a5a157fc44b5b8dc6c10da6a4d773e0852f44dbe00858d`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdf0cb1de4095f820f4c8c8efceb14c92129cdbe45aa9cdd593dca9fd07a7b8`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37189b96bd4dc00a49598b397f12db3b2b04922f15cafe76bbfda6c47a53d211`  
		Last Modified: Tue, 04 Jul 2023 16:58:18 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
