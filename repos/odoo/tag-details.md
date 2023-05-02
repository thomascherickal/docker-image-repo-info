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
$ docker pull odoo@sha256:9ee99a3df291e57854f8345d61db9f0e81cd5cb2cd8bd0a25f71b1d051e9f908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:cff2774814ee649d01b2d66398e1e5aec7cfe9065688762fd4184f0000cd4bef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.3 MB (532349252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edd35cff658f07bd317d5bd96df53aab5f92d58e97efba981a027414bbe85d92`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:25 GMT
ADD file:e614539607055bdbde0cc1a94ef9783fe3627c8553ef1b21071ecb5c27ea27e4 in / 
# Wed, 12 Apr 2023 00:20:26 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:58:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:58:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:58:51 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 09:00:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 09:00:27 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:00:29 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 09:00:30 GMT
ENV ODOO_VERSION=14.0
# Tue, 02 May 2023 21:57:55 GMT
ARG ODOO_RELEASE=20230430
# Tue, 02 May 2023 21:57:55 GMT
ARG ODOO_SHA=06586ebb9902fa4840fb177f5e45f98d19dadf6d
# Tue, 02 May 2023 21:59:17 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=06586ebb9902fa4840fb177f5e45f98d19dadf6d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 02 May 2023 21:59:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 02 May 2023 21:59:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 02 May 2023 21:59:21 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=06586ebb9902fa4840fb177f5e45f98d19dadf6d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 02 May 2023 21:59:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 02 May 2023 21:59:21 GMT
EXPOSE 8069 8071 8072
# Tue, 02 May 2023 21:59:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 02 May 2023 21:59:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 02 May 2023 21:59:21 GMT
USER odoo
# Tue, 02 May 2023 21:59:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 May 2023 21:59:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9fbefa3370776b7ec7633cf07efc14cc24e0c0cd53893ad0e7e3f44ffdc1bedb`  
		Last Modified: Wed, 12 Apr 2023 00:24:22 GMT  
		Size: 27.1 MB (27138920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00d75581d1741b260047f82ac192a761c24b6c2d68e527e4a0de334335aa31`  
		Last Modified: Wed, 12 Apr 2023 09:04:00 GMT  
		Size: 213.2 MB (213203787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41383b72b69d61dc58305cf803eb49130c28b9c3978783268058f107ef8f2c35`  
		Last Modified: Wed, 12 Apr 2023 09:03:39 GMT  
		Size: 13.5 MB (13517731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6cb4d73ac452284f4e76b99129bce0d2ad7863d895cfd103f629d01b3b1e38`  
		Last Modified: Wed, 12 Apr 2023 09:03:37 GMT  
		Size: 453.9 KB (453862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3143616918572e8ad51fb40469140a56f7f12b6fb65f406412c467d7239f43bd`  
		Last Modified: Tue, 02 May 2023 22:01:41 GMT  
		Size: 278.0 MB (278032487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7206ef42bd8abf96550ea1e1769f5bb05819316ce5c4f5ebb1137fe5eabd7ebe`  
		Last Modified: Tue, 02 May 2023 22:01:07 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdca882423748b436bcf0d8fe2ac6820716147b1aff1bb4e6980d62e697672e`  
		Last Modified: Tue, 02 May 2023 22:01:07 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb058627d58fa39b05ecceadcf81e8b40536afcb32b0b38bc2e8513bb305ee2`  
		Last Modified: Tue, 02 May 2023 22:01:07 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e52002e597334a5f01db4f4a0d35ebf599e9b001cf5f780a27a0d37c7ac6dd9`  
		Last Modified: Tue, 02 May 2023 22:01:07 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:9ee99a3df291e57854f8345d61db9f0e81cd5cb2cd8bd0a25f71b1d051e9f908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:cff2774814ee649d01b2d66398e1e5aec7cfe9065688762fd4184f0000cd4bef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.3 MB (532349252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edd35cff658f07bd317d5bd96df53aab5f92d58e97efba981a027414bbe85d92`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:25 GMT
ADD file:e614539607055bdbde0cc1a94ef9783fe3627c8553ef1b21071ecb5c27ea27e4 in / 
# Wed, 12 Apr 2023 00:20:26 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:58:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:58:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:58:51 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 09:00:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 09:00:27 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:00:29 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 09:00:30 GMT
ENV ODOO_VERSION=14.0
# Tue, 02 May 2023 21:57:55 GMT
ARG ODOO_RELEASE=20230430
# Tue, 02 May 2023 21:57:55 GMT
ARG ODOO_SHA=06586ebb9902fa4840fb177f5e45f98d19dadf6d
# Tue, 02 May 2023 21:59:17 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=06586ebb9902fa4840fb177f5e45f98d19dadf6d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 02 May 2023 21:59:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 02 May 2023 21:59:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 02 May 2023 21:59:21 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=06586ebb9902fa4840fb177f5e45f98d19dadf6d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 02 May 2023 21:59:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 02 May 2023 21:59:21 GMT
EXPOSE 8069 8071 8072
# Tue, 02 May 2023 21:59:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 02 May 2023 21:59:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 02 May 2023 21:59:21 GMT
USER odoo
# Tue, 02 May 2023 21:59:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 May 2023 21:59:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9fbefa3370776b7ec7633cf07efc14cc24e0c0cd53893ad0e7e3f44ffdc1bedb`  
		Last Modified: Wed, 12 Apr 2023 00:24:22 GMT  
		Size: 27.1 MB (27138920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00d75581d1741b260047f82ac192a761c24b6c2d68e527e4a0de334335aa31`  
		Last Modified: Wed, 12 Apr 2023 09:04:00 GMT  
		Size: 213.2 MB (213203787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41383b72b69d61dc58305cf803eb49130c28b9c3978783268058f107ef8f2c35`  
		Last Modified: Wed, 12 Apr 2023 09:03:39 GMT  
		Size: 13.5 MB (13517731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6cb4d73ac452284f4e76b99129bce0d2ad7863d895cfd103f629d01b3b1e38`  
		Last Modified: Wed, 12 Apr 2023 09:03:37 GMT  
		Size: 453.9 KB (453862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3143616918572e8ad51fb40469140a56f7f12b6fb65f406412c467d7239f43bd`  
		Last Modified: Tue, 02 May 2023 22:01:41 GMT  
		Size: 278.0 MB (278032487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7206ef42bd8abf96550ea1e1769f5bb05819316ce5c4f5ebb1137fe5eabd7ebe`  
		Last Modified: Tue, 02 May 2023 22:01:07 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdca882423748b436bcf0d8fe2ac6820716147b1aff1bb4e6980d62e697672e`  
		Last Modified: Tue, 02 May 2023 22:01:07 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb058627d58fa39b05ecceadcf81e8b40536afcb32b0b38bc2e8513bb305ee2`  
		Last Modified: Tue, 02 May 2023 22:01:07 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e52002e597334a5f01db4f4a0d35ebf599e9b001cf5f780a27a0d37c7ac6dd9`  
		Last Modified: Tue, 02 May 2023 22:01:07 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:be5147bcfb055e76a233f75abe9ca8ba47e0234cdcb4dc7c01c786f512e1c1ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:9a71776060f27c67933547e751d2f9c743c9454ee388c776e52fb4f1d528677e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **560.8 MB (560828748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9e863115e8dc0c993aaaaf97b1b5bf4f8b10a6b585e42829a3ecf6e5750bd72`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:54:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:54:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:54:35 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:55:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 08:55:53 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:55:54 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 08:57:28 GMT
ENV ODOO_VERSION=15.0
# Tue, 02 May 2023 21:56:32 GMT
ARG ODOO_RELEASE=20230430
# Tue, 02 May 2023 21:56:32 GMT
ARG ODOO_SHA=af1128e5d8126e079a968ec22696a122965a4404
# Tue, 02 May 2023 21:57:44 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=af1128e5d8126e079a968ec22696a122965a4404
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 02 May 2023 21:57:48 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 02 May 2023 21:57:48 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 02 May 2023 21:57:49 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=af1128e5d8126e079a968ec22696a122965a4404
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 02 May 2023 21:57:49 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 02 May 2023 21:57:49 GMT
EXPOSE 8069 8071 8072
# Tue, 02 May 2023 21:57:49 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 02 May 2023 21:57:49 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 02 May 2023 21:57:49 GMT
USER odoo
# Tue, 02 May 2023 21:57:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 May 2023 21:57:49 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc072a51e9ff1e113fd7d7e6e812f69acee46b65fdb5e60e6a6977ab04867f8f`  
		Last Modified: Wed, 12 Apr 2023 09:02:33 GMT  
		Size: 220.3 MB (220298412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea2cf4d76c14443a63296eecd70cd09a9af720ca062d516b3f41535b435edf2`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 2.6 MB (2575214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfcc7225c9d8a7756bbe895737596be4bb564e0e7223b89b59cd40b96d7735b`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 449.3 KB (449266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b75cb0983bb9c95cbdcef8c652935381a57749a963ad260ad0f8561a884e83`  
		Last Modified: Tue, 02 May 2023 22:00:58 GMT  
		Size: 306.1 MB (306085168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a2df90b875f328a8aed26cc148fa15bdcc4183f5abbb67b98b191d36aaac`  
		Last Modified: Tue, 02 May 2023 22:00:25 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc84d813e6e2db5abe3bfcbb66ee5f97b58ed3701e4079d820d2428a618d5d8`  
		Last Modified: Tue, 02 May 2023 22:00:25 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716492ec80c1519b595ba5c90f6551617ff3a363dbfb674ced7ce79a5418604d`  
		Last Modified: Tue, 02 May 2023 22:00:25 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bbc52586409fb196178873d8e77e366b8d50a7a90d04a2dcae9de72462a9d8`  
		Last Modified: Tue, 02 May 2023 22:00:25 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:be5147bcfb055e76a233f75abe9ca8ba47e0234cdcb4dc7c01c786f512e1c1ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:9a71776060f27c67933547e751d2f9c743c9454ee388c776e52fb4f1d528677e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **560.8 MB (560828748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9e863115e8dc0c993aaaaf97b1b5bf4f8b10a6b585e42829a3ecf6e5750bd72`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:54:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:54:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:54:35 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:55:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 08:55:53 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:55:54 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 08:57:28 GMT
ENV ODOO_VERSION=15.0
# Tue, 02 May 2023 21:56:32 GMT
ARG ODOO_RELEASE=20230430
# Tue, 02 May 2023 21:56:32 GMT
ARG ODOO_SHA=af1128e5d8126e079a968ec22696a122965a4404
# Tue, 02 May 2023 21:57:44 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=af1128e5d8126e079a968ec22696a122965a4404
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 02 May 2023 21:57:48 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 02 May 2023 21:57:48 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 02 May 2023 21:57:49 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=af1128e5d8126e079a968ec22696a122965a4404
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 02 May 2023 21:57:49 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 02 May 2023 21:57:49 GMT
EXPOSE 8069 8071 8072
# Tue, 02 May 2023 21:57:49 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 02 May 2023 21:57:49 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 02 May 2023 21:57:49 GMT
USER odoo
# Tue, 02 May 2023 21:57:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 May 2023 21:57:49 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc072a51e9ff1e113fd7d7e6e812f69acee46b65fdb5e60e6a6977ab04867f8f`  
		Last Modified: Wed, 12 Apr 2023 09:02:33 GMT  
		Size: 220.3 MB (220298412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea2cf4d76c14443a63296eecd70cd09a9af720ca062d516b3f41535b435edf2`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 2.6 MB (2575214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfcc7225c9d8a7756bbe895737596be4bb564e0e7223b89b59cd40b96d7735b`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 449.3 KB (449266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b75cb0983bb9c95cbdcef8c652935381a57749a963ad260ad0f8561a884e83`  
		Last Modified: Tue, 02 May 2023 22:00:58 GMT  
		Size: 306.1 MB (306085168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a1a2df90b875f328a8aed26cc148fa15bdcc4183f5abbb67b98b191d36aaac`  
		Last Modified: Tue, 02 May 2023 22:00:25 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc84d813e6e2db5abe3bfcbb66ee5f97b58ed3701e4079d820d2428a618d5d8`  
		Last Modified: Tue, 02 May 2023 22:00:25 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716492ec80c1519b595ba5c90f6551617ff3a363dbfb674ced7ce79a5418604d`  
		Last Modified: Tue, 02 May 2023 22:00:25 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bbc52586409fb196178873d8e77e366b8d50a7a90d04a2dcae9de72462a9d8`  
		Last Modified: Tue, 02 May 2023 22:00:25 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:740e9028486134994b5969bd6017e82dfbf1596e53164ebd99cf69dbf7d28cea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:3431e17e222e798bd55a3119deb02655cab84bd23108513a6b9ade876801551f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.6 MB (569640746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd5fb87e48598118316e8fe34c5e08a1c4526cec064146e4b0823b8f35ed0f4e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:54:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:54:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:54:35 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:55:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 08:55:53 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:55:54 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 08:55:54 GMT
ENV ODOO_VERSION=16.0
# Tue, 02 May 2023 21:54:54 GMT
ARG ODOO_RELEASE=20230430
# Tue, 02 May 2023 21:54:54 GMT
ARG ODOO_SHA=1d8d64fec19fc1c31e13d9d9cdc4b127ba4e72cd
# Tue, 02 May 2023 21:56:16 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=1d8d64fec19fc1c31e13d9d9cdc4b127ba4e72cd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 02 May 2023 21:56:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 02 May 2023 21:56:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 02 May 2023 21:56:21 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=1d8d64fec19fc1c31e13d9d9cdc4b127ba4e72cd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 02 May 2023 21:56:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 02 May 2023 21:56:21 GMT
EXPOSE 8069 8071 8072
# Tue, 02 May 2023 21:56:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 02 May 2023 21:56:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 02 May 2023 21:56:21 GMT
USER odoo
# Tue, 02 May 2023 21:56:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 May 2023 21:56:21 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc072a51e9ff1e113fd7d7e6e812f69acee46b65fdb5e60e6a6977ab04867f8f`  
		Last Modified: Wed, 12 Apr 2023 09:02:33 GMT  
		Size: 220.3 MB (220298412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea2cf4d76c14443a63296eecd70cd09a9af720ca062d516b3f41535b435edf2`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 2.6 MB (2575214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfcc7225c9d8a7756bbe895737596be4bb564e0e7223b89b59cd40b96d7735b`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 449.3 KB (449266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce7ef10c4e2df0043c9f1072f391552144662bd86c945e038c973cf8653cfc`  
		Last Modified: Tue, 02 May 2023 22:00:15 GMT  
		Size: 314.9 MB (314897163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dca830e3cbcfd90f157756addbc6f39865b4bb4f7cf39cef7691e9b638bdca6`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b95106802f94f70c4273f56ada2a19fdf3619ac39ccbe833a6fe9c4438c175`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c637251cd62bc0e252f7078d240b1a833f99124b52f232c5c7a2977d8acc638`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cd1dd80e4751fb6b2f92b49bc191b07e6cf4147f2f68e9ea4c01b4b441a749`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:740e9028486134994b5969bd6017e82dfbf1596e53164ebd99cf69dbf7d28cea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:3431e17e222e798bd55a3119deb02655cab84bd23108513a6b9ade876801551f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.6 MB (569640746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd5fb87e48598118316e8fe34c5e08a1c4526cec064146e4b0823b8f35ed0f4e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:54:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:54:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:54:35 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:55:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 08:55:53 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:55:54 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 08:55:54 GMT
ENV ODOO_VERSION=16.0
# Tue, 02 May 2023 21:54:54 GMT
ARG ODOO_RELEASE=20230430
# Tue, 02 May 2023 21:54:54 GMT
ARG ODOO_SHA=1d8d64fec19fc1c31e13d9d9cdc4b127ba4e72cd
# Tue, 02 May 2023 21:56:16 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=1d8d64fec19fc1c31e13d9d9cdc4b127ba4e72cd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 02 May 2023 21:56:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 02 May 2023 21:56:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 02 May 2023 21:56:21 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=1d8d64fec19fc1c31e13d9d9cdc4b127ba4e72cd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 02 May 2023 21:56:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 02 May 2023 21:56:21 GMT
EXPOSE 8069 8071 8072
# Tue, 02 May 2023 21:56:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 02 May 2023 21:56:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 02 May 2023 21:56:21 GMT
USER odoo
# Tue, 02 May 2023 21:56:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 May 2023 21:56:21 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc072a51e9ff1e113fd7d7e6e812f69acee46b65fdb5e60e6a6977ab04867f8f`  
		Last Modified: Wed, 12 Apr 2023 09:02:33 GMT  
		Size: 220.3 MB (220298412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea2cf4d76c14443a63296eecd70cd09a9af720ca062d516b3f41535b435edf2`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 2.6 MB (2575214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfcc7225c9d8a7756bbe895737596be4bb564e0e7223b89b59cd40b96d7735b`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 449.3 KB (449266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce7ef10c4e2df0043c9f1072f391552144662bd86c945e038c973cf8653cfc`  
		Last Modified: Tue, 02 May 2023 22:00:15 GMT  
		Size: 314.9 MB (314897163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dca830e3cbcfd90f157756addbc6f39865b4bb4f7cf39cef7691e9b638bdca6`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b95106802f94f70c4273f56ada2a19fdf3619ac39ccbe833a6fe9c4438c175`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c637251cd62bc0e252f7078d240b1a833f99124b52f232c5c7a2977d8acc638`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cd1dd80e4751fb6b2f92b49bc191b07e6cf4147f2f68e9ea4c01b4b441a749`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:740e9028486134994b5969bd6017e82dfbf1596e53164ebd99cf69dbf7d28cea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:3431e17e222e798bd55a3119deb02655cab84bd23108513a6b9ade876801551f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.6 MB (569640746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd5fb87e48598118316e8fe34c5e08a1c4526cec064146e4b0823b8f35ed0f4e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:54:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:54:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:54:35 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:55:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 08:55:53 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:55:54 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 08:55:54 GMT
ENV ODOO_VERSION=16.0
# Tue, 02 May 2023 21:54:54 GMT
ARG ODOO_RELEASE=20230430
# Tue, 02 May 2023 21:54:54 GMT
ARG ODOO_SHA=1d8d64fec19fc1c31e13d9d9cdc4b127ba4e72cd
# Tue, 02 May 2023 21:56:16 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=1d8d64fec19fc1c31e13d9d9cdc4b127ba4e72cd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 02 May 2023 21:56:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 02 May 2023 21:56:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 02 May 2023 21:56:21 GMT
# ARGS: ODOO_RELEASE=20230430 ODOO_SHA=1d8d64fec19fc1c31e13d9d9cdc4b127ba4e72cd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 02 May 2023 21:56:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 02 May 2023 21:56:21 GMT
EXPOSE 8069 8071 8072
# Tue, 02 May 2023 21:56:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 02 May 2023 21:56:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 02 May 2023 21:56:21 GMT
USER odoo
# Tue, 02 May 2023 21:56:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 May 2023 21:56:21 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc072a51e9ff1e113fd7d7e6e812f69acee46b65fdb5e60e6a6977ab04867f8f`  
		Last Modified: Wed, 12 Apr 2023 09:02:33 GMT  
		Size: 220.3 MB (220298412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea2cf4d76c14443a63296eecd70cd09a9af720ca062d516b3f41535b435edf2`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 2.6 MB (2575214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfcc7225c9d8a7756bbe895737596be4bb564e0e7223b89b59cd40b96d7735b`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 449.3 KB (449266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce7ef10c4e2df0043c9f1072f391552144662bd86c945e038c973cf8653cfc`  
		Last Modified: Tue, 02 May 2023 22:00:15 GMT  
		Size: 314.9 MB (314897163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dca830e3cbcfd90f157756addbc6f39865b4bb4f7cf39cef7691e9b638bdca6`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b95106802f94f70c4273f56ada2a19fdf3619ac39ccbe833a6fe9c4438c175`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c637251cd62bc0e252f7078d240b1a833f99124b52f232c5c7a2977d8acc638`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cd1dd80e4751fb6b2f92b49bc191b07e6cf4147f2f68e9ea4c01b4b441a749`  
		Last Modified: Tue, 02 May 2023 21:59:40 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
