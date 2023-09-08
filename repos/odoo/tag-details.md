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
$ docker pull odoo@sha256:56209c38c51a9d5b1c89fe8e21edec4c2afc03748715a9a95c99fe37f4027217
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:3c7fed1a0475bf77a80efd319931dc3f6b73f05dde4eee4c58aca6d175af73e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.1 MB (533143710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b98351e7552f19278c4c84608983f430a6cc7341633fcae716cf892f31e2f3f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:26:18 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 07 Sep 2023 02:26:18 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 07 Sep 2023 02:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 02:27:34 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 07 Sep 2023 02:27:46 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:27:48 GMT
RUN npm install -g rtlcss
# Thu, 07 Sep 2023 02:27:48 GMT
ENV ODOO_VERSION=14.0
# Fri, 08 Sep 2023 19:53:26 GMT
ARG ODOO_RELEASE=20230908
# Fri, 08 Sep 2023 19:53:26 GMT
ARG ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
# Fri, 08 Sep 2023 19:54:41 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Sep 2023 19:54:45 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Sep 2023 19:54:45 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Sep 2023 19:54:46 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Sep 2023 19:54:46 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Sep 2023 19:54:46 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Sep 2023 19:54:46 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Sep 2023 19:54:46 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Sep 2023 19:54:46 GMT
USER odoo
# Fri, 08 Sep 2023 19:54:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Sep 2023 19:54:46 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940672322c8453d8f08692d07ca2e5e4ebb1320e1c84350aaabdd24bafce6cb0`  
		Last Modified: Thu, 07 Sep 2023 02:31:20 GMT  
		Size: 213.2 MB (213181707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527a05543a28635818dba1cc0ab4d4098637423c0741a6e782b784820618d6d9`  
		Last Modified: Thu, 07 Sep 2023 02:31:00 GMT  
		Size: 13.5 MB (13522728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938de5b6d3ea80d4eac894fafbab9f362a2a851997bf684bf68b776a5062d37a`  
		Last Modified: Thu, 07 Sep 2023 02:30:57 GMT  
		Size: 460.1 KB (460142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55338cbc04149c88faf538a4728dfe82931fee92d305ff576874fe8013462e3e`  
		Last Modified: Fri, 08 Sep 2023 19:56:58 GMT  
		Size: 278.8 MB (278789284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff51c7aa73fc6b7182e95b3f26d7a419de7cb0e6be678fab19d80a5c76eb56f`  
		Last Modified: Fri, 08 Sep 2023 19:56:28 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581c27681330abaaf94ad7dccdd674cfcc85d496f25c1381fa67cd7709ffb365`  
		Last Modified: Fri, 08 Sep 2023 19:56:28 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797fb8a1dcb8c29bc61b033edc66a1775722b8f6b86b9a34f47dcf0427189742`  
		Last Modified: Fri, 08 Sep 2023 19:56:28 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff40916989351a1c58fc695501da13106cc97d231a2618e730cacf6c2ee9e4dd`  
		Last Modified: Fri, 08 Sep 2023 19:56:28 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:56209c38c51a9d5b1c89fe8e21edec4c2afc03748715a9a95c99fe37f4027217
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:3c7fed1a0475bf77a80efd319931dc3f6b73f05dde4eee4c58aca6d175af73e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.1 MB (533143710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b98351e7552f19278c4c84608983f430a6cc7341633fcae716cf892f31e2f3f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:26:18 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 07 Sep 2023 02:26:18 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 07 Sep 2023 02:26:18 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 02:27:34 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 07 Sep 2023 02:27:46 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:27:48 GMT
RUN npm install -g rtlcss
# Thu, 07 Sep 2023 02:27:48 GMT
ENV ODOO_VERSION=14.0
# Fri, 08 Sep 2023 19:53:26 GMT
ARG ODOO_RELEASE=20230908
# Fri, 08 Sep 2023 19:53:26 GMT
ARG ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
# Fri, 08 Sep 2023 19:54:41 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Sep 2023 19:54:45 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Sep 2023 19:54:45 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Sep 2023 19:54:46 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Sep 2023 19:54:46 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Sep 2023 19:54:46 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Sep 2023 19:54:46 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Sep 2023 19:54:46 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Sep 2023 19:54:46 GMT
USER odoo
# Fri, 08 Sep 2023 19:54:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Sep 2023 19:54:46 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940672322c8453d8f08692d07ca2e5e4ebb1320e1c84350aaabdd24bafce6cb0`  
		Last Modified: Thu, 07 Sep 2023 02:31:20 GMT  
		Size: 213.2 MB (213181707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527a05543a28635818dba1cc0ab4d4098637423c0741a6e782b784820618d6d9`  
		Last Modified: Thu, 07 Sep 2023 02:31:00 GMT  
		Size: 13.5 MB (13522728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938de5b6d3ea80d4eac894fafbab9f362a2a851997bf684bf68b776a5062d37a`  
		Last Modified: Thu, 07 Sep 2023 02:30:57 GMT  
		Size: 460.1 KB (460142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55338cbc04149c88faf538a4728dfe82931fee92d305ff576874fe8013462e3e`  
		Last Modified: Fri, 08 Sep 2023 19:56:58 GMT  
		Size: 278.8 MB (278789284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff51c7aa73fc6b7182e95b3f26d7a419de7cb0e6be678fab19d80a5c76eb56f`  
		Last Modified: Fri, 08 Sep 2023 19:56:28 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581c27681330abaaf94ad7dccdd674cfcc85d496f25c1381fa67cd7709ffb365`  
		Last Modified: Fri, 08 Sep 2023 19:56:28 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797fb8a1dcb8c29bc61b033edc66a1775722b8f6b86b9a34f47dcf0427189742`  
		Last Modified: Fri, 08 Sep 2023 19:56:28 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff40916989351a1c58fc695501da13106cc97d231a2618e730cacf6c2ee9e4dd`  
		Last Modified: Fri, 08 Sep 2023 19:56:28 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:ff6d3733461adb31e930c7f2e4825fd238b3019b9bab0dbd56d04a664e06280c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:3989991657ff1f11f1e03e4be64e0771b6ac010e04fcf51019053b7d407543c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.3 MB (562261782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27530eff48c818e3f4f909782ed85ba372cc4b0a7ca622f5454887220bd2b81`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:21:01 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 07 Sep 2023 02:21:01 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 07 Sep 2023 02:21:01 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 02:24:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 07 Sep 2023 02:24:51 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:24:53 GMT
RUN npm install -g rtlcss
# Thu, 07 Sep 2023 02:24:53 GMT
ENV ODOO_VERSION=15.0
# Fri, 08 Sep 2023 19:52:02 GMT
ARG ODOO_RELEASE=20230908
# Fri, 08 Sep 2023 19:52:02 GMT
ARG ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
# Fri, 08 Sep 2023 19:53:14 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Sep 2023 19:53:18 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Sep 2023 19:53:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Sep 2023 19:53:19 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Sep 2023 19:53:19 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Sep 2023 19:53:19 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Sep 2023 19:53:19 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Sep 2023 19:53:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Sep 2023 19:53:19 GMT
USER odoo
# Fri, 08 Sep 2023 19:53:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Sep 2023 19:53:20 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5d5974a7fe984f9ed75a81bee2adca298a731040afb6f935a1665727b14bec`  
		Last Modified: Thu, 07 Sep 2023 02:30:37 GMT  
		Size: 220.3 MB (220302684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb58d10540b49101750bab050b9d3f58734d7593f35dad8ab4ae9101580de4e`  
		Last Modified: Thu, 07 Sep 2023 02:30:13 GMT  
		Size: 2.6 MB (2576464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7235349850c57657a3c2e0191b357dbebb26946868008648786cb479cd300d00`  
		Last Modified: Thu, 07 Sep 2023 02:30:13 GMT  
		Size: 455.8 KB (455771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf62198885c03f0eb882a12d02c70c5865ef9c20c9495212246a77c1cc5b54c`  
		Last Modified: Fri, 08 Sep 2023 19:56:19 GMT  
		Size: 307.5 MB (307506894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76a29a92e62fbd87d098ccbe08fee16435c997653a223e96204281794cff420`  
		Last Modified: Fri, 08 Sep 2023 19:55:46 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ece2ba3df40d3880730f8f5df7a6730666346d2f6dc69a959bec2ab31d648e`  
		Last Modified: Fri, 08 Sep 2023 19:55:46 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c510048e5e2d784ed7dcf2f2dd7d9f6e24ca9abfd14ba56b5a0ad68d076f1b8`  
		Last Modified: Fri, 08 Sep 2023 19:55:46 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f29660f67901b667ebb6617aa056c4675b70e66223943f789cd9f46f9fc00b`  
		Last Modified: Fri, 08 Sep 2023 19:55:46 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:ff6d3733461adb31e930c7f2e4825fd238b3019b9bab0dbd56d04a664e06280c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:3989991657ff1f11f1e03e4be64e0771b6ac010e04fcf51019053b7d407543c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.3 MB (562261782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27530eff48c818e3f4f909782ed85ba372cc4b0a7ca622f5454887220bd2b81`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:21:01 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 07 Sep 2023 02:21:01 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 07 Sep 2023 02:21:01 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 02:24:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 07 Sep 2023 02:24:51 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:24:53 GMT
RUN npm install -g rtlcss
# Thu, 07 Sep 2023 02:24:53 GMT
ENV ODOO_VERSION=15.0
# Fri, 08 Sep 2023 19:52:02 GMT
ARG ODOO_RELEASE=20230908
# Fri, 08 Sep 2023 19:52:02 GMT
ARG ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
# Fri, 08 Sep 2023 19:53:14 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Sep 2023 19:53:18 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Sep 2023 19:53:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Sep 2023 19:53:19 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Sep 2023 19:53:19 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Sep 2023 19:53:19 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Sep 2023 19:53:19 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Sep 2023 19:53:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Sep 2023 19:53:19 GMT
USER odoo
# Fri, 08 Sep 2023 19:53:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Sep 2023 19:53:20 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5d5974a7fe984f9ed75a81bee2adca298a731040afb6f935a1665727b14bec`  
		Last Modified: Thu, 07 Sep 2023 02:30:37 GMT  
		Size: 220.3 MB (220302684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb58d10540b49101750bab050b9d3f58734d7593f35dad8ab4ae9101580de4e`  
		Last Modified: Thu, 07 Sep 2023 02:30:13 GMT  
		Size: 2.6 MB (2576464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7235349850c57657a3c2e0191b357dbebb26946868008648786cb479cd300d00`  
		Last Modified: Thu, 07 Sep 2023 02:30:13 GMT  
		Size: 455.8 KB (455771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf62198885c03f0eb882a12d02c70c5865ef9c20c9495212246a77c1cc5b54c`  
		Last Modified: Fri, 08 Sep 2023 19:56:19 GMT  
		Size: 307.5 MB (307506894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76a29a92e62fbd87d098ccbe08fee16435c997653a223e96204281794cff420`  
		Last Modified: Fri, 08 Sep 2023 19:55:46 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ece2ba3df40d3880730f8f5df7a6730666346d2f6dc69a959bec2ab31d648e`  
		Last Modified: Fri, 08 Sep 2023 19:55:46 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c510048e5e2d784ed7dcf2f2dd7d9f6e24ca9abfd14ba56b5a0ad68d076f1b8`  
		Last Modified: Fri, 08 Sep 2023 19:55:46 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f29660f67901b667ebb6617aa056c4675b70e66223943f789cd9f46f9fc00b`  
		Last Modified: Fri, 08 Sep 2023 19:55:46 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:dd4c542be757fd563e9ebddd1fb17624afc2b5216ed2af5d607c5eda2d14cfac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:647ff55c7579da4a93a55a54314b592920473e453f9efd84a83402a8b6d0a94e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.4 MB (576439329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4aaf2433ece87b122d7eedf903445dd86179d14a09b9e62a3f73b93bf245d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:21:01 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 07 Sep 2023 02:21:01 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 07 Sep 2023 02:21:01 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 02:22:07 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 07 Sep 2023 02:22:18 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:19 GMT
RUN npm install -g rtlcss
# Thu, 07 Sep 2023 02:22:19 GMT
ENV ODOO_VERSION=16.0
# Fri, 08 Sep 2023 19:50:23 GMT
ARG ODOO_RELEASE=20230908
# Fri, 08 Sep 2023 19:50:23 GMT
ARG ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
# Fri, 08 Sep 2023 19:51:45 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Sep 2023 19:51:49 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Sep 2023 19:51:49 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Sep 2023 19:51:50 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Sep 2023 19:51:50 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Sep 2023 19:51:50 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Sep 2023 19:51:50 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Sep 2023 19:51:50 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Sep 2023 19:51:50 GMT
USER odoo
# Fri, 08 Sep 2023 19:51:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Sep 2023 19:51:50 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aee24f7779098be746c2ccfd465a71089f8fabdd3871b79af9060fc44a2911b`  
		Last Modified: Thu, 07 Sep 2023 02:29:47 GMT  
		Size: 221.0 MB (220992957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bb15e16ded7af3729af7fcb014075bc7146c328b39adade6d7a98d491b1b28`  
		Last Modified: Thu, 07 Sep 2023 02:29:22 GMT  
		Size: 2.6 MB (2579967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9358b870e15ee771e762346a77778b643846ade6027dab02e21d6024a92eff6`  
		Last Modified: Thu, 07 Sep 2023 02:29:22 GMT  
		Size: 455.7 KB (455729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf374f63aace759174d640cefd61864a0897bf91d13cea764aac115c2106a693`  
		Last Modified: Fri, 08 Sep 2023 19:55:34 GMT  
		Size: 321.0 MB (320990708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90af3ab57be5d3b288d5c921040ba0e7bb7327cd119ad1f78450da6ed27d2cf0`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df73b362c90b9c9a3e905866586798739d3b74a8c4619fe405335ba6903d1c24`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b00dd2e63764e7fd92689f2450840d41a80db767d51ea5aa58f425c3b14b51`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0f772f596c4e4031f7db2519f6aaf5ee55c2618eef9faaf1e2b61b3cf1010f`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:dd4c542be757fd563e9ebddd1fb17624afc2b5216ed2af5d607c5eda2d14cfac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:647ff55c7579da4a93a55a54314b592920473e453f9efd84a83402a8b6d0a94e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.4 MB (576439329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4aaf2433ece87b122d7eedf903445dd86179d14a09b9e62a3f73b93bf245d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:21:01 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 07 Sep 2023 02:21:01 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 07 Sep 2023 02:21:01 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 02:22:07 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 07 Sep 2023 02:22:18 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:19 GMT
RUN npm install -g rtlcss
# Thu, 07 Sep 2023 02:22:19 GMT
ENV ODOO_VERSION=16.0
# Fri, 08 Sep 2023 19:50:23 GMT
ARG ODOO_RELEASE=20230908
# Fri, 08 Sep 2023 19:50:23 GMT
ARG ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
# Fri, 08 Sep 2023 19:51:45 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Sep 2023 19:51:49 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Sep 2023 19:51:49 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Sep 2023 19:51:50 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Sep 2023 19:51:50 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Sep 2023 19:51:50 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Sep 2023 19:51:50 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Sep 2023 19:51:50 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Sep 2023 19:51:50 GMT
USER odoo
# Fri, 08 Sep 2023 19:51:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Sep 2023 19:51:50 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aee24f7779098be746c2ccfd465a71089f8fabdd3871b79af9060fc44a2911b`  
		Last Modified: Thu, 07 Sep 2023 02:29:47 GMT  
		Size: 221.0 MB (220992957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bb15e16ded7af3729af7fcb014075bc7146c328b39adade6d7a98d491b1b28`  
		Last Modified: Thu, 07 Sep 2023 02:29:22 GMT  
		Size: 2.6 MB (2579967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9358b870e15ee771e762346a77778b643846ade6027dab02e21d6024a92eff6`  
		Last Modified: Thu, 07 Sep 2023 02:29:22 GMT  
		Size: 455.7 KB (455729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf374f63aace759174d640cefd61864a0897bf91d13cea764aac115c2106a693`  
		Last Modified: Fri, 08 Sep 2023 19:55:34 GMT  
		Size: 321.0 MB (320990708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90af3ab57be5d3b288d5c921040ba0e7bb7327cd119ad1f78450da6ed27d2cf0`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df73b362c90b9c9a3e905866586798739d3b74a8c4619fe405335ba6903d1c24`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b00dd2e63764e7fd92689f2450840d41a80db767d51ea5aa58f425c3b14b51`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0f772f596c4e4031f7db2519f6aaf5ee55c2618eef9faaf1e2b61b3cf1010f`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:dd4c542be757fd563e9ebddd1fb17624afc2b5216ed2af5d607c5eda2d14cfac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:647ff55c7579da4a93a55a54314b592920473e453f9efd84a83402a8b6d0a94e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.4 MB (576439329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4aaf2433ece87b122d7eedf903445dd86179d14a09b9e62a3f73b93bf245d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:21:01 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 07 Sep 2023 02:21:01 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 07 Sep 2023 02:21:01 GMT
ENV LANG=C.UTF-8
# Thu, 07 Sep 2023 02:22:07 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 07 Sep 2023 02:22:18 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:19 GMT
RUN npm install -g rtlcss
# Thu, 07 Sep 2023 02:22:19 GMT
ENV ODOO_VERSION=16.0
# Fri, 08 Sep 2023 19:50:23 GMT
ARG ODOO_RELEASE=20230908
# Fri, 08 Sep 2023 19:50:23 GMT
ARG ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
# Fri, 08 Sep 2023 19:51:45 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Sep 2023 19:51:49 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Sep 2023 19:51:49 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Sep 2023 19:51:50 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Sep 2023 19:51:50 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Sep 2023 19:51:50 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Sep 2023 19:51:50 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Sep 2023 19:51:50 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Sep 2023 19:51:50 GMT
USER odoo
# Fri, 08 Sep 2023 19:51:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Sep 2023 19:51:50 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aee24f7779098be746c2ccfd465a71089f8fabdd3871b79af9060fc44a2911b`  
		Last Modified: Thu, 07 Sep 2023 02:29:47 GMT  
		Size: 221.0 MB (220992957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bb15e16ded7af3729af7fcb014075bc7146c328b39adade6d7a98d491b1b28`  
		Last Modified: Thu, 07 Sep 2023 02:29:22 GMT  
		Size: 2.6 MB (2579967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9358b870e15ee771e762346a77778b643846ade6027dab02e21d6024a92eff6`  
		Last Modified: Thu, 07 Sep 2023 02:29:22 GMT  
		Size: 455.7 KB (455729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf374f63aace759174d640cefd61864a0897bf91d13cea764aac115c2106a693`  
		Last Modified: Fri, 08 Sep 2023 19:55:34 GMT  
		Size: 321.0 MB (320990708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90af3ab57be5d3b288d5c921040ba0e7bb7327cd119ad1f78450da6ed27d2cf0`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df73b362c90b9c9a3e905866586798739d3b74a8c4619fe405335ba6903d1c24`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b00dd2e63764e7fd92689f2450840d41a80db767d51ea5aa58f425c3b14b51`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0f772f596c4e4031f7db2519f6aaf5ee55c2618eef9faaf1e2b61b3cf1010f`  
		Last Modified: Fri, 08 Sep 2023 19:54:58 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
