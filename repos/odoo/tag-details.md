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
$ docker pull odoo@sha256:ae526e1779a736591e9e7ca31ab177e6c7ce490c17e3ffa9c195ed67ed69ae3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:4ee87c2bff891c957437081509f8edd79cc1142a244f267a8858c3655e01b774
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.0 MB (563043964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a7974f41b128ec05dcd506cd6857cf30539bad87918f14bab190edb92fe30bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:00 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 21 Nov 2023 06:06:00 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 21 Nov 2023 06:06:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 06:09:59 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 21 Nov 2023 06:10:06 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:10:07 GMT
RUN npm install -g rtlcss
# Tue, 21 Nov 2023 06:10:07 GMT
ENV ODOO_VERSION=15.0
# Tue, 28 Nov 2023 23:37:59 GMT
ARG ODOO_RELEASE=20231127
# Tue, 28 Nov 2023 23:37:59 GMT
ARG ODOO_SHA=c0e91e4d03ffa8a72db550389f33b7c3577fa829
# Tue, 28 Nov 2023 23:39:10 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=c0e91e4d03ffa8a72db550389f33b7c3577fa829
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 28 Nov 2023 23:39:14 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 28 Nov 2023 23:39:14 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 28 Nov 2023 23:39:15 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=c0e91e4d03ffa8a72db550389f33b7c3577fa829
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 28 Nov 2023 23:39:15 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 28 Nov 2023 23:39:15 GMT
EXPOSE 8069 8071 8072
# Tue, 28 Nov 2023 23:39:15 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 28 Nov 2023 23:39:15 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 28 Nov 2023 23:39:15 GMT
USER odoo
# Tue, 28 Nov 2023 23:39:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Nov 2023 23:39:15 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a28800da8ad810dcb3060b9a249d76f10fc059eb9ea15aa7bb1fcfd0755b607`  
		Last Modified: Tue, 21 Nov 2023 06:13:44 GMT  
		Size: 220.3 MB (220297479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd5e822cfaa6f1e0ff1254d563b0f9fae55e9a37a6461f685b61ba68642687e`  
		Last Modified: Tue, 21 Nov 2023 06:13:20 GMT  
		Size: 2.6 MB (2625685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c2fe85ca0f057eeac7b5d2f65043d55dd0192357c143eca092e3fcdb6f1826`  
		Last Modified: Tue, 21 Nov 2023 06:13:20 GMT  
		Size: 459.5 KB (459485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2d62dc7a84225d80e241450ca7f1c3c8352369bab05d6ab9503a472caf32ba`  
		Last Modified: Tue, 28 Nov 2023 23:41:43 GMT  
		Size: 308.2 MB (308241022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc53506b74d5f16bfb8f2f9818f90fcf74f7382e5634f9c6b84990564363a44a`  
		Last Modified: Tue, 28 Nov 2023 23:41:10 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84884fc611d342bb1c81fdac836a35499c4a8916b6fb07a0104559fff4724586`  
		Last Modified: Tue, 28 Nov 2023 23:41:10 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ee7833223295aa1607a3c5007b9ed6c45822b87a6378964d67c3239943d141`  
		Last Modified: Tue, 28 Nov 2023 23:41:10 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5afe1ec8c776632dce8a00e55efcbfd0b25bd07093b6dc81802688e197ac2a`  
		Last Modified: Tue, 28 Nov 2023 23:41:10 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:ae526e1779a736591e9e7ca31ab177e6c7ce490c17e3ffa9c195ed67ed69ae3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:4ee87c2bff891c957437081509f8edd79cc1142a244f267a8858c3655e01b774
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.0 MB (563043964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a7974f41b128ec05dcd506cd6857cf30539bad87918f14bab190edb92fe30bd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:00 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 21 Nov 2023 06:06:00 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 21 Nov 2023 06:06:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 06:09:59 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 21 Nov 2023 06:10:06 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:10:07 GMT
RUN npm install -g rtlcss
# Tue, 21 Nov 2023 06:10:07 GMT
ENV ODOO_VERSION=15.0
# Tue, 28 Nov 2023 23:37:59 GMT
ARG ODOO_RELEASE=20231127
# Tue, 28 Nov 2023 23:37:59 GMT
ARG ODOO_SHA=c0e91e4d03ffa8a72db550389f33b7c3577fa829
# Tue, 28 Nov 2023 23:39:10 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=c0e91e4d03ffa8a72db550389f33b7c3577fa829
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 28 Nov 2023 23:39:14 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 28 Nov 2023 23:39:14 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 28 Nov 2023 23:39:15 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=c0e91e4d03ffa8a72db550389f33b7c3577fa829
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 28 Nov 2023 23:39:15 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 28 Nov 2023 23:39:15 GMT
EXPOSE 8069 8071 8072
# Tue, 28 Nov 2023 23:39:15 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 28 Nov 2023 23:39:15 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 28 Nov 2023 23:39:15 GMT
USER odoo
# Tue, 28 Nov 2023 23:39:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Nov 2023 23:39:15 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a28800da8ad810dcb3060b9a249d76f10fc059eb9ea15aa7bb1fcfd0755b607`  
		Last Modified: Tue, 21 Nov 2023 06:13:44 GMT  
		Size: 220.3 MB (220297479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd5e822cfaa6f1e0ff1254d563b0f9fae55e9a37a6461f685b61ba68642687e`  
		Last Modified: Tue, 21 Nov 2023 06:13:20 GMT  
		Size: 2.6 MB (2625685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c2fe85ca0f057eeac7b5d2f65043d55dd0192357c143eca092e3fcdb6f1826`  
		Last Modified: Tue, 21 Nov 2023 06:13:20 GMT  
		Size: 459.5 KB (459485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2d62dc7a84225d80e241450ca7f1c3c8352369bab05d6ab9503a472caf32ba`  
		Last Modified: Tue, 28 Nov 2023 23:41:43 GMT  
		Size: 308.2 MB (308241022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc53506b74d5f16bfb8f2f9818f90fcf74f7382e5634f9c6b84990564363a44a`  
		Last Modified: Tue, 28 Nov 2023 23:41:10 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84884fc611d342bb1c81fdac836a35499c4a8916b6fb07a0104559fff4724586`  
		Last Modified: Tue, 28 Nov 2023 23:41:10 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ee7833223295aa1607a3c5007b9ed6c45822b87a6378964d67c3239943d141`  
		Last Modified: Tue, 28 Nov 2023 23:41:10 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5afe1ec8c776632dce8a00e55efcbfd0b25bd07093b6dc81802688e197ac2a`  
		Last Modified: Tue, 28 Nov 2023 23:41:10 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:4c089245a26ad3db9297c3dcf6d586971ee2c1c3c2f4efac3c256f24f5c4303b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:b5d39be042bf07b6f15bd12211cf4bcf217823636792cf6c459bfeab3746f36b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.3 MB (577299005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e7d957b83fff0620627dbe7fa94700876bce0bc3c5db97f728a6f6642782803`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:00 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 21 Nov 2023 06:06:00 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 21 Nov 2023 06:06:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 06:06:00 GMT
ARG TARGETARCH
# Tue, 21 Nov 2023 06:07:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 21 Nov 2023 06:07:24 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:07:25 GMT
RUN npm install -g rtlcss
# Tue, 21 Nov 2023 06:07:25 GMT
ENV ODOO_VERSION=16.0
# Tue, 28 Nov 2023 23:36:20 GMT
ARG ODOO_RELEASE=20231127
# Tue, 28 Nov 2023 23:36:20 GMT
ARG ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
# Tue, 28 Nov 2023 23:37:40 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 28 Nov 2023 23:37:45 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 28 Nov 2023 23:37:45 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 28 Nov 2023 23:37:45 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 28 Nov 2023 23:37:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 28 Nov 2023 23:37:45 GMT
EXPOSE 8069 8071 8072
# Tue, 28 Nov 2023 23:37:46 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 28 Nov 2023 23:37:46 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 28 Nov 2023 23:37:46 GMT
USER odoo
# Tue, 28 Nov 2023 23:37:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Nov 2023 23:37:46 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66dcf73708692fc6d6dee7d004e9c2f7d2fb47f905fbbc62dc61f2daffceb17`  
		Last Modified: Tue, 21 Nov 2023 06:12:58 GMT  
		Size: 219.6 MB (219606563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f096532668b80e067c70ebffa93b9ba9b5efa7080f7cf42b36ccb58a90e3508`  
		Last Modified: Tue, 21 Nov 2023 06:12:34 GMT  
		Size: 2.6 MB (2629834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ce0ca6176cbb017ef1b39cc6364b8f0620ac11996f8f6f959fb01195040a7b`  
		Last Modified: Tue, 21 Nov 2023 06:12:33 GMT  
		Size: 459.5 KB (459472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2802c5ce230e9ccea7da615906364d23deb330209c9e73afcfd021c25c167bf6`  
		Last Modified: Tue, 28 Nov 2023 23:41:00 GMT  
		Size: 323.2 MB (323182849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d03116eb0dc8e1cc72568d9efd2224eb5d8dc0438b9bfc33a07675786f289a`  
		Last Modified: Tue, 28 Nov 2023 23:40:24 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121a4fca1aeb8664f35503052bb16ba656c3ca322aa944e75a400338c3033ff0`  
		Last Modified: Tue, 28 Nov 2023 23:40:24 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d93a81fba2a56b164c488d207177b6979414161f55dc7d8b05961c3ec5cce2`  
		Last Modified: Tue, 28 Nov 2023 23:40:24 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc9dffbaf1db9065dad5aeab3ff57d7b3b98dc81977e19d2c33c10c1abc1656`  
		Last Modified: Tue, 28 Nov 2023 23:40:24 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:11ee49f510f40f61a7be75b8221bcde84320ca5d1d2ca943f6010e8ee95e7dc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.9 MB (572915587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6a83d4d02d85f700a89b5af7b2084c26585d6b1d6214974937f028ab33304e`
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
# Tue, 28 Nov 2023 23:56:35 GMT
ARG ODOO_RELEASE=20231127
# Tue, 28 Nov 2023 23:56:35 GMT
ARG ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
# Tue, 28 Nov 2023 23:57:50 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 28 Nov 2023 23:57:57 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 28 Nov 2023 23:57:57 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 28 Nov 2023 23:57:57 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 28 Nov 2023 23:57:58 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 28 Nov 2023 23:57:58 GMT
EXPOSE 8069 8071 8072
# Tue, 28 Nov 2023 23:57:58 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 28 Nov 2023 23:57:58 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 28 Nov 2023 23:57:58 GMT
USER odoo
# Tue, 28 Nov 2023 23:57:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Nov 2023 23:57:58 GMT
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
	-	`sha256:86cbb6e4cc780b8d58b6d67601ffc48c6c4d735b3b63feb3346da17b1e501863`  
		Last Modified: Tue, 28 Nov 2023 23:59:40 GMT  
		Size: 322.8 MB (322846403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa67c5dad3ca8eee6dc993708f0d4bfeb1969a20ab795c6b629ce2b6ec4f246`  
		Last Modified: Tue, 28 Nov 2023 23:59:11 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f1e168b52fab7401e5ab018f68f464cc34a16afcc79b3f826b8246ccbc4472`  
		Last Modified: Tue, 28 Nov 2023 23:59:11 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724cd6c49ffcff2bfeb098705d2aec6309c18426a70214bbae7ca177fbb6dfbf`  
		Last Modified: Tue, 28 Nov 2023 23:59:11 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf0c643f2e1b6270c09939dfe5d7fc1b03f7b456e72043b01ae81a56655aa94`  
		Last Modified: Tue, 28 Nov 2023 23:59:11 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16` - linux; ppc64le

```console
$ docker pull odoo@sha256:88121765b1a6469f8f0fe6d29d9e7bc24e2242bc751fa1b1f2255dd3b7a57506
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **591.8 MB (591838095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2c895fc081d72d2e1ebac2cdf92b23359f4bd0fbebb9c06e512da1f8be9300f`
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
# Tue, 28 Nov 2023 23:25:53 GMT
ARG ODOO_RELEASE=20231127
# Tue, 28 Nov 2023 23:25:54 GMT
ARG ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
# Tue, 28 Nov 2023 23:28:09 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 28 Nov 2023 23:28:28 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 28 Nov 2023 23:28:28 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 28 Nov 2023 23:28:29 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 28 Nov 2023 23:28:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 28 Nov 2023 23:28:30 GMT
EXPOSE 8069 8071 8072
# Tue, 28 Nov 2023 23:28:31 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 28 Nov 2023 23:28:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 28 Nov 2023 23:28:31 GMT
USER odoo
# Tue, 28 Nov 2023 23:28:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Nov 2023 23:28:32 GMT
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
	-	`sha256:ec1bb8e020e98e71023b53e75057a7a2f00d8f9061aedba34eea06d135af55ed`  
		Last Modified: Tue, 28 Nov 2023 23:30:38 GMT  
		Size: 324.6 MB (324608574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab63dc7971c6de9f051218064e755d018d356be99c2e24223a1b75783cc4bd1`  
		Last Modified: Tue, 28 Nov 2023 23:29:54 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a69ff9a7a00031ee77d8f16b56e22dc03cd35f02202510cf1505d22f515306d`  
		Last Modified: Tue, 28 Nov 2023 23:29:54 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c182ff19ecce1588d7b08e32948a679b77bf6b7cc202f4f5218132d4469c3224`  
		Last Modified: Tue, 28 Nov 2023 23:29:54 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658e9bbbd117fd6c48ab7c076c4fef6a53b2bfcccaaa2ebe37e0510dc0134c7`  
		Last Modified: Tue, 28 Nov 2023 23:29:54 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:4c089245a26ad3db9297c3dcf6d586971ee2c1c3c2f4efac3c256f24f5c4303b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:b5d39be042bf07b6f15bd12211cf4bcf217823636792cf6c459bfeab3746f36b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.3 MB (577299005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e7d957b83fff0620627dbe7fa94700876bce0bc3c5db97f728a6f6642782803`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:06:00 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 21 Nov 2023 06:06:00 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 21 Nov 2023 06:06:00 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 06:06:00 GMT
ARG TARGETARCH
# Tue, 21 Nov 2023 06:07:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 21 Nov 2023 06:07:24 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:07:25 GMT
RUN npm install -g rtlcss
# Tue, 21 Nov 2023 06:07:25 GMT
ENV ODOO_VERSION=16.0
# Tue, 28 Nov 2023 23:36:20 GMT
ARG ODOO_RELEASE=20231127
# Tue, 28 Nov 2023 23:36:20 GMT
ARG ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
# Tue, 28 Nov 2023 23:37:40 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 28 Nov 2023 23:37:45 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 28 Nov 2023 23:37:45 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 28 Nov 2023 23:37:45 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 28 Nov 2023 23:37:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 28 Nov 2023 23:37:45 GMT
EXPOSE 8069 8071 8072
# Tue, 28 Nov 2023 23:37:46 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 28 Nov 2023 23:37:46 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 28 Nov 2023 23:37:46 GMT
USER odoo
# Tue, 28 Nov 2023 23:37:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Nov 2023 23:37:46 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66dcf73708692fc6d6dee7d004e9c2f7d2fb47f905fbbc62dc61f2daffceb17`  
		Last Modified: Tue, 21 Nov 2023 06:12:58 GMT  
		Size: 219.6 MB (219606563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f096532668b80e067c70ebffa93b9ba9b5efa7080f7cf42b36ccb58a90e3508`  
		Last Modified: Tue, 21 Nov 2023 06:12:34 GMT  
		Size: 2.6 MB (2629834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ce0ca6176cbb017ef1b39cc6364b8f0620ac11996f8f6f959fb01195040a7b`  
		Last Modified: Tue, 21 Nov 2023 06:12:33 GMT  
		Size: 459.5 KB (459472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2802c5ce230e9ccea7da615906364d23deb330209c9e73afcfd021c25c167bf6`  
		Last Modified: Tue, 28 Nov 2023 23:41:00 GMT  
		Size: 323.2 MB (323182849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d03116eb0dc8e1cc72568d9efd2224eb5d8dc0438b9bfc33a07675786f289a`  
		Last Modified: Tue, 28 Nov 2023 23:40:24 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121a4fca1aeb8664f35503052bb16ba656c3ca322aa944e75a400338c3033ff0`  
		Last Modified: Tue, 28 Nov 2023 23:40:24 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d93a81fba2a56b164c488d207177b6979414161f55dc7d8b05961c3ec5cce2`  
		Last Modified: Tue, 28 Nov 2023 23:40:24 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc9dffbaf1db9065dad5aeab3ff57d7b3b98dc81977e19d2c33c10c1abc1656`  
		Last Modified: Tue, 28 Nov 2023 23:40:24 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16.0` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:11ee49f510f40f61a7be75b8221bcde84320ca5d1d2ca943f6010e8ee95e7dc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.9 MB (572915587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6a83d4d02d85f700a89b5af7b2084c26585d6b1d6214974937f028ab33304e`
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
# Tue, 28 Nov 2023 23:56:35 GMT
ARG ODOO_RELEASE=20231127
# Tue, 28 Nov 2023 23:56:35 GMT
ARG ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
# Tue, 28 Nov 2023 23:57:50 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 28 Nov 2023 23:57:57 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 28 Nov 2023 23:57:57 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 28 Nov 2023 23:57:57 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 28 Nov 2023 23:57:58 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 28 Nov 2023 23:57:58 GMT
EXPOSE 8069 8071 8072
# Tue, 28 Nov 2023 23:57:58 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 28 Nov 2023 23:57:58 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 28 Nov 2023 23:57:58 GMT
USER odoo
# Tue, 28 Nov 2023 23:57:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Nov 2023 23:57:58 GMT
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
	-	`sha256:86cbb6e4cc780b8d58b6d67601ffc48c6c4d735b3b63feb3346da17b1e501863`  
		Last Modified: Tue, 28 Nov 2023 23:59:40 GMT  
		Size: 322.8 MB (322846403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa67c5dad3ca8eee6dc993708f0d4bfeb1969a20ab795c6b629ce2b6ec4f246`  
		Last Modified: Tue, 28 Nov 2023 23:59:11 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f1e168b52fab7401e5ab018f68f464cc34a16afcc79b3f826b8246ccbc4472`  
		Last Modified: Tue, 28 Nov 2023 23:59:11 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724cd6c49ffcff2bfeb098705d2aec6309c18426a70214bbae7ca177fbb6dfbf`  
		Last Modified: Tue, 28 Nov 2023 23:59:11 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf0c643f2e1b6270c09939dfe5d7fc1b03f7b456e72043b01ae81a56655aa94`  
		Last Modified: Tue, 28 Nov 2023 23:59:11 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16.0` - linux; ppc64le

```console
$ docker pull odoo@sha256:88121765b1a6469f8f0fe6d29d9e7bc24e2242bc751fa1b1f2255dd3b7a57506
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **591.8 MB (591838095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2c895fc081d72d2e1ebac2cdf92b23359f4bd0fbebb9c06e512da1f8be9300f`
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
# Tue, 28 Nov 2023 23:25:53 GMT
ARG ODOO_RELEASE=20231127
# Tue, 28 Nov 2023 23:25:54 GMT
ARG ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
# Tue, 28 Nov 2023 23:28:09 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 28 Nov 2023 23:28:28 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 28 Nov 2023 23:28:28 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 28 Nov 2023 23:28:29 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=cf3fe2729f489476b5a07411a647667ed21e5208
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 28 Nov 2023 23:28:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 28 Nov 2023 23:28:30 GMT
EXPOSE 8069 8071 8072
# Tue, 28 Nov 2023 23:28:31 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 28 Nov 2023 23:28:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 28 Nov 2023 23:28:31 GMT
USER odoo
# Tue, 28 Nov 2023 23:28:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 28 Nov 2023 23:28:32 GMT
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
	-	`sha256:ec1bb8e020e98e71023b53e75057a7a2f00d8f9061aedba34eea06d135af55ed`  
		Last Modified: Tue, 28 Nov 2023 23:30:38 GMT  
		Size: 324.6 MB (324608574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab63dc7971c6de9f051218064e755d018d356be99c2e24223a1b75783cc4bd1`  
		Last Modified: Tue, 28 Nov 2023 23:29:54 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a69ff9a7a00031ee77d8f16b56e22dc03cd35f02202510cf1505d22f515306d`  
		Last Modified: Tue, 28 Nov 2023 23:29:54 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c182ff19ecce1588d7b08e32948a679b77bf6b7cc202f4f5218132d4469c3224`  
		Last Modified: Tue, 28 Nov 2023 23:29:54 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658e9bbbd117fd6c48ab7c076c4fef6a53b2bfcccaaa2ebe37e0510dc0134c7`  
		Last Modified: Tue, 28 Nov 2023 23:29:54 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:17`

```console
$ docker pull odoo@sha256:c5f6adf5b291de86c8cee45dadf6a64e1601d8ad03771ddb8d0ab32ba5cf15e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:17` - linux; amd64

```console
$ docker pull odoo@sha256:9614fa7a5aa72d4cd462dd286eb7520681e3ef7149f2a8c3c6575bdbfc1e7ee2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.2 MB (593182110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c299d6f2e0704e14f7cb259ee0f48b435465f884c7d02d7f022f5a7bd9bbf9e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:47:37 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 02 Dec 2023 04:47:37 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 02 Dec 2023 04:47:37 GMT
ENV LANG=en_US.UTF-8
# Sat, 02 Dec 2023 04:47:38 GMT
ARG TARGETARCH
# Sat, 02 Dec 2023 04:50:45 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 02 Dec 2023 04:50:57 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 04:50:59 GMT
RUN npm install -g rtlcss
# Sat, 02 Dec 2023 04:50:59 GMT
ENV ODOO_VERSION=17.0
# Sat, 02 Dec 2023 04:50:59 GMT
ARG ODOO_RELEASE=20231127
# Sat, 02 Dec 2023 04:50:59 GMT
ARG ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
# Sat, 02 Dec 2023 04:53:17 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 02 Dec 2023 04:53:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 02 Dec 2023 04:53:22 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 02 Dec 2023 04:53:22 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 02 Dec 2023 04:53:22 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 02 Dec 2023 04:53:22 GMT
EXPOSE 8069 8071 8072
# Sat, 02 Dec 2023 04:53:23 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 02 Dec 2023 04:53:23 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 02 Dec 2023 04:53:23 GMT
USER odoo
# Sat, 02 Dec 2023 04:53:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:53:23 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b6d74eb5ad38b6aacfcfa4daf56cc8c38f636f6a9ddc69a04479cc6ac5c9d6`  
		Last Modified: Sat, 02 Dec 2023 04:54:11 GMT  
		Size: 233.7 MB (233729758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80d621136e37a3ed7ade9ae6cb3ea6e0f4a6e19048001676d922e096d79dd1`  
		Last Modified: Sat, 02 Dec 2023 04:53:45 GMT  
		Size: 2.5 MB (2526589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2c0ff2e7c8fdf34a67f3c215228454c4fab667f328176b9dbc46170300ae6c`  
		Last Modified: Sat, 02 Dec 2023 04:53:44 GMT  
		Size: 461.1 KB (461067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d38fd572133930f4031eda2a43ea7de8f2a03995164899e2f68439f2512d85`  
		Last Modified: Sat, 02 Dec 2023 04:54:20 GMT  
		Size: 326.0 MB (326015907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977a9e535a18c9ad9de47f0d5fab0102a3daa589edf56ac68896939bcaa18d2c`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7d453e835c2abaa9d5257da5952e4048289969fdaca59fc9e7ee02af9baf0c`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76040b268990ece48bbf93da6184ad8ef22850c910b3057ec42d39c9b17d3aa`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7704ddbd5791b40a71bcee8e16e9997f28bd65710d5c7d9988aaec5931d70e3`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:8edf84a1f05de7ebe89bfa3effc1eb0ab7ee41afaf91891aede684bd8e973e0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.1 MB (588132889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15b6f400f0ce6451fe4da113a118d3b5e5263cd06541a0ae462fdbbdd04afee6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:15:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 02 Dec 2023 06:15:40 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 02 Dec 2023 06:15:40 GMT
ENV LANG=en_US.UTF-8
# Sat, 02 Dec 2023 06:15:40 GMT
ARG TARGETARCH
# Sat, 02 Dec 2023 06:18:17 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 02 Dec 2023 06:18:30 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:18:32 GMT
RUN npm install -g rtlcss
# Sat, 02 Dec 2023 06:18:32 GMT
ENV ODOO_VERSION=17.0
# Sat, 02 Dec 2023 06:18:32 GMT
ARG ODOO_RELEASE=20231127
# Sat, 02 Dec 2023 06:18:32 GMT
ARG ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
# Sat, 02 Dec 2023 06:20:22 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 02 Dec 2023 06:20:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 02 Dec 2023 06:20:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 02 Dec 2023 06:20:30 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 02 Dec 2023 06:20:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 02 Dec 2023 06:20:30 GMT
EXPOSE 8069 8071 8072
# Sat, 02 Dec 2023 06:20:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 02 Dec 2023 06:20:30 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 02 Dec 2023 06:20:30 GMT
USER odoo
# Sat, 02 Dec 2023 06:20:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 06:20:30 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2fbd5e011298a1d82b09d9b103b3c85586d12025686fb197205c02c5e340a2`  
		Last Modified: Sat, 02 Dec 2023 06:21:02 GMT  
		Size: 231.1 MB (231107816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c833560543c45eaf5583c723b991238f3600ac24ba07a362da30f82f6be8dc6`  
		Last Modified: Sat, 02 Dec 2023 06:20:43 GMT  
		Size: 2.5 MB (2520301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1617b34d74ba2e5b95ad66ee5cbc43579012bff1caa24cc6327fee160dc62cc`  
		Last Modified: Sat, 02 Dec 2023 06:20:43 GMT  
		Size: 461.1 KB (461073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d888e8255b1b19ae2041842ea868c82ea9590dd521248d48b5e7cc901c8d5f75`  
		Last Modified: Sat, 02 Dec 2023 06:21:10 GMT  
		Size: 325.6 MB (325641300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e6a1d338f2174c7ee9e44d8d00bb69f3d5f7a4a5b1e40abd6208ab1111750e`  
		Last Modified: Sat, 02 Dec 2023 06:20:40 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896d01bcc6c7996029b9dd77ba2e4f5ccd6ae97c3d481b15de2cea21a2eb9bdc`  
		Last Modified: Sat, 02 Dec 2023 06:20:41 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0871c8844791b9a4cd6936e9573838c17187dfaec99605f6b4cf8393446cf721`  
		Last Modified: Sat, 02 Dec 2023 06:20:41 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3540901db512165b70093e595a95ab04525bdec5fd1abd93f4b10a4bf5e748d`  
		Last Modified: Sat, 02 Dec 2023 06:20:40 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17` - linux; ppc64le

```console
$ docker pull odoo@sha256:6d493aef39fcf0d2fcbfc9d008d19d0bfa9a348a5a42b39c33ab2f5935507fce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.0 MB (609989156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad770c0893e4bad5fbb22b436a589d10d159996e7eecc4136caf68c61845e410`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:09:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 02 Dec 2023 05:09:22 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 02 Dec 2023 05:09:22 GMT
ENV LANG=en_US.UTF-8
# Sat, 02 Dec 2023 05:09:22 GMT
ARG TARGETARCH
# Sat, 02 Dec 2023 05:13:13 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 02 Dec 2023 05:13:36 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:13:39 GMT
RUN npm install -g rtlcss
# Sat, 02 Dec 2023 05:13:40 GMT
ENV ODOO_VERSION=17.0
# Sat, 02 Dec 2023 05:13:40 GMT
ARG ODOO_RELEASE=20231127
# Sat, 02 Dec 2023 05:13:40 GMT
ARG ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
# Sat, 02 Dec 2023 05:16:33 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 02 Dec 2023 05:16:48 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 02 Dec 2023 05:16:48 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 02 Dec 2023 05:16:49 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 02 Dec 2023 05:16:50 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 02 Dec 2023 05:16:50 GMT
EXPOSE 8069 8071 8072
# Sat, 02 Dec 2023 05:16:51 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 02 Dec 2023 05:16:51 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 02 Dec 2023 05:16:52 GMT
USER odoo
# Sat, 02 Dec 2023 05:16:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 05:16:53 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c3606768af36fe4984cee7cfc0c9d919a7adf83ac4c1849c30da06916b9ec921`  
		Last Modified: Sat, 02 Dec 2023 04:49:10 GMT  
		Size: 35.7 MB (35662741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cab7e6a789250f903ab04c7af36f05cd95ad421f0010687d51d44f865da474e`  
		Last Modified: Sat, 02 Dec 2023 05:17:45 GMT  
		Size: 243.3 MB (243295005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd18f49b132cf82e3cdcec078326873093460ffc189fa35b8d1f0e19e565cfc8`  
		Last Modified: Sat, 02 Dec 2023 05:17:14 GMT  
		Size: 2.8 MB (2803163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83d21ff7071f1369530b67a6fb2780158786764eba5660a64fcde9124c5fe65`  
		Last Modified: Sat, 02 Dec 2023 05:17:13 GMT  
		Size: 461.2 KB (461214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25473efa8f0b4c53797f1a140c30d35e307f37c8792f1eed88cba359489fa472`  
		Last Modified: Sat, 02 Dec 2023 05:17:54 GMT  
		Size: 327.8 MB (327764570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263dd6b71ac44399dc380fe76de830702f54b627aed16c8eedacbe5cbdcb34ab`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40399667f6471bbcc7152ccdc91b29ebfe7704fe71536353a90231b3e3158b2`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c772392219d0ef8acd7992c480cb13d54fac3d5f39c30859896b882ca9b7cbfd`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6effa562135750af2f2b02da1db4a13707bebc6554ae44e4221e3068499061b`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:17.0`

```console
$ docker pull odoo@sha256:c5f6adf5b291de86c8cee45dadf6a64e1601d8ad03771ddb8d0ab32ba5cf15e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:17.0` - linux; amd64

```console
$ docker pull odoo@sha256:9614fa7a5aa72d4cd462dd286eb7520681e3ef7149f2a8c3c6575bdbfc1e7ee2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.2 MB (593182110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c299d6f2e0704e14f7cb259ee0f48b435465f884c7d02d7f022f5a7bd9bbf9e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:47:37 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 02 Dec 2023 04:47:37 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 02 Dec 2023 04:47:37 GMT
ENV LANG=en_US.UTF-8
# Sat, 02 Dec 2023 04:47:38 GMT
ARG TARGETARCH
# Sat, 02 Dec 2023 04:50:45 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 02 Dec 2023 04:50:57 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 04:50:59 GMT
RUN npm install -g rtlcss
# Sat, 02 Dec 2023 04:50:59 GMT
ENV ODOO_VERSION=17.0
# Sat, 02 Dec 2023 04:50:59 GMT
ARG ODOO_RELEASE=20231127
# Sat, 02 Dec 2023 04:50:59 GMT
ARG ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
# Sat, 02 Dec 2023 04:53:17 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 02 Dec 2023 04:53:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 02 Dec 2023 04:53:22 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 02 Dec 2023 04:53:22 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 02 Dec 2023 04:53:22 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 02 Dec 2023 04:53:22 GMT
EXPOSE 8069 8071 8072
# Sat, 02 Dec 2023 04:53:23 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 02 Dec 2023 04:53:23 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 02 Dec 2023 04:53:23 GMT
USER odoo
# Sat, 02 Dec 2023 04:53:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:53:23 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b6d74eb5ad38b6aacfcfa4daf56cc8c38f636f6a9ddc69a04479cc6ac5c9d6`  
		Last Modified: Sat, 02 Dec 2023 04:54:11 GMT  
		Size: 233.7 MB (233729758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80d621136e37a3ed7ade9ae6cb3ea6e0f4a6e19048001676d922e096d79dd1`  
		Last Modified: Sat, 02 Dec 2023 04:53:45 GMT  
		Size: 2.5 MB (2526589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2c0ff2e7c8fdf34a67f3c215228454c4fab667f328176b9dbc46170300ae6c`  
		Last Modified: Sat, 02 Dec 2023 04:53:44 GMT  
		Size: 461.1 KB (461067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d38fd572133930f4031eda2a43ea7de8f2a03995164899e2f68439f2512d85`  
		Last Modified: Sat, 02 Dec 2023 04:54:20 GMT  
		Size: 326.0 MB (326015907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977a9e535a18c9ad9de47f0d5fab0102a3daa589edf56ac68896939bcaa18d2c`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7d453e835c2abaa9d5257da5952e4048289969fdaca59fc9e7ee02af9baf0c`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76040b268990ece48bbf93da6184ad8ef22850c910b3057ec42d39c9b17d3aa`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7704ddbd5791b40a71bcee8e16e9997f28bd65710d5c7d9988aaec5931d70e3`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17.0` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:8edf84a1f05de7ebe89bfa3effc1eb0ab7ee41afaf91891aede684bd8e973e0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.1 MB (588132889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15b6f400f0ce6451fe4da113a118d3b5e5263cd06541a0ae462fdbbdd04afee6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:15:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 02 Dec 2023 06:15:40 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 02 Dec 2023 06:15:40 GMT
ENV LANG=en_US.UTF-8
# Sat, 02 Dec 2023 06:15:40 GMT
ARG TARGETARCH
# Sat, 02 Dec 2023 06:18:17 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 02 Dec 2023 06:18:30 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:18:32 GMT
RUN npm install -g rtlcss
# Sat, 02 Dec 2023 06:18:32 GMT
ENV ODOO_VERSION=17.0
# Sat, 02 Dec 2023 06:18:32 GMT
ARG ODOO_RELEASE=20231127
# Sat, 02 Dec 2023 06:18:32 GMT
ARG ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
# Sat, 02 Dec 2023 06:20:22 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 02 Dec 2023 06:20:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 02 Dec 2023 06:20:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 02 Dec 2023 06:20:30 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 02 Dec 2023 06:20:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 02 Dec 2023 06:20:30 GMT
EXPOSE 8069 8071 8072
# Sat, 02 Dec 2023 06:20:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 02 Dec 2023 06:20:30 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 02 Dec 2023 06:20:30 GMT
USER odoo
# Sat, 02 Dec 2023 06:20:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 06:20:30 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2fbd5e011298a1d82b09d9b103b3c85586d12025686fb197205c02c5e340a2`  
		Last Modified: Sat, 02 Dec 2023 06:21:02 GMT  
		Size: 231.1 MB (231107816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c833560543c45eaf5583c723b991238f3600ac24ba07a362da30f82f6be8dc6`  
		Last Modified: Sat, 02 Dec 2023 06:20:43 GMT  
		Size: 2.5 MB (2520301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1617b34d74ba2e5b95ad66ee5cbc43579012bff1caa24cc6327fee160dc62cc`  
		Last Modified: Sat, 02 Dec 2023 06:20:43 GMT  
		Size: 461.1 KB (461073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d888e8255b1b19ae2041842ea868c82ea9590dd521248d48b5e7cc901c8d5f75`  
		Last Modified: Sat, 02 Dec 2023 06:21:10 GMT  
		Size: 325.6 MB (325641300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e6a1d338f2174c7ee9e44d8d00bb69f3d5f7a4a5b1e40abd6208ab1111750e`  
		Last Modified: Sat, 02 Dec 2023 06:20:40 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896d01bcc6c7996029b9dd77ba2e4f5ccd6ae97c3d481b15de2cea21a2eb9bdc`  
		Last Modified: Sat, 02 Dec 2023 06:20:41 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0871c8844791b9a4cd6936e9573838c17187dfaec99605f6b4cf8393446cf721`  
		Last Modified: Sat, 02 Dec 2023 06:20:41 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3540901db512165b70093e595a95ab04525bdec5fd1abd93f4b10a4bf5e748d`  
		Last Modified: Sat, 02 Dec 2023 06:20:40 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17.0` - linux; ppc64le

```console
$ docker pull odoo@sha256:6d493aef39fcf0d2fcbfc9d008d19d0bfa9a348a5a42b39c33ab2f5935507fce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.0 MB (609989156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad770c0893e4bad5fbb22b436a589d10d159996e7eecc4136caf68c61845e410`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:09:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 02 Dec 2023 05:09:22 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 02 Dec 2023 05:09:22 GMT
ENV LANG=en_US.UTF-8
# Sat, 02 Dec 2023 05:09:22 GMT
ARG TARGETARCH
# Sat, 02 Dec 2023 05:13:13 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 02 Dec 2023 05:13:36 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:13:39 GMT
RUN npm install -g rtlcss
# Sat, 02 Dec 2023 05:13:40 GMT
ENV ODOO_VERSION=17.0
# Sat, 02 Dec 2023 05:13:40 GMT
ARG ODOO_RELEASE=20231127
# Sat, 02 Dec 2023 05:13:40 GMT
ARG ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
# Sat, 02 Dec 2023 05:16:33 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 02 Dec 2023 05:16:48 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 02 Dec 2023 05:16:48 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 02 Dec 2023 05:16:49 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 02 Dec 2023 05:16:50 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 02 Dec 2023 05:16:50 GMT
EXPOSE 8069 8071 8072
# Sat, 02 Dec 2023 05:16:51 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 02 Dec 2023 05:16:51 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 02 Dec 2023 05:16:52 GMT
USER odoo
# Sat, 02 Dec 2023 05:16:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 05:16:53 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c3606768af36fe4984cee7cfc0c9d919a7adf83ac4c1849c30da06916b9ec921`  
		Last Modified: Sat, 02 Dec 2023 04:49:10 GMT  
		Size: 35.7 MB (35662741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cab7e6a789250f903ab04c7af36f05cd95ad421f0010687d51d44f865da474e`  
		Last Modified: Sat, 02 Dec 2023 05:17:45 GMT  
		Size: 243.3 MB (243295005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd18f49b132cf82e3cdcec078326873093460ffc189fa35b8d1f0e19e565cfc8`  
		Last Modified: Sat, 02 Dec 2023 05:17:14 GMT  
		Size: 2.8 MB (2803163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83d21ff7071f1369530b67a6fb2780158786764eba5660a64fcde9124c5fe65`  
		Last Modified: Sat, 02 Dec 2023 05:17:13 GMT  
		Size: 461.2 KB (461214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25473efa8f0b4c53797f1a140c30d35e307f37c8792f1eed88cba359489fa472`  
		Last Modified: Sat, 02 Dec 2023 05:17:54 GMT  
		Size: 327.8 MB (327764570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263dd6b71ac44399dc380fe76de830702f54b627aed16c8eedacbe5cbdcb34ab`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40399667f6471bbcc7152ccdc91b29ebfe7704fe71536353a90231b3e3158b2`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c772392219d0ef8acd7992c480cb13d54fac3d5f39c30859896b882ca9b7cbfd`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6effa562135750af2f2b02da1db4a13707bebc6554ae44e4221e3068499061b`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:c5f6adf5b291de86c8cee45dadf6a64e1601d8ad03771ddb8d0ab32ba5cf15e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:9614fa7a5aa72d4cd462dd286eb7520681e3ef7149f2a8c3c6575bdbfc1e7ee2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.2 MB (593182110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c299d6f2e0704e14f7cb259ee0f48b435465f884c7d02d7f022f5a7bd9bbf9e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 01 Dec 2023 07:49:48 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:49:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:49:48 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:49:50 GMT
ADD file:36d444e2cede3abe58191dcf28890b874c0908f5259bf7e8855338555701c4c5 in / 
# Fri, 01 Dec 2023 07:49:50 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:47:37 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 02 Dec 2023 04:47:37 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 02 Dec 2023 04:47:37 GMT
ENV LANG=en_US.UTF-8
# Sat, 02 Dec 2023 04:47:38 GMT
ARG TARGETARCH
# Sat, 02 Dec 2023 04:50:45 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 02 Dec 2023 04:50:57 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 04:50:59 GMT
RUN npm install -g rtlcss
# Sat, 02 Dec 2023 04:50:59 GMT
ENV ODOO_VERSION=17.0
# Sat, 02 Dec 2023 04:50:59 GMT
ARG ODOO_RELEASE=20231127
# Sat, 02 Dec 2023 04:50:59 GMT
ARG ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
# Sat, 02 Dec 2023 04:53:17 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 02 Dec 2023 04:53:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 02 Dec 2023 04:53:22 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 02 Dec 2023 04:53:22 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 02 Dec 2023 04:53:22 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 02 Dec 2023 04:53:22 GMT
EXPOSE 8069 8071 8072
# Sat, 02 Dec 2023 04:53:23 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 02 Dec 2023 04:53:23 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 02 Dec 2023 04:53:23 GMT
USER odoo
# Sat, 02 Dec 2023 04:53:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 04:53:23 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:cbe3537751ce03ea42788c2fbe2d5d336180dc2e20472c8cdba8b3224191d101`  
		Last Modified: Wed, 29 Nov 2023 19:24:54 GMT  
		Size: 30.4 MB (30446322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b6d74eb5ad38b6aacfcfa4daf56cc8c38f636f6a9ddc69a04479cc6ac5c9d6`  
		Last Modified: Sat, 02 Dec 2023 04:54:11 GMT  
		Size: 233.7 MB (233729758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80d621136e37a3ed7ade9ae6cb3ea6e0f4a6e19048001676d922e096d79dd1`  
		Last Modified: Sat, 02 Dec 2023 04:53:45 GMT  
		Size: 2.5 MB (2526589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2c0ff2e7c8fdf34a67f3c215228454c4fab667f328176b9dbc46170300ae6c`  
		Last Modified: Sat, 02 Dec 2023 04:53:44 GMT  
		Size: 461.1 KB (461067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d38fd572133930f4031eda2a43ea7de8f2a03995164899e2f68439f2512d85`  
		Last Modified: Sat, 02 Dec 2023 04:54:20 GMT  
		Size: 326.0 MB (326015907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977a9e535a18c9ad9de47f0d5fab0102a3daa589edf56ac68896939bcaa18d2c`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7d453e835c2abaa9d5257da5952e4048289969fdaca59fc9e7ee02af9baf0c`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76040b268990ece48bbf93da6184ad8ef22850c910b3057ec42d39c9b17d3aa`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7704ddbd5791b40a71bcee8e16e9997f28bd65710d5c7d9988aaec5931d70e3`  
		Last Modified: Sat, 02 Dec 2023 04:53:42 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:latest` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:8edf84a1f05de7ebe89bfa3effc1eb0ab7ee41afaf91891aede684bd8e973e0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.1 MB (588132889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15b6f400f0ce6451fe4da113a118d3b5e5263cd06541a0ae462fdbbdd04afee6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 01 Dec 2023 07:43:19 GMT
ARG RELEASE
# Fri, 01 Dec 2023 07:43:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 07:43:20 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 07:43:21 GMT
ADD file:891dcab0c4ce2880c4dca013d326a3efd7601003b6f5076938d678101e301b79 in / 
# Fri, 01 Dec 2023 07:43:22 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:15:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 02 Dec 2023 06:15:40 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 02 Dec 2023 06:15:40 GMT
ENV LANG=en_US.UTF-8
# Sat, 02 Dec 2023 06:15:40 GMT
ARG TARGETARCH
# Sat, 02 Dec 2023 06:18:17 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 02 Dec 2023 06:18:30 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:18:32 GMT
RUN npm install -g rtlcss
# Sat, 02 Dec 2023 06:18:32 GMT
ENV ODOO_VERSION=17.0
# Sat, 02 Dec 2023 06:18:32 GMT
ARG ODOO_RELEASE=20231127
# Sat, 02 Dec 2023 06:18:32 GMT
ARG ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
# Sat, 02 Dec 2023 06:20:22 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 02 Dec 2023 06:20:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 02 Dec 2023 06:20:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 02 Dec 2023 06:20:30 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 02 Dec 2023 06:20:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 02 Dec 2023 06:20:30 GMT
EXPOSE 8069 8071 8072
# Sat, 02 Dec 2023 06:20:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 02 Dec 2023 06:20:30 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 02 Dec 2023 06:20:30 GMT
USER odoo
# Sat, 02 Dec 2023 06:20:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 06:20:30 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:aeb9f260d781cd1e09daf0d0a9e5bcb581efce5b33b221f2f4a27de8db66e463`  
		Last Modified: Thu, 30 Nov 2023 02:35:43 GMT  
		Size: 28.4 MB (28399939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2fbd5e011298a1d82b09d9b103b3c85586d12025686fb197205c02c5e340a2`  
		Last Modified: Sat, 02 Dec 2023 06:21:02 GMT  
		Size: 231.1 MB (231107816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c833560543c45eaf5583c723b991238f3600ac24ba07a362da30f82f6be8dc6`  
		Last Modified: Sat, 02 Dec 2023 06:20:43 GMT  
		Size: 2.5 MB (2520301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1617b34d74ba2e5b95ad66ee5cbc43579012bff1caa24cc6327fee160dc62cc`  
		Last Modified: Sat, 02 Dec 2023 06:20:43 GMT  
		Size: 461.1 KB (461073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d888e8255b1b19ae2041842ea868c82ea9590dd521248d48b5e7cc901c8d5f75`  
		Last Modified: Sat, 02 Dec 2023 06:21:10 GMT  
		Size: 325.6 MB (325641300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e6a1d338f2174c7ee9e44d8d00bb69f3d5f7a4a5b1e40abd6208ab1111750e`  
		Last Modified: Sat, 02 Dec 2023 06:20:40 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896d01bcc6c7996029b9dd77ba2e4f5ccd6ae97c3d481b15de2cea21a2eb9bdc`  
		Last Modified: Sat, 02 Dec 2023 06:20:41 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0871c8844791b9a4cd6936e9573838c17187dfaec99605f6b4cf8393446cf721`  
		Last Modified: Sat, 02 Dec 2023 06:20:41 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3540901db512165b70093e595a95ab04525bdec5fd1abd93f4b10a4bf5e748d`  
		Last Modified: Sat, 02 Dec 2023 06:20:40 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:latest` - linux; ppc64le

```console
$ docker pull odoo@sha256:6d493aef39fcf0d2fcbfc9d008d19d0bfa9a348a5a42b39c33ab2f5935507fce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.0 MB (609989156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad770c0893e4bad5fbb22b436a589d10d159996e7eecc4136caf68c61845e410`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 01 Dec 2023 08:12:00 GMT
ARG RELEASE
# Fri, 01 Dec 2023 08:12:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 01 Dec 2023 08:12:00 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 01 Dec 2023 08:12:03 GMT
ADD file:80047e51fa5311c19317ab688acec0517d98f1cbf74fa4c22a7105e80ebaf610 in / 
# Fri, 01 Dec 2023 08:12:04 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:09:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 02 Dec 2023 05:09:22 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 02 Dec 2023 05:09:22 GMT
ENV LANG=en_US.UTF-8
# Sat, 02 Dec 2023 05:09:22 GMT
ARG TARGETARCH
# Sat, 02 Dec 2023 05:13:13 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 02 Dec 2023 05:13:36 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:13:39 GMT
RUN npm install -g rtlcss
# Sat, 02 Dec 2023 05:13:40 GMT
ENV ODOO_VERSION=17.0
# Sat, 02 Dec 2023 05:13:40 GMT
ARG ODOO_RELEASE=20231127
# Sat, 02 Dec 2023 05:13:40 GMT
ARG ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
# Sat, 02 Dec 2023 05:16:33 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 02 Dec 2023 05:16:48 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 02 Dec 2023 05:16:48 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 02 Dec 2023 05:16:49 GMT
# ARGS: ODOO_RELEASE=20231127 ODOO_SHA=b6953cecd2f06a24dc509cef277ffcd03f243a97
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 02 Dec 2023 05:16:50 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 02 Dec 2023 05:16:50 GMT
EXPOSE 8069 8071 8072
# Sat, 02 Dec 2023 05:16:51 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 02 Dec 2023 05:16:51 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 02 Dec 2023 05:16:52 GMT
USER odoo
# Sat, 02 Dec 2023 05:16:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 02 Dec 2023 05:16:53 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c3606768af36fe4984cee7cfc0c9d919a7adf83ac4c1849c30da06916b9ec921`  
		Last Modified: Sat, 02 Dec 2023 04:49:10 GMT  
		Size: 35.7 MB (35662741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cab7e6a789250f903ab04c7af36f05cd95ad421f0010687d51d44f865da474e`  
		Last Modified: Sat, 02 Dec 2023 05:17:45 GMT  
		Size: 243.3 MB (243295005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd18f49b132cf82e3cdcec078326873093460ffc189fa35b8d1f0e19e565cfc8`  
		Last Modified: Sat, 02 Dec 2023 05:17:14 GMT  
		Size: 2.8 MB (2803163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83d21ff7071f1369530b67a6fb2780158786764eba5660a64fcde9124c5fe65`  
		Last Modified: Sat, 02 Dec 2023 05:17:13 GMT  
		Size: 461.2 KB (461214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25473efa8f0b4c53797f1a140c30d35e307f37c8792f1eed88cba359489fa472`  
		Last Modified: Sat, 02 Dec 2023 05:17:54 GMT  
		Size: 327.8 MB (327764570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263dd6b71ac44399dc380fe76de830702f54b627aed16c8eedacbe5cbdcb34ab`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40399667f6471bbcc7152ccdc91b29ebfe7704fe71536353a90231b3e3158b2`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c772392219d0ef8acd7992c480cb13d54fac3d5f39c30859896b882ca9b7cbfd`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6effa562135750af2f2b02da1db4a13707bebc6554ae44e4221e3068499061b`  
		Last Modified: Sat, 02 Dec 2023 05:17:10 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
