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
$ docker pull odoo@sha256:e10b3f026c5ddca9661d390e3a06e57138a8e679d038b63d4a715d516c6da12b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:93632a1c503918a814e39b1bf869199e75438d008d0212230c87fd081350f474
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.2 MB (563194501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f01486064aece4be19508f13044319ad7098f8f54d0532ba609764c0eb56898c`
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
# Fri, 22 Dec 2023 17:52:06 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:52:06 GMT
ARG ODOO_SHA=475688179c3857aa76c46f86486d848812ba046b
# Fri, 22 Dec 2023 17:53:21 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=475688179c3857aa76c46f86486d848812ba046b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:53:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:53:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:53:24 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=475688179c3857aa76c46f86486d848812ba046b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:53:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:53:24 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:53:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:53:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:53:24 GMT
USER odoo
# Fri, 22 Dec 2023 17:53:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:53:25 GMT
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
	-	`sha256:5df4a99878fd03792febc29486ebd41d82c18ac7a71adadc76bf3303cbe59e29`  
		Last Modified: Fri, 22 Dec 2023 17:55:46 GMT  
		Size: 308.4 MB (308390257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c986928d1ad89a16f0e6f94298fa1dca768983bc9d3988dc1fe4d497534628b`  
		Last Modified: Fri, 22 Dec 2023 17:55:13 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b492f4d0de2339ab9d8a4725c9ead0b9f93cac799c651a4704819b6c699aaaa`  
		Last Modified: Fri, 22 Dec 2023 17:55:13 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1479e228fa58d8b3f0543a813b193cee131387aade1dd3269df6632db35e896f`  
		Last Modified: Fri, 22 Dec 2023 17:55:13 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c8e21d24ebc1ce75f19ef328c27916b1a825868880d6dbd803b17d10a7fab2`  
		Last Modified: Fri, 22 Dec 2023 17:55:13 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:e10b3f026c5ddca9661d390e3a06e57138a8e679d038b63d4a715d516c6da12b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:93632a1c503918a814e39b1bf869199e75438d008d0212230c87fd081350f474
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.2 MB (563194501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f01486064aece4be19508f13044319ad7098f8f54d0532ba609764c0eb56898c`
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
# Fri, 22 Dec 2023 17:52:06 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:52:06 GMT
ARG ODOO_SHA=475688179c3857aa76c46f86486d848812ba046b
# Fri, 22 Dec 2023 17:53:21 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=475688179c3857aa76c46f86486d848812ba046b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:53:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:53:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:53:24 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=475688179c3857aa76c46f86486d848812ba046b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:53:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:53:24 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:53:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:53:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:53:24 GMT
USER odoo
# Fri, 22 Dec 2023 17:53:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:53:25 GMT
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
	-	`sha256:5df4a99878fd03792febc29486ebd41d82c18ac7a71adadc76bf3303cbe59e29`  
		Last Modified: Fri, 22 Dec 2023 17:55:46 GMT  
		Size: 308.4 MB (308390257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c986928d1ad89a16f0e6f94298fa1dca768983bc9d3988dc1fe4d497534628b`  
		Last Modified: Fri, 22 Dec 2023 17:55:13 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b492f4d0de2339ab9d8a4725c9ead0b9f93cac799c651a4704819b6c699aaaa`  
		Last Modified: Fri, 22 Dec 2023 17:55:13 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1479e228fa58d8b3f0543a813b193cee131387aade1dd3269df6632db35e896f`  
		Last Modified: Fri, 22 Dec 2023 17:55:13 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c8e21d24ebc1ce75f19ef328c27916b1a825868880d6dbd803b17d10a7fab2`  
		Last Modified: Fri, 22 Dec 2023 17:55:13 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:db06f985e0e90aa24e06dd27497c4d50918a94ccd4131c6d5ea13f8d80306f9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:b9db539d62df6fc3a0c6e6498641c49340de728e63b22cc9608de5882d989137
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.6 MB (577601573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84e9bf40475d20b447d36174f4b3fbb52e76f7ef76efadab26c02c4286ba636f`
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
# Fri, 22 Dec 2023 17:50:27 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:50:27 GMT
ARG ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
# Fri, 22 Dec 2023 17:51:51 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:51:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:51:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:51:57 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:51:57 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:51:57 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:51:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:51:57 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:51:57 GMT
USER odoo
# Fri, 22 Dec 2023 17:51:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:51:57 GMT
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
	-	`sha256:cb059352b2bbb36c1790922d351a1a3bf8cdb73630e4fcbac62991b7cb254a40`  
		Last Modified: Fri, 22 Dec 2023 17:55:04 GMT  
		Size: 323.5 MB (323485752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37898499563ada78295c8ce270cbcbaed54f6dd245665f4d5ba05f84411c462e`  
		Last Modified: Fri, 22 Dec 2023 17:54:27 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebfdf62374597cc7e43a62dac3f774cfd33e8163cdadb716f3a76c733682b86`  
		Last Modified: Fri, 22 Dec 2023 17:54:27 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d789e259cc357446142e46b928034795f4744c8de3b2fc58dc010b01419ddb6`  
		Last Modified: Fri, 22 Dec 2023 17:54:27 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963657f8b3efac757a4ebaff24ec868e96636a429c18b42ad6e7a763da9fb0f4`  
		Last Modified: Fri, 22 Dec 2023 17:54:27 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:8d133e3f374a50ff776c09e0e1cec956c01113e63ef2b471250a429551f51356
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.2 MB (573201029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c0883b6bf98a68d6aa39825bf8c21ae36cb55efb942ec355097dde18d922bcf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:25 GMT
ADD file:4dd1c5e17a5e57644787f37e8ad290baef6c93f4f112b976f19136480a293713 in / 
# Tue, 19 Dec 2023 01:41:25 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:22:44 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 19 Dec 2023 03:22:45 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 19 Dec 2023 03:22:45 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 03:22:45 GMT
ARG TARGETARCH
# Tue, 19 Dec 2023 03:23:46 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 19 Dec 2023 03:23:59 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:24:00 GMT
RUN npm install -g rtlcss
# Tue, 19 Dec 2023 03:24:00 GMT
ENV ODOO_VERSION=16.0
# Fri, 22 Dec 2023 16:49:04 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 16:49:04 GMT
ARG ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
# Fri, 22 Dec 2023 16:50:19 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 16:50:25 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 16:50:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 16:50:26 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 16:50:26 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 16:50:26 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 16:50:26 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 16:50:26 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 16:50:26 GMT
USER odoo
# Fri, 22 Dec 2023 16:50:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 16:50:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:2244706f264b35566276550fbc21ada79613ddfff850e372b8f5113110a67c93`  
		Last Modified: Tue, 19 Dec 2023 01:45:22 GMT  
		Size: 30.1 MB (30064052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ad9b105863f2fc14a5eef7551b0e02b42125be8cf06d2b399cca8dd47b9024`  
		Last Modified: Tue, 19 Dec 2023 03:25:50 GMT  
		Size: 216.9 MB (216906264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585aa02a509f7adac375bec76b48202f6c03b9204aeeda420abd6a05fd26b625`  
		Last Modified: Tue, 19 Dec 2023 03:25:32 GMT  
		Size: 2.6 MB (2634790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7efcf8969b0a1f21c021a830c4005ce948c2d74c14f20ee46a0c716d9a9406`  
		Last Modified: Tue, 19 Dec 2023 03:25:32 GMT  
		Size: 459.6 KB (459615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a606d384a7bccdd5ab3ca7b1d1ac595047c1413d7467af6a06aa1f911e50b985`  
		Last Modified: Fri, 22 Dec 2023 16:51:58 GMT  
		Size: 323.1 MB (323133849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956274bd5bdf74befc2a60b2624f78c442276df4ba44ee6206aa6fd1f94881ca`  
		Last Modified: Fri, 22 Dec 2023 16:51:28 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac63dfd6bdce548a1ddc91179205290b1f8fd2fe3f67b66e7adb9b597fe263a`  
		Last Modified: Fri, 22 Dec 2023 16:51:28 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d9576b31e4d8ba35b9aa7a75a74362394a69829580c901a257528c56874f89`  
		Last Modified: Fri, 22 Dec 2023 16:51:28 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eb4f98bc9609ce8775c40b173b53f946aa7d31a8b7e899eea9fc4b16cfc4c5`  
		Last Modified: Fri, 22 Dec 2023 16:51:28 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16` - linux; ppc64le

```console
$ docker pull odoo@sha256:a4d07029cb4479af43fd58db5cd7647595d86bfd93c665077cf12cc497b78684
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.1 MB (592146907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9afa82592dd810c95ba54bed2a5c1c333dde96b994c75a4e75fd7656a53a0bd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:19 GMT
ADD file:1cb772a6ad8ca6301624db3141029490564de7673bc0f2d4bedb5a1578ea85bd in / 
# Tue, 19 Dec 2023 01:22:21 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 11:32:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 19 Dec 2023 11:32:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 19 Dec 2023 11:32:33 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 11:32:33 GMT
ARG TARGETARCH
# Tue, 19 Dec 2023 11:36:42 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 19 Dec 2023 11:37:07 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:37:11 GMT
RUN npm install -g rtlcss
# Tue, 19 Dec 2023 11:37:11 GMT
ENV ODOO_VERSION=16.0
# Fri, 22 Dec 2023 17:39:22 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:39:23 GMT
ARG ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
# Fri, 22 Dec 2023 17:41:45 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:42:00 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:42:00 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:42:02 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:42:03 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:42:04 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:42:05 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:42:05 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:42:07 GMT
USER odoo
# Fri, 22 Dec 2023 17:42:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:42:09 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c9f6fac7f65cfc65b7f8de8bc377b135ca95e45a3246cf2bd1bb90922679553e`  
		Last Modified: Tue, 19 Dec 2023 01:27:11 GMT  
		Size: 35.3 MB (35293807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88fea3758d5ffc8bbed4ff1cd482391eb784ecb8fdf0fccc40ecab99f6d81b5`  
		Last Modified: Tue, 19 Dec 2023 11:41:51 GMT  
		Size: 228.6 MB (228600468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f58b4419e778e33dcd191af8d04181e44a270299c462948597ec439045dad1d`  
		Last Modified: Tue, 19 Dec 2023 11:41:23 GMT  
		Size: 2.9 MB (2875892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4ed1b99ef0fdc1c48d1e6a751842151cc11abdc88b7b28c0d17f6bf2664d1f`  
		Last Modified: Tue, 19 Dec 2023 11:41:23 GMT  
		Size: 459.6 KB (459595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2856176d540968410eaf15620d61a881c85244264be178fdc93a0a1844305b`  
		Last Modified: Fri, 22 Dec 2023 17:44:00 GMT  
		Size: 324.9 MB (324914678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9500c6c704e6b6597411553e0de8ba0e7db9d93ca93e83ae6a6213fe802864a8`  
		Last Modified: Fri, 22 Dec 2023 17:43:18 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1385427a66e991ad932c94c491d28b3fa4e5c0e8e6ba5c7f6d26a4858f88b5b`  
		Last Modified: Fri, 22 Dec 2023 17:43:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e746bd783ce8695e588b568e4dde2df5f8c977a03df79a53801c83f8a2a253`  
		Last Modified: Fri, 22 Dec 2023 17:43:18 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b0e520ae4c622bc7c6b98b4559c2fa0dd7fbbb434df6bd46a9b49d19715fd3`  
		Last Modified: Fri, 22 Dec 2023 17:43:18 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:db06f985e0e90aa24e06dd27497c4d50918a94ccd4131c6d5ea13f8d80306f9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:b9db539d62df6fc3a0c6e6498641c49340de728e63b22cc9608de5882d989137
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.6 MB (577601573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84e9bf40475d20b447d36174f4b3fbb52e76f7ef76efadab26c02c4286ba636f`
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
# Fri, 22 Dec 2023 17:50:27 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:50:27 GMT
ARG ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
# Fri, 22 Dec 2023 17:51:51 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:51:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:51:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:51:57 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:51:57 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:51:57 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:51:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:51:57 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:51:57 GMT
USER odoo
# Fri, 22 Dec 2023 17:51:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:51:57 GMT
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
	-	`sha256:cb059352b2bbb36c1790922d351a1a3bf8cdb73630e4fcbac62991b7cb254a40`  
		Last Modified: Fri, 22 Dec 2023 17:55:04 GMT  
		Size: 323.5 MB (323485752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37898499563ada78295c8ce270cbcbaed54f6dd245665f4d5ba05f84411c462e`  
		Last Modified: Fri, 22 Dec 2023 17:54:27 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebfdf62374597cc7e43a62dac3f774cfd33e8163cdadb716f3a76c733682b86`  
		Last Modified: Fri, 22 Dec 2023 17:54:27 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d789e259cc357446142e46b928034795f4744c8de3b2fc58dc010b01419ddb6`  
		Last Modified: Fri, 22 Dec 2023 17:54:27 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963657f8b3efac757a4ebaff24ec868e96636a429c18b42ad6e7a763da9fb0f4`  
		Last Modified: Fri, 22 Dec 2023 17:54:27 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16.0` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:8d133e3f374a50ff776c09e0e1cec956c01113e63ef2b471250a429551f51356
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.2 MB (573201029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c0883b6bf98a68d6aa39825bf8c21ae36cb55efb942ec355097dde18d922bcf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:25 GMT
ADD file:4dd1c5e17a5e57644787f37e8ad290baef6c93f4f112b976f19136480a293713 in / 
# Tue, 19 Dec 2023 01:41:25 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:22:44 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 19 Dec 2023 03:22:45 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 19 Dec 2023 03:22:45 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 03:22:45 GMT
ARG TARGETARCH
# Tue, 19 Dec 2023 03:23:46 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 19 Dec 2023 03:23:59 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:24:00 GMT
RUN npm install -g rtlcss
# Tue, 19 Dec 2023 03:24:00 GMT
ENV ODOO_VERSION=16.0
# Fri, 22 Dec 2023 16:49:04 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 16:49:04 GMT
ARG ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
# Fri, 22 Dec 2023 16:50:19 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 16:50:25 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 16:50:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 16:50:26 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 16:50:26 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 16:50:26 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 16:50:26 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 16:50:26 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 16:50:26 GMT
USER odoo
# Fri, 22 Dec 2023 16:50:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 16:50:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:2244706f264b35566276550fbc21ada79613ddfff850e372b8f5113110a67c93`  
		Last Modified: Tue, 19 Dec 2023 01:45:22 GMT  
		Size: 30.1 MB (30064052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ad9b105863f2fc14a5eef7551b0e02b42125be8cf06d2b399cca8dd47b9024`  
		Last Modified: Tue, 19 Dec 2023 03:25:50 GMT  
		Size: 216.9 MB (216906264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585aa02a509f7adac375bec76b48202f6c03b9204aeeda420abd6a05fd26b625`  
		Last Modified: Tue, 19 Dec 2023 03:25:32 GMT  
		Size: 2.6 MB (2634790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7efcf8969b0a1f21c021a830c4005ce948c2d74c14f20ee46a0c716d9a9406`  
		Last Modified: Tue, 19 Dec 2023 03:25:32 GMT  
		Size: 459.6 KB (459615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a606d384a7bccdd5ab3ca7b1d1ac595047c1413d7467af6a06aa1f911e50b985`  
		Last Modified: Fri, 22 Dec 2023 16:51:58 GMT  
		Size: 323.1 MB (323133849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956274bd5bdf74befc2a60b2624f78c442276df4ba44ee6206aa6fd1f94881ca`  
		Last Modified: Fri, 22 Dec 2023 16:51:28 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac63dfd6bdce548a1ddc91179205290b1f8fd2fe3f67b66e7adb9b597fe263a`  
		Last Modified: Fri, 22 Dec 2023 16:51:28 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d9576b31e4d8ba35b9aa7a75a74362394a69829580c901a257528c56874f89`  
		Last Modified: Fri, 22 Dec 2023 16:51:28 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eb4f98bc9609ce8775c40b173b53f946aa7d31a8b7e899eea9fc4b16cfc4c5`  
		Last Modified: Fri, 22 Dec 2023 16:51:28 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16.0` - linux; ppc64le

```console
$ docker pull odoo@sha256:a4d07029cb4479af43fd58db5cd7647595d86bfd93c665077cf12cc497b78684
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.1 MB (592146907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9afa82592dd810c95ba54bed2a5c1c333dde96b994c75a4e75fd7656a53a0bd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:19 GMT
ADD file:1cb772a6ad8ca6301624db3141029490564de7673bc0f2d4bedb5a1578ea85bd in / 
# Tue, 19 Dec 2023 01:22:21 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 11:32:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 19 Dec 2023 11:32:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 19 Dec 2023 11:32:33 GMT
ENV LANG=C.UTF-8
# Tue, 19 Dec 2023 11:32:33 GMT
ARG TARGETARCH
# Tue, 19 Dec 2023 11:36:42 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 19 Dec 2023 11:37:07 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:37:11 GMT
RUN npm install -g rtlcss
# Tue, 19 Dec 2023 11:37:11 GMT
ENV ODOO_VERSION=16.0
# Fri, 22 Dec 2023 17:39:22 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:39:23 GMT
ARG ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
# Fri, 22 Dec 2023 17:41:45 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:42:00 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:42:00 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:42:02 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=739d7dd119c00fa27ab1bcd140b70389ce271170
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:42:03 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:42:04 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:42:05 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:42:05 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:42:07 GMT
USER odoo
# Fri, 22 Dec 2023 17:42:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:42:09 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c9f6fac7f65cfc65b7f8de8bc377b135ca95e45a3246cf2bd1bb90922679553e`  
		Last Modified: Tue, 19 Dec 2023 01:27:11 GMT  
		Size: 35.3 MB (35293807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88fea3758d5ffc8bbed4ff1cd482391eb784ecb8fdf0fccc40ecab99f6d81b5`  
		Last Modified: Tue, 19 Dec 2023 11:41:51 GMT  
		Size: 228.6 MB (228600468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f58b4419e778e33dcd191af8d04181e44a270299c462948597ec439045dad1d`  
		Last Modified: Tue, 19 Dec 2023 11:41:23 GMT  
		Size: 2.9 MB (2875892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4ed1b99ef0fdc1c48d1e6a751842151cc11abdc88b7b28c0d17f6bf2664d1f`  
		Last Modified: Tue, 19 Dec 2023 11:41:23 GMT  
		Size: 459.6 KB (459595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2856176d540968410eaf15620d61a881c85244264be178fdc93a0a1844305b`  
		Last Modified: Fri, 22 Dec 2023 17:44:00 GMT  
		Size: 324.9 MB (324914678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9500c6c704e6b6597411553e0de8ba0e7db9d93ca93e83ae6a6213fe802864a8`  
		Last Modified: Fri, 22 Dec 2023 17:43:18 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1385427a66e991ad932c94c491d28b3fa4e5c0e8e6ba5c7f6d26a4858f88b5b`  
		Last Modified: Fri, 22 Dec 2023 17:43:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e746bd783ce8695e588b568e4dde2df5f8c977a03df79a53801c83f8a2a253`  
		Last Modified: Fri, 22 Dec 2023 17:43:18 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b0e520ae4c622bc7c6b98b4559c2fa0dd7fbbb434df6bd46a9b49d19715fd3`  
		Last Modified: Fri, 22 Dec 2023 17:43:18 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:17`

```console
$ docker pull odoo@sha256:5ecf94e562ce5bbe3dacd02e6ea37e75b74d486d30a591b1f7237cc85e2aad3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:17` - linux; amd64

```console
$ docker pull odoo@sha256:7e3dd3ecd44d80b02493f4dfd64fc339de1dddcb6f21f06af77f1a214648dac5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **594.0 MB (593963640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402b31d048a3229970bcf62b30abd2b55ef253a4d8d0ccbbb50cb654b48b8dba`
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
# Fri, 22 Dec 2023 17:47:33 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:47:33 GMT
ARG ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
# Fri, 22 Dec 2023 17:50:20 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:50:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:50:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:50:23 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:50:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:50:24 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:50:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:50:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:50:24 GMT
USER odoo
# Fri, 22 Dec 2023 17:50:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:50:24 GMT
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
	-	`sha256:99151833ee6a31bc1a360745ba224ffd711082248d9b1812d2941441901d8d88`  
		Last Modified: Fri, 22 Dec 2023 17:54:16 GMT  
		Size: 326.8 MB (326796802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b9a45ce1f6c10bab09cd549322b7556dda5cb45212a7bc10f698daa5970a14`  
		Last Modified: Fri, 22 Dec 2023 17:53:38 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d3065cbff168dc65a6e97fb822649716521b4f898676ee5111bd4213739433`  
		Last Modified: Fri, 22 Dec 2023 17:53:37 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56afa8d8c75fdd79efac5d5e253a6d39bc932b1b89efee5ce52688d9aec6f921`  
		Last Modified: Fri, 22 Dec 2023 17:53:37 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363950e2794fa16f8907b511dad36c33f87762dc194233fe5b721e43d983da9`  
		Last Modified: Fri, 22 Dec 2023 17:53:37 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:300dd13668e5b5ed6b59378d27854d5b5dda076eef7ea539db4ae779ace315cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.9 MB (588885704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a572e4b0d21d2ad6ba118a7855787dfbd752e909af98774ec11bfa45940155c`
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
# Fri, 22 Dec 2023 16:46:41 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 16:46:42 GMT
ARG ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
# Fri, 22 Dec 2023 16:48:56 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 16:48:57 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 16:48:57 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 16:48:58 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 16:48:58 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 16:48:58 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 16:48:58 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 16:48:58 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 16:48:58 GMT
USER odoo
# Fri, 22 Dec 2023 16:48:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 16:48:58 GMT
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
	-	`sha256:920dc9bb46def116df27c61388ac7e7d94b04ef0b632b42f41115ac7f2b37cfa`  
		Last Modified: Fri, 22 Dec 2023 16:51:18 GMT  
		Size: 326.4 MB (326393874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae3dfe3591be279d953268e06c54420a75aa15f6eb619ed689cd2f13d3e3dc7`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f46763b2337dd6ab314cdbce644b2d8c795c03331d80b782815142e30e2934`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c35bdf7aaa0b48d9fa9e4d9f5ee561852d74e07b0aba6bc4aa842de93e4590`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6a96dc852ebe618061ceccb6a6c66fbd018b06ff30345a6eba673e691a8acc`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17` - linux; ppc64le

```console
$ docker pull odoo@sha256:9edd7609c024ed84f8da9970d470447c4ac816f4b8bfdd96beb1229843308fe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.7 MB (610736860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14adda89fb2f29d4e944b2d82622f5b1fb7e0141b98b473dcca9ca7e557e66a2`
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
# Fri, 22 Dec 2023 17:35:43 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:35:43 GMT
ARG ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
# Fri, 22 Dec 2023 17:38:55 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:39:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:39:08 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:39:10 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:39:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:39:12 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:39:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:39:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:39:13 GMT
USER odoo
# Fri, 22 Dec 2023 17:39:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:39:14 GMT
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
	-	`sha256:ff3d783d6d3d7462123a43c11a6960b4593c4724729c2101ebaa79ea7b66304f`  
		Last Modified: Fri, 22 Dec 2023 17:43:05 GMT  
		Size: 328.5 MB (328518273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf952c691833c17fd98596eb83dc03e4e0b6fdfc8ea59f1e21964fc14bdf646`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de469a81b2904e80e7ec875c46d15570e7579dfb0d86282bf279de96a80b02ad`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62a40bbbfd9730e1e5b2c52cfee9449bb37405e9ada11cd182529644abc9693`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5ff2d981d5b436dddb678421b3a2a98ce061f089e35b0da70d83fb85375ade`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:17.0`

```console
$ docker pull odoo@sha256:5ecf94e562ce5bbe3dacd02e6ea37e75b74d486d30a591b1f7237cc85e2aad3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:17.0` - linux; amd64

```console
$ docker pull odoo@sha256:7e3dd3ecd44d80b02493f4dfd64fc339de1dddcb6f21f06af77f1a214648dac5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **594.0 MB (593963640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402b31d048a3229970bcf62b30abd2b55ef253a4d8d0ccbbb50cb654b48b8dba`
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
# Fri, 22 Dec 2023 17:47:33 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:47:33 GMT
ARG ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
# Fri, 22 Dec 2023 17:50:20 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:50:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:50:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:50:23 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:50:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:50:24 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:50:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:50:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:50:24 GMT
USER odoo
# Fri, 22 Dec 2023 17:50:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:50:24 GMT
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
	-	`sha256:99151833ee6a31bc1a360745ba224ffd711082248d9b1812d2941441901d8d88`  
		Last Modified: Fri, 22 Dec 2023 17:54:16 GMT  
		Size: 326.8 MB (326796802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b9a45ce1f6c10bab09cd549322b7556dda5cb45212a7bc10f698daa5970a14`  
		Last Modified: Fri, 22 Dec 2023 17:53:38 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d3065cbff168dc65a6e97fb822649716521b4f898676ee5111bd4213739433`  
		Last Modified: Fri, 22 Dec 2023 17:53:37 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56afa8d8c75fdd79efac5d5e253a6d39bc932b1b89efee5ce52688d9aec6f921`  
		Last Modified: Fri, 22 Dec 2023 17:53:37 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363950e2794fa16f8907b511dad36c33f87762dc194233fe5b721e43d983da9`  
		Last Modified: Fri, 22 Dec 2023 17:53:37 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17.0` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:300dd13668e5b5ed6b59378d27854d5b5dda076eef7ea539db4ae779ace315cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.9 MB (588885704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a572e4b0d21d2ad6ba118a7855787dfbd752e909af98774ec11bfa45940155c`
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
# Fri, 22 Dec 2023 16:46:41 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 16:46:42 GMT
ARG ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
# Fri, 22 Dec 2023 16:48:56 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 16:48:57 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 16:48:57 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 16:48:58 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 16:48:58 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 16:48:58 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 16:48:58 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 16:48:58 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 16:48:58 GMT
USER odoo
# Fri, 22 Dec 2023 16:48:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 16:48:58 GMT
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
	-	`sha256:920dc9bb46def116df27c61388ac7e7d94b04ef0b632b42f41115ac7f2b37cfa`  
		Last Modified: Fri, 22 Dec 2023 16:51:18 GMT  
		Size: 326.4 MB (326393874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae3dfe3591be279d953268e06c54420a75aa15f6eb619ed689cd2f13d3e3dc7`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f46763b2337dd6ab314cdbce644b2d8c795c03331d80b782815142e30e2934`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c35bdf7aaa0b48d9fa9e4d9f5ee561852d74e07b0aba6bc4aa842de93e4590`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6a96dc852ebe618061ceccb6a6c66fbd018b06ff30345a6eba673e691a8acc`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17.0` - linux; ppc64le

```console
$ docker pull odoo@sha256:9edd7609c024ed84f8da9970d470447c4ac816f4b8bfdd96beb1229843308fe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.7 MB (610736860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14adda89fb2f29d4e944b2d82622f5b1fb7e0141b98b473dcca9ca7e557e66a2`
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
# Fri, 22 Dec 2023 17:35:43 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:35:43 GMT
ARG ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
# Fri, 22 Dec 2023 17:38:55 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:39:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:39:08 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:39:10 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:39:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:39:12 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:39:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:39:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:39:13 GMT
USER odoo
# Fri, 22 Dec 2023 17:39:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:39:14 GMT
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
	-	`sha256:ff3d783d6d3d7462123a43c11a6960b4593c4724729c2101ebaa79ea7b66304f`  
		Last Modified: Fri, 22 Dec 2023 17:43:05 GMT  
		Size: 328.5 MB (328518273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf952c691833c17fd98596eb83dc03e4e0b6fdfc8ea59f1e21964fc14bdf646`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de469a81b2904e80e7ec875c46d15570e7579dfb0d86282bf279de96a80b02ad`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62a40bbbfd9730e1e5b2c52cfee9449bb37405e9ada11cd182529644abc9693`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5ff2d981d5b436dddb678421b3a2a98ce061f089e35b0da70d83fb85375ade`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:5ecf94e562ce5bbe3dacd02e6ea37e75b74d486d30a591b1f7237cc85e2aad3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:7e3dd3ecd44d80b02493f4dfd64fc339de1dddcb6f21f06af77f1a214648dac5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **594.0 MB (593963640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402b31d048a3229970bcf62b30abd2b55ef253a4d8d0ccbbb50cb654b48b8dba`
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
# Fri, 22 Dec 2023 17:47:33 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:47:33 GMT
ARG ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
# Fri, 22 Dec 2023 17:50:20 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:50:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:50:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:50:23 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:50:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:50:24 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:50:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:50:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:50:24 GMT
USER odoo
# Fri, 22 Dec 2023 17:50:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:50:24 GMT
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
	-	`sha256:99151833ee6a31bc1a360745ba224ffd711082248d9b1812d2941441901d8d88`  
		Last Modified: Fri, 22 Dec 2023 17:54:16 GMT  
		Size: 326.8 MB (326796802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b9a45ce1f6c10bab09cd549322b7556dda5cb45212a7bc10f698daa5970a14`  
		Last Modified: Fri, 22 Dec 2023 17:53:38 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d3065cbff168dc65a6e97fb822649716521b4f898676ee5111bd4213739433`  
		Last Modified: Fri, 22 Dec 2023 17:53:37 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56afa8d8c75fdd79efac5d5e253a6d39bc932b1b89efee5ce52688d9aec6f921`  
		Last Modified: Fri, 22 Dec 2023 17:53:37 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363950e2794fa16f8907b511dad36c33f87762dc194233fe5b721e43d983da9`  
		Last Modified: Fri, 22 Dec 2023 17:53:37 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:latest` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:300dd13668e5b5ed6b59378d27854d5b5dda076eef7ea539db4ae779ace315cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.9 MB (588885704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a572e4b0d21d2ad6ba118a7855787dfbd752e909af98774ec11bfa45940155c`
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
# Fri, 22 Dec 2023 16:46:41 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 16:46:42 GMT
ARG ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
# Fri, 22 Dec 2023 16:48:56 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 16:48:57 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 16:48:57 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 16:48:58 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 16:48:58 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 16:48:58 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 16:48:58 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 16:48:58 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 16:48:58 GMT
USER odoo
# Fri, 22 Dec 2023 16:48:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 16:48:58 GMT
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
	-	`sha256:920dc9bb46def116df27c61388ac7e7d94b04ef0b632b42f41115ac7f2b37cfa`  
		Last Modified: Fri, 22 Dec 2023 16:51:18 GMT  
		Size: 326.4 MB (326393874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae3dfe3591be279d953268e06c54420a75aa15f6eb619ed689cd2f13d3e3dc7`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f46763b2337dd6ab314cdbce644b2d8c795c03331d80b782815142e30e2934`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c35bdf7aaa0b48d9fa9e4d9f5ee561852d74e07b0aba6bc4aa842de93e4590`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6a96dc852ebe618061ceccb6a6c66fbd018b06ff30345a6eba673e691a8acc`  
		Last Modified: Fri, 22 Dec 2023 16:50:49 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:latest` - linux; ppc64le

```console
$ docker pull odoo@sha256:9edd7609c024ed84f8da9970d470447c4ac816f4b8bfdd96beb1229843308fe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.7 MB (610736860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14adda89fb2f29d4e944b2d82622f5b1fb7e0141b98b473dcca9ca7e557e66a2`
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
# Fri, 22 Dec 2023 17:35:43 GMT
ARG ODOO_RELEASE=20231222
# Fri, 22 Dec 2023 17:35:43 GMT
ARG ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
# Fri, 22 Dec 2023 17:38:55 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 22 Dec 2023 17:39:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 22 Dec 2023 17:39:08 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 22 Dec 2023 17:39:10 GMT
# ARGS: ODOO_RELEASE=20231222 ODOO_SHA=77d67d4b3f66db72c0f5a63eae7ab32fea4774b2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 22 Dec 2023 17:39:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 22 Dec 2023 17:39:12 GMT
EXPOSE 8069 8071 8072
# Fri, 22 Dec 2023 17:39:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 22 Dec 2023 17:39:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 22 Dec 2023 17:39:13 GMT
USER odoo
# Fri, 22 Dec 2023 17:39:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Dec 2023 17:39:14 GMT
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
	-	`sha256:ff3d783d6d3d7462123a43c11a6960b4593c4724729c2101ebaa79ea7b66304f`  
		Last Modified: Fri, 22 Dec 2023 17:43:05 GMT  
		Size: 328.5 MB (328518273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf952c691833c17fd98596eb83dc03e4e0b6fdfc8ea59f1e21964fc14bdf646`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de469a81b2904e80e7ec875c46d15570e7579dfb0d86282bf279de96a80b02ad`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62a40bbbfd9730e1e5b2c52cfee9449bb37405e9ada11cd182529644abc9693`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5ff2d981d5b436dddb678421b3a2a98ce061f089e35b0da70d83fb85375ade`  
		Last Modified: Fri, 22 Dec 2023 17:42:23 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
