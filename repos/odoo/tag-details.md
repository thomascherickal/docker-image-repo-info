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
$ docker pull odoo@sha256:26e11e955c884495762bb9428382f423ef4eb6217477dd9aea21ddcddb5bcba0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:6604dd9af2d4e86e143c7e8303cf24c58be32877117ad2ee46428d6e0247df6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.3 MB (531296938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b1af9ba66b082f131d048ebab1b64b32f21dc6ac65b7f0c3c73cc6dc6ab630`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:59:39 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 06 Dec 2022 04:59:39 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 06 Dec 2022 04:59:39 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 05:01:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 06 Dec 2022 05:01:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 05:01:20 GMT
RUN npm install -g rtlcss
# Tue, 06 Dec 2022 05:01:20 GMT
ENV ODOO_VERSION=14.0
# Fri, 16 Dec 2022 18:23:04 GMT
ARG ODOO_RELEASE=20221216
# Fri, 16 Dec 2022 18:23:04 GMT
ARG ODOO_SHA=cf0fc33d169a845691b71cc03cfbaa7787b20b04
# Fri, 16 Dec 2022 18:24:28 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=cf0fc33d169a845691b71cc03cfbaa7787b20b04
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 16 Dec 2022 18:24:32 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 16 Dec 2022 18:24:32 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 16 Dec 2022 18:24:33 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=cf0fc33d169a845691b71cc03cfbaa7787b20b04
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 16 Dec 2022 18:24:33 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 16 Dec 2022 18:24:33 GMT
EXPOSE 8069 8071 8072
# Fri, 16 Dec 2022 18:24:33 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 16 Dec 2022 18:24:33 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 16 Dec 2022 18:24:33 GMT
USER odoo
# Fri, 16 Dec 2022 18:24:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 18:24:34 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af30673d5a4116eb1f89960ac4d2b3cae0170f811e374c73a5df8208d6f7500`  
		Last Modified: Tue, 06 Dec 2022 05:04:59 GMT  
		Size: 213.2 MB (213186295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4381f1f9a7360d0508554e5175276e416035990ce6573d412b392d4b800fd0b1`  
		Last Modified: Tue, 06 Dec 2022 05:04:37 GMT  
		Size: 13.5 MB (13515336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d93c08705e82f4f5007ec163c3c518f76d8dd974b4b62d5b1f844f2dc08b9a1`  
		Last Modified: Tue, 06 Dec 2022 05:04:35 GMT  
		Size: 454.3 KB (454349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbdfa25775ed23ae1f30d39c4766955af0ffec4c6c714a6c28c27365bd7628`  
		Last Modified: Fri, 16 Dec 2022 18:27:43 GMT  
		Size: 277.0 MB (276998142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d44a56fe1a1511a1539770b7743e49868d31cb4be7de91f176e845bda05e4e`  
		Last Modified: Fri, 16 Dec 2022 18:27:11 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4f1be906a2b357e0a86ae72e47042aa63fe045e11abf527517b4e4cf69774e`  
		Last Modified: Fri, 16 Dec 2022 18:27:11 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d55ff8e524767f9ad5bbdd65fe10b4a5967a05495620dae37440bde6073b98c`  
		Last Modified: Fri, 16 Dec 2022 18:27:11 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7b47f2825739523bf79b5b45afdb6b4c9c413e88053904954eefe95b71bbf2`  
		Last Modified: Fri, 16 Dec 2022 18:27:11 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:26e11e955c884495762bb9428382f423ef4eb6217477dd9aea21ddcddb5bcba0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:6604dd9af2d4e86e143c7e8303cf24c58be32877117ad2ee46428d6e0247df6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.3 MB (531296938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b1af9ba66b082f131d048ebab1b64b32f21dc6ac65b7f0c3c73cc6dc6ab630`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:59:39 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 06 Dec 2022 04:59:39 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 06 Dec 2022 04:59:39 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 05:01:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 06 Dec 2022 05:01:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 05:01:20 GMT
RUN npm install -g rtlcss
# Tue, 06 Dec 2022 05:01:20 GMT
ENV ODOO_VERSION=14.0
# Fri, 16 Dec 2022 18:23:04 GMT
ARG ODOO_RELEASE=20221216
# Fri, 16 Dec 2022 18:23:04 GMT
ARG ODOO_SHA=cf0fc33d169a845691b71cc03cfbaa7787b20b04
# Fri, 16 Dec 2022 18:24:28 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=cf0fc33d169a845691b71cc03cfbaa7787b20b04
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 16 Dec 2022 18:24:32 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 16 Dec 2022 18:24:32 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 16 Dec 2022 18:24:33 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=cf0fc33d169a845691b71cc03cfbaa7787b20b04
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 16 Dec 2022 18:24:33 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 16 Dec 2022 18:24:33 GMT
EXPOSE 8069 8071 8072
# Fri, 16 Dec 2022 18:24:33 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 16 Dec 2022 18:24:33 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 16 Dec 2022 18:24:33 GMT
USER odoo
# Fri, 16 Dec 2022 18:24:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 18:24:34 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af30673d5a4116eb1f89960ac4d2b3cae0170f811e374c73a5df8208d6f7500`  
		Last Modified: Tue, 06 Dec 2022 05:04:59 GMT  
		Size: 213.2 MB (213186295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4381f1f9a7360d0508554e5175276e416035990ce6573d412b392d4b800fd0b1`  
		Last Modified: Tue, 06 Dec 2022 05:04:37 GMT  
		Size: 13.5 MB (13515336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d93c08705e82f4f5007ec163c3c518f76d8dd974b4b62d5b1f844f2dc08b9a1`  
		Last Modified: Tue, 06 Dec 2022 05:04:35 GMT  
		Size: 454.3 KB (454349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbdfa25775ed23ae1f30d39c4766955af0ffec4c6c714a6c28c27365bd7628`  
		Last Modified: Fri, 16 Dec 2022 18:27:43 GMT  
		Size: 277.0 MB (276998142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d44a56fe1a1511a1539770b7743e49868d31cb4be7de91f176e845bda05e4e`  
		Last Modified: Fri, 16 Dec 2022 18:27:11 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4f1be906a2b357e0a86ae72e47042aa63fe045e11abf527517b4e4cf69774e`  
		Last Modified: Fri, 16 Dec 2022 18:27:11 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d55ff8e524767f9ad5bbdd65fe10b4a5967a05495620dae37440bde6073b98c`  
		Last Modified: Fri, 16 Dec 2022 18:27:11 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7b47f2825739523bf79b5b45afdb6b4c9c413e88053904954eefe95b71bbf2`  
		Last Modified: Fri, 16 Dec 2022 18:27:11 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:a252743851e10ba4945f29f14284345be49edb36d537cde39b5e4a5302075342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:f9411b1dfa1662b4d9ae0c7471c62efa893d046292af6229b7097ba424c0496f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **559.3 MB (559326530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfeee7929ab569d1a0b1119838a07d740fb48667247700c2bb9dbcaa7e89ddf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:54:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 06 Dec 2022 04:54:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 06 Dec 2022 04:54:53 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 04:56:06 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 06 Dec 2022 04:56:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:56:17 GMT
RUN npm install -g rtlcss
# Tue, 06 Dec 2022 04:58:01 GMT
ENV ODOO_VERSION=15.0
# Fri, 16 Dec 2022 18:21:41 GMT
ARG ODOO_RELEASE=20221216
# Fri, 16 Dec 2022 18:21:41 GMT
ARG ODOO_SHA=db18fade18d691716ccb67ddbd583e288d4762be
# Fri, 16 Dec 2022 18:22:56 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=db18fade18d691716ccb67ddbd583e288d4762be
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 16 Dec 2022 18:23:00 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 16 Dec 2022 18:23:00 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 16 Dec 2022 18:23:01 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=db18fade18d691716ccb67ddbd583e288d4762be
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 16 Dec 2022 18:23:01 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 16 Dec 2022 18:23:01 GMT
EXPOSE 8069 8071 8072
# Fri, 16 Dec 2022 18:23:01 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 16 Dec 2022 18:23:01 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 16 Dec 2022 18:23:01 GMT
USER odoo
# Fri, 16 Dec 2022 18:23:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 18:23:02 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62d2d2e9280928e4c397ed19ec2b4af396124dfbfd06a0b8372f1df0dac2a7`  
		Last Modified: Tue, 06 Dec 2022 05:03:27 GMT  
		Size: 220.3 MB (220299260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529c7b2aaceeff3cca4d4068174375f09342ade1bbd073db1f28665e5330d97d`  
		Last Modified: Tue, 06 Dec 2022 05:03:00 GMT  
		Size: 2.6 MB (2574808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9299a7ee5c1f3e4ed14ed62e0b9d5bb4a94ba7342c4352ad7e967a16b6c2c653`  
		Last Modified: Tue, 06 Dec 2022 05:03:00 GMT  
		Size: 450.3 KB (450264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af7e752039e3def9ce7b9ed3ad4942da8e22b024f6284d27770dcbf36db1414`  
		Last Modified: Fri, 16 Dec 2022 18:26:47 GMT  
		Size: 304.6 MB (304586880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a45f025ba060836230ed1cc869effd6452f862354d119474503c8925c900b1`  
		Last Modified: Fri, 16 Dec 2022 18:26:12 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16004e5f7248481762ebf26e59c95c6561b18da8818eb9933815425ce838c26`  
		Last Modified: Fri, 16 Dec 2022 18:26:12 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038bb27ec569662f14ceeff48eed65e797eca752ee5a6ebeb9c1bdd7b4a1ee1b`  
		Last Modified: Fri, 16 Dec 2022 18:26:12 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a93838c579d97df117f0889dbabe630dd4f7e7ed869e0e34680d24ffa6976`  
		Last Modified: Fri, 16 Dec 2022 18:26:12 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:a252743851e10ba4945f29f14284345be49edb36d537cde39b5e4a5302075342
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:f9411b1dfa1662b4d9ae0c7471c62efa893d046292af6229b7097ba424c0496f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **559.3 MB (559326530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfeee7929ab569d1a0b1119838a07d740fb48667247700c2bb9dbcaa7e89ddf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:54:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 06 Dec 2022 04:54:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 06 Dec 2022 04:54:53 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 04:56:06 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 06 Dec 2022 04:56:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:56:17 GMT
RUN npm install -g rtlcss
# Tue, 06 Dec 2022 04:58:01 GMT
ENV ODOO_VERSION=15.0
# Fri, 16 Dec 2022 18:21:41 GMT
ARG ODOO_RELEASE=20221216
# Fri, 16 Dec 2022 18:21:41 GMT
ARG ODOO_SHA=db18fade18d691716ccb67ddbd583e288d4762be
# Fri, 16 Dec 2022 18:22:56 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=db18fade18d691716ccb67ddbd583e288d4762be
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 16 Dec 2022 18:23:00 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 16 Dec 2022 18:23:00 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 16 Dec 2022 18:23:01 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=db18fade18d691716ccb67ddbd583e288d4762be
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 16 Dec 2022 18:23:01 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 16 Dec 2022 18:23:01 GMT
EXPOSE 8069 8071 8072
# Fri, 16 Dec 2022 18:23:01 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 16 Dec 2022 18:23:01 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 16 Dec 2022 18:23:01 GMT
USER odoo
# Fri, 16 Dec 2022 18:23:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 18:23:02 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62d2d2e9280928e4c397ed19ec2b4af396124dfbfd06a0b8372f1df0dac2a7`  
		Last Modified: Tue, 06 Dec 2022 05:03:27 GMT  
		Size: 220.3 MB (220299260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529c7b2aaceeff3cca4d4068174375f09342ade1bbd073db1f28665e5330d97d`  
		Last Modified: Tue, 06 Dec 2022 05:03:00 GMT  
		Size: 2.6 MB (2574808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9299a7ee5c1f3e4ed14ed62e0b9d5bb4a94ba7342c4352ad7e967a16b6c2c653`  
		Last Modified: Tue, 06 Dec 2022 05:03:00 GMT  
		Size: 450.3 KB (450264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af7e752039e3def9ce7b9ed3ad4942da8e22b024f6284d27770dcbf36db1414`  
		Last Modified: Fri, 16 Dec 2022 18:26:47 GMT  
		Size: 304.6 MB (304586880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a45f025ba060836230ed1cc869effd6452f862354d119474503c8925c900b1`  
		Last Modified: Fri, 16 Dec 2022 18:26:12 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16004e5f7248481762ebf26e59c95c6561b18da8818eb9933815425ce838c26`  
		Last Modified: Fri, 16 Dec 2022 18:26:12 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038bb27ec569662f14ceeff48eed65e797eca752ee5a6ebeb9c1bdd7b4a1ee1b`  
		Last Modified: Fri, 16 Dec 2022 18:26:12 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9a93838c579d97df117f0889dbabe630dd4f7e7ed869e0e34680d24ffa6976`  
		Last Modified: Fri, 16 Dec 2022 18:26:12 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:d0343c30b9e153dfadcb74aab7e408c1d61319aa103a8c31a7b46db6c08b1f1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:81d8fa6a60a0959d17eea2f112b33742d30022fb8b4d5d1478b985cb3f8eea4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.4 MB (562359667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef0f861ad9ff0fb09b809dec7ed5487f5b83c8cfeb0d4633af43fce6379b929`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:54:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 06 Dec 2022 04:54:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 06 Dec 2022 04:54:53 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 04:56:06 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 06 Dec 2022 04:56:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:56:17 GMT
RUN npm install -g rtlcss
# Tue, 06 Dec 2022 04:56:17 GMT
ENV ODOO_VERSION=16.0
# Fri, 16 Dec 2022 18:20:02 GMT
ARG ODOO_RELEASE=20221216
# Fri, 16 Dec 2022 18:20:03 GMT
ARG ODOO_SHA=f6aeed95ae4fe3c891fe7c35e0dc08e83553493d
# Fri, 16 Dec 2022 18:21:32 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=f6aeed95ae4fe3c891fe7c35e0dc08e83553493d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 16 Dec 2022 18:21:36 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 16 Dec 2022 18:21:36 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 16 Dec 2022 18:21:37 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=f6aeed95ae4fe3c891fe7c35e0dc08e83553493d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 16 Dec 2022 18:21:37 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 16 Dec 2022 18:21:37 GMT
EXPOSE 8069 8071 8072
# Fri, 16 Dec 2022 18:21:37 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 16 Dec 2022 18:21:37 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 16 Dec 2022 18:21:37 GMT
USER odoo
# Fri, 16 Dec 2022 18:21:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 18:21:38 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62d2d2e9280928e4c397ed19ec2b4af396124dfbfd06a0b8372f1df0dac2a7`  
		Last Modified: Tue, 06 Dec 2022 05:03:27 GMT  
		Size: 220.3 MB (220299260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529c7b2aaceeff3cca4d4068174375f09342ade1bbd073db1f28665e5330d97d`  
		Last Modified: Tue, 06 Dec 2022 05:03:00 GMT  
		Size: 2.6 MB (2574808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9299a7ee5c1f3e4ed14ed62e0b9d5bb4a94ba7342c4352ad7e967a16b6c2c653`  
		Last Modified: Tue, 06 Dec 2022 05:03:00 GMT  
		Size: 450.3 KB (450264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1208939ca11e8d8cf308e59aed315dd2584246a633329aef6c9498e7655553`  
		Last Modified: Fri, 16 Dec 2022 18:25:55 GMT  
		Size: 307.6 MB (307620017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05dd3e7a53864178dec548e15beb022834a0c8c21daf7a2450658c1714521a`  
		Last Modified: Fri, 16 Dec 2022 18:25:20 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1e0d67420599088f2ebd4d629a9b58edf9266c70e398475669ae18a5f698a8`  
		Last Modified: Fri, 16 Dec 2022 18:25:20 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c023f2e6cd84218282fe73fb42c85a55a4280f0758dedb6971c1c1b72e3eaa9b`  
		Last Modified: Fri, 16 Dec 2022 18:25:20 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3883472ed2e332f1b42130d6eae08bbabb231f387b58f15b950da9ebaa5c8bb9`  
		Last Modified: Fri, 16 Dec 2022 18:25:23 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:d0343c30b9e153dfadcb74aab7e408c1d61319aa103a8c31a7b46db6c08b1f1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:81d8fa6a60a0959d17eea2f112b33742d30022fb8b4d5d1478b985cb3f8eea4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.4 MB (562359667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef0f861ad9ff0fb09b809dec7ed5487f5b83c8cfeb0d4633af43fce6379b929`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:54:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 06 Dec 2022 04:54:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 06 Dec 2022 04:54:53 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 04:56:06 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 06 Dec 2022 04:56:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:56:17 GMT
RUN npm install -g rtlcss
# Tue, 06 Dec 2022 04:56:17 GMT
ENV ODOO_VERSION=16.0
# Fri, 16 Dec 2022 18:20:02 GMT
ARG ODOO_RELEASE=20221216
# Fri, 16 Dec 2022 18:20:03 GMT
ARG ODOO_SHA=f6aeed95ae4fe3c891fe7c35e0dc08e83553493d
# Fri, 16 Dec 2022 18:21:32 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=f6aeed95ae4fe3c891fe7c35e0dc08e83553493d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 16 Dec 2022 18:21:36 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 16 Dec 2022 18:21:36 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 16 Dec 2022 18:21:37 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=f6aeed95ae4fe3c891fe7c35e0dc08e83553493d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 16 Dec 2022 18:21:37 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 16 Dec 2022 18:21:37 GMT
EXPOSE 8069 8071 8072
# Fri, 16 Dec 2022 18:21:37 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 16 Dec 2022 18:21:37 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 16 Dec 2022 18:21:37 GMT
USER odoo
# Fri, 16 Dec 2022 18:21:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 18:21:38 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62d2d2e9280928e4c397ed19ec2b4af396124dfbfd06a0b8372f1df0dac2a7`  
		Last Modified: Tue, 06 Dec 2022 05:03:27 GMT  
		Size: 220.3 MB (220299260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529c7b2aaceeff3cca4d4068174375f09342ade1bbd073db1f28665e5330d97d`  
		Last Modified: Tue, 06 Dec 2022 05:03:00 GMT  
		Size: 2.6 MB (2574808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9299a7ee5c1f3e4ed14ed62e0b9d5bb4a94ba7342c4352ad7e967a16b6c2c653`  
		Last Modified: Tue, 06 Dec 2022 05:03:00 GMT  
		Size: 450.3 KB (450264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1208939ca11e8d8cf308e59aed315dd2584246a633329aef6c9498e7655553`  
		Last Modified: Fri, 16 Dec 2022 18:25:55 GMT  
		Size: 307.6 MB (307620017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05dd3e7a53864178dec548e15beb022834a0c8c21daf7a2450658c1714521a`  
		Last Modified: Fri, 16 Dec 2022 18:25:20 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1e0d67420599088f2ebd4d629a9b58edf9266c70e398475669ae18a5f698a8`  
		Last Modified: Fri, 16 Dec 2022 18:25:20 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c023f2e6cd84218282fe73fb42c85a55a4280f0758dedb6971c1c1b72e3eaa9b`  
		Last Modified: Fri, 16 Dec 2022 18:25:20 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3883472ed2e332f1b42130d6eae08bbabb231f387b58f15b950da9ebaa5c8bb9`  
		Last Modified: Fri, 16 Dec 2022 18:25:23 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:d0343c30b9e153dfadcb74aab7e408c1d61319aa103a8c31a7b46db6c08b1f1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:81d8fa6a60a0959d17eea2f112b33742d30022fb8b4d5d1478b985cb3f8eea4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.4 MB (562359667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef0f861ad9ff0fb09b809dec7ed5487f5b83c8cfeb0d4633af43fce6379b929`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:54:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 06 Dec 2022 04:54:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 06 Dec 2022 04:54:53 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 04:56:06 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 06 Dec 2022 04:56:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 04:56:17 GMT
RUN npm install -g rtlcss
# Tue, 06 Dec 2022 04:56:17 GMT
ENV ODOO_VERSION=16.0
# Fri, 16 Dec 2022 18:20:02 GMT
ARG ODOO_RELEASE=20221216
# Fri, 16 Dec 2022 18:20:03 GMT
ARG ODOO_SHA=f6aeed95ae4fe3c891fe7c35e0dc08e83553493d
# Fri, 16 Dec 2022 18:21:32 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=f6aeed95ae4fe3c891fe7c35e0dc08e83553493d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 16 Dec 2022 18:21:36 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 16 Dec 2022 18:21:36 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 16 Dec 2022 18:21:37 GMT
# ARGS: ODOO_RELEASE=20221216 ODOO_SHA=f6aeed95ae4fe3c891fe7c35e0dc08e83553493d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 16 Dec 2022 18:21:37 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 16 Dec 2022 18:21:37 GMT
EXPOSE 8069 8071 8072
# Fri, 16 Dec 2022 18:21:37 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 16 Dec 2022 18:21:37 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 16 Dec 2022 18:21:37 GMT
USER odoo
# Fri, 16 Dec 2022 18:21:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 16 Dec 2022 18:21:38 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62d2d2e9280928e4c397ed19ec2b4af396124dfbfd06a0b8372f1df0dac2a7`  
		Last Modified: Tue, 06 Dec 2022 05:03:27 GMT  
		Size: 220.3 MB (220299260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529c7b2aaceeff3cca4d4068174375f09342ade1bbd073db1f28665e5330d97d`  
		Last Modified: Tue, 06 Dec 2022 05:03:00 GMT  
		Size: 2.6 MB (2574808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9299a7ee5c1f3e4ed14ed62e0b9d5bb4a94ba7342c4352ad7e967a16b6c2c653`  
		Last Modified: Tue, 06 Dec 2022 05:03:00 GMT  
		Size: 450.3 KB (450264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1208939ca11e8d8cf308e59aed315dd2584246a633329aef6c9498e7655553`  
		Last Modified: Fri, 16 Dec 2022 18:25:55 GMT  
		Size: 307.6 MB (307620017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e05dd3e7a53864178dec548e15beb022834a0c8c21daf7a2450658c1714521a`  
		Last Modified: Fri, 16 Dec 2022 18:25:20 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1e0d67420599088f2ebd4d629a9b58edf9266c70e398475669ae18a5f698a8`  
		Last Modified: Fri, 16 Dec 2022 18:25:20 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c023f2e6cd84218282fe73fb42c85a55a4280f0758dedb6971c1c1b72e3eaa9b`  
		Last Modified: Fri, 16 Dec 2022 18:25:20 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3883472ed2e332f1b42130d6eae08bbabb231f387b58f15b950da9ebaa5c8bb9`  
		Last Modified: Fri, 16 Dec 2022 18:25:23 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
