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
$ docker pull odoo@sha256:1d981aa3abb3f282920284628fe05d34458845662f0f99bb7016cf4295bbf9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:b14eb9efff25191c381f75ff52e53ad6ae25e154685b258d0e317ad3138725e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.1 MB (563093108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899e8247ee70a30d7e50fb515c78b5e7baff832ee3e5e249ace1381810aa1b3e`
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
# Fri, 08 Dec 2023 20:45:18 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:45:18 GMT
ARG ODOO_SHA=ff20de27db7ead0a2fd690d4aa73ff9a47b0f09f
# Fri, 08 Dec 2023 20:46:33 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=ff20de27db7ead0a2fd690d4aa73ff9a47b0f09f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:46:37 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:46:37 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:46:38 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=ff20de27db7ead0a2fd690d4aa73ff9a47b0f09f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:46:38 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:46:38 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:46:38 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:46:38 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:46:38 GMT
USER odoo
# Fri, 08 Dec 2023 20:46:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:46:38 GMT
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
	-	`sha256:701cc6625581155da543d5ddab67f0f3393a7c6d7d9d5be0c02dbf2be7bf4627`  
		Last Modified: Fri, 08 Dec 2023 20:48:58 GMT  
		Size: 308.3 MB (308290172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baf687daf40964ce6a56ba6f2c5d7ad62f0e579edaa725fba99e3cd69dbb0c`  
		Last Modified: Fri, 08 Dec 2023 20:48:25 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6d5e29e3cb7cf72215ecf26d925aeb2b5d662d14baaf76751ac7e2abc68605`  
		Last Modified: Fri, 08 Dec 2023 20:48:25 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa13fbcda322479ba1be386a4fe5be00580a495375ee5793750b1296bff6c5f0`  
		Last Modified: Fri, 08 Dec 2023 20:48:25 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf74224e6f955dea1683cf37a5d37223ab88e1da6e9b6c694d35d41d8cc205f`  
		Last Modified: Fri, 08 Dec 2023 20:48:25 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:1d981aa3abb3f282920284628fe05d34458845662f0f99bb7016cf4295bbf9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:b14eb9efff25191c381f75ff52e53ad6ae25e154685b258d0e317ad3138725e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.1 MB (563093108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899e8247ee70a30d7e50fb515c78b5e7baff832ee3e5e249ace1381810aa1b3e`
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
# Fri, 08 Dec 2023 20:45:18 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:45:18 GMT
ARG ODOO_SHA=ff20de27db7ead0a2fd690d4aa73ff9a47b0f09f
# Fri, 08 Dec 2023 20:46:33 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=ff20de27db7ead0a2fd690d4aa73ff9a47b0f09f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:46:37 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:46:37 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:46:38 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=ff20de27db7ead0a2fd690d4aa73ff9a47b0f09f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:46:38 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:46:38 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:46:38 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:46:38 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:46:38 GMT
USER odoo
# Fri, 08 Dec 2023 20:46:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:46:38 GMT
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
	-	`sha256:701cc6625581155da543d5ddab67f0f3393a7c6d7d9d5be0c02dbf2be7bf4627`  
		Last Modified: Fri, 08 Dec 2023 20:48:58 GMT  
		Size: 308.3 MB (308290172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baf687daf40964ce6a56ba6f2c5d7ad62f0e579edaa725fba99e3cd69dbb0c`  
		Last Modified: Fri, 08 Dec 2023 20:48:25 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6d5e29e3cb7cf72215ecf26d925aeb2b5d662d14baaf76751ac7e2abc68605`  
		Last Modified: Fri, 08 Dec 2023 20:48:25 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa13fbcda322479ba1be386a4fe5be00580a495375ee5793750b1296bff6c5f0`  
		Last Modified: Fri, 08 Dec 2023 20:48:25 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf74224e6f955dea1683cf37a5d37223ab88e1da6e9b6c694d35d41d8cc205f`  
		Last Modified: Fri, 08 Dec 2023 20:48:25 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:5b65b8ce25fc15545c8781a1bcddf3627f74c954d542d268f5825bb1fdb50c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:6a11de1e6d641c6980a331b6113ea0e7fe26ced6ab5049c48fc221962022d4ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.4 MB (577431560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3038e167dd77f2564f4515388e55220052b3c3875a140fd0e780ffe0b8fa395`
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
# Fri, 08 Dec 2023 20:43:39 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:43:39 GMT
ARG ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
# Fri, 08 Dec 2023 20:45:02 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:45:05 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:45:06 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:45:06 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:45:06 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:45:06 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:45:06 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:45:07 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:45:07 GMT
USER odoo
# Fri, 08 Dec 2023 20:45:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:45:07 GMT
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
	-	`sha256:37f707bd79248dc4a0068dc8035be8b6fc33fe9d6bb2efea334ef73bcbc52da2`  
		Last Modified: Fri, 08 Dec 2023 20:48:15 GMT  
		Size: 323.3 MB (323315394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01bd0cda71d6674543ca736b840c622eabe42317757297a6ba306a95fdbb64e`  
		Last Modified: Fri, 08 Dec 2023 20:47:38 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884c169ca1b0a859b2e4a99db995cc296efb4589566d410802915fa9126ae27c`  
		Last Modified: Fri, 08 Dec 2023 20:47:38 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12135faee5518f22f029b4949eeaa6f3b31d0c4c4206ec07f48196bc9dc9bf3`  
		Last Modified: Fri, 08 Dec 2023 20:47:38 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a7a6aedbeab994a61db496169c616d97593c0624114550c0be7ae8118c1686`  
		Last Modified: Fri, 08 Dec 2023 20:47:38 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:a8f53468664cd1f8c249a638e4afa6d44c072861ea65f9865aeb911a8c359771
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.0 MB (573029481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:633d876138dfea48b2e4bc427ae378ae82b69c8aa6809be60094d9d6e78e8ea6`
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
# Fri, 08 Dec 2023 19:59:18 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 19:59:18 GMT
ARG ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
# Fri, 08 Dec 2023 20:00:31 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:00:38 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:00:38 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:00:39 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:00:39 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:00:39 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:00:39 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:00:39 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:00:39 GMT
USER odoo
# Fri, 08 Dec 2023 20:00:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:00:39 GMT
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
	-	`sha256:dca6c9a31e3038c6c59c584514d3543a5ed04d65585417fad7bd1a08779fa67f`  
		Last Modified: Fri, 08 Dec 2023 20:02:21 GMT  
		Size: 323.0 MB (322960299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339dd557785899b6ce705230df2b02bbe26c15935e86053d6f2939fcfee59d90`  
		Last Modified: Fri, 08 Dec 2023 20:01:52 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcae721c673b10423a864878a5efcc2b65e3405e07d4c76dd34348a4bf805c0a`  
		Last Modified: Fri, 08 Dec 2023 20:01:52 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ac15a8b5ddfe6eb46a71b3f7f59c5ef91d296d27f24ff38f7b859442b192e5`  
		Last Modified: Fri, 08 Dec 2023 20:01:52 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad95cab6488c0bde41a53c09c33e0e8163c540a7d13e04f3b25273fc71872490`  
		Last Modified: Fri, 08 Dec 2023 20:01:52 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16` - linux; ppc64le

```console
$ docker pull odoo@sha256:53ba84b6c68d61769a86cc877df73145163fe9d6aa544460d8e18b2df8bd51e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.0 MB (591985599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6224fc3ec9d500aab0c050c4998ca6d820606369c51bf6b7c67436431a240663`
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
# Fri, 08 Dec 2023 20:49:07 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:49:08 GMT
ARG ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
# Fri, 08 Dec 2023 20:51:44 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:52:04 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:52:05 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:52:06 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:52:07 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:52:08 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:52:08 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:52:09 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:52:11 GMT
USER odoo
# Fri, 08 Dec 2023 20:52:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:52:12 GMT
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
	-	`sha256:03322b58d7809de36be6d5fc87a142b6bf429d189b18e279da2525c0d44d46f1`  
		Last Modified: Fri, 08 Dec 2023 20:54:15 GMT  
		Size: 324.8 MB (324756073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e64f4d117675449eb0708db0fed39c6b83e6d0566349226dda5b307f1e5ed6`  
		Last Modified: Fri, 08 Dec 2023 20:53:31 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea8c3c55f7bae2089152930ca7e33cdbc5e3adeffd3613ed40bf636cb8a8a51`  
		Last Modified: Fri, 08 Dec 2023 20:53:31 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85bec24deab524fc3cf80b50304550adc3352f1ad26a227a3d32bfdc484c17b`  
		Last Modified: Fri, 08 Dec 2023 20:53:31 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd8a8d0a7ba36a73fdba14e2e3946c56ffcd8a7b94d2289f0e8cd6f226c2a82`  
		Last Modified: Fri, 08 Dec 2023 20:53:31 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:5b65b8ce25fc15545c8781a1bcddf3627f74c954d542d268f5825bb1fdb50c9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:6a11de1e6d641c6980a331b6113ea0e7fe26ced6ab5049c48fc221962022d4ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.4 MB (577431560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3038e167dd77f2564f4515388e55220052b3c3875a140fd0e780ffe0b8fa395`
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
# Fri, 08 Dec 2023 20:43:39 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:43:39 GMT
ARG ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
# Fri, 08 Dec 2023 20:45:02 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:45:05 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:45:06 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:45:06 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:45:06 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:45:06 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:45:06 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:45:07 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:45:07 GMT
USER odoo
# Fri, 08 Dec 2023 20:45:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:45:07 GMT
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
	-	`sha256:37f707bd79248dc4a0068dc8035be8b6fc33fe9d6bb2efea334ef73bcbc52da2`  
		Last Modified: Fri, 08 Dec 2023 20:48:15 GMT  
		Size: 323.3 MB (323315394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01bd0cda71d6674543ca736b840c622eabe42317757297a6ba306a95fdbb64e`  
		Last Modified: Fri, 08 Dec 2023 20:47:38 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884c169ca1b0a859b2e4a99db995cc296efb4589566d410802915fa9126ae27c`  
		Last Modified: Fri, 08 Dec 2023 20:47:38 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12135faee5518f22f029b4949eeaa6f3b31d0c4c4206ec07f48196bc9dc9bf3`  
		Last Modified: Fri, 08 Dec 2023 20:47:38 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a7a6aedbeab994a61db496169c616d97593c0624114550c0be7ae8118c1686`  
		Last Modified: Fri, 08 Dec 2023 20:47:38 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16.0` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:a8f53468664cd1f8c249a638e4afa6d44c072861ea65f9865aeb911a8c359771
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.0 MB (573029481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:633d876138dfea48b2e4bc427ae378ae82b69c8aa6809be60094d9d6e78e8ea6`
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
# Fri, 08 Dec 2023 19:59:18 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 19:59:18 GMT
ARG ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
# Fri, 08 Dec 2023 20:00:31 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:00:38 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:00:38 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:00:39 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:00:39 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:00:39 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:00:39 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:00:39 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:00:39 GMT
USER odoo
# Fri, 08 Dec 2023 20:00:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:00:39 GMT
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
	-	`sha256:dca6c9a31e3038c6c59c584514d3543a5ed04d65585417fad7bd1a08779fa67f`  
		Last Modified: Fri, 08 Dec 2023 20:02:21 GMT  
		Size: 323.0 MB (322960299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339dd557785899b6ce705230df2b02bbe26c15935e86053d6f2939fcfee59d90`  
		Last Modified: Fri, 08 Dec 2023 20:01:52 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcae721c673b10423a864878a5efcc2b65e3405e07d4c76dd34348a4bf805c0a`  
		Last Modified: Fri, 08 Dec 2023 20:01:52 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ac15a8b5ddfe6eb46a71b3f7f59c5ef91d296d27f24ff38f7b859442b192e5`  
		Last Modified: Fri, 08 Dec 2023 20:01:52 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad95cab6488c0bde41a53c09c33e0e8163c540a7d13e04f3b25273fc71872490`  
		Last Modified: Fri, 08 Dec 2023 20:01:52 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16.0` - linux; ppc64le

```console
$ docker pull odoo@sha256:53ba84b6c68d61769a86cc877df73145163fe9d6aa544460d8e18b2df8bd51e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.0 MB (591985599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6224fc3ec9d500aab0c050c4998ca6d820606369c51bf6b7c67436431a240663`
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
# Fri, 08 Dec 2023 20:49:07 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:49:08 GMT
ARG ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
# Fri, 08 Dec 2023 20:51:44 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:52:04 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:52:05 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:52:06 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=468d34eb1d78003d832515f7f2bbc0cc90ab1cc0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:52:07 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:52:08 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:52:08 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:52:09 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:52:11 GMT
USER odoo
# Fri, 08 Dec 2023 20:52:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:52:12 GMT
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
	-	`sha256:03322b58d7809de36be6d5fc87a142b6bf429d189b18e279da2525c0d44d46f1`  
		Last Modified: Fri, 08 Dec 2023 20:54:15 GMT  
		Size: 324.8 MB (324756073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e64f4d117675449eb0708db0fed39c6b83e6d0566349226dda5b307f1e5ed6`  
		Last Modified: Fri, 08 Dec 2023 20:53:31 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea8c3c55f7bae2089152930ca7e33cdbc5e3adeffd3613ed40bf636cb8a8a51`  
		Last Modified: Fri, 08 Dec 2023 20:53:31 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85bec24deab524fc3cf80b50304550adc3352f1ad26a227a3d32bfdc484c17b`  
		Last Modified: Fri, 08 Dec 2023 20:53:31 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd8a8d0a7ba36a73fdba14e2e3946c56ffcd8a7b94d2289f0e8cd6f226c2a82`  
		Last Modified: Fri, 08 Dec 2023 20:53:31 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:17`

```console
$ docker pull odoo@sha256:041b8daf52d73d9047675e1add4a30002ef3d177ef2681a01a5f0d3bbfaa3dd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:17` - linux; amd64

```console
$ docker pull odoo@sha256:5514feddd1d5ad6ae56b9faa3ef3f6de961eaa37ffdc621eb80ab8cdc99242df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.5 MB (593460850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e86c119132ecb0dacd90d42961c948b7bb14535f3faa45a7206595d1c4f80dd`
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
# Fri, 08 Dec 2023 20:41:30 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:41:30 GMT
ARG ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
# Fri, 08 Dec 2023 20:43:30 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:43:33 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:43:33 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:43:33 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:43:33 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:43:33 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:43:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:43:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:43:34 GMT
USER odoo
# Fri, 08 Dec 2023 20:43:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:43:34 GMT
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
	-	`sha256:2bbcc6e3b1f75c140161a4edef6d9b934855ead4326a22c01019680543f9554a`  
		Last Modified: Fri, 08 Dec 2023 20:47:27 GMT  
		Size: 326.3 MB (326294645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79902a1deaa9580ed1355c6990bbc5fbb5a3c6810cd99c61fc7ec168580aac13`  
		Last Modified: Fri, 08 Dec 2023 20:46:49 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1386e163e7318c10e1339bddb2f2e92896a045defc494cc4d23600e5247941b`  
		Last Modified: Fri, 08 Dec 2023 20:46:50 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b03d25acc9c10362cd06dbc6eea20fe2495d3a0b9fb1a0b57dafec0fb41793`  
		Last Modified: Fri, 08 Dec 2023 20:46:49 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5615e00e4902fd07c77284f34220c3c15eb26bc7cf259e8af42111d1aaf3ea3`  
		Last Modified: Fri, 08 Dec 2023 20:46:49 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:9c7e9fdb15ab0037c886505db0118ab7d08bb21b16d81e7d3c5e70b50c371f6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.4 MB (588406780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d84651aaaa6020e29b8c8118ee6af5f20b340172c546510e770d46771eb272c2`
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
# Fri, 08 Dec 2023 19:56:55 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 19:56:55 GMT
ARG ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
# Fri, 08 Dec 2023 19:59:08 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 19:59:15 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 19:59:15 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 19:59:15 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 19:59:15 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 19:59:15 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 19:59:16 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 19:59:16 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 19:59:16 GMT
USER odoo
# Fri, 08 Dec 2023 19:59:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 19:59:16 GMT
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
	-	`sha256:103d4b1aabad0bc38d42fcf94bd4a2972bb665d0103933d13ec5194d3351cdb8`  
		Last Modified: Fri, 08 Dec 2023 20:01:41 GMT  
		Size: 325.9 MB (325915185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b54be8f355648f9e799b7b1cca832d7d3e561a3c40cdab8c79eb66abf7a499`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51531d7f1ff1834ff7ffe2de8652d8e0c94d6624cd3080dfc420aa3b26bbf9bb`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1427aa84d3d480ff14462ba1b91108d72011ea1496dbc121ef55f0026550fe84`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065449cd7b89b82483c096451cf6c72014dd766ebecd2f7d6047550013815dc4`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17` - linux; ppc64le

```console
$ docker pull odoo@sha256:34d4788a572746c166a2511c93611eb9ca4355a182c7b02107d7fc710824fb0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.3 MB (610267697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47dc6937c7a5e3d2052e80abe540a958550b925841e4bf25c2f5b9065cb05248`
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
# Fri, 08 Dec 2023 20:44:42 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:44:42 GMT
ARG ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
# Fri, 08 Dec 2023 20:48:16 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:48:43 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:48:45 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:48:47 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:48:48 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:48:50 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:48:50 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:48:50 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:48:51 GMT
USER odoo
# Fri, 08 Dec 2023 20:48:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:48:52 GMT
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
	-	`sha256:a15c2c9f48c075e16a306f91ba68152fdc181c4f3bcf774afb952dd0c648427a`  
		Last Modified: Fri, 08 Dec 2023 20:53:18 GMT  
		Size: 328.0 MB (328043109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac6b3e0703a262943477a46543df1e33965b5c0030fed43ea968004e6e40da0`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbe8aa57614423ecbdfea0227699c3642aa7bbfec76b5f6d96a5692997c12cc`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608b9cf636a57805303237a069b3c28602d5e86b8ade56cc020bc8403a987715`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707cde99fec645879fc4c91cacdfa4d4032260bc7cdf694e0156554c56294d6`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:17.0`

```console
$ docker pull odoo@sha256:041b8daf52d73d9047675e1add4a30002ef3d177ef2681a01a5f0d3bbfaa3dd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:17.0` - linux; amd64

```console
$ docker pull odoo@sha256:5514feddd1d5ad6ae56b9faa3ef3f6de961eaa37ffdc621eb80ab8cdc99242df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.5 MB (593460850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e86c119132ecb0dacd90d42961c948b7bb14535f3faa45a7206595d1c4f80dd`
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
# Fri, 08 Dec 2023 20:41:30 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:41:30 GMT
ARG ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
# Fri, 08 Dec 2023 20:43:30 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:43:33 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:43:33 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:43:33 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:43:33 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:43:33 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:43:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:43:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:43:34 GMT
USER odoo
# Fri, 08 Dec 2023 20:43:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:43:34 GMT
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
	-	`sha256:2bbcc6e3b1f75c140161a4edef6d9b934855ead4326a22c01019680543f9554a`  
		Last Modified: Fri, 08 Dec 2023 20:47:27 GMT  
		Size: 326.3 MB (326294645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79902a1deaa9580ed1355c6990bbc5fbb5a3c6810cd99c61fc7ec168580aac13`  
		Last Modified: Fri, 08 Dec 2023 20:46:49 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1386e163e7318c10e1339bddb2f2e92896a045defc494cc4d23600e5247941b`  
		Last Modified: Fri, 08 Dec 2023 20:46:50 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b03d25acc9c10362cd06dbc6eea20fe2495d3a0b9fb1a0b57dafec0fb41793`  
		Last Modified: Fri, 08 Dec 2023 20:46:49 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5615e00e4902fd07c77284f34220c3c15eb26bc7cf259e8af42111d1aaf3ea3`  
		Last Modified: Fri, 08 Dec 2023 20:46:49 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17.0` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:9c7e9fdb15ab0037c886505db0118ab7d08bb21b16d81e7d3c5e70b50c371f6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.4 MB (588406780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d84651aaaa6020e29b8c8118ee6af5f20b340172c546510e770d46771eb272c2`
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
# Fri, 08 Dec 2023 19:56:55 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 19:56:55 GMT
ARG ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
# Fri, 08 Dec 2023 19:59:08 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 19:59:15 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 19:59:15 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 19:59:15 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 19:59:15 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 19:59:15 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 19:59:16 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 19:59:16 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 19:59:16 GMT
USER odoo
# Fri, 08 Dec 2023 19:59:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 19:59:16 GMT
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
	-	`sha256:103d4b1aabad0bc38d42fcf94bd4a2972bb665d0103933d13ec5194d3351cdb8`  
		Last Modified: Fri, 08 Dec 2023 20:01:41 GMT  
		Size: 325.9 MB (325915185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b54be8f355648f9e799b7b1cca832d7d3e561a3c40cdab8c79eb66abf7a499`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51531d7f1ff1834ff7ffe2de8652d8e0c94d6624cd3080dfc420aa3b26bbf9bb`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1427aa84d3d480ff14462ba1b91108d72011ea1496dbc121ef55f0026550fe84`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065449cd7b89b82483c096451cf6c72014dd766ebecd2f7d6047550013815dc4`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:17.0` - linux; ppc64le

```console
$ docker pull odoo@sha256:34d4788a572746c166a2511c93611eb9ca4355a182c7b02107d7fc710824fb0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.3 MB (610267697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47dc6937c7a5e3d2052e80abe540a958550b925841e4bf25c2f5b9065cb05248`
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
# Fri, 08 Dec 2023 20:44:42 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:44:42 GMT
ARG ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
# Fri, 08 Dec 2023 20:48:16 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:48:43 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:48:45 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:48:47 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:48:48 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:48:50 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:48:50 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:48:50 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:48:51 GMT
USER odoo
# Fri, 08 Dec 2023 20:48:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:48:52 GMT
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
	-	`sha256:a15c2c9f48c075e16a306f91ba68152fdc181c4f3bcf774afb952dd0c648427a`  
		Last Modified: Fri, 08 Dec 2023 20:53:18 GMT  
		Size: 328.0 MB (328043109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac6b3e0703a262943477a46543df1e33965b5c0030fed43ea968004e6e40da0`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbe8aa57614423ecbdfea0227699c3642aa7bbfec76b5f6d96a5692997c12cc`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608b9cf636a57805303237a069b3c28602d5e86b8ade56cc020bc8403a987715`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707cde99fec645879fc4c91cacdfa4d4032260bc7cdf694e0156554c56294d6`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:041b8daf52d73d9047675e1add4a30002ef3d177ef2681a01a5f0d3bbfaa3dd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:5514feddd1d5ad6ae56b9faa3ef3f6de961eaa37ffdc621eb80ab8cdc99242df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.5 MB (593460850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e86c119132ecb0dacd90d42961c948b7bb14535f3faa45a7206595d1c4f80dd`
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
# Fri, 08 Dec 2023 20:41:30 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:41:30 GMT
ARG ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
# Fri, 08 Dec 2023 20:43:30 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:43:33 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:43:33 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:43:33 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:43:33 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:43:33 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:43:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:43:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:43:34 GMT
USER odoo
# Fri, 08 Dec 2023 20:43:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:43:34 GMT
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
	-	`sha256:2bbcc6e3b1f75c140161a4edef6d9b934855ead4326a22c01019680543f9554a`  
		Last Modified: Fri, 08 Dec 2023 20:47:27 GMT  
		Size: 326.3 MB (326294645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79902a1deaa9580ed1355c6990bbc5fbb5a3c6810cd99c61fc7ec168580aac13`  
		Last Modified: Fri, 08 Dec 2023 20:46:49 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1386e163e7318c10e1339bddb2f2e92896a045defc494cc4d23600e5247941b`  
		Last Modified: Fri, 08 Dec 2023 20:46:50 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b03d25acc9c10362cd06dbc6eea20fe2495d3a0b9fb1a0b57dafec0fb41793`  
		Last Modified: Fri, 08 Dec 2023 20:46:49 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5615e00e4902fd07c77284f34220c3c15eb26bc7cf259e8af42111d1aaf3ea3`  
		Last Modified: Fri, 08 Dec 2023 20:46:49 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:latest` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:9c7e9fdb15ab0037c886505db0118ab7d08bb21b16d81e7d3c5e70b50c371f6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.4 MB (588406780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d84651aaaa6020e29b8c8118ee6af5f20b340172c546510e770d46771eb272c2`
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
# Fri, 08 Dec 2023 19:56:55 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 19:56:55 GMT
ARG ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
# Fri, 08 Dec 2023 19:59:08 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 19:59:15 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 19:59:15 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 19:59:15 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 19:59:15 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 19:59:15 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 19:59:16 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 19:59:16 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 19:59:16 GMT
USER odoo
# Fri, 08 Dec 2023 19:59:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 19:59:16 GMT
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
	-	`sha256:103d4b1aabad0bc38d42fcf94bd4a2972bb665d0103933d13ec5194d3351cdb8`  
		Last Modified: Fri, 08 Dec 2023 20:01:41 GMT  
		Size: 325.9 MB (325915185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b54be8f355648f9e799b7b1cca832d7d3e561a3c40cdab8c79eb66abf7a499`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51531d7f1ff1834ff7ffe2de8652d8e0c94d6624cd3080dfc420aa3b26bbf9bb`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1427aa84d3d480ff14462ba1b91108d72011ea1496dbc121ef55f0026550fe84`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065449cd7b89b82483c096451cf6c72014dd766ebecd2f7d6047550013815dc4`  
		Last Modified: Fri, 08 Dec 2023 20:01:02 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:latest` - linux; ppc64le

```console
$ docker pull odoo@sha256:34d4788a572746c166a2511c93611eb9ca4355a182c7b02107d7fc710824fb0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.3 MB (610267697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47dc6937c7a5e3d2052e80abe540a958550b925841e4bf25c2f5b9065cb05248`
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
# Fri, 08 Dec 2023 20:44:42 GMT
ARG ODOO_RELEASE=20231208
# Fri, 08 Dec 2023 20:44:42 GMT
ARG ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
# Fri, 08 Dec 2023 20:48:16 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Dec 2023 20:48:43 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Dec 2023 20:48:45 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Dec 2023 20:48:47 GMT
# ARGS: ODOO_RELEASE=20231208 ODOO_SHA=22fee8e6b6f6e61236198eca5b01e2ebd223844d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Dec 2023 20:48:48 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Dec 2023 20:48:50 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Dec 2023 20:48:50 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Dec 2023 20:48:50 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Dec 2023 20:48:51 GMT
USER odoo
# Fri, 08 Dec 2023 20:48:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Dec 2023 20:48:52 GMT
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
	-	`sha256:a15c2c9f48c075e16a306f91ba68152fdc181c4f3bcf774afb952dd0c648427a`  
		Last Modified: Fri, 08 Dec 2023 20:53:18 GMT  
		Size: 328.0 MB (328043109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac6b3e0703a262943477a46543df1e33965b5c0030fed43ea968004e6e40da0`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbe8aa57614423ecbdfea0227699c3642aa7bbfec76b5f6d96a5692997c12cc`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608b9cf636a57805303237a069b3c28602d5e86b8ade56cc020bc8403a987715`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f707cde99fec645879fc4c91cacdfa4d4032260bc7cdf694e0156554c56294d6`  
		Last Modified: Fri, 08 Dec 2023 20:52:23 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
