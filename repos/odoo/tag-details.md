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
$ docker pull odoo@sha256:3516999f142fcb5e6c7af763bdd34410049bd2fbb373b11c0871dca831c1fbca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:e3065cb7fb2659a76b5b5f4006aaf041e57a3ad37d5ff0df8632aa8df188c68d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.4 MB (532438847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29248f1d042b51915a47c05a325d23d068043d483cc74270680d836f871ff391`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:30:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 May 2023 04:30:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 May 2023 04:30:10 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 04:31:59 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 May 2023 04:32:10 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:32:13 GMT
RUN npm install -g rtlcss
# Tue, 23 May 2023 04:32:13 GMT
ENV ODOO_VERSION=14.0
# Tue, 23 May 2023 04:32:13 GMT
ARG ODOO_RELEASE=20230517
# Tue, 23 May 2023 04:32:13 GMT
ARG ODOO_SHA=9c10e921b14f55e1d2c24283f5485037428b7c78
# Tue, 23 May 2023 04:33:37 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=9c10e921b14f55e1d2c24283f5485037428b7c78
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 23 May 2023 04:33:40 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 23 May 2023 04:33:40 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 23 May 2023 04:33:41 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=9c10e921b14f55e1d2c24283f5485037428b7c78
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 23 May 2023 04:33:41 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 23 May 2023 04:33:41 GMT
EXPOSE 8069 8071 8072
# Tue, 23 May 2023 04:33:41 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 23 May 2023 04:33:41 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 23 May 2023 04:33:41 GMT
USER odoo
# Tue, 23 May 2023 04:33:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 04:33:41 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aca9b3ba696a60bb5aefda89b215fb65bea612b9473c5bb7742a12d457b43c8`  
		Last Modified: Tue, 23 May 2023 04:35:47 GMT  
		Size: 213.2 MB (213200599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867a72128df6cf291a48f4eac739e1141e8731a8f7bd8ff82010ed2f2b912b15`  
		Last Modified: Tue, 23 May 2023 04:35:27 GMT  
		Size: 13.5 MB (13520105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33611cbfda398265d43bf6f537232ff1dfb60c7079746976ee090dbec1ddbf30`  
		Last Modified: Tue, 23 May 2023 04:35:25 GMT  
		Size: 456.7 KB (456694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017987b77c5601e89e830092c250065972624112831e33a459479d4df49eb695`  
		Last Modified: Tue, 23 May 2023 04:35:54 GMT  
		Size: 278.1 MB (278120408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11da4a258c45a896e58936dc9f20af44e58f4bac269fc2c139a8bb49b0f78cb`  
		Last Modified: Tue, 23 May 2023 04:35:23 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36ac25abcde972cb5a4432a03b34ee4b29ad33bbc864d66b9748aeacbf93b88`  
		Last Modified: Tue, 23 May 2023 04:35:23 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f2f3eaea0754bfbab9dbd111210c6a45e15f7585b4def9b6bdfcc7bf0d9581`  
		Last Modified: Tue, 23 May 2023 04:35:23 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a253545f794ce6f86fdb630efb15f693bd09bcad897f27d7e79ebc17884fcc4`  
		Last Modified: Tue, 23 May 2023 04:35:23 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:3516999f142fcb5e6c7af763bdd34410049bd2fbb373b11c0871dca831c1fbca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:e3065cb7fb2659a76b5b5f4006aaf041e57a3ad37d5ff0df8632aa8df188c68d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.4 MB (532438847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29248f1d042b51915a47c05a325d23d068043d483cc74270680d836f871ff391`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:30:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 May 2023 04:30:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 May 2023 04:30:10 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 04:31:59 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 May 2023 04:32:10 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:32:13 GMT
RUN npm install -g rtlcss
# Tue, 23 May 2023 04:32:13 GMT
ENV ODOO_VERSION=14.0
# Tue, 23 May 2023 04:32:13 GMT
ARG ODOO_RELEASE=20230517
# Tue, 23 May 2023 04:32:13 GMT
ARG ODOO_SHA=9c10e921b14f55e1d2c24283f5485037428b7c78
# Tue, 23 May 2023 04:33:37 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=9c10e921b14f55e1d2c24283f5485037428b7c78
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 23 May 2023 04:33:40 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 23 May 2023 04:33:40 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 23 May 2023 04:33:41 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=9c10e921b14f55e1d2c24283f5485037428b7c78
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 23 May 2023 04:33:41 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 23 May 2023 04:33:41 GMT
EXPOSE 8069 8071 8072
# Tue, 23 May 2023 04:33:41 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 23 May 2023 04:33:41 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 23 May 2023 04:33:41 GMT
USER odoo
# Tue, 23 May 2023 04:33:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 04:33:41 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aca9b3ba696a60bb5aefda89b215fb65bea612b9473c5bb7742a12d457b43c8`  
		Last Modified: Tue, 23 May 2023 04:35:47 GMT  
		Size: 213.2 MB (213200599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867a72128df6cf291a48f4eac739e1141e8731a8f7bd8ff82010ed2f2b912b15`  
		Last Modified: Tue, 23 May 2023 04:35:27 GMT  
		Size: 13.5 MB (13520105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33611cbfda398265d43bf6f537232ff1dfb60c7079746976ee090dbec1ddbf30`  
		Last Modified: Tue, 23 May 2023 04:35:25 GMT  
		Size: 456.7 KB (456694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017987b77c5601e89e830092c250065972624112831e33a459479d4df49eb695`  
		Last Modified: Tue, 23 May 2023 04:35:54 GMT  
		Size: 278.1 MB (278120408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11da4a258c45a896e58936dc9f20af44e58f4bac269fc2c139a8bb49b0f78cb`  
		Last Modified: Tue, 23 May 2023 04:35:23 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36ac25abcde972cb5a4432a03b34ee4b29ad33bbc864d66b9748aeacbf93b88`  
		Last Modified: Tue, 23 May 2023 04:35:23 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f2f3eaea0754bfbab9dbd111210c6a45e15f7585b4def9b6bdfcc7bf0d9581`  
		Last Modified: Tue, 23 May 2023 04:35:23 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a253545f794ce6f86fdb630efb15f693bd09bcad897f27d7e79ebc17884fcc4`  
		Last Modified: Tue, 23 May 2023 04:35:23 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:94d6a0ebb8f8c865a1e50b5b6889c3adc0f77774965d9068053322c39368609f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:5ed8f34bc64a805d62a8a0d5e8b689a1f9219f2ada3e40c464da0d783ed0a41c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **560.9 MB (560920638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b3f2ae18c3f814d1850fcd9910b8260428adf121445c7637aa44489bb96520`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:25:09 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 May 2023 04:25:09 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 May 2023 04:25:09 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 04:26:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 May 2023 04:26:54 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:26:56 GMT
RUN npm install -g rtlcss
# Tue, 23 May 2023 04:28:47 GMT
ENV ODOO_VERSION=15.0
# Tue, 23 May 2023 04:28:47 GMT
ARG ODOO_RELEASE=20230517
# Tue, 23 May 2023 04:28:47 GMT
ARG ODOO_SHA=63d84430c70fef2fdf8d384c7e58bd563c287b2b
# Tue, 23 May 2023 04:29:57 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=63d84430c70fef2fdf8d384c7e58bd563c287b2b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 23 May 2023 04:30:01 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 23 May 2023 04:30:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 23 May 2023 04:30:02 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=63d84430c70fef2fdf8d384c7e58bd563c287b2b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 23 May 2023 04:30:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 23 May 2023 04:30:02 GMT
EXPOSE 8069 8071 8072
# Tue, 23 May 2023 04:30:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 23 May 2023 04:30:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 23 May 2023 04:30:02 GMT
USER odoo
# Tue, 23 May 2023 04:30:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 04:30:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1e9686d13cba605592a655c33e96fc273869f0b8c2767aea698575f4a1b0f8`  
		Last Modified: Tue, 23 May 2023 04:34:21 GMT  
		Size: 220.3 MB (220298635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7e1c3238f65b74dbec3b8f1d37c83ba05c91cdc1519bc296572d0344d0bcc2`  
		Last Modified: Tue, 23 May 2023 04:33:57 GMT  
		Size: 2.6 MB (2576158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28ae768ba0baf0ccb8a34bf4c776dfd95d57e763b4152c3bd0f4125ef41c0dc`  
		Last Modified: Tue, 23 May 2023 04:33:57 GMT  
		Size: 452.2 KB (452212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca09a8987ffafc4a84529cc06195c9e9e8f9d7d7c3a7643087739641c84da707`  
		Last Modified: Tue, 23 May 2023 04:35:15 GMT  
		Size: 306.2 MB (306187582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098fddf70716ac185ba84a08933e851af842dec435b1a06b47e7c9bf1d775b0c`  
		Last Modified: Tue, 23 May 2023 04:34:42 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6ea0e9a92198136125e0faca1608a5310b2637e43d71065e3a9d427c968136`  
		Last Modified: Tue, 23 May 2023 04:34:42 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f80884b58405394799cfaae85158929ce239eca60aee1835432c8240c8008e`  
		Last Modified: Tue, 23 May 2023 04:34:42 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5417f7f91666674eed928ba75e8d000a61eb350a7de2fbd6ea206693cd1bfa04`  
		Last Modified: Tue, 23 May 2023 04:34:42 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:94d6a0ebb8f8c865a1e50b5b6889c3adc0f77774965d9068053322c39368609f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:5ed8f34bc64a805d62a8a0d5e8b689a1f9219f2ada3e40c464da0d783ed0a41c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **560.9 MB (560920638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b3f2ae18c3f814d1850fcd9910b8260428adf121445c7637aa44489bb96520`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:25:09 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 May 2023 04:25:09 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 May 2023 04:25:09 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 04:26:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 May 2023 04:26:54 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:26:56 GMT
RUN npm install -g rtlcss
# Tue, 23 May 2023 04:28:47 GMT
ENV ODOO_VERSION=15.0
# Tue, 23 May 2023 04:28:47 GMT
ARG ODOO_RELEASE=20230517
# Tue, 23 May 2023 04:28:47 GMT
ARG ODOO_SHA=63d84430c70fef2fdf8d384c7e58bd563c287b2b
# Tue, 23 May 2023 04:29:57 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=63d84430c70fef2fdf8d384c7e58bd563c287b2b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 23 May 2023 04:30:01 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 23 May 2023 04:30:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 23 May 2023 04:30:02 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=63d84430c70fef2fdf8d384c7e58bd563c287b2b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 23 May 2023 04:30:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 23 May 2023 04:30:02 GMT
EXPOSE 8069 8071 8072
# Tue, 23 May 2023 04:30:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 23 May 2023 04:30:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 23 May 2023 04:30:02 GMT
USER odoo
# Tue, 23 May 2023 04:30:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 04:30:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1e9686d13cba605592a655c33e96fc273869f0b8c2767aea698575f4a1b0f8`  
		Last Modified: Tue, 23 May 2023 04:34:21 GMT  
		Size: 220.3 MB (220298635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7e1c3238f65b74dbec3b8f1d37c83ba05c91cdc1519bc296572d0344d0bcc2`  
		Last Modified: Tue, 23 May 2023 04:33:57 GMT  
		Size: 2.6 MB (2576158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28ae768ba0baf0ccb8a34bf4c776dfd95d57e763b4152c3bd0f4125ef41c0dc`  
		Last Modified: Tue, 23 May 2023 04:33:57 GMT  
		Size: 452.2 KB (452212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca09a8987ffafc4a84529cc06195c9e9e8f9d7d7c3a7643087739641c84da707`  
		Last Modified: Tue, 23 May 2023 04:35:15 GMT  
		Size: 306.2 MB (306187582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098fddf70716ac185ba84a08933e851af842dec435b1a06b47e7c9bf1d775b0c`  
		Last Modified: Tue, 23 May 2023 04:34:42 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6ea0e9a92198136125e0faca1608a5310b2637e43d71065e3a9d427c968136`  
		Last Modified: Tue, 23 May 2023 04:34:42 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f80884b58405394799cfaae85158929ce239eca60aee1835432c8240c8008e`  
		Last Modified: Tue, 23 May 2023 04:34:42 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5417f7f91666674eed928ba75e8d000a61eb350a7de2fbd6ea206693cd1bfa04`  
		Last Modified: Tue, 23 May 2023 04:34:42 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:8607964d8aa6ace6123af0901336da8eb7ff64ff2a806ff3f15893de9b48abb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:a11212341f44959ca49b24f0bb8de75eb42f2e03eb2116513e64199fda13edcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.6 MB (572575560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85521d08aa1cf2ed25acc4f5f7879455c60ff1ce815416900f45c0ed85e7d615`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:25:09 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 May 2023 04:25:09 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 May 2023 04:25:09 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 04:26:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 May 2023 04:26:54 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:26:56 GMT
RUN npm install -g rtlcss
# Tue, 23 May 2023 04:26:56 GMT
ENV ODOO_VERSION=16.0
# Tue, 23 May 2023 04:26:56 GMT
ARG ODOO_RELEASE=20230517
# Tue, 23 May 2023 04:26:56 GMT
ARG ODOO_SHA=e737da6d601f011803fa66c6af297688c3e45fd4
# Tue, 23 May 2023 04:28:29 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=e737da6d601f011803fa66c6af297688c3e45fd4
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 23 May 2023 04:28:33 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 23 May 2023 04:28:33 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 23 May 2023 04:28:33 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=e737da6d601f011803fa66c6af297688c3e45fd4
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 23 May 2023 04:28:34 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 23 May 2023 04:28:34 GMT
EXPOSE 8069 8071 8072
# Tue, 23 May 2023 04:28:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 23 May 2023 04:28:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 23 May 2023 04:28:34 GMT
USER odoo
# Tue, 23 May 2023 04:28:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 04:28:34 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1e9686d13cba605592a655c33e96fc273869f0b8c2767aea698575f4a1b0f8`  
		Last Modified: Tue, 23 May 2023 04:34:21 GMT  
		Size: 220.3 MB (220298635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7e1c3238f65b74dbec3b8f1d37c83ba05c91cdc1519bc296572d0344d0bcc2`  
		Last Modified: Tue, 23 May 2023 04:33:57 GMT  
		Size: 2.6 MB (2576158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28ae768ba0baf0ccb8a34bf4c776dfd95d57e763b4152c3bd0f4125ef41c0dc`  
		Last Modified: Tue, 23 May 2023 04:33:57 GMT  
		Size: 452.2 KB (452212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776b4ca67994d77af494ba1c433e4702001773929bef69fa7dcba432097b3484`  
		Last Modified: Tue, 23 May 2023 04:34:31 GMT  
		Size: 317.8 MB (317842511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342e71de92eaea5d93552fa88d6c0997f437d2545359ba994db2cc4ba6a029e`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f452f9e644672ac7d6eac229e99ab83821f3b1b4492f3e218e3ac04e1347c4`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953246e8817eca0d80e4742525eb5fbf466eb7eefc8172e7c8d805cd9856d586`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67178b39842594f618399bd8ad70e8eda23980de4231b7c7b4a9c0ffcf332110`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:8607964d8aa6ace6123af0901336da8eb7ff64ff2a806ff3f15893de9b48abb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:a11212341f44959ca49b24f0bb8de75eb42f2e03eb2116513e64199fda13edcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.6 MB (572575560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85521d08aa1cf2ed25acc4f5f7879455c60ff1ce815416900f45c0ed85e7d615`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:25:09 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 May 2023 04:25:09 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 May 2023 04:25:09 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 04:26:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 May 2023 04:26:54 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:26:56 GMT
RUN npm install -g rtlcss
# Tue, 23 May 2023 04:26:56 GMT
ENV ODOO_VERSION=16.0
# Tue, 23 May 2023 04:26:56 GMT
ARG ODOO_RELEASE=20230517
# Tue, 23 May 2023 04:26:56 GMT
ARG ODOO_SHA=e737da6d601f011803fa66c6af297688c3e45fd4
# Tue, 23 May 2023 04:28:29 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=e737da6d601f011803fa66c6af297688c3e45fd4
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 23 May 2023 04:28:33 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 23 May 2023 04:28:33 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 23 May 2023 04:28:33 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=e737da6d601f011803fa66c6af297688c3e45fd4
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 23 May 2023 04:28:34 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 23 May 2023 04:28:34 GMT
EXPOSE 8069 8071 8072
# Tue, 23 May 2023 04:28:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 23 May 2023 04:28:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 23 May 2023 04:28:34 GMT
USER odoo
# Tue, 23 May 2023 04:28:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 04:28:34 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1e9686d13cba605592a655c33e96fc273869f0b8c2767aea698575f4a1b0f8`  
		Last Modified: Tue, 23 May 2023 04:34:21 GMT  
		Size: 220.3 MB (220298635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7e1c3238f65b74dbec3b8f1d37c83ba05c91cdc1519bc296572d0344d0bcc2`  
		Last Modified: Tue, 23 May 2023 04:33:57 GMT  
		Size: 2.6 MB (2576158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28ae768ba0baf0ccb8a34bf4c776dfd95d57e763b4152c3bd0f4125ef41c0dc`  
		Last Modified: Tue, 23 May 2023 04:33:57 GMT  
		Size: 452.2 KB (452212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776b4ca67994d77af494ba1c433e4702001773929bef69fa7dcba432097b3484`  
		Last Modified: Tue, 23 May 2023 04:34:31 GMT  
		Size: 317.8 MB (317842511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342e71de92eaea5d93552fa88d6c0997f437d2545359ba994db2cc4ba6a029e`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f452f9e644672ac7d6eac229e99ab83821f3b1b4492f3e218e3ac04e1347c4`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953246e8817eca0d80e4742525eb5fbf466eb7eefc8172e7c8d805cd9856d586`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67178b39842594f618399bd8ad70e8eda23980de4231b7c7b4a9c0ffcf332110`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:8607964d8aa6ace6123af0901336da8eb7ff64ff2a806ff3f15893de9b48abb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:a11212341f44959ca49b24f0bb8de75eb42f2e03eb2116513e64199fda13edcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.6 MB (572575560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85521d08aa1cf2ed25acc4f5f7879455c60ff1ce815416900f45c0ed85e7d615`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:25:09 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 May 2023 04:25:09 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 May 2023 04:25:09 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 04:26:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 May 2023 04:26:54 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:26:56 GMT
RUN npm install -g rtlcss
# Tue, 23 May 2023 04:26:56 GMT
ENV ODOO_VERSION=16.0
# Tue, 23 May 2023 04:26:56 GMT
ARG ODOO_RELEASE=20230517
# Tue, 23 May 2023 04:26:56 GMT
ARG ODOO_SHA=e737da6d601f011803fa66c6af297688c3e45fd4
# Tue, 23 May 2023 04:28:29 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=e737da6d601f011803fa66c6af297688c3e45fd4
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 23 May 2023 04:28:33 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 23 May 2023 04:28:33 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 23 May 2023 04:28:33 GMT
# ARGS: ODOO_RELEASE=20230517 ODOO_SHA=e737da6d601f011803fa66c6af297688c3e45fd4
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 23 May 2023 04:28:34 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 23 May 2023 04:28:34 GMT
EXPOSE 8069 8071 8072
# Tue, 23 May 2023 04:28:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 23 May 2023 04:28:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 23 May 2023 04:28:34 GMT
USER odoo
# Tue, 23 May 2023 04:28:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 04:28:34 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1e9686d13cba605592a655c33e96fc273869f0b8c2767aea698575f4a1b0f8`  
		Last Modified: Tue, 23 May 2023 04:34:21 GMT  
		Size: 220.3 MB (220298635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7e1c3238f65b74dbec3b8f1d37c83ba05c91cdc1519bc296572d0344d0bcc2`  
		Last Modified: Tue, 23 May 2023 04:33:57 GMT  
		Size: 2.6 MB (2576158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28ae768ba0baf0ccb8a34bf4c776dfd95d57e763b4152c3bd0f4125ef41c0dc`  
		Last Modified: Tue, 23 May 2023 04:33:57 GMT  
		Size: 452.2 KB (452212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776b4ca67994d77af494ba1c433e4702001773929bef69fa7dcba432097b3484`  
		Last Modified: Tue, 23 May 2023 04:34:31 GMT  
		Size: 317.8 MB (317842511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6342e71de92eaea5d93552fa88d6c0997f437d2545359ba994db2cc4ba6a029e`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f452f9e644672ac7d6eac229e99ab83821f3b1b4492f3e218e3ac04e1347c4`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953246e8817eca0d80e4742525eb5fbf466eb7eefc8172e7c8d805cd9856d586`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67178b39842594f618399bd8ad70e8eda23980de4231b7c7b4a9c0ffcf332110`  
		Last Modified: Tue, 23 May 2023 04:33:55 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
