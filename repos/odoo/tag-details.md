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
$ docker pull odoo@sha256:5169ddb3b87cff30cea27dcfce9139314e5dea70b10e42a827f01762cf70f93b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:0792706f71355f041895197ad3e776f577277fd22cab6d9a7a0a893dc29891e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.1 MB (563140418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3cc4b62b25aa258edddec3f2b0b0b41390fd2969197c1c593a125b158c69274`
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
# Fri, 15 Dec 2023 19:35:31 GMT
ARG ODOO_RELEASE=20231215
# Fri, 15 Dec 2023 19:35:31 GMT
ARG ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
# Fri, 15 Dec 2023 19:36:44 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 15 Dec 2023 19:36:48 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 15 Dec 2023 19:36:48 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 15 Dec 2023 19:36:49 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 15 Dec 2023 19:36:49 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 15 Dec 2023 19:36:49 GMT
EXPOSE 8069 8071 8072
# Fri, 15 Dec 2023 19:36:49 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 15 Dec 2023 19:36:49 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 15 Dec 2023 19:36:49 GMT
USER odoo
# Fri, 15 Dec 2023 19:36:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Dec 2023 19:36:49 GMT
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
	-	`sha256:57a703f8024a34101b938db0db0397334678a236e07d2b635317620908c8bd96`  
		Last Modified: Fri, 15 Dec 2023 19:39:06 GMT  
		Size: 308.3 MB (308337482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65c6f6abb15c03b11c8be9678aade4b60d0af5b53778677ec55b2e413585f64`  
		Last Modified: Fri, 15 Dec 2023 19:38:34 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2de21c2b8bf0ce9eae2b74c0a5f67eca804f566b19510bc13baa5022e12eb8`  
		Last Modified: Fri, 15 Dec 2023 19:38:34 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60711fb41440263b3116fec430aac986831a53ae08d11ff0b73855836bc95322`  
		Last Modified: Fri, 15 Dec 2023 19:38:34 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e8b2a923d1a58472bcf2e33df0220f13354d4a0dd3863f0254a8dcf9f63b73`  
		Last Modified: Fri, 15 Dec 2023 19:38:34 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:5169ddb3b87cff30cea27dcfce9139314e5dea70b10e42a827f01762cf70f93b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:0792706f71355f041895197ad3e776f577277fd22cab6d9a7a0a893dc29891e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.1 MB (563140418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3cc4b62b25aa258edddec3f2b0b0b41390fd2969197c1c593a125b158c69274`
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
# Fri, 15 Dec 2023 19:35:31 GMT
ARG ODOO_RELEASE=20231215
# Fri, 15 Dec 2023 19:35:31 GMT
ARG ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
# Fri, 15 Dec 2023 19:36:44 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 15 Dec 2023 19:36:48 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 15 Dec 2023 19:36:48 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 15 Dec 2023 19:36:49 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=a67e5a8be2d8b5c2da4f95614782ab4bcc0a17ec
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 15 Dec 2023 19:36:49 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 15 Dec 2023 19:36:49 GMT
EXPOSE 8069 8071 8072
# Fri, 15 Dec 2023 19:36:49 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 15 Dec 2023 19:36:49 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 15 Dec 2023 19:36:49 GMT
USER odoo
# Fri, 15 Dec 2023 19:36:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Dec 2023 19:36:49 GMT
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
	-	`sha256:57a703f8024a34101b938db0db0397334678a236e07d2b635317620908c8bd96`  
		Last Modified: Fri, 15 Dec 2023 19:39:06 GMT  
		Size: 308.3 MB (308337482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65c6f6abb15c03b11c8be9678aade4b60d0af5b53778677ec55b2e413585f64`  
		Last Modified: Fri, 15 Dec 2023 19:38:34 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2de21c2b8bf0ce9eae2b74c0a5f67eca804f566b19510bc13baa5022e12eb8`  
		Last Modified: Fri, 15 Dec 2023 19:38:34 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60711fb41440263b3116fec430aac986831a53ae08d11ff0b73855836bc95322`  
		Last Modified: Fri, 15 Dec 2023 19:38:34 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e8b2a923d1a58472bcf2e33df0220f13354d4a0dd3863f0254a8dcf9f63b73`  
		Last Modified: Fri, 15 Dec 2023 19:38:34 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:690557599fe82f5ee4496734dc8e3b84d443590bb80941cb3ccacf4e12504301
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:19e2d2ddabe02e6fffbdee3f9d6734920dfbac7d0df0cc84626d8835ea0491c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.5 MB (577503235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a5c0d3c8248b836829417063e3f497d9460d0170adfc27cecb924916de2baa6`
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
# Fri, 15 Dec 2023 19:33:52 GMT
ARG ODOO_RELEASE=20231215
# Fri, 15 Dec 2023 19:33:52 GMT
ARG ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
# Fri, 15 Dec 2023 19:35:13 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 15 Dec 2023 19:35:18 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 15 Dec 2023 19:35:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 15 Dec 2023 19:35:18 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 15 Dec 2023 19:35:18 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 15 Dec 2023 19:35:18 GMT
EXPOSE 8069 8071 8072
# Fri, 15 Dec 2023 19:35:18 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 15 Dec 2023 19:35:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 15 Dec 2023 19:35:19 GMT
USER odoo
# Fri, 15 Dec 2023 19:35:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Dec 2023 19:35:19 GMT
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
	-	`sha256:b398bea99bf8c83e634e8bddda6cfb44052f45cc0e905cb2ac39a51a3856796a`  
		Last Modified: Fri, 15 Dec 2023 19:38:25 GMT  
		Size: 323.4 MB (323387080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5647b0142c1e2b87c441cdfb34fb7b3d1217ab7451ed89edb44b73178014ab`  
		Last Modified: Fri, 15 Dec 2023 19:37:49 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bd58eb2637e9b0c6d6a7584a9ffebd9f9962917ff504e9a22a52f6e697350b`  
		Last Modified: Fri, 15 Dec 2023 19:37:49 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74e139ddb09b7f4d74053600ceec1c3a75d4f8cf88234e5a6e856c79d90f803`  
		Last Modified: Fri, 15 Dec 2023 19:37:49 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd02a8fa4086aabd9fc6d3b2ad9f6e0faa4d76bbb63c97876c547a07f9a75b1`  
		Last Modified: Fri, 15 Dec 2023 19:37:49 GMT  
		Size: 584.0 B  
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
$ docker pull odoo@sha256:690557599fe82f5ee4496734dc8e3b84d443590bb80941cb3ccacf4e12504301
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:19e2d2ddabe02e6fffbdee3f9d6734920dfbac7d0df0cc84626d8835ea0491c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.5 MB (577503235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a5c0d3c8248b836829417063e3f497d9460d0170adfc27cecb924916de2baa6`
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
# Fri, 15 Dec 2023 19:33:52 GMT
ARG ODOO_RELEASE=20231215
# Fri, 15 Dec 2023 19:33:52 GMT
ARG ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
# Fri, 15 Dec 2023 19:35:13 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 15 Dec 2023 19:35:18 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 15 Dec 2023 19:35:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 15 Dec 2023 19:35:18 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=dd439ff587a574a886855a9901d83d312214cdaf
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 15 Dec 2023 19:35:18 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 15 Dec 2023 19:35:18 GMT
EXPOSE 8069 8071 8072
# Fri, 15 Dec 2023 19:35:18 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 15 Dec 2023 19:35:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 15 Dec 2023 19:35:19 GMT
USER odoo
# Fri, 15 Dec 2023 19:35:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Dec 2023 19:35:19 GMT
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
	-	`sha256:b398bea99bf8c83e634e8bddda6cfb44052f45cc0e905cb2ac39a51a3856796a`  
		Last Modified: Fri, 15 Dec 2023 19:38:25 GMT  
		Size: 323.4 MB (323387080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5647b0142c1e2b87c441cdfb34fb7b3d1217ab7451ed89edb44b73178014ab`  
		Last Modified: Fri, 15 Dec 2023 19:37:49 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bd58eb2637e9b0c6d6a7584a9ffebd9f9962917ff504e9a22a52f6e697350b`  
		Last Modified: Fri, 15 Dec 2023 19:37:49 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74e139ddb09b7f4d74053600ceec1c3a75d4f8cf88234e5a6e856c79d90f803`  
		Last Modified: Fri, 15 Dec 2023 19:37:49 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd02a8fa4086aabd9fc6d3b2ad9f6e0faa4d76bbb63c97876c547a07f9a75b1`  
		Last Modified: Fri, 15 Dec 2023 19:37:49 GMT  
		Size: 584.0 B  
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
$ docker pull odoo@sha256:30daa984ae6d3cd2814532dd528ab84f39f08b5799a02386ce6d808a51619ac1
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
$ docker pull odoo@sha256:8f93498227ce95872600f724a2a29041511bc4a7332b540b73fa6e9afc709520
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.6 MB (610577108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3489e88b86852152fb33de09b5ca08880c041bb25a9354fad5a062dd4766ea`
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
# Fri, 15 Dec 2023 19:34:38 GMT
ARG ODOO_RELEASE=20231215
# Fri, 15 Dec 2023 19:34:38 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Fri, 15 Dec 2023 19:38:17 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 15 Dec 2023 19:38:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 15 Dec 2023 19:38:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 15 Dec 2023 19:38:31 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 15 Dec 2023 19:38:31 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 15 Dec 2023 19:38:32 GMT
EXPOSE 8069 8071 8072
# Fri, 15 Dec 2023 19:38:33 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 15 Dec 2023 19:38:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 15 Dec 2023 19:38:35 GMT
USER odoo
# Fri, 15 Dec 2023 19:38:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Dec 2023 19:38:36 GMT
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
	-	`sha256:df0a7bc3530ba030477d500024a24c2f552d3a077012d7ae4f8f65e8d3010bbf`  
		Last Modified: Fri, 15 Dec 2023 19:42:37 GMT  
		Size: 328.4 MB (328352525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09520552b4a4cfff2e2a5bf2e4d3d701ae6dfab035c358bbd16d604644a8df`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1a2e3d1ad0eb5ed45ef535d08041edb754624bbc8ffbd630110a199b563dcc`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f19db4d5add10d1510fd0c4a26e7497ad4288cf5daf9a6abd5b3b666daff48`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61992da5ba5f9038e35d9be6159557f05856f8c55765ae7cedcee3962afbdcae`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:17.0`

```console
$ docker pull odoo@sha256:30daa984ae6d3cd2814532dd528ab84f39f08b5799a02386ce6d808a51619ac1
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
$ docker pull odoo@sha256:8f93498227ce95872600f724a2a29041511bc4a7332b540b73fa6e9afc709520
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.6 MB (610577108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3489e88b86852152fb33de09b5ca08880c041bb25a9354fad5a062dd4766ea`
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
# Fri, 15 Dec 2023 19:34:38 GMT
ARG ODOO_RELEASE=20231215
# Fri, 15 Dec 2023 19:34:38 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Fri, 15 Dec 2023 19:38:17 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 15 Dec 2023 19:38:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 15 Dec 2023 19:38:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 15 Dec 2023 19:38:31 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 15 Dec 2023 19:38:31 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 15 Dec 2023 19:38:32 GMT
EXPOSE 8069 8071 8072
# Fri, 15 Dec 2023 19:38:33 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 15 Dec 2023 19:38:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 15 Dec 2023 19:38:35 GMT
USER odoo
# Fri, 15 Dec 2023 19:38:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Dec 2023 19:38:36 GMT
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
	-	`sha256:df0a7bc3530ba030477d500024a24c2f552d3a077012d7ae4f8f65e8d3010bbf`  
		Last Modified: Fri, 15 Dec 2023 19:42:37 GMT  
		Size: 328.4 MB (328352525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09520552b4a4cfff2e2a5bf2e4d3d701ae6dfab035c358bbd16d604644a8df`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1a2e3d1ad0eb5ed45ef535d08041edb754624bbc8ffbd630110a199b563dcc`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f19db4d5add10d1510fd0c4a26e7497ad4288cf5daf9a6abd5b3b666daff48`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61992da5ba5f9038e35d9be6159557f05856f8c55765ae7cedcee3962afbdcae`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:30daa984ae6d3cd2814532dd528ab84f39f08b5799a02386ce6d808a51619ac1
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
$ docker pull odoo@sha256:8f93498227ce95872600f724a2a29041511bc4a7332b540b73fa6e9afc709520
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.6 MB (610577108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3489e88b86852152fb33de09b5ca08880c041bb25a9354fad5a062dd4766ea`
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
# Fri, 15 Dec 2023 19:34:38 GMT
ARG ODOO_RELEASE=20231215
# Fri, 15 Dec 2023 19:34:38 GMT
ARG ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
# Fri, 15 Dec 2023 19:38:17 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 15 Dec 2023 19:38:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 15 Dec 2023 19:38:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 15 Dec 2023 19:38:31 GMT
# ARGS: ODOO_RELEASE=20231215 ODOO_SHA=e5073e19f71cbf056e2e647aa667d95b6f903901
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 15 Dec 2023 19:38:31 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 15 Dec 2023 19:38:32 GMT
EXPOSE 8069 8071 8072
# Fri, 15 Dec 2023 19:38:33 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 15 Dec 2023 19:38:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 15 Dec 2023 19:38:35 GMT
USER odoo
# Fri, 15 Dec 2023 19:38:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 Dec 2023 19:38:36 GMT
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
	-	`sha256:df0a7bc3530ba030477d500024a24c2f552d3a077012d7ae4f8f65e8d3010bbf`  
		Last Modified: Fri, 15 Dec 2023 19:42:37 GMT  
		Size: 328.4 MB (328352525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09520552b4a4cfff2e2a5bf2e4d3d701ae6dfab035c358bbd16d604644a8df`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1a2e3d1ad0eb5ed45ef535d08041edb754624bbc8ffbd630110a199b563dcc`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f19db4d5add10d1510fd0c4a26e7497ad4288cf5daf9a6abd5b3b666daff48`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61992da5ba5f9038e35d9be6159557f05856f8c55765ae7cedcee3962afbdcae`  
		Last Modified: Fri, 15 Dec 2023 19:41:49 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
