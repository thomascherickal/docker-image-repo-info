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
$ docker pull odoo@sha256:846cfec78a7a0c2d4ddcd19401f69e0c79f0723d1f8aab612b9dca9885fc4414
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:5d94518fa1da64752ab062a8587891c3215a09b051c7f88047b3c97d8e2edff7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.3 MB (540261672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f76261781335097ca39e63850822ee00a24f281722505d13aa265d699a349b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 05:07:11 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Jul 2022 05:07:12 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Jul 2022 05:07:12 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 05:12:01 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Jul 2022 05:12:10 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 05:12:13 GMT
RUN npm install -g rtlcss
# Tue, 12 Jul 2022 05:12:13 GMT
ENV ODOO_VERSION=13.0
# Mon, 18 Jul 2022 19:42:55 GMT
ARG ODOO_RELEASE=20220718
# Mon, 18 Jul 2022 19:42:55 GMT
ARG ODOO_SHA=c96fedf5e961122bc9face8dba102105070cbfb7
# Mon, 18 Jul 2022 19:44:09 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=c96fedf5e961122bc9face8dba102105070cbfb7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Jul 2022 19:44:13 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Jul 2022 19:44:13 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Jul 2022 19:44:13 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=c96fedf5e961122bc9face8dba102105070cbfb7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Jul 2022 19:44:14 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Jul 2022 19:44:14 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Jul 2022 19:44:14 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Jul 2022 19:44:14 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Jul 2022 19:44:14 GMT
USER odoo
# Mon, 18 Jul 2022 19:44:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Jul 2022 19:44:14 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852edb0bc3cf7963a8d53091d65864192ba609316a32de7d373812c11a43e28`  
		Last Modified: Tue, 12 Jul 2022 05:15:58 GMT  
		Size: 207.1 MB (207143706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eea1562761dce01430688c0be779ab4da5abf82e2aa502688ff39d9785fa17f`  
		Last Modified: Tue, 12 Jul 2022 05:15:36 GMT  
		Size: 13.4 MB (13442978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c92a3860784edf4233f1a93fc66b06c2d4a3cb36d3a60f468648fa36cad3a5`  
		Last Modified: Tue, 12 Jul 2022 05:15:33 GMT  
		Size: 507.3 KB (507319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a38c1b9f5adc13be44340bbec59654e2693b78919d3f47f6a21cb95c0841d5d`  
		Last Modified: Mon, 18 Jul 2022 19:46:40 GMT  
		Size: 292.0 MB (292025353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa09843442d115d46f66f3640639ff4d1889238dd9f229a4c986fb74e822be1`  
		Last Modified: Mon, 18 Jul 2022 19:46:06 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7175a686ed1cc54737c83880d0647578cfa2b9f71f6e3314f7850abd697f4`  
		Last Modified: Mon, 18 Jul 2022 19:46:06 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b3818b5f0a287df59ab3ee497361b4731080016254ee14e769b235f67bf922`  
		Last Modified: Mon, 18 Jul 2022 19:46:06 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239f7b74693d48ba6a8896db140b0fecf0e0998ef353e5b87756c6da2df184b`  
		Last Modified: Mon, 18 Jul 2022 19:46:06 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:846cfec78a7a0c2d4ddcd19401f69e0c79f0723d1f8aab612b9dca9885fc4414
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:5d94518fa1da64752ab062a8587891c3215a09b051c7f88047b3c97d8e2edff7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.3 MB (540261672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f76261781335097ca39e63850822ee00a24f281722505d13aa265d699a349b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 05:07:11 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Jul 2022 05:07:12 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Jul 2022 05:07:12 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 05:12:01 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Jul 2022 05:12:10 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 05:12:13 GMT
RUN npm install -g rtlcss
# Tue, 12 Jul 2022 05:12:13 GMT
ENV ODOO_VERSION=13.0
# Mon, 18 Jul 2022 19:42:55 GMT
ARG ODOO_RELEASE=20220718
# Mon, 18 Jul 2022 19:42:55 GMT
ARG ODOO_SHA=c96fedf5e961122bc9face8dba102105070cbfb7
# Mon, 18 Jul 2022 19:44:09 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=c96fedf5e961122bc9face8dba102105070cbfb7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Jul 2022 19:44:13 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Jul 2022 19:44:13 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Jul 2022 19:44:13 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=c96fedf5e961122bc9face8dba102105070cbfb7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Jul 2022 19:44:14 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Jul 2022 19:44:14 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Jul 2022 19:44:14 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Jul 2022 19:44:14 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Jul 2022 19:44:14 GMT
USER odoo
# Mon, 18 Jul 2022 19:44:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Jul 2022 19:44:14 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852edb0bc3cf7963a8d53091d65864192ba609316a32de7d373812c11a43e28`  
		Last Modified: Tue, 12 Jul 2022 05:15:58 GMT  
		Size: 207.1 MB (207143706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eea1562761dce01430688c0be779ab4da5abf82e2aa502688ff39d9785fa17f`  
		Last Modified: Tue, 12 Jul 2022 05:15:36 GMT  
		Size: 13.4 MB (13442978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c92a3860784edf4233f1a93fc66b06c2d4a3cb36d3a60f468648fa36cad3a5`  
		Last Modified: Tue, 12 Jul 2022 05:15:33 GMT  
		Size: 507.3 KB (507319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a38c1b9f5adc13be44340bbec59654e2693b78919d3f47f6a21cb95c0841d5d`  
		Last Modified: Mon, 18 Jul 2022 19:46:40 GMT  
		Size: 292.0 MB (292025353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa09843442d115d46f66f3640639ff4d1889238dd9f229a4c986fb74e822be1`  
		Last Modified: Mon, 18 Jul 2022 19:46:06 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7175a686ed1cc54737c83880d0647578cfa2b9f71f6e3314f7850abd697f4`  
		Last Modified: Mon, 18 Jul 2022 19:46:06 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b3818b5f0a287df59ab3ee497361b4731080016254ee14e769b235f67bf922`  
		Last Modified: Mon, 18 Jul 2022 19:46:06 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239f7b74693d48ba6a8896db140b0fecf0e0998ef353e5b87756c6da2df184b`  
		Last Modified: Mon, 18 Jul 2022 19:46:06 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:4275209e9798defb129ead30cdee0e4e373efac35e02e5848fdabe65ebaa92bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:f5a211f21546dbd9e257b014fdc64b2c48dd39f5bfdfbf2c9e62d99414eea98d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.7 MB (530669977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c38986fa52bd19322a9de8286fe2e8ade256bc3f9d6e6a4757286a36e0176605`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 05:07:11 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Jul 2022 05:07:12 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Jul 2022 05:07:12 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 05:09:19 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Jul 2022 05:09:30 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 05:09:33 GMT
RUN npm install -g rtlcss
# Tue, 12 Jul 2022 05:09:33 GMT
ENV ODOO_VERSION=14.0
# Mon, 18 Jul 2022 19:41:32 GMT
ARG ODOO_RELEASE=20220718
# Mon, 18 Jul 2022 19:41:32 GMT
ARG ODOO_SHA=c93ae8c22679a87d649157a3ddcc761600e28ee0
# Mon, 18 Jul 2022 19:42:47 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=c93ae8c22679a87d649157a3ddcc761600e28ee0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Jul 2022 19:42:51 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Jul 2022 19:42:51 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Jul 2022 19:42:51 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=c93ae8c22679a87d649157a3ddcc761600e28ee0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Jul 2022 19:42:51 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Jul 2022 19:42:52 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Jul 2022 19:42:52 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Jul 2022 19:42:52 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Jul 2022 19:42:52 GMT
USER odoo
# Mon, 18 Jul 2022 19:42:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Jul 2022 19:42:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7db92b31c88865d67202221ad996ca6f787faca3044b81dfa2f2d0aba24d76c`  
		Last Modified: Tue, 12 Jul 2022 05:15:14 GMT  
		Size: 213.2 MB (213181225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a26123be6a074f5572314d58f00bdce78d718ad7637c765aed5cb40216aa68f`  
		Last Modified: Tue, 12 Jul 2022 05:14:51 GMT  
		Size: 13.4 MB (13444821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f6a2f05ad0ade1ec05cf84832a9f66415f833cf01f60102a4206e5254e1d73`  
		Last Modified: Tue, 12 Jul 2022 05:14:48 GMT  
		Size: 507.3 KB (507328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5524b4100618d79ac8a6bc83303b47779fdebb122e1b5d55e5aaf1ecc279130`  
		Last Modified: Mon, 18 Jul 2022 19:45:56 GMT  
		Size: 276.4 MB (276394291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d83634b89be7d559f678db259911f45c226cb762574f20289cab16de5dd3fd1`  
		Last Modified: Mon, 18 Jul 2022 19:45:20 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baed28c48cccb8d713f265bcec43342866951bac5164eccb05296e64f5ed4b54`  
		Last Modified: Mon, 18 Jul 2022 19:45:20 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5fc4576541c5e07903ff386a01f18839d2e694bf4e49ea95096e911be9e7c4`  
		Last Modified: Mon, 18 Jul 2022 19:45:20 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b14a4418c0880a8223800519fbecf407002e3888a3d2a1cdbc399d1769b1c35`  
		Last Modified: Mon, 18 Jul 2022 19:45:20 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:4275209e9798defb129ead30cdee0e4e373efac35e02e5848fdabe65ebaa92bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:f5a211f21546dbd9e257b014fdc64b2c48dd39f5bfdfbf2c9e62d99414eea98d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.7 MB (530669977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c38986fa52bd19322a9de8286fe2e8ade256bc3f9d6e6a4757286a36e0176605`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 05:07:11 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Jul 2022 05:07:12 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Jul 2022 05:07:12 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 05:09:19 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Jul 2022 05:09:30 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 05:09:33 GMT
RUN npm install -g rtlcss
# Tue, 12 Jul 2022 05:09:33 GMT
ENV ODOO_VERSION=14.0
# Mon, 18 Jul 2022 19:41:32 GMT
ARG ODOO_RELEASE=20220718
# Mon, 18 Jul 2022 19:41:32 GMT
ARG ODOO_SHA=c93ae8c22679a87d649157a3ddcc761600e28ee0
# Mon, 18 Jul 2022 19:42:47 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=c93ae8c22679a87d649157a3ddcc761600e28ee0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Jul 2022 19:42:51 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Jul 2022 19:42:51 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Jul 2022 19:42:51 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=c93ae8c22679a87d649157a3ddcc761600e28ee0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Jul 2022 19:42:51 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Jul 2022 19:42:52 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Jul 2022 19:42:52 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Jul 2022 19:42:52 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Jul 2022 19:42:52 GMT
USER odoo
# Mon, 18 Jul 2022 19:42:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Jul 2022 19:42:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7db92b31c88865d67202221ad996ca6f787faca3044b81dfa2f2d0aba24d76c`  
		Last Modified: Tue, 12 Jul 2022 05:15:14 GMT  
		Size: 213.2 MB (213181225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a26123be6a074f5572314d58f00bdce78d718ad7637c765aed5cb40216aa68f`  
		Last Modified: Tue, 12 Jul 2022 05:14:51 GMT  
		Size: 13.4 MB (13444821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f6a2f05ad0ade1ec05cf84832a9f66415f833cf01f60102a4206e5254e1d73`  
		Last Modified: Tue, 12 Jul 2022 05:14:48 GMT  
		Size: 507.3 KB (507328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5524b4100618d79ac8a6bc83303b47779fdebb122e1b5d55e5aaf1ecc279130`  
		Last Modified: Mon, 18 Jul 2022 19:45:56 GMT  
		Size: 276.4 MB (276394291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d83634b89be7d559f678db259911f45c226cb762574f20289cab16de5dd3fd1`  
		Last Modified: Mon, 18 Jul 2022 19:45:20 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baed28c48cccb8d713f265bcec43342866951bac5164eccb05296e64f5ed4b54`  
		Last Modified: Mon, 18 Jul 2022 19:45:20 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5fc4576541c5e07903ff386a01f18839d2e694bf4e49ea95096e911be9e7c4`  
		Last Modified: Mon, 18 Jul 2022 19:45:20 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b14a4418c0880a8223800519fbecf407002e3888a3d2a1cdbc399d1769b1c35`  
		Last Modified: Mon, 18 Jul 2022 19:45:20 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:485464c5a716238b3777f174a918b62647a20b3f9d7771b6f8cd9beba34d1553
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:04abd658385ba21236732e4ad4468f6e20572926da636b68ae76c9e37f2b322a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **556.1 MB (556102838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3651d492adc238d8865bdb3a8a9fc057f2cf06ef7fb2709f8bbb33ce5db2b11c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 05:04:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Jul 2022 05:04:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Jul 2022 05:04:34 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 05:05:32 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Jul 2022 05:05:43 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 05:05:44 GMT
RUN npm install -g rtlcss
# Tue, 12 Jul 2022 05:05:45 GMT
ENV ODOO_VERSION=15.0
# Mon, 18 Jul 2022 19:39:54 GMT
ARG ODOO_RELEASE=20220718
# Mon, 18 Jul 2022 19:39:54 GMT
ARG ODOO_SHA=dc4a5b8c5be8f873e751539117f5aa41d9f7b217
# Mon, 18 Jul 2022 19:41:12 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=dc4a5b8c5be8f873e751539117f5aa41d9f7b217
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Jul 2022 19:41:14 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Jul 2022 19:41:14 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Jul 2022 19:41:15 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=dc4a5b8c5be8f873e751539117f5aa41d9f7b217
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Jul 2022 19:41:15 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Jul 2022 19:41:15 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Jul 2022 19:41:15 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Jul 2022 19:41:16 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Jul 2022 19:41:16 GMT
USER odoo
# Mon, 18 Jul 2022 19:41:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Jul 2022 19:41:16 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd973b6810fdbba62ef6caa3ec20f653447cd19ce0363dc02605f788609e3250`  
		Last Modified: Tue, 12 Jul 2022 05:14:24 GMT  
		Size: 220.3 MB (220289612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f428c41f4b038745626ff998e2d14ffd12d10db8fd0ca26db599d6427281e19`  
		Last Modified: Tue, 12 Jul 2022 05:13:58 GMT  
		Size: 2.5 MB (2513248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb3d7b1346d040310c399b056054bed18f042bdc35c215a26e90aaa77cc27c0`  
		Last Modified: Tue, 12 Jul 2022 05:13:58 GMT  
		Size: 500.9 KB (500921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10bca7e4fbe2df0312874dd91b38092b0341b243098fc9b655f10e3642b9f95`  
		Last Modified: Mon, 18 Jul 2022 19:45:07 GMT  
		Size: 301.4 MB (301429979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238f7340c39c9d30a7cd02d7b8d84c16116afc6eb7459f1bde5288c9a74e3e7d`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8001ab93bb35c091ee6bbe0ee8a348c12ddbda4b099a2b5c7fbdf68b5936cd79`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919c771689fbbedb64e28ce6a6559a3968cf01b1994110094b1b2266005feaf9`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b3ff8523517986c1acca320e83a0ea42ce7df0a18cde64075692768d138be`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:485464c5a716238b3777f174a918b62647a20b3f9d7771b6f8cd9beba34d1553
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:04abd658385ba21236732e4ad4468f6e20572926da636b68ae76c9e37f2b322a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **556.1 MB (556102838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3651d492adc238d8865bdb3a8a9fc057f2cf06ef7fb2709f8bbb33ce5db2b11c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 05:04:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Jul 2022 05:04:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Jul 2022 05:04:34 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 05:05:32 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Jul 2022 05:05:43 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 05:05:44 GMT
RUN npm install -g rtlcss
# Tue, 12 Jul 2022 05:05:45 GMT
ENV ODOO_VERSION=15.0
# Mon, 18 Jul 2022 19:39:54 GMT
ARG ODOO_RELEASE=20220718
# Mon, 18 Jul 2022 19:39:54 GMT
ARG ODOO_SHA=dc4a5b8c5be8f873e751539117f5aa41d9f7b217
# Mon, 18 Jul 2022 19:41:12 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=dc4a5b8c5be8f873e751539117f5aa41d9f7b217
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Jul 2022 19:41:14 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Jul 2022 19:41:14 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Jul 2022 19:41:15 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=dc4a5b8c5be8f873e751539117f5aa41d9f7b217
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Jul 2022 19:41:15 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Jul 2022 19:41:15 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Jul 2022 19:41:15 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Jul 2022 19:41:16 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Jul 2022 19:41:16 GMT
USER odoo
# Mon, 18 Jul 2022 19:41:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Jul 2022 19:41:16 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd973b6810fdbba62ef6caa3ec20f653447cd19ce0363dc02605f788609e3250`  
		Last Modified: Tue, 12 Jul 2022 05:14:24 GMT  
		Size: 220.3 MB (220289612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f428c41f4b038745626ff998e2d14ffd12d10db8fd0ca26db599d6427281e19`  
		Last Modified: Tue, 12 Jul 2022 05:13:58 GMT  
		Size: 2.5 MB (2513248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb3d7b1346d040310c399b056054bed18f042bdc35c215a26e90aaa77cc27c0`  
		Last Modified: Tue, 12 Jul 2022 05:13:58 GMT  
		Size: 500.9 KB (500921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10bca7e4fbe2df0312874dd91b38092b0341b243098fc9b655f10e3642b9f95`  
		Last Modified: Mon, 18 Jul 2022 19:45:07 GMT  
		Size: 301.4 MB (301429979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238f7340c39c9d30a7cd02d7b8d84c16116afc6eb7459f1bde5288c9a74e3e7d`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8001ab93bb35c091ee6bbe0ee8a348c12ddbda4b099a2b5c7fbdf68b5936cd79`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919c771689fbbedb64e28ce6a6559a3968cf01b1994110094b1b2266005feaf9`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b3ff8523517986c1acca320e83a0ea42ce7df0a18cde64075692768d138be`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:485464c5a716238b3777f174a918b62647a20b3f9d7771b6f8cd9beba34d1553
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:04abd658385ba21236732e4ad4468f6e20572926da636b68ae76c9e37f2b322a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **556.1 MB (556102838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3651d492adc238d8865bdb3a8a9fc057f2cf06ef7fb2709f8bbb33ce5db2b11c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 05:04:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Jul 2022 05:04:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Jul 2022 05:04:34 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jul 2022 05:05:32 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Jul 2022 05:05:43 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 05:05:44 GMT
RUN npm install -g rtlcss
# Tue, 12 Jul 2022 05:05:45 GMT
ENV ODOO_VERSION=15.0
# Mon, 18 Jul 2022 19:39:54 GMT
ARG ODOO_RELEASE=20220718
# Mon, 18 Jul 2022 19:39:54 GMT
ARG ODOO_SHA=dc4a5b8c5be8f873e751539117f5aa41d9f7b217
# Mon, 18 Jul 2022 19:41:12 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=dc4a5b8c5be8f873e751539117f5aa41d9f7b217
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 18 Jul 2022 19:41:14 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 18 Jul 2022 19:41:14 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 18 Jul 2022 19:41:15 GMT
# ARGS: ODOO_RELEASE=20220718 ODOO_SHA=dc4a5b8c5be8f873e751539117f5aa41d9f7b217
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 18 Jul 2022 19:41:15 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 18 Jul 2022 19:41:15 GMT
EXPOSE 8069 8071 8072
# Mon, 18 Jul 2022 19:41:15 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 18 Jul 2022 19:41:16 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 18 Jul 2022 19:41:16 GMT
USER odoo
# Mon, 18 Jul 2022 19:41:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 18 Jul 2022 19:41:16 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd973b6810fdbba62ef6caa3ec20f653447cd19ce0363dc02605f788609e3250`  
		Last Modified: Tue, 12 Jul 2022 05:14:24 GMT  
		Size: 220.3 MB (220289612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f428c41f4b038745626ff998e2d14ffd12d10db8fd0ca26db599d6427281e19`  
		Last Modified: Tue, 12 Jul 2022 05:13:58 GMT  
		Size: 2.5 MB (2513248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb3d7b1346d040310c399b056054bed18f042bdc35c215a26e90aaa77cc27c0`  
		Last Modified: Tue, 12 Jul 2022 05:13:58 GMT  
		Size: 500.9 KB (500921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10bca7e4fbe2df0312874dd91b38092b0341b243098fc9b655f10e3642b9f95`  
		Last Modified: Mon, 18 Jul 2022 19:45:07 GMT  
		Size: 301.4 MB (301429979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238f7340c39c9d30a7cd02d7b8d84c16116afc6eb7459f1bde5288c9a74e3e7d`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8001ab93bb35c091ee6bbe0ee8a348c12ddbda4b099a2b5c7fbdf68b5936cd79`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919c771689fbbedb64e28ce6a6559a3968cf01b1994110094b1b2266005feaf9`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46b3ff8523517986c1acca320e83a0ea42ce7df0a18cde64075692768d138be`  
		Last Modified: Mon, 18 Jul 2022 19:44:29 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
