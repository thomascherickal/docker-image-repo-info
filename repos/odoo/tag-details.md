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
$ docker pull odoo@sha256:7973e5cd6b1a18dfde56d644bb44b9b1b0839344a466f80562990f46895530be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:73091efa7985cb37ba5777548a9c2fd98ddda4f9b574dd81dc800c8a15f57672
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.2 MB (531217379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c46b9f4fc34538238f4c7dbbd4d1358f2b56a616fb9b457fadd889ef88a4b`
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
# Tue, 06 Dec 2022 05:01:21 GMT
ARG ODOO_RELEASE=20221202
# Tue, 06 Dec 2022 05:01:21 GMT
ARG ODOO_SHA=41a75eecbf06b0adfc5537a476e406d28557f938
# Tue, 06 Dec 2022 05:02:38 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=41a75eecbf06b0adfc5537a476e406d28557f938
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 06 Dec 2022 05:02:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 06 Dec 2022 05:02:42 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 06 Dec 2022 05:02:43 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=41a75eecbf06b0adfc5537a476e406d28557f938
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 06 Dec 2022 05:02:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 06 Dec 2022 05:02:43 GMT
EXPOSE 8069 8071 8072
# Tue, 06 Dec 2022 05:02:43 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 06 Dec 2022 05:02:43 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 06 Dec 2022 05:02:44 GMT
USER odoo
# Tue, 06 Dec 2022 05:02:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 05:02:44 GMT
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
	-	`sha256:0950f75689acfcea781f7824cd0eb3bfe1b257c8b2c658fa4676eb42c5d2ed98`  
		Last Modified: Tue, 06 Dec 2022 05:05:07 GMT  
		Size: 276.9 MB (276918582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c445b2b448acba07bbc318cb96b3a846b76c322dff2a7a33aa243bb005e01c28`  
		Last Modified: Tue, 06 Dec 2022 05:04:33 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4959a599db4c2166530a56f76019aa4b0b5e11243655307a6a3159f6a346ced`  
		Last Modified: Tue, 06 Dec 2022 05:04:33 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc34efd4b9767caa94b0da275c0b5f0af1563ad366dd696b5ec64ee284568921`  
		Last Modified: Tue, 06 Dec 2022 05:04:33 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab699306c821ea5acffbf41e67495af54ff7b5c0a0a7da20cd0fdb72bbf83d2`  
		Last Modified: Tue, 06 Dec 2022 05:04:33 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:7973e5cd6b1a18dfde56d644bb44b9b1b0839344a466f80562990f46895530be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:73091efa7985cb37ba5777548a9c2fd98ddda4f9b574dd81dc800c8a15f57672
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.2 MB (531217379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c46b9f4fc34538238f4c7dbbd4d1358f2b56a616fb9b457fadd889ef88a4b`
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
# Tue, 06 Dec 2022 05:01:21 GMT
ARG ODOO_RELEASE=20221202
# Tue, 06 Dec 2022 05:01:21 GMT
ARG ODOO_SHA=41a75eecbf06b0adfc5537a476e406d28557f938
# Tue, 06 Dec 2022 05:02:38 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=41a75eecbf06b0adfc5537a476e406d28557f938
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 06 Dec 2022 05:02:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 06 Dec 2022 05:02:42 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 06 Dec 2022 05:02:43 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=41a75eecbf06b0adfc5537a476e406d28557f938
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 06 Dec 2022 05:02:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 06 Dec 2022 05:02:43 GMT
EXPOSE 8069 8071 8072
# Tue, 06 Dec 2022 05:02:43 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 06 Dec 2022 05:02:43 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 06 Dec 2022 05:02:44 GMT
USER odoo
# Tue, 06 Dec 2022 05:02:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 05:02:44 GMT
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
	-	`sha256:0950f75689acfcea781f7824cd0eb3bfe1b257c8b2c658fa4676eb42c5d2ed98`  
		Last Modified: Tue, 06 Dec 2022 05:05:07 GMT  
		Size: 276.9 MB (276918582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c445b2b448acba07bbc318cb96b3a846b76c322dff2a7a33aa243bb005e01c28`  
		Last Modified: Tue, 06 Dec 2022 05:04:33 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4959a599db4c2166530a56f76019aa4b0b5e11243655307a6a3159f6a346ced`  
		Last Modified: Tue, 06 Dec 2022 05:04:33 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc34efd4b9767caa94b0da275c0b5f0af1563ad366dd696b5ec64ee284568921`  
		Last Modified: Tue, 06 Dec 2022 05:04:33 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab699306c821ea5acffbf41e67495af54ff7b5c0a0a7da20cd0fdb72bbf83d2`  
		Last Modified: Tue, 06 Dec 2022 05:04:33 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:f62d3c80552a8f3ae5f405d9bc418531f39aa811fc9ac727c3a1568e2cbfe0d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:2de369c9b6fee6c4040425471794b3afd44b63353c8f9299e8040fff762c9eb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **559.3 MB (559254989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f5c4e280ad234af379eacbb574965c2abc1fbf37611b2bd08b89beeab755754`
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
# Tue, 06 Dec 2022 04:58:01 GMT
ARG ODOO_RELEASE=20221202
# Tue, 06 Dec 2022 04:58:01 GMT
ARG ODOO_SHA=d0ee50281624260267085ee90302d1fe422eebbb
# Tue, 06 Dec 2022 04:59:18 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=d0ee50281624260267085ee90302d1fe422eebbb
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 06 Dec 2022 04:59:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 06 Dec 2022 04:59:22 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 06 Dec 2022 04:59:23 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=d0ee50281624260267085ee90302d1fe422eebbb
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 06 Dec 2022 04:59:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 06 Dec 2022 04:59:23 GMT
EXPOSE 8069 8071 8072
# Tue, 06 Dec 2022 04:59:23 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 06 Dec 2022 04:59:23 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 06 Dec 2022 04:59:23 GMT
USER odoo
# Tue, 06 Dec 2022 04:59:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 04:59:23 GMT
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
	-	`sha256:a3d76906584144f2b5150ca0de429bfc0ed011c89c4cbc0ad89427d7ab78d8f5`  
		Last Modified: Tue, 06 Dec 2022 05:04:23 GMT  
		Size: 304.5 MB (304515345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c074368a724a96e4e302f687a42f2828dae044d837edbaef2f9970bd21a8959e`  
		Last Modified: Tue, 06 Dec 2022 05:03:47 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3c241ac0e5047b43eb162e3da63dd5881592cf383c63a96116d7c393bbe228`  
		Last Modified: Tue, 06 Dec 2022 05:03:47 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec98d68bc0d608718853226d628e3e40530a8fb5d35605776d9b0870c4b9a5d3`  
		Last Modified: Tue, 06 Dec 2022 05:03:47 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ab78cac3150fb48c827c8e5b72407741c49a5a36b524010f33f7e85db7b87`  
		Last Modified: Tue, 06 Dec 2022 05:03:47 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:f62d3c80552a8f3ae5f405d9bc418531f39aa811fc9ac727c3a1568e2cbfe0d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:2de369c9b6fee6c4040425471794b3afd44b63353c8f9299e8040fff762c9eb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **559.3 MB (559254989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f5c4e280ad234af379eacbb574965c2abc1fbf37611b2bd08b89beeab755754`
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
# Tue, 06 Dec 2022 04:58:01 GMT
ARG ODOO_RELEASE=20221202
# Tue, 06 Dec 2022 04:58:01 GMT
ARG ODOO_SHA=d0ee50281624260267085ee90302d1fe422eebbb
# Tue, 06 Dec 2022 04:59:18 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=d0ee50281624260267085ee90302d1fe422eebbb
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 06 Dec 2022 04:59:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 06 Dec 2022 04:59:22 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 06 Dec 2022 04:59:23 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=d0ee50281624260267085ee90302d1fe422eebbb
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 06 Dec 2022 04:59:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 06 Dec 2022 04:59:23 GMT
EXPOSE 8069 8071 8072
# Tue, 06 Dec 2022 04:59:23 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 06 Dec 2022 04:59:23 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 06 Dec 2022 04:59:23 GMT
USER odoo
# Tue, 06 Dec 2022 04:59:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 04:59:23 GMT
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
	-	`sha256:a3d76906584144f2b5150ca0de429bfc0ed011c89c4cbc0ad89427d7ab78d8f5`  
		Last Modified: Tue, 06 Dec 2022 05:04:23 GMT  
		Size: 304.5 MB (304515345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c074368a724a96e4e302f687a42f2828dae044d837edbaef2f9970bd21a8959e`  
		Last Modified: Tue, 06 Dec 2022 05:03:47 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3c241ac0e5047b43eb162e3da63dd5881592cf383c63a96116d7c393bbe228`  
		Last Modified: Tue, 06 Dec 2022 05:03:47 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec98d68bc0d608718853226d628e3e40530a8fb5d35605776d9b0870c4b9a5d3`  
		Last Modified: Tue, 06 Dec 2022 05:03:47 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752ab78cac3150fb48c827c8e5b72407741c49a5a36b524010f33f7e85db7b87`  
		Last Modified: Tue, 06 Dec 2022 05:03:47 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:dfd805931eb12ce775349d0a29d5aface6e7a75b79505259d7eb0c856681dc6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:934395bd7417e808266666b8e57dc67afc9057f5ba64abb62563b1d2f3869e77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.9 MB (561932871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa12c926fe40867692a4f3aaf06cd2027addb6769513ff9f73e6500e847ff3dd`
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
# Tue, 06 Dec 2022 04:56:18 GMT
ARG ODOO_RELEASE=20221202
# Tue, 06 Dec 2022 04:56:18 GMT
ARG ODOO_SHA=3ffc37e18490c281cae46fc5cb52edbf7e41738a
# Tue, 06 Dec 2022 04:57:40 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=3ffc37e18490c281cae46fc5cb52edbf7e41738a
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 06 Dec 2022 04:57:45 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 06 Dec 2022 04:57:45 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 06 Dec 2022 04:57:45 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=3ffc37e18490c281cae46fc5cb52edbf7e41738a
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 06 Dec 2022 04:57:46 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 06 Dec 2022 04:57:46 GMT
EXPOSE 8069 8071 8072
# Tue, 06 Dec 2022 04:57:46 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 06 Dec 2022 04:57:46 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 06 Dec 2022 04:57:46 GMT
USER odoo
# Tue, 06 Dec 2022 04:57:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 04:57:46 GMT
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
	-	`sha256:9976b835c9e4b2bb51fa8fd06a06bdb646f7a994b968049fc7a095d7ed31251d`  
		Last Modified: Tue, 06 Dec 2022 05:03:36 GMT  
		Size: 307.2 MB (307193228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df42e21e51d577be95848ac4e5f7070cf4c9372ea2d471d762b8a9f17d99af2`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7374868d57f0cbfffddea6fc1c38a0e0c3f913f083cd6f297f87279b30390d`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21e1530957b06abe66969ed49e01505203383828ee8df00299ead5a13f3b3a6`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3bcd34f8b2d30e5edb5a1fd8a3452e18ba0e6eb624b4c475e991cacbf0af7f`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:dfd805931eb12ce775349d0a29d5aface6e7a75b79505259d7eb0c856681dc6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:934395bd7417e808266666b8e57dc67afc9057f5ba64abb62563b1d2f3869e77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.9 MB (561932871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa12c926fe40867692a4f3aaf06cd2027addb6769513ff9f73e6500e847ff3dd`
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
# Tue, 06 Dec 2022 04:56:18 GMT
ARG ODOO_RELEASE=20221202
# Tue, 06 Dec 2022 04:56:18 GMT
ARG ODOO_SHA=3ffc37e18490c281cae46fc5cb52edbf7e41738a
# Tue, 06 Dec 2022 04:57:40 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=3ffc37e18490c281cae46fc5cb52edbf7e41738a
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 06 Dec 2022 04:57:45 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 06 Dec 2022 04:57:45 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 06 Dec 2022 04:57:45 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=3ffc37e18490c281cae46fc5cb52edbf7e41738a
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 06 Dec 2022 04:57:46 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 06 Dec 2022 04:57:46 GMT
EXPOSE 8069 8071 8072
# Tue, 06 Dec 2022 04:57:46 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 06 Dec 2022 04:57:46 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 06 Dec 2022 04:57:46 GMT
USER odoo
# Tue, 06 Dec 2022 04:57:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 04:57:46 GMT
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
	-	`sha256:9976b835c9e4b2bb51fa8fd06a06bdb646f7a994b968049fc7a095d7ed31251d`  
		Last Modified: Tue, 06 Dec 2022 05:03:36 GMT  
		Size: 307.2 MB (307193228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df42e21e51d577be95848ac4e5f7070cf4c9372ea2d471d762b8a9f17d99af2`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7374868d57f0cbfffddea6fc1c38a0e0c3f913f083cd6f297f87279b30390d`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21e1530957b06abe66969ed49e01505203383828ee8df00299ead5a13f3b3a6`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3bcd34f8b2d30e5edb5a1fd8a3452e18ba0e6eb624b4c475e991cacbf0af7f`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:dfd805931eb12ce775349d0a29d5aface6e7a75b79505259d7eb0c856681dc6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:934395bd7417e808266666b8e57dc67afc9057f5ba64abb62563b1d2f3869e77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.9 MB (561932871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa12c926fe40867692a4f3aaf06cd2027addb6769513ff9f73e6500e847ff3dd`
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
# Tue, 06 Dec 2022 04:56:18 GMT
ARG ODOO_RELEASE=20221202
# Tue, 06 Dec 2022 04:56:18 GMT
ARG ODOO_SHA=3ffc37e18490c281cae46fc5cb52edbf7e41738a
# Tue, 06 Dec 2022 04:57:40 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=3ffc37e18490c281cae46fc5cb52edbf7e41738a
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 06 Dec 2022 04:57:45 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 06 Dec 2022 04:57:45 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 06 Dec 2022 04:57:45 GMT
# ARGS: ODOO_RELEASE=20221202 ODOO_SHA=3ffc37e18490c281cae46fc5cb52edbf7e41738a
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 06 Dec 2022 04:57:46 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 06 Dec 2022 04:57:46 GMT
EXPOSE 8069 8071 8072
# Tue, 06 Dec 2022 04:57:46 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 06 Dec 2022 04:57:46 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 06 Dec 2022 04:57:46 GMT
USER odoo
# Tue, 06 Dec 2022 04:57:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Dec 2022 04:57:46 GMT
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
	-	`sha256:9976b835c9e4b2bb51fa8fd06a06bdb646f7a994b968049fc7a095d7ed31251d`  
		Last Modified: Tue, 06 Dec 2022 05:03:36 GMT  
		Size: 307.2 MB (307193228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df42e21e51d577be95848ac4e5f7070cf4c9372ea2d471d762b8a9f17d99af2`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7374868d57f0cbfffddea6fc1c38a0e0c3f913f083cd6f297f87279b30390d`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21e1530957b06abe66969ed49e01505203383828ee8df00299ead5a13f3b3a6`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3bcd34f8b2d30e5edb5a1fd8a3452e18ba0e6eb624b4c475e991cacbf0af7f`  
		Last Modified: Tue, 06 Dec 2022 05:02:58 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
