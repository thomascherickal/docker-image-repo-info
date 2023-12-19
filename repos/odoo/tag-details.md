<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `odoo`

-	[`odoo:15`](#odoo15)
-	[`odoo:15.0`](#odoo150)
-	[`odoo:16`](#odoo16)
-	[`odoo:16.0`](#odoo160)
-	[`odoo:17`](#odoo17)
-	[`odoo:17.0`](#odoo170)
-	[`odoo:latest`](#odoolatest)

## `odoo:15`

```console
$ docker pull odoo@sha256:8ea5660cf9b495c6ed243ec43dff446150d23fb31001895799ce68fd884326b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:b49a6a36647446c03995ccbc3dc8b89191532630e2c70f60c13f33d43958a680
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.1 MB (563146606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40b79033b6f4e1414bf629bebc33bbf3e3422925cbf175c255f20e73ca24eb1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:31:59 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 19 Dec 2023 02:31:59 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 19 Dec 2023 02:31:59 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 02:36:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 19 Dec 2023 02:36:09 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 02:36:11 GMT
RUN npm install -g rtlcss
# Tue, 19 Dec 2023 02:36:11 GMT
ENV ODOO_VERSION=15.0
# Tue, 19 Dec 2023 02:36:11 GMT
ARG ODOO_RELEASE=20231215
# Tue, 19 Dec 2023 02:36:11 GMT
ARG ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
# Tue, 19 Dec 2023 02:37:23 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 19 Dec 2023 02:37:27 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 19 Dec 2023 02:37:27 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 19 Dec 2023 02:37:28 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 19 Dec 2023 02:37:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 19 Dec 2023 02:37:28 GMT
EXPOSE 8069 8071 8072
# Tue, 19 Dec 2023 02:37:28 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 19 Dec 2023 02:37:28 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 19 Dec 2023 02:37:28 GMT
USER odoo
# Tue, 19 Dec 2023 02:37:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Dec 2023 02:37:29 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5d69e2605b2bccd82e2df0551e09fb8dc42447b60a2bc93b59aa605c3591c`  
		Last Modified: Tue, 19 Dec 2023 02:38:55 GMT  
		Size: 220.3 MB (220298621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ce1ef12f1e24c3c6833763c9d4f4161f145a75c469ea11118c3d89f26cb5da`  
		Last Modified: Tue, 19 Dec 2023 02:38:30 GMT  
		Size: 2.6 MB (2625731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8705a2eadf4550b011bb15758e88dfa0da3ae5e3cc226a651ae08f0cccd49ae`  
		Last Modified: Tue, 19 Dec 2023 02:38:30 GMT  
		Size: 459.6 KB (459552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd1b81bb48d56d2bb4db13688b2ddb704cfc4f119dbfc1907fafad7e0c743f`  
		Last Modified: Tue, 19 Dec 2023 02:39:03 GMT  
		Size: 308.3 MB (308342366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e5f9ec49a7d3978dd565ae9ec535442d8ae10ee8c5243c08b4417a1ed6776`  
		Last Modified: Tue, 19 Dec 2023 02:38:27 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9389b4595a453b04a2cfe23d5b168f224d5a397211567aba2cd6f17eac9bf1a7`  
		Last Modified: Tue, 19 Dec 2023 02:38:28 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67297242529db3490bb614328dfbc7bf09ab2f54a0605922239bc2dc559d682e`  
		Last Modified: Tue, 19 Dec 2023 02:38:27 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234c05454ece8adb50c55bf3a375658964f6993ac726fa0cc0cddc2e9abbe302`  
		Last Modified: Tue, 19 Dec 2023 02:38:27 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:8ea5660cf9b495c6ed243ec43dff446150d23fb31001895799ce68fd884326b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:b49a6a36647446c03995ccbc3dc8b89191532630e2c70f60c13f33d43958a680
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.1 MB (563146606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40b79033b6f4e1414bf629bebc33bbf3e3422925cbf175c255f20e73ca24eb1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:31:59 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 19 Dec 2023 02:31:59 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 19 Dec 2023 02:31:59 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 02:36:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 19 Dec 2023 02:36:09 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 02:36:11 GMT
RUN npm install -g rtlcss
# Tue, 19 Dec 2023 02:36:11 GMT
ENV ODOO_VERSION=15.0
# Tue, 19 Dec 2023 02:36:11 GMT
ARG ODOO_RELEASE=20231215
# Tue, 19 Dec 2023 02:36:11 GMT
ARG ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
# Tue, 19 Dec 2023 02:37:23 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 19 Dec 2023 02:37:27 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 19 Dec 2023 02:37:27 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 19 Dec 2023 02:37:28 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 19 Dec 2023 02:37:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 19 Dec 2023 02:37:28 GMT
EXPOSE 8069 8071 8072
# Tue, 19 Dec 2023 02:37:28 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 19 Dec 2023 02:37:28 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 19 Dec 2023 02:37:28 GMT
USER odoo
# Tue, 19 Dec 2023 02:37:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Dec 2023 02:37:29 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5d69e2605b2bccd82e2df0551e09fb8dc42447b60a2bc93b59aa605c3591c`  
		Last Modified: Tue, 19 Dec 2023 02:38:55 GMT  
		Size: 220.3 MB (220298621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ce1ef12f1e24c3c6833763c9d4f4161f145a75c469ea11118c3d89f26cb5da`  
		Last Modified: Tue, 19 Dec 2023 02:38:30 GMT  
		Size: 2.6 MB (2625731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8705a2eadf4550b011bb15758e88dfa0da3ae5e3cc226a651ae08f0cccd49ae`  
		Last Modified: Tue, 19 Dec 2023 02:38:30 GMT  
		Size: 459.6 KB (459552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd1b81bb48d56d2bb4db13688b2ddb704cfc4f119dbfc1907fafad7e0c743f`  
		Last Modified: Tue, 19 Dec 2023 02:39:03 GMT  
		Size: 308.3 MB (308342366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e5f9ec49a7d3978dd565ae9ec535442d8ae10ee8c5243c08b4417a1ed6776`  
		Last Modified: Tue, 19 Dec 2023 02:38:27 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9389b4595a453b04a2cfe23d5b168f224d5a397211567aba2cd6f17eac9bf1a7`  
		Last Modified: Tue, 19 Dec 2023 02:38:28 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67297242529db3490bb614328dfbc7bf09ab2f54a0605922239bc2dc559d682e`  
		Last Modified: Tue, 19 Dec 2023 02:38:27 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234c05454ece8adb50c55bf3a375658964f6993ac726fa0cc0cddc2e9abbe302`  
		Last Modified: Tue, 19 Dec 2023 02:38:27 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:db2136489ab4f902bb4cf02d22d53ed154241f9fdc1c962d3f57c0c0727e8757
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:04dbf90b06153439c100db5cb5593a15e092424d74dcb3bbcf019dd634323dbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.5 MB (577504557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec80163e24b61bdab6e0a06fc808783d34808dd2750c8b763be49cb4c2ac8f96`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:31:59 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 19 Dec 2023 02:31:59 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 19 Dec 2023 02:31:59 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 02:31:59 GMT
ARG TARGETARCH
# Tue, 19 Dec 2023 02:33:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 19 Dec 2023 02:33:22 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 02:33:23 GMT
RUN npm install -g rtlcss
# Tue, 19 Dec 2023 02:33:24 GMT
ENV ODOO_VERSION=16.0
# Tue, 19 Dec 2023 02:33:24 GMT
ARG ODOO_RELEASE=20231215
# Tue, 19 Dec 2023 02:33:24 GMT
ARG ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
# Tue, 19 Dec 2023 02:34:46 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 19 Dec 2023 02:34:50 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 19 Dec 2023 02:34:50 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 19 Dec 2023 02:34:51 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 19 Dec 2023 02:34:51 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 19 Dec 2023 02:34:51 GMT
EXPOSE 8069 8071 8072
# Tue, 19 Dec 2023 02:34:51 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 19 Dec 2023 02:34:51 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 19 Dec 2023 02:34:51 GMT
USER odoo
# Tue, 19 Dec 2023 02:34:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Dec 2023 02:34:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21397601f383856bad1be67c360c70e98e2164b6d334345340ef77aab8d01277`  
		Last Modified: Tue, 19 Dec 2023 02:38:06 GMT  
		Size: 219.6 MB (219606068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a886ed10d0ec268c641a802cb8a7cd4bb0276e9f273a6d084fb8d663d99492e9`  
		Last Modified: Tue, 19 Dec 2023 02:37:41 GMT  
		Size: 2.6 MB (2629859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3109584422e3b3ffbbfc68a4bf5323d9a355db5e6aeeeefbd90a419167213c1`  
		Last Modified: Tue, 19 Dec 2023 02:37:41 GMT  
		Size: 459.6 KB (459559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5750f89ea7c001109085bc36618d43c52d56987b70ddd8aefa86f7ce9233ddd`  
		Last Modified: Tue, 19 Dec 2023 02:38:18 GMT  
		Size: 323.4 MB (323388735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ad9aa1c9315b001dcf3f34b2fa658943884b52e4b4c1d49cd9b2388a31b89c`  
		Last Modified: Tue, 19 Dec 2023 02:37:39 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f05d1be462172fd30bb8f4c7fd5dd9a3732624d591a8c5b7478ac02d5011ea0`  
		Last Modified: Tue, 19 Dec 2023 02:37:39 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99914033492ddc60d464b998e4d6b7d9755aa6eba5024089f9482d3e878c2ff`  
		Last Modified: Tue, 19 Dec 2023 02:37:39 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2067402a6dc12ad747ec9c63ee990adc647bc54af01153ae380b821cd8ba400d`  
		Last Modified: Tue, 19 Dec 2023 02:37:39 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:7aaf28e5e60643eae9be3876a4e188d54de5168921ff0c64e6f4b792c5ad68ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.1 MB (573089616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b648ff1ff0b128b2f2fdf31e0286027dada65e6448b5eb31c656eed3ae0bd6f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:24:02 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 21 Nov 2023 10:24:03 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 21 Nov 2023 10:24:03 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 10:24:03 GMT
ARG TARGETARCH
# Tue, 21 Nov 2023 10:25:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 21 Nov 2023 10:25:14 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:25:16 GMT
RUN npm install -g rtlcss
# Tue, 21 Nov 2023 10:25:16 GMT
ENV ODOO_VERSION=16.0
# Fri, 15 Dec 2023 20:02:45 GMT
ARG ODOO_RELEASE=20231215
# Fri, 15 Dec 2023 20:02:45 GMT
ARG ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
# Fri, 15 Dec 2023 20:03:57 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 15 Dec 2023 20:04:04 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 15 Dec 2023 20:04:05 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 15 Dec 2023 20:04:05 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 15 Dec 2023 20:04:05 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 15 Dec 2023 20:04:05 GMT
EXPOSE 8069 8071 8072
# Fri, 15 Dec 2023 20:04:05 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 15 Dec 2023 20:04:05 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 15 Dec 2023 20:04:05 GMT
USER odoo
# Fri, 15 Dec 2023 20:04:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Dec 2023 20:04:06 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729ab9b0a137551e75078132a976e9e490b4eb1fc07fe87beb915c8f0be0988b`  
		Last Modified: Tue, 21 Nov 2023 10:27:07 GMT  
		Size: 216.9 MB (216908243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8451f82e1e1d62729c32c647a135084aeea39e2eecdfab5f468e549adbe642a1`  
		Last Modified: Tue, 21 Nov 2023 10:26:50 GMT  
		Size: 2.6 MB (2634860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006d5b0160b4770a0c5d2bbe136fec01bf9daa283a549aceba5449dcc1b0eb7a`  
		Last Modified: Tue, 21 Nov 2023 10:26:49 GMT  
		Size: 459.5 KB (459492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b8350a820edfd835b5c7481c9b0739dbef2f4ddb85e9ae38ea8145c556e9b6`  
		Last Modified: Fri, 15 Dec 2023 20:05:24 GMT  
		Size: 323.0 MB (323020435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561d7ea3af6577c0cd7334b3ec34f9b3791945cfed5ef1091d9de8bd50d27f4e`  
		Last Modified: Fri, 15 Dec 2023 20:04:54 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db97d2f3e9fdc78ab2d82c8cb440efa79a009ca91fe5389c1075f5658668996a`  
		Last Modified: Fri, 15 Dec 2023 20:04:55 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8724d220e645666b7fc774a032db1ff716d6d9ce6438d2042e3c7ef3080c65e7`  
		Last Modified: Fri, 15 Dec 2023 20:04:54 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692ca9bc7bd9ae525d364ca6e09f64014ff0047f7b607bd362194e473ba7071f`  
		Last Modified: Fri, 15 Dec 2023 20:04:54 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16` - linux; ppc64le

```console
$ docker pull odoo@sha256:24c67dadf8be5c956cd25f59f1d72980a44d81badb38905ecb2f37f0633c0216
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.0 MB (592017390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af1b2371017686992430eb718879dea7368f7f828f2d298a4b9e7e3deaed153c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:37:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 21 Nov 2023 04:37:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 21 Nov 2023 04:37:34 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:37:34 GMT
ARG TARGETARCH
# Tue, 21 Nov 2023 04:40:16 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 21 Nov 2023 04:40:36 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 04:40:39 GMT
RUN npm install -g rtlcss
# Tue, 21 Nov 2023 04:40:39 GMT
ENV ODOO_VERSION=16.0
# Fri, 15 Dec 2023 19:38:47 GMT
ARG ODOO_RELEASE=20231215
# Fri, 15 Dec 2023 19:38:47 GMT
ARG ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
# Fri, 15 Dec 2023 19:41:07 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 15 Dec 2023 19:41:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 15 Dec 2023 19:41:22 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 15 Dec 2023 19:41:23 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 15 Dec 2023 19:41:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 15 Dec 2023 19:41:24 GMT
EXPOSE 8069 8071 8072
# Fri, 15 Dec 2023 19:41:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 15 Dec 2023 19:41:25 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 15 Dec 2023 19:41:25 GMT
USER odoo
# Fri, 15 Dec 2023 19:41:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Dec 2023 19:41:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9412e97f56973d23e9dad0c3fcfd85b2446ed64817cf494fd8c0d7e8a361d2b6`  
		Last Modified: Tue, 21 Nov 2023 04:44:49 GMT  
		Size: 228.6 MB (228598187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a33d7cd62e6b8c2d2d1f1384daa821c3fbc171b6a3fb9296592372045d33751`  
		Last Modified: Tue, 21 Nov 2023 04:44:20 GMT  
		Size: 2.9 MB (2875641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d656925877eaa583e8f5dde6fd482750adc09d25cdd8ac87e6345c0b308d1b97`  
		Last Modified: Tue, 21 Nov 2023 04:44:19 GMT  
		Size: 459.5 KB (459505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f8fa92895b64c4834b7ff3ee299080bc3976e7ea85211a4ea0999605f795bc`  
		Last Modified: Fri, 15 Dec 2023 19:43:33 GMT  
		Size: 324.8 MB (324787864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aa28b20f0f24f94ea91818d99d75eeef6dd040227466e246194e6fed65cb77`  
		Last Modified: Fri, 15 Dec 2023 19:42:50 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2cbb9d1b434cb777d1f65623a9ea12dd9b109dd3e5be2c6da9dd89f0b1bc086`  
		Last Modified: Fri, 15 Dec 2023 19:42:49 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0916130b01370e099a5e97fd34804a9cff2b6ca6a3caa398c607e7d543f473bb`  
		Last Modified: Fri, 15 Dec 2023 19:42:50 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab79c5f227822466354cf40ccebe0bf09cdd6f32cec479e7234a2a73f9ff410`  
		Last Modified: Fri, 15 Dec 2023 19:42:50 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:db2136489ab4f902bb4cf02d22d53ed154241f9fdc1c962d3f57c0c0727e8757
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:04dbf90b06153439c100db5cb5593a15e092424d74dcb3bbcf019dd634323dbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.5 MB (577504557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec80163e24b61bdab6e0a06fc808783d34808dd2750c8b763be49cb4c2ac8f96`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:31:59 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 19 Dec 2023 02:31:59 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 19 Dec 2023 02:31:59 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 02:31:59 GMT
ARG TARGETARCH
# Tue, 19 Dec 2023 02:33:11 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 19 Dec 2023 02:33:22 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 02:33:23 GMT
RUN npm install -g rtlcss
# Tue, 19 Dec 2023 02:33:24 GMT
ENV ODOO_VERSION=16.0
# Tue, 19 Dec 2023 02:33:24 GMT
ARG ODOO_RELEASE=20231215
# Tue, 19 Dec 2023 02:33:24 GMT
ARG ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
# Tue, 19 Dec 2023 02:34:46 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 19 Dec 2023 02:34:50 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 19 Dec 2023 02:34:50 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 19 Dec 2023 02:34:51 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 19 Dec 2023 02:34:51 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 19 Dec 2023 02:34:51 GMT
EXPOSE 8069 8071 8072
# Tue, 19 Dec 2023 02:34:51 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 19 Dec 2023 02:34:51 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 19 Dec 2023 02:34:51 GMT
USER odoo
# Tue, 19 Dec 2023 02:34:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Dec 2023 02:34:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21397601f383856bad1be67c360c70e98e2164b6d334345340ef77aab8d01277`  
		Last Modified: Tue, 19 Dec 2023 02:38:06 GMT  
		Size: 219.6 MB (219606068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a886ed10d0ec268c641a802cb8a7cd4bb0276e9f273a6d084fb8d663d99492e9`  
		Last Modified: Tue, 19 Dec 2023 02:37:41 GMT  
		Size: 2.6 MB (2629859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3109584422e3b3ffbbfc68a4bf5323d9a355db5e6aeeeefbd90a419167213c1`  
		Last Modified: Tue, 19 Dec 2023 02:37:41 GMT  
		Size: 459.6 KB (459559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5750f89ea7c001109085bc36618d43c52d56987b70ddd8aefa86f7ce9233ddd`  
		Last Modified: Tue, 19 Dec 2023 02:38:18 GMT  
		Size: 323.4 MB (323388735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ad9aa1c9315b001dcf3f34b2fa658943884b52e4b4c1d49cd9b2388a31b89c`  
		Last Modified: Tue, 19 Dec 2023 02:37:39 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f05d1be462172fd30bb8f4c7fd5dd9a3732624d591a8c5b7478ac02d5011ea0`  
		Last Modified: Tue, 19 Dec 2023 02:37:39 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99914033492ddc60d464b998e4d6b7d9755aa6eba5024089f9482d3e878c2ff`  
		Last Modified: Tue, 19 Dec 2023 02:37:39 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2067402a6dc12ad747ec9c63ee990adc647bc54af01153ae380b821cd8ba400d`  
		Last Modified: Tue, 19 Dec 2023 02:37:39 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16.0` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:7aaf28e5e60643eae9be3876a4e188d54de5168921ff0c64e6f4b792c5ad68ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.1 MB (573089616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b648ff1ff0b128b2f2fdf31e0286027dada65e6448b5eb31c656eed3ae0bd6f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:24:02 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 21 Nov 2023 10:24:03 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 21 Nov 2023 10:24:03 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 10:24:03 GMT
ARG TARGETARCH
# Tue, 21 Nov 2023 10:25:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 21 Nov 2023 10:25:14 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:25:16 GMT
RUN npm install -g rtlcss
# Tue, 21 Nov 2023 10:25:16 GMT
ENV ODOO_VERSION=16.0
# Fri, 15 Dec 2023 20:02:45 GMT
ARG ODOO_RELEASE=20231215
# Fri, 15 Dec 2023 20:02:45 GMT
ARG ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
# Fri, 15 Dec 2023 20:03:57 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 15 Dec 2023 20:04:04 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 15 Dec 2023 20:04:05 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 15 Dec 2023 20:04:05 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 15 Dec 2023 20:04:05 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 15 Dec 2023 20:04:05 GMT
EXPOSE 8069 8071 8072
# Fri, 15 Dec 2023 20:04:05 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 15 Dec 2023 20:04:05 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 15 Dec 2023 20:04:05 GMT
USER odoo
# Fri, 15 Dec 2023 20:04:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Dec 2023 20:04:06 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729ab9b0a137551e75078132a976e9e490b4eb1fc07fe87beb915c8f0be0988b`  
		Last Modified: Tue, 21 Nov 2023 10:27:07 GMT  
		Size: 216.9 MB (216908243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8451f82e1e1d62729c32c647a135084aeea39e2eecdfab5f468e549adbe642a1`  
		Last Modified: Tue, 21 Nov 2023 10:26:50 GMT  
		Size: 2.6 MB (2634860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006d5b0160b4770a0c5d2bbe136fec01bf9daa283a549aceba5449dcc1b0eb7a`  
		Last Modified: Tue, 21 Nov 2023 10:26:49 GMT  
		Size: 459.5 KB (459492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b8350a820edfd835b5c7481c9b0739dbef2f4ddb85e9ae38ea8145c556e9b6`  
		Last Modified: Fri, 15 Dec 2023 20:05:24 GMT  
		Size: 323.0 MB (323020435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561d7ea3af6577c0cd7334b3ec34f9b3791945cfed5ef1091d9de8bd50d27f4e`  
		Last Modified: Fri, 15 Dec 2023 20:04:54 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db97d2f3e9fdc78ab2d82c8cb440efa79a009ca91fe5389c1075f5658668996a`  
		Last Modified: Fri, 15 Dec 2023 20:04:55 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8724d220e645666b7fc774a032db1ff716d6d9ce6438d2042e3c7ef3080c65e7`  
		Last Modified: Fri, 15 Dec 2023 20:04:54 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692ca9bc7bd9ae525d364ca6e09f64014ff0047f7b607bd362194e473ba7071f`  
		Last Modified: Fri, 15 Dec 2023 20:04:54 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16.0` - linux; ppc64le

```console
$ docker pull odoo@sha256:24c67dadf8be5c956cd25f59f1d72980a44d81badb38905ecb2f37f0633c0216
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.0 MB (592017390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af1b2371017686992430eb718879dea7368f7f828f2d298a4b9e7e3deaed153c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:37:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 21 Nov 2023 04:37:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 21 Nov 2023 04:37:34 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:37:34 GMT
ARG TARGETARCH
# Tue, 21 Nov 2023 04:40:16 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 21 Nov 2023 04:40:36 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 04:40:39 GMT
RUN npm install -g rtlcss
# Tue, 21 Nov 2023 04:40:39 GMT
ENV ODOO_VERSION=16.0
# Fri, 15 Dec 2023 19:38:47 GMT
ARG ODOO_RELEASE=20231215
# Fri, 15 Dec 2023 19:38:47 GMT
ARG ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
# Fri, 15 Dec 2023 19:41:07 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 15 Dec 2023 19:41:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 15 Dec 2023 19:41:22 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 15 Dec 2023 19:41:23 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 15 Dec 2023 19:41:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 15 Dec 2023 19:41:24 GMT
EXPOSE 8069 8071 8072
# Fri, 15 Dec 2023 19:41:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 15 Dec 2023 19:41:25 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 15 Dec 2023 19:41:25 GMT
USER odoo
# Fri, 15 Dec 2023 19:41:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Dec 2023 19:41:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9412e97f56973d23e9dad0c3fcfd85b2446ed64817cf494fd8c0d7e8a361d2b6`  
		Last Modified: Tue, 21 Nov 2023 04:44:49 GMT  
		Size: 228.6 MB (228598187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a33d7cd62e6b8c2d2d1f1384daa821c3fbc171b6a3fb9296592372045d33751`  
		Last Modified: Tue, 21 Nov 2023 04:44:20 GMT  
		Size: 2.9 MB (2875641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d656925877eaa583e8f5dde6fd482750adc09d25cdd8ac87e6345c0b308d1b97`  
		Last Modified: Tue, 21 Nov 2023 04:44:19 GMT  
		Size: 459.5 KB (459505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f8fa92895b64c4834b7ff3ee299080bc3976e7ea85211a4ea0999605f795bc`  
		Last Modified: Fri, 15 Dec 2023 19:43:33 GMT  
		Size: 324.8 MB (324787864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29aa28b20f0f24f94ea91818d99d75eeef6dd040227466e246194e6fed65cb77`  
		Last Modified: Fri, 15 Dec 2023 19:42:50 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2cbb9d1b434cb777d1f65623a9ea12dd9b109dd3e5be2c6da9dd89f0b1bc086`  
		Last Modified: Fri, 15 Dec 2023 19:42:49 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0916130b01370e099a5e97fd34804a9cff2b6ca6a3caa398c607e7d543f473bb`  
		Last Modified: Fri, 15 Dec 2023 19:42:50 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab79c5f227822466354cf40ccebe0bf09cdd6f32cec479e7234a2a73f9ff410`  
		Last Modified: Fri, 15 Dec 2023 19:42:50 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:17`

```console
$ docker pull odoo@sha256:ad3f0906fc4c3bba4e2a36ccb193cc548b308cf3cc45c7e87b7df4f6a2aa3c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:17` - linux; amd64

```console
$ docker pull odoo@sha256:30b6a127a18ac6af593b7a56602f112b7b4cb260001f136e445110bee4ca23fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.8 MB (593757757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29220a79cacc7f2e4a59d9f60eef8bf84df39f34338351b6ef73963c973671d3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:29:57 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 16 Dec 2023 09:29:57 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 16 Dec 2023 09:29:57 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Dec 2023 09:29:57 GMT
ARG TARGETARCH
# Sat, 16 Dec 2023 09:32:06 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 16 Dec 2023 09:32:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:32:18 GMT
RUN npm install -g rtlcss
# Sat, 16 Dec 2023 09:32:18 GMT
ENV ODOO_VERSION=17.0
# Sat, 16 Dec 2023 09:32:18 GMT
ARG ODOO_RELEASE=20231215
# Sat, 16 Dec 2023 09:32:18 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Sat, 16 Dec 2023 09:33:48 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 16 Dec 2023 09:33:53 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 16 Dec 2023 09:33:53 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 16 Dec 2023 09:33:53 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 16 Dec 2023 09:33:53 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 16 Dec 2023 09:33:53 GMT
EXPOSE 8069 8071 8072
# Sat, 16 Dec 2023 09:33:54 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 16 Dec 2023 09:33:54 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 16 Dec 2023 09:33:54 GMT
USER odoo
# Sat, 16 Dec 2023 09:33:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Dec 2023 09:33:54 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89681bc3d92fa58300c17f37a8c00221342b77325e00deb20e71ea410071d500`  
		Last Modified: Sat, 16 Dec 2023 09:34:46 GMT  
		Size: 233.7 MB (233730172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a3dc4306b241f9806eface9e5fe3c10ef771e41f03509a141414da8bb7c04`  
		Last Modified: Sat, 16 Dec 2023 09:34:19 GMT  
		Size: 2.5 MB (2526485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746699b2b8c3aebf90f574a4692f492e2e617506c92d7a00874d79e4fddaf014`  
		Last Modified: Sat, 16 Dec 2023 09:34:19 GMT  
		Size: 461.1 KB (461135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b67a8d3db9081841dc9d808b5e78e43a7e30a435eb0f57330a1de521fcfc9`  
		Last Modified: Sat, 16 Dec 2023 09:34:55 GMT  
		Size: 326.6 MB (326590922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f2852418032bfe4c1c35bfa16ad612d51baddd3818f8af6895d2f740da6277`  
		Last Modified: Sat, 16 Dec 2023 09:34:17 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257ebd1f11921d56dcf37b6e4a3c58eb50cc3213e71bce9d10abbfad992f28f9`  
		Last Modified: Sat, 16 Dec 2023 09:34:17 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9233a18d9fd9ba41414598ce2a94bc9ff23e95f0f703dbf1a5cbbfb869b2f90`  
		Last Modified: Sat, 16 Dec 2023 09:34:17 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fec152432475ca632e2e45f4b2bf57245f6ed21fe0fb35820ba0a2319bccaa`  
		Last Modified: Sat, 16 Dec 2023 09:34:16 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:45033b789835cff1c70920db2280ee06659916f9d565dfa18d8d11d64f89a21a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588711441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7eb80af58fee94d481b5000a5963ae21b2dd2a611b6ed247c9e46630be35b2b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Dec 2023 11:41:50 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:41:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:41:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:41:51 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:41:54 GMT
ADD file:50f947da69b3b6c63695be9c49eee16f7a7dcdecdceb51e5bee1609b845bf483 in / 
# Tue, 12 Dec 2023 11:41:54 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:59:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 16 Dec 2023 10:59:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 16 Dec 2023 10:59:32 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Dec 2023 10:59:32 GMT
ARG TARGETARCH
# Sat, 16 Dec 2023 11:01:54 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 16 Dec 2023 11:02:08 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:02:09 GMT
RUN npm install -g rtlcss
# Sat, 16 Dec 2023 11:02:09 GMT
ENV ODOO_VERSION=17.0
# Sat, 16 Dec 2023 11:02:09 GMT
ARG ODOO_RELEASE=20231215
# Sat, 16 Dec 2023 11:02:09 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Sat, 16 Dec 2023 11:04:00 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 16 Dec 2023 11:04:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 16 Dec 2023 11:04:07 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 16 Dec 2023 11:04:08 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 16 Dec 2023 11:04:08 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 16 Dec 2023 11:04:08 GMT
EXPOSE 8069 8071 8072
# Sat, 16 Dec 2023 11:04:08 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 16 Dec 2023 11:04:08 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 16 Dec 2023 11:04:08 GMT
USER odoo
# Sat, 16 Dec 2023 11:04:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Dec 2023 11:04:08 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7734efb8b826f955c6a3bb51d7c84cb262d0e600ea3980f5bce69fa7f4f92d24`  
		Last Modified: Tue, 12 Dec 2023 16:00:15 GMT  
		Size: 28.4 MB (28400282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed064f4459a4f1ab48040e16f6b55972797bd014de0d33737d676d7a1a25db4`  
		Last Modified: Sat, 16 Dec 2023 11:04:40 GMT  
		Size: 231.1 MB (231107542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217c6a3bbcbbb21c659f79f47bd7f96d743d57cfd0fe0b1678b81f7ff769a77`  
		Last Modified: Sat, 16 Dec 2023 11:04:20 GMT  
		Size: 2.5 MB (2520464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce39a7573fc5d23b0ecb7a2dc95f9c6c6ea441c6712f6c192b2807e2aa72feb`  
		Last Modified: Sat, 16 Dec 2023 11:04:20 GMT  
		Size: 461.1 KB (461075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d4aa89e67bac0554e241b242eb40964169e55a857220a7ce13ee3a59882ecd`  
		Last Modified: Sat, 16 Dec 2023 11:04:47 GMT  
		Size: 326.2 MB (326219611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984169afba305c7e0dbb5f8be73e8ffc1d3d118be93d882307cb5d888bb1fb5a`  
		Last Modified: Sat, 16 Dec 2023 11:04:17 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1f1e4dc45e16096cc8251bb9060adf0abb8f07a1ec363cd457ac28b2c08422`  
		Last Modified: Sat, 16 Dec 2023 11:04:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad914934c1124d6de9bc06d30871a9eb568c5f305beabe0589784f269cbe87a`  
		Last Modified: Sat, 16 Dec 2023 11:04:17 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab065eddb817943bba284eb1dacbfb531e9f03e37645f79822d53fb41cee7c`  
		Last Modified: Sat, 16 Dec 2023 11:04:18 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17` - linux; ppc64le

```console
$ docker pull odoo@sha256:d2d7d75efa6ff5e1d80130e274dc5f6191b166ac34b22d0f5f23e2915221245f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.6 MB (610570813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7591462b0a8b8d4c5453a280fa686f8e29ce6a1bb2689f4738bfbb53befb5376`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Dec 2023 11:43:51 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:43:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:43:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:43:52 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:43:55 GMT
ADD file:bda128b553d54e39b55daceea1f0ad351c73f83835bbf65d10e5af879ce6fee7 in / 
# Tue, 12 Dec 2023 11:43:56 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:18:22 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 16 Dec 2023 11:18:22 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 16 Dec 2023 11:18:23 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Dec 2023 11:18:23 GMT
ARG TARGETARCH
# Sat, 16 Dec 2023 11:22:08 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 16 Dec 2023 11:22:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:22:30 GMT
RUN npm install -g rtlcss
# Sat, 16 Dec 2023 11:22:30 GMT
ENV ODOO_VERSION=17.0
# Sat, 16 Dec 2023 11:22:31 GMT
ARG ODOO_RELEASE=20231215
# Sat, 16 Dec 2023 11:22:31 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Sat, 16 Dec 2023 11:25:16 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 16 Dec 2023 11:25:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 16 Dec 2023 11:25:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 16 Dec 2023 11:25:33 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 16 Dec 2023 11:25:33 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 16 Dec 2023 11:25:34 GMT
EXPOSE 8069 8071 8072
# Sat, 16 Dec 2023 11:25:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 16 Dec 2023 11:25:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 16 Dec 2023 11:25:35 GMT
USER odoo
# Sat, 16 Dec 2023 11:25:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Dec 2023 11:25:36 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7775720178c79208fc0d1b977c06891ef7230f39bc02e948d233c49f8a202fcf`  
		Last Modified: Sat, 16 Dec 2023 10:35:18 GMT  
		Size: 35.7 MB (35655287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc829e9bac0988cf5b8041cc64556998568034e96cd72e93b700c2ac4d3f6330`  
		Last Modified: Sat, 16 Dec 2023 11:26:30 GMT  
		Size: 243.3 MB (243296411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77915009472ee87b9142650dd27d791d648dc1cb35fd84a5b5e471802c2476ab`  
		Last Modified: Sat, 16 Dec 2023 11:25:58 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b76a07b6810b56620d5e557ab7a8e64c61a46a1af3a1452dc22677cd585e67`  
		Last Modified: Sat, 16 Dec 2023 11:25:58 GMT  
		Size: 461.2 KB (461168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84004797700930196d2fec76610101e813f5d61f7209f55db42f7dc6eb05ae4b`  
		Last Modified: Sat, 16 Dec 2023 11:26:39 GMT  
		Size: 328.4 MB (328352223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5436a4615a439344a39b355d42d22a263e5ed3be8512bc75716f6350bd152bdf`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6da7f44ddebb885659331932de9332285b0e1cc7501b85e9230e6ed0ca9951`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652edc554772ab19cfefc24f5abdd2e74c95718c52086583b31e99e4df450ee0`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545f4de9ba62bd8bda73a2b2a1e98abbf4e0705f19d02b4fbdd8d6a9d7ea251`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:17.0`

```console
$ docker pull odoo@sha256:ad3f0906fc4c3bba4e2a36ccb193cc548b308cf3cc45c7e87b7df4f6a2aa3c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:17.0` - linux; amd64

```console
$ docker pull odoo@sha256:30b6a127a18ac6af593b7a56602f112b7b4cb260001f136e445110bee4ca23fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.8 MB (593757757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29220a79cacc7f2e4a59d9f60eef8bf84df39f34338351b6ef73963c973671d3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:29:57 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 16 Dec 2023 09:29:57 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 16 Dec 2023 09:29:57 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Dec 2023 09:29:57 GMT
ARG TARGETARCH
# Sat, 16 Dec 2023 09:32:06 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 16 Dec 2023 09:32:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:32:18 GMT
RUN npm install -g rtlcss
# Sat, 16 Dec 2023 09:32:18 GMT
ENV ODOO_VERSION=17.0
# Sat, 16 Dec 2023 09:32:18 GMT
ARG ODOO_RELEASE=20231215
# Sat, 16 Dec 2023 09:32:18 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Sat, 16 Dec 2023 09:33:48 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 16 Dec 2023 09:33:53 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 16 Dec 2023 09:33:53 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 16 Dec 2023 09:33:53 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 16 Dec 2023 09:33:53 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 16 Dec 2023 09:33:53 GMT
EXPOSE 8069 8071 8072
# Sat, 16 Dec 2023 09:33:54 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 16 Dec 2023 09:33:54 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 16 Dec 2023 09:33:54 GMT
USER odoo
# Sat, 16 Dec 2023 09:33:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Dec 2023 09:33:54 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89681bc3d92fa58300c17f37a8c00221342b77325e00deb20e71ea410071d500`  
		Last Modified: Sat, 16 Dec 2023 09:34:46 GMT  
		Size: 233.7 MB (233730172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a3dc4306b241f9806eface9e5fe3c10ef771e41f03509a141414da8bb7c04`  
		Last Modified: Sat, 16 Dec 2023 09:34:19 GMT  
		Size: 2.5 MB (2526485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746699b2b8c3aebf90f574a4692f492e2e617506c92d7a00874d79e4fddaf014`  
		Last Modified: Sat, 16 Dec 2023 09:34:19 GMT  
		Size: 461.1 KB (461135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b67a8d3db9081841dc9d808b5e78e43a7e30a435eb0f57330a1de521fcfc9`  
		Last Modified: Sat, 16 Dec 2023 09:34:55 GMT  
		Size: 326.6 MB (326590922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f2852418032bfe4c1c35bfa16ad612d51baddd3818f8af6895d2f740da6277`  
		Last Modified: Sat, 16 Dec 2023 09:34:17 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257ebd1f11921d56dcf37b6e4a3c58eb50cc3213e71bce9d10abbfad992f28f9`  
		Last Modified: Sat, 16 Dec 2023 09:34:17 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9233a18d9fd9ba41414598ce2a94bc9ff23e95f0f703dbf1a5cbbfb869b2f90`  
		Last Modified: Sat, 16 Dec 2023 09:34:17 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fec152432475ca632e2e45f4b2bf57245f6ed21fe0fb35820ba0a2319bccaa`  
		Last Modified: Sat, 16 Dec 2023 09:34:16 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17.0` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:45033b789835cff1c70920db2280ee06659916f9d565dfa18d8d11d64f89a21a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588711441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7eb80af58fee94d481b5000a5963ae21b2dd2a611b6ed247c9e46630be35b2b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Dec 2023 11:41:50 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:41:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:41:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:41:51 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:41:54 GMT
ADD file:50f947da69b3b6c63695be9c49eee16f7a7dcdecdceb51e5bee1609b845bf483 in / 
# Tue, 12 Dec 2023 11:41:54 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:59:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 16 Dec 2023 10:59:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 16 Dec 2023 10:59:32 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Dec 2023 10:59:32 GMT
ARG TARGETARCH
# Sat, 16 Dec 2023 11:01:54 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 16 Dec 2023 11:02:08 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:02:09 GMT
RUN npm install -g rtlcss
# Sat, 16 Dec 2023 11:02:09 GMT
ENV ODOO_VERSION=17.0
# Sat, 16 Dec 2023 11:02:09 GMT
ARG ODOO_RELEASE=20231215
# Sat, 16 Dec 2023 11:02:09 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Sat, 16 Dec 2023 11:04:00 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 16 Dec 2023 11:04:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 16 Dec 2023 11:04:07 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 16 Dec 2023 11:04:08 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 16 Dec 2023 11:04:08 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 16 Dec 2023 11:04:08 GMT
EXPOSE 8069 8071 8072
# Sat, 16 Dec 2023 11:04:08 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 16 Dec 2023 11:04:08 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 16 Dec 2023 11:04:08 GMT
USER odoo
# Sat, 16 Dec 2023 11:04:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Dec 2023 11:04:08 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7734efb8b826f955c6a3bb51d7c84cb262d0e600ea3980f5bce69fa7f4f92d24`  
		Last Modified: Tue, 12 Dec 2023 16:00:15 GMT  
		Size: 28.4 MB (28400282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed064f4459a4f1ab48040e16f6b55972797bd014de0d33737d676d7a1a25db4`  
		Last Modified: Sat, 16 Dec 2023 11:04:40 GMT  
		Size: 231.1 MB (231107542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217c6a3bbcbbb21c659f79f47bd7f96d743d57cfd0fe0b1678b81f7ff769a77`  
		Last Modified: Sat, 16 Dec 2023 11:04:20 GMT  
		Size: 2.5 MB (2520464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce39a7573fc5d23b0ecb7a2dc95f9c6c6ea441c6712f6c192b2807e2aa72feb`  
		Last Modified: Sat, 16 Dec 2023 11:04:20 GMT  
		Size: 461.1 KB (461075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d4aa89e67bac0554e241b242eb40964169e55a857220a7ce13ee3a59882ecd`  
		Last Modified: Sat, 16 Dec 2023 11:04:47 GMT  
		Size: 326.2 MB (326219611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984169afba305c7e0dbb5f8be73e8ffc1d3d118be93d882307cb5d888bb1fb5a`  
		Last Modified: Sat, 16 Dec 2023 11:04:17 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1f1e4dc45e16096cc8251bb9060adf0abb8f07a1ec363cd457ac28b2c08422`  
		Last Modified: Sat, 16 Dec 2023 11:04:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad914934c1124d6de9bc06d30871a9eb568c5f305beabe0589784f269cbe87a`  
		Last Modified: Sat, 16 Dec 2023 11:04:17 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab065eddb817943bba284eb1dacbfb531e9f03e37645f79822d53fb41cee7c`  
		Last Modified: Sat, 16 Dec 2023 11:04:18 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17.0` - linux; ppc64le

```console
$ docker pull odoo@sha256:d2d7d75efa6ff5e1d80130e274dc5f6191b166ac34b22d0f5f23e2915221245f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.6 MB (610570813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7591462b0a8b8d4c5453a280fa686f8e29ce6a1bb2689f4738bfbb53befb5376`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Dec 2023 11:43:51 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:43:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:43:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:43:52 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:43:55 GMT
ADD file:bda128b553d54e39b55daceea1f0ad351c73f83835bbf65d10e5af879ce6fee7 in / 
# Tue, 12 Dec 2023 11:43:56 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:18:22 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 16 Dec 2023 11:18:22 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 16 Dec 2023 11:18:23 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Dec 2023 11:18:23 GMT
ARG TARGETARCH
# Sat, 16 Dec 2023 11:22:08 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 16 Dec 2023 11:22:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:22:30 GMT
RUN npm install -g rtlcss
# Sat, 16 Dec 2023 11:22:30 GMT
ENV ODOO_VERSION=17.0
# Sat, 16 Dec 2023 11:22:31 GMT
ARG ODOO_RELEASE=20231215
# Sat, 16 Dec 2023 11:22:31 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Sat, 16 Dec 2023 11:25:16 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 16 Dec 2023 11:25:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 16 Dec 2023 11:25:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 16 Dec 2023 11:25:33 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 16 Dec 2023 11:25:33 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 16 Dec 2023 11:25:34 GMT
EXPOSE 8069 8071 8072
# Sat, 16 Dec 2023 11:25:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 16 Dec 2023 11:25:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 16 Dec 2023 11:25:35 GMT
USER odoo
# Sat, 16 Dec 2023 11:25:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Dec 2023 11:25:36 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7775720178c79208fc0d1b977c06891ef7230f39bc02e948d233c49f8a202fcf`  
		Last Modified: Sat, 16 Dec 2023 10:35:18 GMT  
		Size: 35.7 MB (35655287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc829e9bac0988cf5b8041cc64556998568034e96cd72e93b700c2ac4d3f6330`  
		Last Modified: Sat, 16 Dec 2023 11:26:30 GMT  
		Size: 243.3 MB (243296411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77915009472ee87b9142650dd27d791d648dc1cb35fd84a5b5e471802c2476ab`  
		Last Modified: Sat, 16 Dec 2023 11:25:58 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b76a07b6810b56620d5e557ab7a8e64c61a46a1af3a1452dc22677cd585e67`  
		Last Modified: Sat, 16 Dec 2023 11:25:58 GMT  
		Size: 461.2 KB (461168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84004797700930196d2fec76610101e813f5d61f7209f55db42f7dc6eb05ae4b`  
		Last Modified: Sat, 16 Dec 2023 11:26:39 GMT  
		Size: 328.4 MB (328352223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5436a4615a439344a39b355d42d22a263e5ed3be8512bc75716f6350bd152bdf`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6da7f44ddebb885659331932de9332285b0e1cc7501b85e9230e6ed0ca9951`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652edc554772ab19cfefc24f5abdd2e74c95718c52086583b31e99e4df450ee0`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545f4de9ba62bd8bda73a2b2a1e98abbf4e0705f19d02b4fbdd8d6a9d7ea251`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:ad3f0906fc4c3bba4e2a36ccb193cc548b308cf3cc45c7e87b7df4f6a2aa3c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:30b6a127a18ac6af593b7a56602f112b7b4cb260001f136e445110bee4ca23fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.8 MB (593757757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29220a79cacc7f2e4a59d9f60eef8bf84df39f34338351b6ef73963c973671d3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Dec 2023 11:38:57 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:38:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:38:57 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:38:59 GMT
ADD file:2b3b5254f38a790d40e31cb26155609f7fc99ef7bc99eae1e0d67fa9ae605f77 in / 
# Tue, 12 Dec 2023 11:38:59 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:29:57 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 16 Dec 2023 09:29:57 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 16 Dec 2023 09:29:57 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Dec 2023 09:29:57 GMT
ARG TARGETARCH
# Sat, 16 Dec 2023 09:32:06 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 16 Dec 2023 09:32:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:32:18 GMT
RUN npm install -g rtlcss
# Sat, 16 Dec 2023 09:32:18 GMT
ENV ODOO_VERSION=17.0
# Sat, 16 Dec 2023 09:32:18 GMT
ARG ODOO_RELEASE=20231215
# Sat, 16 Dec 2023 09:32:18 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Sat, 16 Dec 2023 09:33:48 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 16 Dec 2023 09:33:53 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 16 Dec 2023 09:33:53 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 16 Dec 2023 09:33:53 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 16 Dec 2023 09:33:53 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 16 Dec 2023 09:33:53 GMT
EXPOSE 8069 8071 8072
# Sat, 16 Dec 2023 09:33:54 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 16 Dec 2023 09:33:54 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 16 Dec 2023 09:33:54 GMT
USER odoo
# Sat, 16 Dec 2023 09:33:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Dec 2023 09:33:54 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3dd181f9be599de628e1bc6d868d517125e07f968824bcf7b7ed8d28ad1026b1`  
		Last Modified: Tue, 12 Dec 2023 12:46:19 GMT  
		Size: 30.4 MB (30446577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89681bc3d92fa58300c17f37a8c00221342b77325e00deb20e71ea410071d500`  
		Last Modified: Sat, 16 Dec 2023 09:34:46 GMT  
		Size: 233.7 MB (233730172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a3dc4306b241f9806eface9e5fe3c10ef771e41f03509a141414da8bb7c04`  
		Last Modified: Sat, 16 Dec 2023 09:34:19 GMT  
		Size: 2.5 MB (2526485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746699b2b8c3aebf90f574a4692f492e2e617506c92d7a00874d79e4fddaf014`  
		Last Modified: Sat, 16 Dec 2023 09:34:19 GMT  
		Size: 461.1 KB (461135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65b67a8d3db9081841dc9d808b5e78e43a7e30a435eb0f57330a1de521fcfc9`  
		Last Modified: Sat, 16 Dec 2023 09:34:55 GMT  
		Size: 326.6 MB (326590922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f2852418032bfe4c1c35bfa16ad612d51baddd3818f8af6895d2f740da6277`  
		Last Modified: Sat, 16 Dec 2023 09:34:17 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257ebd1f11921d56dcf37b6e4a3c58eb50cc3213e71bce9d10abbfad992f28f9`  
		Last Modified: Sat, 16 Dec 2023 09:34:17 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9233a18d9fd9ba41414598ce2a94bc9ff23e95f0f703dbf1a5cbbfb869b2f90`  
		Last Modified: Sat, 16 Dec 2023 09:34:17 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fec152432475ca632e2e45f4b2bf57245f6ed21fe0fb35820ba0a2319bccaa`  
		Last Modified: Sat, 16 Dec 2023 09:34:16 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:latest` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:45033b789835cff1c70920db2280ee06659916f9d565dfa18d8d11d64f89a21a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588711441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7eb80af58fee94d481b5000a5963ae21b2dd2a611b6ed247c9e46630be35b2b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Dec 2023 11:41:50 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:41:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:41:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:41:51 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:41:54 GMT
ADD file:50f947da69b3b6c63695be9c49eee16f7a7dcdecdceb51e5bee1609b845bf483 in / 
# Tue, 12 Dec 2023 11:41:54 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 10:59:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 16 Dec 2023 10:59:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 16 Dec 2023 10:59:32 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Dec 2023 10:59:32 GMT
ARG TARGETARCH
# Sat, 16 Dec 2023 11:01:54 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 16 Dec 2023 11:02:08 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:02:09 GMT
RUN npm install -g rtlcss
# Sat, 16 Dec 2023 11:02:09 GMT
ENV ODOO_VERSION=17.0
# Sat, 16 Dec 2023 11:02:09 GMT
ARG ODOO_RELEASE=20231215
# Sat, 16 Dec 2023 11:02:09 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Sat, 16 Dec 2023 11:04:00 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 16 Dec 2023 11:04:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 16 Dec 2023 11:04:07 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 16 Dec 2023 11:04:08 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 16 Dec 2023 11:04:08 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 16 Dec 2023 11:04:08 GMT
EXPOSE 8069 8071 8072
# Sat, 16 Dec 2023 11:04:08 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 16 Dec 2023 11:04:08 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 16 Dec 2023 11:04:08 GMT
USER odoo
# Sat, 16 Dec 2023 11:04:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Dec 2023 11:04:08 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7734efb8b826f955c6a3bb51d7c84cb262d0e600ea3980f5bce69fa7f4f92d24`  
		Last Modified: Tue, 12 Dec 2023 16:00:15 GMT  
		Size: 28.4 MB (28400282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed064f4459a4f1ab48040e16f6b55972797bd014de0d33737d676d7a1a25db4`  
		Last Modified: Sat, 16 Dec 2023 11:04:40 GMT  
		Size: 231.1 MB (231107542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217c6a3bbcbbb21c659f79f47bd7f96d743d57cfd0fe0b1678b81f7ff769a77`  
		Last Modified: Sat, 16 Dec 2023 11:04:20 GMT  
		Size: 2.5 MB (2520464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce39a7573fc5d23b0ecb7a2dc95f9c6c6ea441c6712f6c192b2807e2aa72feb`  
		Last Modified: Sat, 16 Dec 2023 11:04:20 GMT  
		Size: 461.1 KB (461075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d4aa89e67bac0554e241b242eb40964169e55a857220a7ce13ee3a59882ecd`  
		Last Modified: Sat, 16 Dec 2023 11:04:47 GMT  
		Size: 326.2 MB (326219611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984169afba305c7e0dbb5f8be73e8ffc1d3d118be93d882307cb5d888bb1fb5a`  
		Last Modified: Sat, 16 Dec 2023 11:04:17 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1f1e4dc45e16096cc8251bb9060adf0abb8f07a1ec363cd457ac28b2c08422`  
		Last Modified: Sat, 16 Dec 2023 11:04:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad914934c1124d6de9bc06d30871a9eb568c5f305beabe0589784f269cbe87a`  
		Last Modified: Sat, 16 Dec 2023 11:04:17 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab065eddb817943bba284eb1dacbfb531e9f03e37645f79822d53fb41cee7c`  
		Last Modified: Sat, 16 Dec 2023 11:04:18 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:latest` - linux; ppc64le

```console
$ docker pull odoo@sha256:d2d7d75efa6ff5e1d80130e274dc5f6191b166ac34b22d0f5f23e2915221245f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.6 MB (610570813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7591462b0a8b8d4c5453a280fa686f8e29ce6a1bb2689f4738bfbb53befb5376`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Dec 2023 11:43:51 GMT
ARG RELEASE
# Tue, 12 Dec 2023 11:43:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 11:43:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 11:43:52 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 12 Dec 2023 11:43:55 GMT
ADD file:bda128b553d54e39b55daceea1f0ad351c73f83835bbf65d10e5af879ce6fee7 in / 
# Tue, 12 Dec 2023 11:43:56 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:18:22 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 16 Dec 2023 11:18:22 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 16 Dec 2023 11:18:23 GMT
ENV LANG=en_US.UTF-8
# Sat, 16 Dec 2023 11:18:23 GMT
ARG TARGETARCH
# Sat, 16 Dec 2023 11:22:08 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 16 Dec 2023 11:22:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:22:30 GMT
RUN npm install -g rtlcss
# Sat, 16 Dec 2023 11:22:30 GMT
ENV ODOO_VERSION=17.0
# Sat, 16 Dec 2023 11:22:31 GMT
ARG ODOO_RELEASE=20231215
# Sat, 16 Dec 2023 11:22:31 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Sat, 16 Dec 2023 11:25:16 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 16 Dec 2023 11:25:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 16 Dec 2023 11:25:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 16 Dec 2023 11:25:33 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 16 Dec 2023 11:25:33 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 16 Dec 2023 11:25:34 GMT
EXPOSE 8069 8071 8072
# Sat, 16 Dec 2023 11:25:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 16 Dec 2023 11:25:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 16 Dec 2023 11:25:35 GMT
USER odoo
# Sat, 16 Dec 2023 11:25:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Dec 2023 11:25:36 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7775720178c79208fc0d1b977c06891ef7230f39bc02e948d233c49f8a202fcf`  
		Last Modified: Sat, 16 Dec 2023 10:35:18 GMT  
		Size: 35.7 MB (35655287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc829e9bac0988cf5b8041cc64556998568034e96cd72e93b700c2ac4d3f6330`  
		Last Modified: Sat, 16 Dec 2023 11:26:30 GMT  
		Size: 243.3 MB (243296411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77915009472ee87b9142650dd27d791d648dc1cb35fd84a5b5e471802c2476ab`  
		Last Modified: Sat, 16 Dec 2023 11:25:58 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b76a07b6810b56620d5e557ab7a8e64c61a46a1af3a1452dc22677cd585e67`  
		Last Modified: Sat, 16 Dec 2023 11:25:58 GMT  
		Size: 461.2 KB (461168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84004797700930196d2fec76610101e813f5d61f7209f55db42f7dc6eb05ae4b`  
		Last Modified: Sat, 16 Dec 2023 11:26:39 GMT  
		Size: 328.4 MB (328352223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5436a4615a439344a39b355d42d22a263e5ed3be8512bc75716f6350bd152bdf`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6da7f44ddebb885659331932de9332285b0e1cc7501b85e9230e6ed0ca9951`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652edc554772ab19cfefc24f5abdd2e74c95718c52086583b31e99e4df450ee0`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545f4de9ba62bd8bda73a2b2a1e98abbf4e0705f19d02b4fbdd8d6a9d7ea251`  
		Last Modified: Sat, 16 Dec 2023 11:25:55 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
