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
$ docker pull odoo@sha256:81ad982f21bd20c976649434f52957fad12141d5a48a31462f0c1c53103e2b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:e02442316bc5eee7a90a3e9e6db9323347df52dac2da17ef4cdb3d9f1c456957
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.5 MB (528495215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84e2b8353114b284c7dcbce9b198f7e56f57e4f137d49a3daeb3c5d80a7958e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 08:57:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 28 Sep 2021 08:57:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 28 Sep 2021 08:57:31 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:02:35 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 28 Sep 2021 09:02:51 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:02:55 GMT
RUN npm install -g rtlcss
# Tue, 28 Sep 2021 09:02:55 GMT
ENV ODOO_VERSION=13.0
# Fri, 08 Oct 2021 17:24:53 GMT
ARG ODOO_RELEASE=20211007
# Fri, 08 Oct 2021 17:24:53 GMT
ARG ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
# Fri, 08 Oct 2021 17:26:06 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Oct 2021 17:26:10 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Oct 2021 17:26:10 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Oct 2021 17:26:11 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Oct 2021 17:26:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Oct 2021 17:26:11 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Oct 2021 17:26:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Oct 2021 17:26:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Oct 2021 17:26:12 GMT
USER odoo
# Fri, 08 Oct 2021 17:26:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Oct 2021 17:26:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c839a5f094fb26110db82ce8478b2716b5ae4a3b1f4787dcf4e42a3ee806fa7`  
		Last Modified: Tue, 28 Sep 2021 09:11:24 GMT  
		Size: 207.1 MB (207131178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9702631183b797e14e02f699e03b5970d762468d09fdf90f68293fa1d190b699`  
		Last Modified: Tue, 28 Sep 2021 09:10:56 GMT  
		Size: 2.3 MB (2347886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d624dc0f4f384ddbee9fa140b492064255415e389bc2188ab634fc3f01234b`  
		Last Modified: Tue, 28 Sep 2021 09:10:56 GMT  
		Size: 882.8 KB (882781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a3254f06b97676cd75010e4691afbba3429b928c5fc6c40d5f13bd7705a490`  
		Last Modified: Fri, 08 Oct 2021 17:28:30 GMT  
		Size: 291.0 MB (290984916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c703fe05fb3af50c202f274506e5bcf43c92a27f8d811b76a8b422abbd56d10`  
		Last Modified: Fri, 08 Oct 2021 17:28:00 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2025f5c509d36a39f86dbc78959adbc019ff869b022c1c1344ca97dfc5c8fbbb`  
		Last Modified: Fri, 08 Oct 2021 17:28:00 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b115fe2722202fbb96328858cf027f4cf9e2eaa5b226fff4af858913fb8b45`  
		Last Modified: Fri, 08 Oct 2021 17:28:00 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b5b361e6885a46a672aca407399671dd720032cc6f50d827608b1cbcb59fc`  
		Last Modified: Fri, 08 Oct 2021 17:28:00 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:81ad982f21bd20c976649434f52957fad12141d5a48a31462f0c1c53103e2b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:e02442316bc5eee7a90a3e9e6db9323347df52dac2da17ef4cdb3d9f1c456957
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.5 MB (528495215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84e2b8353114b284c7dcbce9b198f7e56f57e4f137d49a3daeb3c5d80a7958e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 08:57:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 28 Sep 2021 08:57:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 28 Sep 2021 08:57:31 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:02:35 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 28 Sep 2021 09:02:51 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:02:55 GMT
RUN npm install -g rtlcss
# Tue, 28 Sep 2021 09:02:55 GMT
ENV ODOO_VERSION=13.0
# Fri, 08 Oct 2021 17:24:53 GMT
ARG ODOO_RELEASE=20211007
# Fri, 08 Oct 2021 17:24:53 GMT
ARG ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
# Fri, 08 Oct 2021 17:26:06 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Oct 2021 17:26:10 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Oct 2021 17:26:10 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Oct 2021 17:26:11 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Oct 2021 17:26:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Oct 2021 17:26:11 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Oct 2021 17:26:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Oct 2021 17:26:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Oct 2021 17:26:12 GMT
USER odoo
# Fri, 08 Oct 2021 17:26:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Oct 2021 17:26:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c839a5f094fb26110db82ce8478b2716b5ae4a3b1f4787dcf4e42a3ee806fa7`  
		Last Modified: Tue, 28 Sep 2021 09:11:24 GMT  
		Size: 207.1 MB (207131178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9702631183b797e14e02f699e03b5970d762468d09fdf90f68293fa1d190b699`  
		Last Modified: Tue, 28 Sep 2021 09:10:56 GMT  
		Size: 2.3 MB (2347886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d624dc0f4f384ddbee9fa140b492064255415e389bc2188ab634fc3f01234b`  
		Last Modified: Tue, 28 Sep 2021 09:10:56 GMT  
		Size: 882.8 KB (882781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a3254f06b97676cd75010e4691afbba3429b928c5fc6c40d5f13bd7705a490`  
		Last Modified: Fri, 08 Oct 2021 17:28:30 GMT  
		Size: 291.0 MB (290984916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c703fe05fb3af50c202f274506e5bcf43c92a27f8d811b76a8b422abbd56d10`  
		Last Modified: Fri, 08 Oct 2021 17:28:00 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2025f5c509d36a39f86dbc78959adbc019ff869b022c1c1344ca97dfc5c8fbbb`  
		Last Modified: Fri, 08 Oct 2021 17:28:00 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b115fe2722202fbb96328858cf027f4cf9e2eaa5b226fff4af858913fb8b45`  
		Last Modified: Fri, 08 Oct 2021 17:28:00 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59b5b361e6885a46a672aca407399671dd720032cc6f50d827608b1cbcb59fc`  
		Last Modified: Fri, 08 Oct 2021 17:28:00 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:8167b83f2fcd84f3c9d6bdd2977cb8e352d03088992f0fd54807525275625767
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:c61ec80cdd44a3b0c83b4b230cdca4712689214f6ea26193bade336f06c89bba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **517.1 MB (517071817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b3965392e02577895787ec8b31453a523a32706c99ebc1839cbd3e829df4d83`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 08:57:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 28 Sep 2021 08:57:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 28 Sep 2021 08:57:31 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 08:59:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 28 Sep 2021 08:59:19 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 08:59:24 GMT
RUN npm install -g rtlcss
# Tue, 28 Sep 2021 08:59:24 GMT
ENV ODOO_VERSION=14.0
# Fri, 08 Oct 2021 17:23:27 GMT
ARG ODOO_RELEASE=20211007
# Fri, 08 Oct 2021 17:23:27 GMT
ARG ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
# Fri, 08 Oct 2021 17:24:40 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Oct 2021 17:24:44 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Oct 2021 17:24:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Oct 2021 17:24:45 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Oct 2021 17:24:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Oct 2021 17:24:45 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Oct 2021 17:24:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Oct 2021 17:24:46 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Oct 2021 17:24:46 GMT
USER odoo
# Fri, 08 Oct 2021 17:24:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Oct 2021 17:24:46 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202cc4801528046f1295d1e9fde12d1ca51922bb3bbb78f28414392e496affb`  
		Last Modified: Tue, 28 Sep 2021 09:10:33 GMT  
		Size: 213.2 MB (213172416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f9940244ebdbb6e2808ac61f977f7a881c116cf6b1a5ff5400656affb2122`  
		Last Modified: Tue, 28 Sep 2021 09:10:05 GMT  
		Size: 2.4 MB (2350586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e07d3bb02ae4b65c91447226f5c9402577d6f42a0cc8060e112b073485266a8`  
		Last Modified: Tue, 28 Sep 2021 09:10:05 GMT  
		Size: 882.7 KB (882660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61588da669839de82364b78d7640e8409e08d9283eebd3b14f0211a039fbf59`  
		Last Modified: Fri, 08 Oct 2021 17:27:49 GMT  
		Size: 273.5 MB (273517694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadf30f554605f8e418afecb49c1a0d4b7bd1d2ee3df81fd20648ec4c8fce31b`  
		Last Modified: Fri, 08 Oct 2021 17:27:18 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05388e2cb2ca8c5ec37bac7ed1a440c32d1ce649f4e5c07cd35db626fc00e443`  
		Last Modified: Fri, 08 Oct 2021 17:27:19 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210eeccc32c79232ae7041b4db8682cacc0be1141ae3db45431e6e3d3699335e`  
		Last Modified: Fri, 08 Oct 2021 17:27:18 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65990f72334f23464fc03cebc37ecd237fa29c5e7aff276fa16e157e571ebdf9`  
		Last Modified: Fri, 08 Oct 2021 17:27:18 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:8167b83f2fcd84f3c9d6bdd2977cb8e352d03088992f0fd54807525275625767
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:c61ec80cdd44a3b0c83b4b230cdca4712689214f6ea26193bade336f06c89bba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **517.1 MB (517071817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b3965392e02577895787ec8b31453a523a32706c99ebc1839cbd3e829df4d83`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 08:57:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 28 Sep 2021 08:57:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 28 Sep 2021 08:57:31 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 08:59:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 28 Sep 2021 08:59:19 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 08:59:24 GMT
RUN npm install -g rtlcss
# Tue, 28 Sep 2021 08:59:24 GMT
ENV ODOO_VERSION=14.0
# Fri, 08 Oct 2021 17:23:27 GMT
ARG ODOO_RELEASE=20211007
# Fri, 08 Oct 2021 17:23:27 GMT
ARG ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
# Fri, 08 Oct 2021 17:24:40 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Oct 2021 17:24:44 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Oct 2021 17:24:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Oct 2021 17:24:45 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Oct 2021 17:24:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Oct 2021 17:24:45 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Oct 2021 17:24:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Oct 2021 17:24:46 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Oct 2021 17:24:46 GMT
USER odoo
# Fri, 08 Oct 2021 17:24:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Oct 2021 17:24:46 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202cc4801528046f1295d1e9fde12d1ca51922bb3bbb78f28414392e496affb`  
		Last Modified: Tue, 28 Sep 2021 09:10:33 GMT  
		Size: 213.2 MB (213172416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f9940244ebdbb6e2808ac61f977f7a881c116cf6b1a5ff5400656affb2122`  
		Last Modified: Tue, 28 Sep 2021 09:10:05 GMT  
		Size: 2.4 MB (2350586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e07d3bb02ae4b65c91447226f5c9402577d6f42a0cc8060e112b073485266a8`  
		Last Modified: Tue, 28 Sep 2021 09:10:05 GMT  
		Size: 882.7 KB (882660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61588da669839de82364b78d7640e8409e08d9283eebd3b14f0211a039fbf59`  
		Last Modified: Fri, 08 Oct 2021 17:27:49 GMT  
		Size: 273.5 MB (273517694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadf30f554605f8e418afecb49c1a0d4b7bd1d2ee3df81fd20648ec4c8fce31b`  
		Last Modified: Fri, 08 Oct 2021 17:27:18 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05388e2cb2ca8c5ec37bac7ed1a440c32d1ce649f4e5c07cd35db626fc00e443`  
		Last Modified: Fri, 08 Oct 2021 17:27:19 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210eeccc32c79232ae7041b4db8682cacc0be1141ae3db45431e6e3d3699335e`  
		Last Modified: Fri, 08 Oct 2021 17:27:18 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65990f72334f23464fc03cebc37ecd237fa29c5e7aff276fa16e157e571ebdf9`  
		Last Modified: Fri, 08 Oct 2021 17:27:18 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:31e6b45ce74bf5b90264ca63f7a4d72283ba64b86d930c1482490e38c4a1504d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:7e222384ad337934b7c86db7d7220ac1a44cb58c1ac8e5f012abb7cff5455bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539745637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ff6a85ce52eb4d58c33e35cc098b6962cbd03b8062e279eb0d3f10e2e19a032`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Fri, 08 Oct 2021 17:20:31 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 08 Oct 2021 17:20:31 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 08 Oct 2021 17:20:31 GMT
ENV LANG=C.UTF-8
# Fri, 08 Oct 2021 17:21:31 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         gsfonts         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-openssl         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 08 Oct 2021 17:21:48 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Oct 2021 17:21:51 GMT
RUN npm install -g rtlcss
# Fri, 08 Oct 2021 17:21:51 GMT
ENV ODOO_VERSION=15.0
# Fri, 08 Oct 2021 17:21:51 GMT
ARG ODOO_RELEASE=20211007
# Fri, 08 Oct 2021 17:21:51 GMT
ARG ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
# Fri, 08 Oct 2021 17:23:06 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Oct 2021 17:23:10 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Oct 2021 17:23:10 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Oct 2021 17:23:11 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Oct 2021 17:23:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Oct 2021 17:23:11 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Oct 2021 17:23:11 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Oct 2021 17:23:11 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Oct 2021 17:23:12 GMT
USER odoo
# Fri, 08 Oct 2021 17:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Oct 2021 17:23:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be52707944e2c459c0a114bfbec35c0aec482356baed8e15f747658fcdca6e6`  
		Last Modified: Fri, 08 Oct 2021 17:27:01 GMT  
		Size: 223.8 MB (223814497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c397d8744aa1d4eb6230a18250d33169abf2ae6ab30f09fa5f287c7950bd2`  
		Last Modified: Fri, 08 Oct 2021 17:26:34 GMT  
		Size: 2.5 MB (2506003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4435dbe6255c1f833427223a7e5f73ef0624514d7afece7954d674711d2193e7`  
		Last Modified: Fri, 08 Oct 2021 17:26:33 GMT  
		Size: 853.2 KB (853224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1db7ace550d5156b967f291a8e4c7e6ced71811122cf63105218f1fec0765c`  
		Last Modified: Fri, 08 Oct 2021 17:27:05 GMT  
		Size: 281.2 MB (281200538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fabbe06bcdde04e0b7ef2e9e1501599c3011214e12419e881aae211be58850c`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93d2bb6236506da7b29e172c991710872da38e9ab70ad4c3ff2132756456116`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3682eb88f77b41507ca9c8b7bc2958f0f07845f3b825be6ca9bd2217cb78ff`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90658b550a295730b105270faa8854a617aaa7d765cb3d9dfcec69d7e3c15e1`  
		Last Modified: Fri, 08 Oct 2021 17:26:30 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:31e6b45ce74bf5b90264ca63f7a4d72283ba64b86d930c1482490e38c4a1504d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:7e222384ad337934b7c86db7d7220ac1a44cb58c1ac8e5f012abb7cff5455bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539745637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ff6a85ce52eb4d58c33e35cc098b6962cbd03b8062e279eb0d3f10e2e19a032`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Fri, 08 Oct 2021 17:20:31 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 08 Oct 2021 17:20:31 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 08 Oct 2021 17:20:31 GMT
ENV LANG=C.UTF-8
# Fri, 08 Oct 2021 17:21:31 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         gsfonts         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-openssl         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 08 Oct 2021 17:21:48 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Oct 2021 17:21:51 GMT
RUN npm install -g rtlcss
# Fri, 08 Oct 2021 17:21:51 GMT
ENV ODOO_VERSION=15.0
# Fri, 08 Oct 2021 17:21:51 GMT
ARG ODOO_RELEASE=20211007
# Fri, 08 Oct 2021 17:21:51 GMT
ARG ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
# Fri, 08 Oct 2021 17:23:06 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Oct 2021 17:23:10 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Oct 2021 17:23:10 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Oct 2021 17:23:11 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Oct 2021 17:23:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Oct 2021 17:23:11 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Oct 2021 17:23:11 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Oct 2021 17:23:11 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Oct 2021 17:23:12 GMT
USER odoo
# Fri, 08 Oct 2021 17:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Oct 2021 17:23:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be52707944e2c459c0a114bfbec35c0aec482356baed8e15f747658fcdca6e6`  
		Last Modified: Fri, 08 Oct 2021 17:27:01 GMT  
		Size: 223.8 MB (223814497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c397d8744aa1d4eb6230a18250d33169abf2ae6ab30f09fa5f287c7950bd2`  
		Last Modified: Fri, 08 Oct 2021 17:26:34 GMT  
		Size: 2.5 MB (2506003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4435dbe6255c1f833427223a7e5f73ef0624514d7afece7954d674711d2193e7`  
		Last Modified: Fri, 08 Oct 2021 17:26:33 GMT  
		Size: 853.2 KB (853224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1db7ace550d5156b967f291a8e4c7e6ced71811122cf63105218f1fec0765c`  
		Last Modified: Fri, 08 Oct 2021 17:27:05 GMT  
		Size: 281.2 MB (281200538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fabbe06bcdde04e0b7ef2e9e1501599c3011214e12419e881aae211be58850c`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93d2bb6236506da7b29e172c991710872da38e9ab70ad4c3ff2132756456116`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3682eb88f77b41507ca9c8b7bc2958f0f07845f3b825be6ca9bd2217cb78ff`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90658b550a295730b105270faa8854a617aaa7d765cb3d9dfcec69d7e3c15e1`  
		Last Modified: Fri, 08 Oct 2021 17:26:30 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:31e6b45ce74bf5b90264ca63f7a4d72283ba64b86d930c1482490e38c4a1504d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:7e222384ad337934b7c86db7d7220ac1a44cb58c1ac8e5f012abb7cff5455bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539745637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ff6a85ce52eb4d58c33e35cc098b6962cbd03b8062e279eb0d3f10e2e19a032`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Fri, 08 Oct 2021 17:20:31 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 08 Oct 2021 17:20:31 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 08 Oct 2021 17:20:31 GMT
ENV LANG=C.UTF-8
# Fri, 08 Oct 2021 17:21:31 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         gsfonts         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-openssl         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 08 Oct 2021 17:21:48 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Oct 2021 17:21:51 GMT
RUN npm install -g rtlcss
# Fri, 08 Oct 2021 17:21:51 GMT
ENV ODOO_VERSION=15.0
# Fri, 08 Oct 2021 17:21:51 GMT
ARG ODOO_RELEASE=20211007
# Fri, 08 Oct 2021 17:21:51 GMT
ARG ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
# Fri, 08 Oct 2021 17:23:06 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Oct 2021 17:23:10 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Oct 2021 17:23:10 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Oct 2021 17:23:11 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Oct 2021 17:23:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Oct 2021 17:23:11 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Oct 2021 17:23:11 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Oct 2021 17:23:11 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Oct 2021 17:23:12 GMT
USER odoo
# Fri, 08 Oct 2021 17:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Oct 2021 17:23:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be52707944e2c459c0a114bfbec35c0aec482356baed8e15f747658fcdca6e6`  
		Last Modified: Fri, 08 Oct 2021 17:27:01 GMT  
		Size: 223.8 MB (223814497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c397d8744aa1d4eb6230a18250d33169abf2ae6ab30f09fa5f287c7950bd2`  
		Last Modified: Fri, 08 Oct 2021 17:26:34 GMT  
		Size: 2.5 MB (2506003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4435dbe6255c1f833427223a7e5f73ef0624514d7afece7954d674711d2193e7`  
		Last Modified: Fri, 08 Oct 2021 17:26:33 GMT  
		Size: 853.2 KB (853224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1db7ace550d5156b967f291a8e4c7e6ced71811122cf63105218f1fec0765c`  
		Last Modified: Fri, 08 Oct 2021 17:27:05 GMT  
		Size: 281.2 MB (281200538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fabbe06bcdde04e0b7ef2e9e1501599c3011214e12419e881aae211be58850c`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93d2bb6236506da7b29e172c991710872da38e9ab70ad4c3ff2132756456116`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3682eb88f77b41507ca9c8b7bc2958f0f07845f3b825be6ca9bd2217cb78ff`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90658b550a295730b105270faa8854a617aaa7d765cb3d9dfcec69d7e3c15e1`  
		Last Modified: Fri, 08 Oct 2021 17:26:30 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
