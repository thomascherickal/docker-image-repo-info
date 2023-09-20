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
$ docker pull odoo@sha256:757d206e1d5cfbbaabed5d0d1b50144ad87f73045a3e605ee0973377d6f122c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:542d733253b8092eac7668cf1dba66d6db3c7d964830ad6d24aa7ba70c7e3302
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.2 MB (533181742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:759c4032ca80d789a04bb54750d1c4352804a0be69b74f1bbc65967baa274f3f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:25 GMT
ADD file:a280220815a2a1eb37b2adea38333ec2f2d0c15bef81fb925d2fbb5218f0665f in / 
# Wed, 20 Sep 2023 04:56:25 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:10:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Sep 2023 17:10:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Sep 2023 17:10:35 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:11:58 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Sep 2023 17:12:10 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:12:13 GMT
RUN npm install -g rtlcss
# Wed, 20 Sep 2023 17:12:13 GMT
ENV ODOO_VERSION=14.0
# Wed, 20 Sep 2023 17:12:13 GMT
ARG ODOO_RELEASE=20230908
# Wed, 20 Sep 2023 17:12:13 GMT
ARG ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
# Wed, 20 Sep 2023 17:13:28 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Sep 2023 17:13:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Sep 2023 17:13:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Sep 2023 17:13:32 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Sep 2023 17:13:32 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Sep 2023 17:13:32 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Sep 2023 17:13:32 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Sep 2023 17:13:32 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Sep 2023 17:13:32 GMT
USER odoo
# Wed, 20 Sep 2023 17:13:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Sep 2023 17:13:33 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9f1ecb66bc03eb034c0c89c673def85a052c432125468c04e9aab84714aca0dd`  
		Last Modified: Wed, 20 Sep 2023 05:01:44 GMT  
		Size: 27.2 MB (27187412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2c00cc67825184a50f8ac124275cd02e1cfe225202df2b8529a89b347f17fc`  
		Last Modified: Wed, 20 Sep 2023 17:15:52 GMT  
		Size: 213.2 MB (213177221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e38b6ee0418a568b6723031ee851c0255648d189062f7a34cd082738a5a1da`  
		Last Modified: Wed, 20 Sep 2023 17:15:31 GMT  
		Size: 13.6 MB (13567689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41556b9b524d52ec328e6b0ee7c21deedf8aed8e3e61bae271a9d58162ecaa84`  
		Last Modified: Wed, 20 Sep 2023 17:15:29 GMT  
		Size: 460.0 KB (459973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b34f1c42573d6df23222499e0d32ce9a91a5c1c91374eb89a2c33e37a03cd65`  
		Last Modified: Wed, 20 Sep 2023 17:16:00 GMT  
		Size: 278.8 MB (278786981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535ebfbed99019194329a855b3fe9e8e62a21234acaf6f1d7c4c0c3cdc7c1ec4`  
		Last Modified: Wed, 20 Sep 2023 17:15:27 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881cd89e2632e5ae08897fbb3e801b237f3b15572922cada58b93f0100b60ff6`  
		Last Modified: Wed, 20 Sep 2023 17:15:26 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66dbbc67d120e7b7a185bf9ed50a8482368b26a25d7f732f3ee2868cb826a3e`  
		Last Modified: Wed, 20 Sep 2023 17:15:26 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69c164f881edc549767b3dcee8552db7534a4d545f05c370e46bd57a9f9a528`  
		Last Modified: Wed, 20 Sep 2023 17:15:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:757d206e1d5cfbbaabed5d0d1b50144ad87f73045a3e605ee0973377d6f122c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:542d733253b8092eac7668cf1dba66d6db3c7d964830ad6d24aa7ba70c7e3302
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.2 MB (533181742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:759c4032ca80d789a04bb54750d1c4352804a0be69b74f1bbc65967baa274f3f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:25 GMT
ADD file:a280220815a2a1eb37b2adea38333ec2f2d0c15bef81fb925d2fbb5218f0665f in / 
# Wed, 20 Sep 2023 04:56:25 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:10:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Sep 2023 17:10:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Sep 2023 17:10:35 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:11:58 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Sep 2023 17:12:10 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:12:13 GMT
RUN npm install -g rtlcss
# Wed, 20 Sep 2023 17:12:13 GMT
ENV ODOO_VERSION=14.0
# Wed, 20 Sep 2023 17:12:13 GMT
ARG ODOO_RELEASE=20230908
# Wed, 20 Sep 2023 17:12:13 GMT
ARG ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
# Wed, 20 Sep 2023 17:13:28 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Sep 2023 17:13:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Sep 2023 17:13:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Sep 2023 17:13:32 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=2d87d3ad92af4643873995a0749b3b97cdeb7f73
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Sep 2023 17:13:32 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Sep 2023 17:13:32 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Sep 2023 17:13:32 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Sep 2023 17:13:32 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Sep 2023 17:13:32 GMT
USER odoo
# Wed, 20 Sep 2023 17:13:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Sep 2023 17:13:33 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9f1ecb66bc03eb034c0c89c673def85a052c432125468c04e9aab84714aca0dd`  
		Last Modified: Wed, 20 Sep 2023 05:01:44 GMT  
		Size: 27.2 MB (27187412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2c00cc67825184a50f8ac124275cd02e1cfe225202df2b8529a89b347f17fc`  
		Last Modified: Wed, 20 Sep 2023 17:15:52 GMT  
		Size: 213.2 MB (213177221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e38b6ee0418a568b6723031ee851c0255648d189062f7a34cd082738a5a1da`  
		Last Modified: Wed, 20 Sep 2023 17:15:31 GMT  
		Size: 13.6 MB (13567689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41556b9b524d52ec328e6b0ee7c21deedf8aed8e3e61bae271a9d58162ecaa84`  
		Last Modified: Wed, 20 Sep 2023 17:15:29 GMT  
		Size: 460.0 KB (459973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b34f1c42573d6df23222499e0d32ce9a91a5c1c91374eb89a2c33e37a03cd65`  
		Last Modified: Wed, 20 Sep 2023 17:16:00 GMT  
		Size: 278.8 MB (278786981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535ebfbed99019194329a855b3fe9e8e62a21234acaf6f1d7c4c0c3cdc7c1ec4`  
		Last Modified: Wed, 20 Sep 2023 17:15:27 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881cd89e2632e5ae08897fbb3e801b237f3b15572922cada58b93f0100b60ff6`  
		Last Modified: Wed, 20 Sep 2023 17:15:26 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66dbbc67d120e7b7a185bf9ed50a8482368b26a25d7f732f3ee2868cb826a3e`  
		Last Modified: Wed, 20 Sep 2023 17:15:26 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69c164f881edc549767b3dcee8552db7534a4d545f05c370e46bd57a9f9a528`  
		Last Modified: Wed, 20 Sep 2023 17:15:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:d131456f1b324185e87d28c109fbad78a8348c5d5d21675d7f7ea294c17f3123
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:d824b33cafa8ceaff9c324a7f2968d3538cc753fa35f580c0f99dba737eb0878
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.3 MB (562314013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d616a87faa8950a7a2dab96e86845123afecd08c8854e3e230dba35560993d6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:05:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Sep 2023 17:05:17 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Sep 2023 17:05:17 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:09:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Sep 2023 17:09:09 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:09:10 GMT
RUN npm install -g rtlcss
# Wed, 20 Sep 2023 17:09:10 GMT
ENV ODOO_VERSION=15.0
# Wed, 20 Sep 2023 17:09:10 GMT
ARG ODOO_RELEASE=20230908
# Wed, 20 Sep 2023 17:09:10 GMT
ARG ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
# Wed, 20 Sep 2023 17:10:21 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Sep 2023 17:10:26 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Sep 2023 17:10:26 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Sep 2023 17:10:26 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Sep 2023 17:10:26 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Sep 2023 17:10:26 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Sep 2023 17:10:26 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Sep 2023 17:10:27 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Sep 2023 17:10:27 GMT
USER odoo
# Wed, 20 Sep 2023 17:10:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Sep 2023 17:10:27 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6575baebaed17dfc5bb5620e882ccd394a631c23a37b46b31e8f35be27a5539e`  
		Last Modified: Wed, 20 Sep 2023 17:15:07 GMT  
		Size: 220.3 MB (220302175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd472c483e558655dc4a27e0fbaf86ccab2eca5b2cf1310880f2f0a268b4f0f`  
		Last Modified: Wed, 20 Sep 2023 17:14:43 GMT  
		Size: 2.6 MB (2624479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb18e6c2a98cf38295f637890a9999541712df42f606502c7be9aa8d797db06c`  
		Last Modified: Wed, 20 Sep 2023 17:14:42 GMT  
		Size: 455.5 KB (455523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dce335accc0e04038237a01abc6baa5cb73dcba12d57501edd1495fa15241db`  
		Last Modified: Wed, 20 Sep 2023 17:15:17 GMT  
		Size: 307.5 MB (307511663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c58d2c59f7f8fe000f3a41a0831b7912d6a98cfce84c8cdcf179fbbbeaf47d`  
		Last Modified: Wed, 20 Sep 2023 17:14:40 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12326a12853e67c18cd4558e9777aee16cbfab449e792bf07db700829e1eca2`  
		Last Modified: Wed, 20 Sep 2023 17:14:40 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8b3b8d9dbfc1f61fd5a1f27a122b4918f21b2922045880324b31c83e7d29f`  
		Last Modified: Wed, 20 Sep 2023 17:14:40 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0109d43322193b040e9b7c1117a0e82c4dcb048f0609a21aace36ef53b542caa`  
		Last Modified: Wed, 20 Sep 2023 17:14:40 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:d131456f1b324185e87d28c109fbad78a8348c5d5d21675d7f7ea294c17f3123
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:d824b33cafa8ceaff9c324a7f2968d3538cc753fa35f580c0f99dba737eb0878
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.3 MB (562314013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d616a87faa8950a7a2dab96e86845123afecd08c8854e3e230dba35560993d6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:05:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Sep 2023 17:05:17 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Sep 2023 17:05:17 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:09:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Sep 2023 17:09:09 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:09:10 GMT
RUN npm install -g rtlcss
# Wed, 20 Sep 2023 17:09:10 GMT
ENV ODOO_VERSION=15.0
# Wed, 20 Sep 2023 17:09:10 GMT
ARG ODOO_RELEASE=20230908
# Wed, 20 Sep 2023 17:09:10 GMT
ARG ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
# Wed, 20 Sep 2023 17:10:21 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Sep 2023 17:10:26 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Sep 2023 17:10:26 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Sep 2023 17:10:26 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=ff9c3147d2f2056d1f510958e16fb15d5dc89b6e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Sep 2023 17:10:26 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Sep 2023 17:10:26 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Sep 2023 17:10:26 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Sep 2023 17:10:27 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Sep 2023 17:10:27 GMT
USER odoo
# Wed, 20 Sep 2023 17:10:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Sep 2023 17:10:27 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6575baebaed17dfc5bb5620e882ccd394a631c23a37b46b31e8f35be27a5539e`  
		Last Modified: Wed, 20 Sep 2023 17:15:07 GMT  
		Size: 220.3 MB (220302175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd472c483e558655dc4a27e0fbaf86ccab2eca5b2cf1310880f2f0a268b4f0f`  
		Last Modified: Wed, 20 Sep 2023 17:14:43 GMT  
		Size: 2.6 MB (2624479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb18e6c2a98cf38295f637890a9999541712df42f606502c7be9aa8d797db06c`  
		Last Modified: Wed, 20 Sep 2023 17:14:42 GMT  
		Size: 455.5 KB (455523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dce335accc0e04038237a01abc6baa5cb73dcba12d57501edd1495fa15241db`  
		Last Modified: Wed, 20 Sep 2023 17:15:17 GMT  
		Size: 307.5 MB (307511663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c58d2c59f7f8fe000f3a41a0831b7912d6a98cfce84c8cdcf179fbbbeaf47d`  
		Last Modified: Wed, 20 Sep 2023 17:14:40 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12326a12853e67c18cd4558e9777aee16cbfab449e792bf07db700829e1eca2`  
		Last Modified: Wed, 20 Sep 2023 17:14:40 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee8b3b8d9dbfc1f61fd5a1f27a122b4918f21b2922045880324b31c83e7d29f`  
		Last Modified: Wed, 20 Sep 2023 17:14:40 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0109d43322193b040e9b7c1117a0e82c4dcb048f0609a21aace36ef53b542caa`  
		Last Modified: Wed, 20 Sep 2023 17:14:40 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:61710f0664201d2386121eeadc00758c95b8ecc017058fb3495a4a066579bcf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:ac7e6d9d796e9a3d0bb151a0459a4cefabaa8cf9f7bd29ae914ab806b5a5bda1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.5 MB (576468033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d82015409196228a91fc2d1ea067440ec82935ac0205f74c8211e5b70f95d243`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:05:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Sep 2023 17:05:17 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Sep 2023 17:05:17 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:06:24 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Sep 2023 17:06:32 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:06:34 GMT
RUN npm install -g rtlcss
# Wed, 20 Sep 2023 17:06:34 GMT
ENV ODOO_VERSION=16.0
# Wed, 20 Sep 2023 17:06:34 GMT
ARG ODOO_RELEASE=20230908
# Wed, 20 Sep 2023 17:06:34 GMT
ARG ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
# Wed, 20 Sep 2023 17:07:55 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Sep 2023 17:07:59 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Sep 2023 17:07:59 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Sep 2023 17:07:59 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Sep 2023 17:07:59 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Sep 2023 17:07:59 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Sep 2023 17:08:00 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Sep 2023 17:08:00 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Sep 2023 17:08:00 GMT
USER odoo
# Wed, 20 Sep 2023 17:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Sep 2023 17:08:00 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f11206b2f0b0742a04b2e5aa673cf9bc01605b066d9fb144ce3973545531f57`  
		Last Modified: Wed, 20 Sep 2023 17:14:18 GMT  
		Size: 221.0 MB (220991931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e852d5c710cf3b695ca69683a47c0c02019debf9d920cb9cf770b83b5b466e3`  
		Last Modified: Wed, 20 Sep 2023 17:13:54 GMT  
		Size: 2.6 MB (2627315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2d84b33fdc1c69a8c227d7b0e75f038a4e81d937f06be5b99f42c6ad8c6bc9`  
		Last Modified: Wed, 20 Sep 2023 17:13:53 GMT  
		Size: 455.5 KB (455518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454e2f8c9878ee0f26e873ab2fde3b043062d669cf75f9ca3176a4c1ea816898`  
		Last Modified: Wed, 20 Sep 2023 17:14:29 GMT  
		Size: 321.0 MB (320973095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6270ab7e1c01f846a1729f620f36f2697350796bbe6b9ee038639eccd2e27a11`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b614947c683d68d6249e2c62f2b6a3544361a9ac0ecba8995af77d6ff78979`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b37a88b4fd5a1b8e6c43c9fcd1d0c19ed6e36f7e453328cc2de42069d861be`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290bb762a8ff6f3bb312f2bbaad6d634179c8047299815edd000b6034aae7ea9`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:61710f0664201d2386121eeadc00758c95b8ecc017058fb3495a4a066579bcf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:ac7e6d9d796e9a3d0bb151a0459a4cefabaa8cf9f7bd29ae914ab806b5a5bda1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.5 MB (576468033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d82015409196228a91fc2d1ea067440ec82935ac0205f74c8211e5b70f95d243`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:05:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Sep 2023 17:05:17 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Sep 2023 17:05:17 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:06:24 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Sep 2023 17:06:32 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:06:34 GMT
RUN npm install -g rtlcss
# Wed, 20 Sep 2023 17:06:34 GMT
ENV ODOO_VERSION=16.0
# Wed, 20 Sep 2023 17:06:34 GMT
ARG ODOO_RELEASE=20230908
# Wed, 20 Sep 2023 17:06:34 GMT
ARG ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
# Wed, 20 Sep 2023 17:07:55 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Sep 2023 17:07:59 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Sep 2023 17:07:59 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Sep 2023 17:07:59 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Sep 2023 17:07:59 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Sep 2023 17:07:59 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Sep 2023 17:08:00 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Sep 2023 17:08:00 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Sep 2023 17:08:00 GMT
USER odoo
# Wed, 20 Sep 2023 17:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Sep 2023 17:08:00 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f11206b2f0b0742a04b2e5aa673cf9bc01605b066d9fb144ce3973545531f57`  
		Last Modified: Wed, 20 Sep 2023 17:14:18 GMT  
		Size: 221.0 MB (220991931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e852d5c710cf3b695ca69683a47c0c02019debf9d920cb9cf770b83b5b466e3`  
		Last Modified: Wed, 20 Sep 2023 17:13:54 GMT  
		Size: 2.6 MB (2627315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2d84b33fdc1c69a8c227d7b0e75f038a4e81d937f06be5b99f42c6ad8c6bc9`  
		Last Modified: Wed, 20 Sep 2023 17:13:53 GMT  
		Size: 455.5 KB (455518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454e2f8c9878ee0f26e873ab2fde3b043062d669cf75f9ca3176a4c1ea816898`  
		Last Modified: Wed, 20 Sep 2023 17:14:29 GMT  
		Size: 321.0 MB (320973095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6270ab7e1c01f846a1729f620f36f2697350796bbe6b9ee038639eccd2e27a11`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b614947c683d68d6249e2c62f2b6a3544361a9ac0ecba8995af77d6ff78979`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b37a88b4fd5a1b8e6c43c9fcd1d0c19ed6e36f7e453328cc2de42069d861be`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290bb762a8ff6f3bb312f2bbaad6d634179c8047299815edd000b6034aae7ea9`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:61710f0664201d2386121eeadc00758c95b8ecc017058fb3495a4a066579bcf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:ac7e6d9d796e9a3d0bb151a0459a4cefabaa8cf9f7bd29ae914ab806b5a5bda1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.5 MB (576468033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d82015409196228a91fc2d1ea067440ec82935ac0205f74c8211e5b70f95d243`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:05:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Sep 2023 17:05:17 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Sep 2023 17:05:17 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:06:24 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Sep 2023 17:06:32 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:06:34 GMT
RUN npm install -g rtlcss
# Wed, 20 Sep 2023 17:06:34 GMT
ENV ODOO_VERSION=16.0
# Wed, 20 Sep 2023 17:06:34 GMT
ARG ODOO_RELEASE=20230908
# Wed, 20 Sep 2023 17:06:34 GMT
ARG ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
# Wed, 20 Sep 2023 17:07:55 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Sep 2023 17:07:59 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Sep 2023 17:07:59 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Sep 2023 17:07:59 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Sep 2023 17:07:59 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Sep 2023 17:07:59 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Sep 2023 17:08:00 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Sep 2023 17:08:00 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Sep 2023 17:08:00 GMT
USER odoo
# Wed, 20 Sep 2023 17:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Sep 2023 17:08:00 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f11206b2f0b0742a04b2e5aa673cf9bc01605b066d9fb144ce3973545531f57`  
		Last Modified: Wed, 20 Sep 2023 17:14:18 GMT  
		Size: 221.0 MB (220991931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e852d5c710cf3b695ca69683a47c0c02019debf9d920cb9cf770b83b5b466e3`  
		Last Modified: Wed, 20 Sep 2023 17:13:54 GMT  
		Size: 2.6 MB (2627315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2d84b33fdc1c69a8c227d7b0e75f038a4e81d937f06be5b99f42c6ad8c6bc9`  
		Last Modified: Wed, 20 Sep 2023 17:13:53 GMT  
		Size: 455.5 KB (455518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454e2f8c9878ee0f26e873ab2fde3b043062d669cf75f9ca3176a4c1ea816898`  
		Last Modified: Wed, 20 Sep 2023 17:14:29 GMT  
		Size: 321.0 MB (320973095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6270ab7e1c01f846a1729f620f36f2697350796bbe6b9ee038639eccd2e27a11`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b614947c683d68d6249e2c62f2b6a3544361a9ac0ecba8995af77d6ff78979`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b37a88b4fd5a1b8e6c43c9fcd1d0c19ed6e36f7e453328cc2de42069d861be`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290bb762a8ff6f3bb312f2bbaad6d634179c8047299815edd000b6034aae7ea9`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
