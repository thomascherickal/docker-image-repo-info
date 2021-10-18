<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `odoo`

-	[`odoo:13`](#odoo13)
-	[`odoo:13.0`](#odoo130)
-	[`odoo:14`](#odoo14)
-	[`odoo:14.0`](#odoo140)
-	[`odoo:15`](#odoo15)
-	[`odoo:15.0`](#odoo150)
-	[`odoo:latest`](#odoolatest)

## `odoo:13`

```console
$ docker pull odoo@sha256:57dfe40ef7b01d6b58a45fddfbf0aee32896d12031aca07bd9689c6c9567639c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:8be1c1e77df688272a2239d0072f2d21f73cb1799a97bd1bb484f00e1e40cf15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.6 MB (539586938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a9bb0407c0cdbbe02e31f9bdbbaac7e74eaf3036ed8b0bdbe93d34281e16784`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:04:36 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:04:36 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:04:37 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:09:43 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:09:56 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:10:00 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:10:00 GMT
ENV ODOO_VERSION=13.0
# Mon, 18 Oct 2021 20:23:13 GMT
ARG ODOO_RELEASE=20211018
# Mon, 18 Oct 2021 20:23:13 GMT
ARG ODOO_SHA=39e7ddbb8ef0a011176b4037a572f2dd5c51ef55
# Mon, 18 Oct 2021 20:24:26 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=39e7ddbb8ef0a011176b4037a572f2dd5c51ef55
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Oct 2021 20:24:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Oct 2021 20:24:30 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Oct 2021 20:24:30 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=39e7ddbb8ef0a011176b4037a572f2dd5c51ef55
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Oct 2021 20:24:31 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Oct 2021 20:24:31 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Oct 2021 20:24:31 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Oct 2021 20:24:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Oct 2021 20:24:31 GMT
USER odoo
# Mon, 18 Oct 2021 20:24:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Oct 2021 20:24:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45015eb54192c2e0c507396977810d7fddab577041c6c02a5758bcbf4d855326`  
		Last Modified: Tue, 12 Oct 2021 12:15:15 GMT  
		Size: 207.1 MB (207130926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8865fe285493c649f819eb839e1553c90a3bb6ef50521345f499df0337d093`  
		Last Modified: Tue, 12 Oct 2021 12:14:51 GMT  
		Size: 13.4 MB (13433045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788061f0dbd60660f54795fdbec83e425330c41bd36f2514ddf332ca7304796e`  
		Last Modified: Tue, 12 Oct 2021 12:14:47 GMT  
		Size: 864.8 KB (864751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9f48e18aa389ccdbd72f50d09310999563b4eec6f365a5c6ac752de372d18`  
		Last Modified: Mon, 18 Oct 2021 20:26:45 GMT  
		Size: 291.0 MB (291016236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a14639c7cd6208624be8a0439769e51560c092110c5ea851d5292c44d6464c`  
		Last Modified: Mon, 18 Oct 2021 20:26:15 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f256f0bbb1ddb4228715056c518a21c7d0a63860e94511a295eb202799d39010`  
		Last Modified: Mon, 18 Oct 2021 20:26:15 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c47e80c8c25ff2a1550e4ff0a420c4f11dbdcdffea0af2ece9088f75dd3d7c`  
		Last Modified: Mon, 18 Oct 2021 20:26:16 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399840738fb0b3f005dbd8bc6cd8a8d93a41b637e7147d29cfe93e26a27828f1`  
		Last Modified: Mon, 18 Oct 2021 20:26:15 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:57dfe40ef7b01d6b58a45fddfbf0aee32896d12031aca07bd9689c6c9567639c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:8be1c1e77df688272a2239d0072f2d21f73cb1799a97bd1bb484f00e1e40cf15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.6 MB (539586938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a9bb0407c0cdbbe02e31f9bdbbaac7e74eaf3036ed8b0bdbe93d34281e16784`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:04:36 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:04:36 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:04:37 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:09:43 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:09:56 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:10:00 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:10:00 GMT
ENV ODOO_VERSION=13.0
# Mon, 18 Oct 2021 20:23:13 GMT
ARG ODOO_RELEASE=20211018
# Mon, 18 Oct 2021 20:23:13 GMT
ARG ODOO_SHA=39e7ddbb8ef0a011176b4037a572f2dd5c51ef55
# Mon, 18 Oct 2021 20:24:26 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=39e7ddbb8ef0a011176b4037a572f2dd5c51ef55
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Oct 2021 20:24:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Oct 2021 20:24:30 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Oct 2021 20:24:30 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=39e7ddbb8ef0a011176b4037a572f2dd5c51ef55
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Oct 2021 20:24:31 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Oct 2021 20:24:31 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Oct 2021 20:24:31 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Oct 2021 20:24:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Oct 2021 20:24:31 GMT
USER odoo
# Mon, 18 Oct 2021 20:24:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Oct 2021 20:24:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45015eb54192c2e0c507396977810d7fddab577041c6c02a5758bcbf4d855326`  
		Last Modified: Tue, 12 Oct 2021 12:15:15 GMT  
		Size: 207.1 MB (207130926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8865fe285493c649f819eb839e1553c90a3bb6ef50521345f499df0337d093`  
		Last Modified: Tue, 12 Oct 2021 12:14:51 GMT  
		Size: 13.4 MB (13433045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788061f0dbd60660f54795fdbec83e425330c41bd36f2514ddf332ca7304796e`  
		Last Modified: Tue, 12 Oct 2021 12:14:47 GMT  
		Size: 864.8 KB (864751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef9f48e18aa389ccdbd72f50d09310999563b4eec6f365a5c6ac752de372d18`  
		Last Modified: Mon, 18 Oct 2021 20:26:45 GMT  
		Size: 291.0 MB (291016236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a14639c7cd6208624be8a0439769e51560c092110c5ea851d5292c44d6464c`  
		Last Modified: Mon, 18 Oct 2021 20:26:15 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f256f0bbb1ddb4228715056c518a21c7d0a63860e94511a295eb202799d39010`  
		Last Modified: Mon, 18 Oct 2021 20:26:15 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c47e80c8c25ff2a1550e4ff0a420c4f11dbdcdffea0af2ece9088f75dd3d7c`  
		Last Modified: Mon, 18 Oct 2021 20:26:16 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399840738fb0b3f005dbd8bc6cd8a8d93a41b637e7147d29cfe93e26a27828f1`  
		Last Modified: Mon, 18 Oct 2021 20:26:15 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:495f658221dde57bc02dd7f099f6b5eb430ef5e72e103be33ec6dd92b02a9b03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:e99bc9d31b7de32c7a23f434b8d4707da99ff2d4a34e5b8af7bbe295074eeeca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.2 MB (528236674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfd6dd07aaa5ea5a3a952e45f67f13cb010187b055e7d7b903078bb8ff177165`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:04:36 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:04:36 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:04:37 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:05:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:06:18 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:06:25 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:06:25 GMT
ENV ODOO_VERSION=14.0
# Mon, 18 Oct 2021 20:21:50 GMT
ARG ODOO_RELEASE=20211018
# Mon, 18 Oct 2021 20:21:51 GMT
ARG ODOO_SHA=8b3ecd81fd78b3ff0d93457b005bb4c98a5680b4
# Mon, 18 Oct 2021 20:23:03 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=8b3ecd81fd78b3ff0d93457b005bb4c98a5680b4
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Oct 2021 20:23:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Oct 2021 20:23:08 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Oct 2021 20:23:08 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=8b3ecd81fd78b3ff0d93457b005bb4c98a5680b4
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Oct 2021 20:23:09 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Oct 2021 20:23:09 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Oct 2021 20:23:09 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Oct 2021 20:23:09 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Oct 2021 20:23:09 GMT
USER odoo
# Mon, 18 Oct 2021 20:23:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Oct 2021 20:23:10 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a690652210adb99f7736fa4e78f5c15ebd7443f1779c0f4df93f3ede9b7242f4`  
		Last Modified: Tue, 12 Oct 2021 12:14:26 GMT  
		Size: 213.2 MB (213173260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f39d77a6b54dadd4be888e4329319568a8c6910b227f9968b18b3f32b7e5b8c`  
		Last Modified: Tue, 12 Oct 2021 12:14:00 GMT  
		Size: 13.4 MB (13435702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a022bb6719132cde437ae6e8500998624cebc5c7cfc5a5c69157cb1eeb54eb1`  
		Last Modified: Tue, 12 Oct 2021 12:13:56 GMT  
		Size: 864.7 KB (864743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7934e0014475cf7d39572d07423fe5828b58a8de19be00bd58ba8144d79bf804`  
		Last Modified: Mon, 18 Oct 2021 20:26:05 GMT  
		Size: 273.6 MB (273620991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a511e1e577022dc5b75d1764b1a70fff75105d2944e8910b1bb6d1e1454e28b3`  
		Last Modified: Mon, 18 Oct 2021 20:25:33 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb4d40ad742768eb8b9f9f66af724500f818fcb2ef68c03ba053ed1e905fd46`  
		Last Modified: Mon, 18 Oct 2021 20:25:34 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d3d206ed5ae1602f6e1ebd55ca30951f6161acf507fd327ef03438a6a93735`  
		Last Modified: Mon, 18 Oct 2021 20:25:33 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe43bb00a319ad68ca8cd332d5bf4a744647ded2b1bfe279d09311ea4aaafb7`  
		Last Modified: Mon, 18 Oct 2021 20:25:34 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:495f658221dde57bc02dd7f099f6b5eb430ef5e72e103be33ec6dd92b02a9b03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:e99bc9d31b7de32c7a23f434b8d4707da99ff2d4a34e5b8af7bbe295074eeeca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.2 MB (528236674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfd6dd07aaa5ea5a3a952e45f67f13cb010187b055e7d7b903078bb8ff177165`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:04:36 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:04:36 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:04:37 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:05:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:06:18 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:06:25 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:06:25 GMT
ENV ODOO_VERSION=14.0
# Mon, 18 Oct 2021 20:21:50 GMT
ARG ODOO_RELEASE=20211018
# Mon, 18 Oct 2021 20:21:51 GMT
ARG ODOO_SHA=8b3ecd81fd78b3ff0d93457b005bb4c98a5680b4
# Mon, 18 Oct 2021 20:23:03 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=8b3ecd81fd78b3ff0d93457b005bb4c98a5680b4
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Oct 2021 20:23:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Oct 2021 20:23:08 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Oct 2021 20:23:08 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=8b3ecd81fd78b3ff0d93457b005bb4c98a5680b4
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Oct 2021 20:23:09 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Oct 2021 20:23:09 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Oct 2021 20:23:09 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Oct 2021 20:23:09 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Oct 2021 20:23:09 GMT
USER odoo
# Mon, 18 Oct 2021 20:23:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Oct 2021 20:23:10 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a690652210adb99f7736fa4e78f5c15ebd7443f1779c0f4df93f3ede9b7242f4`  
		Last Modified: Tue, 12 Oct 2021 12:14:26 GMT  
		Size: 213.2 MB (213173260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f39d77a6b54dadd4be888e4329319568a8c6910b227f9968b18b3f32b7e5b8c`  
		Last Modified: Tue, 12 Oct 2021 12:14:00 GMT  
		Size: 13.4 MB (13435702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a022bb6719132cde437ae6e8500998624cebc5c7cfc5a5c69157cb1eeb54eb1`  
		Last Modified: Tue, 12 Oct 2021 12:13:56 GMT  
		Size: 864.7 KB (864743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7934e0014475cf7d39572d07423fe5828b58a8de19be00bd58ba8144d79bf804`  
		Last Modified: Mon, 18 Oct 2021 20:26:05 GMT  
		Size: 273.6 MB (273620991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a511e1e577022dc5b75d1764b1a70fff75105d2944e8910b1bb6d1e1454e28b3`  
		Last Modified: Mon, 18 Oct 2021 20:25:33 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb4d40ad742768eb8b9f9f66af724500f818fcb2ef68c03ba053ed1e905fd46`  
		Last Modified: Mon, 18 Oct 2021 20:25:34 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d3d206ed5ae1602f6e1ebd55ca30951f6161acf507fd327ef03438a6a93735`  
		Last Modified: Mon, 18 Oct 2021 20:25:33 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe43bb00a319ad68ca8cd332d5bf4a744647ded2b1bfe279d09311ea4aaafb7`  
		Last Modified: Mon, 18 Oct 2021 20:25:34 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:840cc5d34a3e4244ce58ae1c457c48373496a7e68fdda3497ee96dcdc4048e2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:fac4419d622149b3ac3b4dac7e7f24902d12b9ae6c71487ef2f4d30612a91736
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.6 MB (542592817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e31bb4d7cd00e5b9fa50ffe66fbfb505399c0149092dbef99f58a62f9a1b5b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:01:12 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:01:12 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:01:12 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:02:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         gsfonts         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-openssl         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:02:30 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:02:33 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:02:33 GMT
ENV ODOO_VERSION=15.0
# Mon, 18 Oct 2021 20:20:13 GMT
ARG ODOO_RELEASE=20211018
# Mon, 18 Oct 2021 20:20:13 GMT
ARG ODOO_SHA=41ddb9e8ea942595786c000f87fc1e045470b2b7
# Mon, 18 Oct 2021 20:21:28 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=41ddb9e8ea942595786c000f87fc1e045470b2b7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Oct 2021 20:21:32 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Oct 2021 20:21:32 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Oct 2021 20:21:33 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=41ddb9e8ea942595786c000f87fc1e045470b2b7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Oct 2021 20:21:33 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Oct 2021 20:21:33 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Oct 2021 20:21:33 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Oct 2021 20:21:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Oct 2021 20:21:34 GMT
USER odoo
# Mon, 18 Oct 2021 20:21:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Oct 2021 20:21:34 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38726de5ed2ec7e468afd026f502bdc97f591e43c0bc8e09ba8b0657c238ac0a`  
		Last Modified: Tue, 12 Oct 2021 12:13:37 GMT  
		Size: 223.8 MB (223816542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f220056c49310bef49e54a44fb6626222df0b73def08a56e1e145c3414d3f1f`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 2.5 MB (2506151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3854229348d451d83ddbf604aba25bf82021f5d0b001918068b73a3d4f6103ad`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 853.4 KB (853380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4216a72a97187686e6c77ced3211bf8b69abc40dda7c2072a58dbf6980984d1`  
		Last Modified: Mon, 18 Oct 2021 20:25:19 GMT  
		Size: 284.1 MB (284056970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2584cc7a31d8780db15bd969e0d1de183c001c1c53f04f470c92a50be34a709f`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f2c52b7f95b944402ecdc0c27a425086d7ece5e675823b084def53bdb0d122`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3dfff3d900ab7fdd5e1c485b6322e1c2e61c3a4b4176aa20f3aba66608cb36`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ac489d25f157821d93a8cfe49a4f049f1a31aed9c67d895fecc11694892984`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:840cc5d34a3e4244ce58ae1c457c48373496a7e68fdda3497ee96dcdc4048e2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:fac4419d622149b3ac3b4dac7e7f24902d12b9ae6c71487ef2f4d30612a91736
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.6 MB (542592817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e31bb4d7cd00e5b9fa50ffe66fbfb505399c0149092dbef99f58a62f9a1b5b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:01:12 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:01:12 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:01:12 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:02:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         gsfonts         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-openssl         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:02:30 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:02:33 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:02:33 GMT
ENV ODOO_VERSION=15.0
# Mon, 18 Oct 2021 20:20:13 GMT
ARG ODOO_RELEASE=20211018
# Mon, 18 Oct 2021 20:20:13 GMT
ARG ODOO_SHA=41ddb9e8ea942595786c000f87fc1e045470b2b7
# Mon, 18 Oct 2021 20:21:28 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=41ddb9e8ea942595786c000f87fc1e045470b2b7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Oct 2021 20:21:32 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Oct 2021 20:21:32 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Oct 2021 20:21:33 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=41ddb9e8ea942595786c000f87fc1e045470b2b7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Oct 2021 20:21:33 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Oct 2021 20:21:33 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Oct 2021 20:21:33 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Oct 2021 20:21:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Oct 2021 20:21:34 GMT
USER odoo
# Mon, 18 Oct 2021 20:21:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Oct 2021 20:21:34 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38726de5ed2ec7e468afd026f502bdc97f591e43c0bc8e09ba8b0657c238ac0a`  
		Last Modified: Tue, 12 Oct 2021 12:13:37 GMT  
		Size: 223.8 MB (223816542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f220056c49310bef49e54a44fb6626222df0b73def08a56e1e145c3414d3f1f`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 2.5 MB (2506151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3854229348d451d83ddbf604aba25bf82021f5d0b001918068b73a3d4f6103ad`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 853.4 KB (853380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4216a72a97187686e6c77ced3211bf8b69abc40dda7c2072a58dbf6980984d1`  
		Last Modified: Mon, 18 Oct 2021 20:25:19 GMT  
		Size: 284.1 MB (284056970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2584cc7a31d8780db15bd969e0d1de183c001c1c53f04f470c92a50be34a709f`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f2c52b7f95b944402ecdc0c27a425086d7ece5e675823b084def53bdb0d122`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3dfff3d900ab7fdd5e1c485b6322e1c2e61c3a4b4176aa20f3aba66608cb36`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ac489d25f157821d93a8cfe49a4f049f1a31aed9c67d895fecc11694892984`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:840cc5d34a3e4244ce58ae1c457c48373496a7e68fdda3497ee96dcdc4048e2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:fac4419d622149b3ac3b4dac7e7f24902d12b9ae6c71487ef2f4d30612a91736
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.6 MB (542592817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e31bb4d7cd00e5b9fa50ffe66fbfb505399c0149092dbef99f58a62f9a1b5b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:01:12 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:01:12 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:01:12 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:02:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         gsfonts         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-openssl         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:02:30 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:02:33 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:02:33 GMT
ENV ODOO_VERSION=15.0
# Mon, 18 Oct 2021 20:20:13 GMT
ARG ODOO_RELEASE=20211018
# Mon, 18 Oct 2021 20:20:13 GMT
ARG ODOO_SHA=41ddb9e8ea942595786c000f87fc1e045470b2b7
# Mon, 18 Oct 2021 20:21:28 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=41ddb9e8ea942595786c000f87fc1e045470b2b7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Oct 2021 20:21:32 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Oct 2021 20:21:32 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Oct 2021 20:21:33 GMT
# ARGS: ODOO_RELEASE=20211018 ODOO_SHA=41ddb9e8ea942595786c000f87fc1e045470b2b7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Oct 2021 20:21:33 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Oct 2021 20:21:33 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Oct 2021 20:21:33 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Oct 2021 20:21:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Oct 2021 20:21:34 GMT
USER odoo
# Mon, 18 Oct 2021 20:21:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Oct 2021 20:21:34 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38726de5ed2ec7e468afd026f502bdc97f591e43c0bc8e09ba8b0657c238ac0a`  
		Last Modified: Tue, 12 Oct 2021 12:13:37 GMT  
		Size: 223.8 MB (223816542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f220056c49310bef49e54a44fb6626222df0b73def08a56e1e145c3414d3f1f`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 2.5 MB (2506151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3854229348d451d83ddbf604aba25bf82021f5d0b001918068b73a3d4f6103ad`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 853.4 KB (853380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4216a72a97187686e6c77ced3211bf8b69abc40dda7c2072a58dbf6980984d1`  
		Last Modified: Mon, 18 Oct 2021 20:25:19 GMT  
		Size: 284.1 MB (284056970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2584cc7a31d8780db15bd969e0d1de183c001c1c53f04f470c92a50be34a709f`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f2c52b7f95b944402ecdc0c27a425086d7ece5e675823b084def53bdb0d122`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3dfff3d900ab7fdd5e1c485b6322e1c2e61c3a4b4176aa20f3aba66608cb36`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ac489d25f157821d93a8cfe49a4f049f1a31aed9c67d895fecc11694892984`  
		Last Modified: Mon, 18 Oct 2021 20:24:48 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
