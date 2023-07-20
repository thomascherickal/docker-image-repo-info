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
$ docker pull odoo@sha256:ea5cde710a9600e7bdd8d81f48ff5897564c47a39655ff55db4275061559887c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:793cb425d91e4ea64082bf5bbee3d872684864321a3ebfff42daa2103093dfbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.9 MB (532931140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:778a631e09838b3d8a4d5d34ef2d4e0e43850195da78cd0196809a803f5b0948`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:47 GMT
ADD file:ca4076bfffab8d09636384070ca253570590554cff76a132afaae5cd89b363b5 in / 
# Tue, 04 Jul 2023 01:20:48 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:54:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:54:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:54:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:23 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:56:34 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:56:37 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:56:37 GMT
ENV ODOO_VERSION=14.0
# Thu, 20 Jul 2023 19:23:05 GMT
ARG ODOO_RELEASE=20230720
# Thu, 20 Jul 2023 19:23:05 GMT
ARG ODOO_SHA=41b37bf9b9e9769045f07c5bbf152e7819f49885
# Thu, 20 Jul 2023 19:24:27 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=41b37bf9b9e9769045f07c5bbf152e7819f49885
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 20 Jul 2023 19:24:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 20 Jul 2023 19:24:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 20 Jul 2023 19:24:32 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=41b37bf9b9e9769045f07c5bbf152e7819f49885
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 20 Jul 2023 19:24:32 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 20 Jul 2023 19:24:32 GMT
EXPOSE 8069 8071 8072
# Thu, 20 Jul 2023 19:24:32 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 20 Jul 2023 19:24:32 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 20 Jul 2023 19:24:32 GMT
USER odoo
# Thu, 20 Jul 2023 19:24:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Jul 2023 19:24:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:90ac1ecaf92c8ae0cb37d29d8cc01b5802612c12edb933c369ad4c586ea94c6c`  
		Last Modified: Tue, 04 Jul 2023 01:26:21 GMT  
		Size: 27.1 MB (27138502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00e825012af0c5f20095b1f8902b3341da662edb2331f4bc160e8291a8d2ff8`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 213.2 MB (213180476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab84fcf971d80a1b3e08f8415ad0ba35cbedb84cb7594ec24c79ad3dab44e84`  
		Last Modified: Tue, 04 Jul 2023 16:59:56 GMT  
		Size: 13.5 MB (13520290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc728f9cb60a83b4ab60b063840b0f84f5855805efe3fee682ef70cb18bb5`  
		Last Modified: Tue, 04 Jul 2023 16:59:54 GMT  
		Size: 458.3 KB (458274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065e25873d9484d6044ee193132e06a5b4e2adce6e9344b06e0475e475d67224`  
		Last Modified: Thu, 20 Jul 2023 19:26:52 GMT  
		Size: 278.6 MB (278631134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b74a25165d8dc6fe04435e7842d29c9944ee7000806b1fe1cebefaf7f835d9`  
		Last Modified: Thu, 20 Jul 2023 19:26:21 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e85d784556b70c04ef25d1969a83a5a8722d59956b6cc09ab30b7ba187548`  
		Last Modified: Thu, 20 Jul 2023 19:26:22 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efb863267edf6c00d9d2fbfe75d6b87a6a434e78b521d2728b79c57f5f43b9a`  
		Last Modified: Thu, 20 Jul 2023 19:26:22 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b2229074ad3f268dcf6ce5068a2371ce5d34010baf8a5b7146d497897dbbad`  
		Last Modified: Thu, 20 Jul 2023 19:26:21 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:ea5cde710a9600e7bdd8d81f48ff5897564c47a39655ff55db4275061559887c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:793cb425d91e4ea64082bf5bbee3d872684864321a3ebfff42daa2103093dfbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.9 MB (532931140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:778a631e09838b3d8a4d5d34ef2d4e0e43850195da78cd0196809a803f5b0948`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:47 GMT
ADD file:ca4076bfffab8d09636384070ca253570590554cff76a132afaae5cd89b363b5 in / 
# Tue, 04 Jul 2023 01:20:48 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:54:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:54:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:54:33 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:56:23 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:56:34 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:56:37 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:56:37 GMT
ENV ODOO_VERSION=14.0
# Thu, 20 Jul 2023 19:23:05 GMT
ARG ODOO_RELEASE=20230720
# Thu, 20 Jul 2023 19:23:05 GMT
ARG ODOO_SHA=41b37bf9b9e9769045f07c5bbf152e7819f49885
# Thu, 20 Jul 2023 19:24:27 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=41b37bf9b9e9769045f07c5bbf152e7819f49885
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 20 Jul 2023 19:24:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 20 Jul 2023 19:24:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 20 Jul 2023 19:24:32 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=41b37bf9b9e9769045f07c5bbf152e7819f49885
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 20 Jul 2023 19:24:32 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 20 Jul 2023 19:24:32 GMT
EXPOSE 8069 8071 8072
# Thu, 20 Jul 2023 19:24:32 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 20 Jul 2023 19:24:32 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 20 Jul 2023 19:24:32 GMT
USER odoo
# Thu, 20 Jul 2023 19:24:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Jul 2023 19:24:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:90ac1ecaf92c8ae0cb37d29d8cc01b5802612c12edb933c369ad4c586ea94c6c`  
		Last Modified: Tue, 04 Jul 2023 01:26:21 GMT  
		Size: 27.1 MB (27138502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00e825012af0c5f20095b1f8902b3341da662edb2331f4bc160e8291a8d2ff8`  
		Last Modified: Tue, 04 Jul 2023 17:00:16 GMT  
		Size: 213.2 MB (213180476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab84fcf971d80a1b3e08f8415ad0ba35cbedb84cb7594ec24c79ad3dab44e84`  
		Last Modified: Tue, 04 Jul 2023 16:59:56 GMT  
		Size: 13.5 MB (13520290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bc728f9cb60a83b4ab60b063840b0f84f5855805efe3fee682ef70cb18bb5`  
		Last Modified: Tue, 04 Jul 2023 16:59:54 GMT  
		Size: 458.3 KB (458274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065e25873d9484d6044ee193132e06a5b4e2adce6e9344b06e0475e475d67224`  
		Last Modified: Thu, 20 Jul 2023 19:26:52 GMT  
		Size: 278.6 MB (278631134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b74a25165d8dc6fe04435e7842d29c9944ee7000806b1fe1cebefaf7f835d9`  
		Last Modified: Thu, 20 Jul 2023 19:26:21 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e85d784556b70c04ef25d1969a83a5a8722d59956b6cc09ab30b7ba187548`  
		Last Modified: Thu, 20 Jul 2023 19:26:22 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efb863267edf6c00d9d2fbfe75d6b87a6a434e78b521d2728b79c57f5f43b9a`  
		Last Modified: Thu, 20 Jul 2023 19:26:22 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b2229074ad3f268dcf6ce5068a2371ce5d34010baf8a5b7146d497897dbbad`  
		Last Modified: Thu, 20 Jul 2023 19:26:21 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:d1773a5b173af4e9921ef46249e0b448fc89bb6ec4a587be162d77dfececc8a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:d7818769f70a9bf2ca77154bb8cbda93103b60c0faa16560c1d58180dd1eb79a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.9 MB (561913916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c87cfe007c05eccb006ff357cbef3a5e8cd67a2b28d7d67eca4a87fdc12fc0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:48:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:52:59 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:53:05 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:53:06 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:53:06 GMT
ENV ODOO_VERSION=15.0
# Thu, 20 Jul 2023 19:21:41 GMT
ARG ODOO_RELEASE=20230720
# Thu, 20 Jul 2023 19:21:41 GMT
ARG ODOO_SHA=5d5fb2e548734dcee584614d2385afc8f877eadc
# Thu, 20 Jul 2023 19:22:57 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=5d5fb2e548734dcee584614d2385afc8f877eadc
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 20 Jul 2023 19:23:01 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 20 Jul 2023 19:23:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 20 Jul 2023 19:23:01 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=5d5fb2e548734dcee584614d2385afc8f877eadc
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 20 Jul 2023 19:23:01 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 20 Jul 2023 19:23:01 GMT
EXPOSE 8069 8071 8072
# Thu, 20 Jul 2023 19:23:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 20 Jul 2023 19:23:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 20 Jul 2023 19:23:02 GMT
USER odoo
# Thu, 20 Jul 2023 19:23:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Jul 2023 19:23:02 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecec17eceb6c3674130e046a294357d03d0a4328163573bf205d3e3313a92b3`  
		Last Modified: Tue, 04 Jul 2023 16:59:33 GMT  
		Size: 220.3 MB (220302668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a3ff92d45f28abea1907822b9422b22044c4d8c3ea79cbbd890eedec7d2a2b`  
		Last Modified: Tue, 04 Jul 2023 16:59:09 GMT  
		Size: 2.6 MB (2576221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae451cd3af67981acb0b0f325d282607dfb4442750de0e5ef333d984e2ecae`  
		Last Modified: Tue, 04 Jul 2023 16:59:08 GMT  
		Size: 453.8 KB (453828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59746f2336c58394cada57b16086217f6b687a57389def53e63078b0ec94b0a9`  
		Last Modified: Thu, 20 Jul 2023 19:26:12 GMT  
		Size: 307.2 MB (307161353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be583dfe46e088a3bc1338365c265680de50534e5badf3115b6f5c3fafe86de9`  
		Last Modified: Thu, 20 Jul 2023 19:25:38 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666c29e4877eb5651dea5bfa67f492c21d913fd2e9c2c9c0ca134ea8837b9e28`  
		Last Modified: Thu, 20 Jul 2023 19:25:38 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b61755483f07f748d13b4af64075ca5c67cab12332b1e443ba64b1c7dded16b`  
		Last Modified: Thu, 20 Jul 2023 19:25:38 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58aeb552472ba22e9268db727c68801b48a51ba25f76f69f874bc19bdc5f8c56`  
		Last Modified: Thu, 20 Jul 2023 19:25:38 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:d1773a5b173af4e9921ef46249e0b448fc89bb6ec4a587be162d77dfececc8a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:d7818769f70a9bf2ca77154bb8cbda93103b60c0faa16560c1d58180dd1eb79a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.9 MB (561913916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c87cfe007c05eccb006ff357cbef3a5e8cd67a2b28d7d67eca4a87fdc12fc0f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:48:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:52:59 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:53:05 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:53:06 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:53:06 GMT
ENV ODOO_VERSION=15.0
# Thu, 20 Jul 2023 19:21:41 GMT
ARG ODOO_RELEASE=20230720
# Thu, 20 Jul 2023 19:21:41 GMT
ARG ODOO_SHA=5d5fb2e548734dcee584614d2385afc8f877eadc
# Thu, 20 Jul 2023 19:22:57 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=5d5fb2e548734dcee584614d2385afc8f877eadc
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 20 Jul 2023 19:23:01 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 20 Jul 2023 19:23:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 20 Jul 2023 19:23:01 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=5d5fb2e548734dcee584614d2385afc8f877eadc
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 20 Jul 2023 19:23:01 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 20 Jul 2023 19:23:01 GMT
EXPOSE 8069 8071 8072
# Thu, 20 Jul 2023 19:23:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 20 Jul 2023 19:23:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 20 Jul 2023 19:23:02 GMT
USER odoo
# Thu, 20 Jul 2023 19:23:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Jul 2023 19:23:02 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecec17eceb6c3674130e046a294357d03d0a4328163573bf205d3e3313a92b3`  
		Last Modified: Tue, 04 Jul 2023 16:59:33 GMT  
		Size: 220.3 MB (220302668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a3ff92d45f28abea1907822b9422b22044c4d8c3ea79cbbd890eedec7d2a2b`  
		Last Modified: Tue, 04 Jul 2023 16:59:09 GMT  
		Size: 2.6 MB (2576221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae451cd3af67981acb0b0f325d282607dfb4442750de0e5ef333d984e2ecae`  
		Last Modified: Tue, 04 Jul 2023 16:59:08 GMT  
		Size: 453.8 KB (453828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59746f2336c58394cada57b16086217f6b687a57389def53e63078b0ec94b0a9`  
		Last Modified: Thu, 20 Jul 2023 19:26:12 GMT  
		Size: 307.2 MB (307161353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be583dfe46e088a3bc1338365c265680de50534e5badf3115b6f5c3fafe86de9`  
		Last Modified: Thu, 20 Jul 2023 19:25:38 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666c29e4877eb5651dea5bfa67f492c21d913fd2e9c2c9c0ca134ea8837b9e28`  
		Last Modified: Thu, 20 Jul 2023 19:25:38 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b61755483f07f748d13b4af64075ca5c67cab12332b1e443ba64b1c7dded16b`  
		Last Modified: Thu, 20 Jul 2023 19:25:38 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58aeb552472ba22e9268db727c68801b48a51ba25f76f69f874bc19bdc5f8c56`  
		Last Modified: Thu, 20 Jul 2023 19:25:38 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:f0c24801e83a3d074cebfbb59c933d0bb34a8a43edaf2d3e695c7741090ac7fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:5447a32b56fd5ce9005126933fb0c39c4ce50dea3fc5174ba82a88c217807b6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **575.0 MB (575013087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cddb3e1fcc0e9921ae129d568d3adc14a660c459afa64a3c5e89fc11ce2fd5cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:48:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:50:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:50:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:50:14 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:50:14 GMT
ENV ODOO_VERSION=16.0
# Thu, 20 Jul 2023 19:20:03 GMT
ARG ODOO_RELEASE=20230720
# Thu, 20 Jul 2023 19:20:03 GMT
ARG ODOO_SHA=a8aa7b6dcd8722065d426526d06b76513fb0500e
# Thu, 20 Jul 2023 19:21:27 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=a8aa7b6dcd8722065d426526d06b76513fb0500e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 20 Jul 2023 19:21:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 20 Jul 2023 19:21:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 20 Jul 2023 19:21:32 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=a8aa7b6dcd8722065d426526d06b76513fb0500e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 20 Jul 2023 19:21:32 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 20 Jul 2023 19:21:32 GMT
EXPOSE 8069 8071 8072
# Thu, 20 Jul 2023 19:21:32 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 20 Jul 2023 19:21:32 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 20 Jul 2023 19:21:32 GMT
USER odoo
# Thu, 20 Jul 2023 19:21:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Jul 2023 19:21:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c7d3da2fbd2d726a8fe59c3992de7895dd89fadab551a495625fa48e8c5e7`  
		Last Modified: Tue, 04 Jul 2023 16:58:45 GMT  
		Size: 221.0 MB (220991764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd6f861e7cdc6a59484c202dc889a03e05ccea95d4463d5151d5d4d453f418b`  
		Last Modified: Tue, 04 Jul 2023 16:58:21 GMT  
		Size: 2.6 MB (2579607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9919e5999fecf8a9ca11971e06d8a9e2cd6d34b66814734d1133fa1a15c18974`  
		Last Modified: Tue, 04 Jul 2023 16:58:20 GMT  
		Size: 453.8 KB (453840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eef08a146fc9507ef71082bc347f0d29ff21bd404e197c7cd85816682fdde6`  
		Last Modified: Thu, 20 Jul 2023 19:25:27 GMT  
		Size: 319.6 MB (319568024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ea62dc068f265547b7860208d20e6fbf27010604f3d94d82eed9aa042e5670`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66983719352291b41b5df36f2218d5efd6c4bbb9fe710deeeba15b0a3b35d6bd`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a70f8bd79baeba3298dfa5ff82ddc1481896e5c5dc929eada3950a00f23440b`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b229fcd08c4172b87cdd056ecd1905003360746d562a456d2e5091d791418b`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:f0c24801e83a3d074cebfbb59c933d0bb34a8a43edaf2d3e695c7741090ac7fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:5447a32b56fd5ce9005126933fb0c39c4ce50dea3fc5174ba82a88c217807b6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **575.0 MB (575013087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cddb3e1fcc0e9921ae129d568d3adc14a660c459afa64a3c5e89fc11ce2fd5cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:48:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:50:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:50:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:50:14 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:50:14 GMT
ENV ODOO_VERSION=16.0
# Thu, 20 Jul 2023 19:20:03 GMT
ARG ODOO_RELEASE=20230720
# Thu, 20 Jul 2023 19:20:03 GMT
ARG ODOO_SHA=a8aa7b6dcd8722065d426526d06b76513fb0500e
# Thu, 20 Jul 2023 19:21:27 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=a8aa7b6dcd8722065d426526d06b76513fb0500e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 20 Jul 2023 19:21:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 20 Jul 2023 19:21:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 20 Jul 2023 19:21:32 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=a8aa7b6dcd8722065d426526d06b76513fb0500e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 20 Jul 2023 19:21:32 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 20 Jul 2023 19:21:32 GMT
EXPOSE 8069 8071 8072
# Thu, 20 Jul 2023 19:21:32 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 20 Jul 2023 19:21:32 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 20 Jul 2023 19:21:32 GMT
USER odoo
# Thu, 20 Jul 2023 19:21:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Jul 2023 19:21:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c7d3da2fbd2d726a8fe59c3992de7895dd89fadab551a495625fa48e8c5e7`  
		Last Modified: Tue, 04 Jul 2023 16:58:45 GMT  
		Size: 221.0 MB (220991764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd6f861e7cdc6a59484c202dc889a03e05ccea95d4463d5151d5d4d453f418b`  
		Last Modified: Tue, 04 Jul 2023 16:58:21 GMT  
		Size: 2.6 MB (2579607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9919e5999fecf8a9ca11971e06d8a9e2cd6d34b66814734d1133fa1a15c18974`  
		Last Modified: Tue, 04 Jul 2023 16:58:20 GMT  
		Size: 453.8 KB (453840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eef08a146fc9507ef71082bc347f0d29ff21bd404e197c7cd85816682fdde6`  
		Last Modified: Thu, 20 Jul 2023 19:25:27 GMT  
		Size: 319.6 MB (319568024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ea62dc068f265547b7860208d20e6fbf27010604f3d94d82eed9aa042e5670`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66983719352291b41b5df36f2218d5efd6c4bbb9fe710deeeba15b0a3b35d6bd`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a70f8bd79baeba3298dfa5ff82ddc1481896e5c5dc929eada3950a00f23440b`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b229fcd08c4172b87cdd056ecd1905003360746d562a456d2e5091d791418b`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:f0c24801e83a3d074cebfbb59c933d0bb34a8a43edaf2d3e695c7741090ac7fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:5447a32b56fd5ce9005126933fb0c39c4ce50dea3fc5174ba82a88c217807b6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **575.0 MB (575013087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cddb3e1fcc0e9921ae129d568d3adc14a660c459afa64a3c5e89fc11ce2fd5cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 16:48:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 04 Jul 2023 16:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 04 Jul 2023 16:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 16:50:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 04 Jul 2023 16:50:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 16:50:14 GMT
RUN npm install -g rtlcss
# Tue, 04 Jul 2023 16:50:14 GMT
ENV ODOO_VERSION=16.0
# Thu, 20 Jul 2023 19:20:03 GMT
ARG ODOO_RELEASE=20230720
# Thu, 20 Jul 2023 19:20:03 GMT
ARG ODOO_SHA=a8aa7b6dcd8722065d426526d06b76513fb0500e
# Thu, 20 Jul 2023 19:21:27 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=a8aa7b6dcd8722065d426526d06b76513fb0500e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 20 Jul 2023 19:21:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 20 Jul 2023 19:21:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 20 Jul 2023 19:21:32 GMT
# ARGS: ODOO_RELEASE=20230720 ODOO_SHA=a8aa7b6dcd8722065d426526d06b76513fb0500e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 20 Jul 2023 19:21:32 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 20 Jul 2023 19:21:32 GMT
EXPOSE 8069 8071 8072
# Thu, 20 Jul 2023 19:21:32 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 20 Jul 2023 19:21:32 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 20 Jul 2023 19:21:32 GMT
USER odoo
# Thu, 20 Jul 2023 19:21:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 20 Jul 2023 19:21:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2c7d3da2fbd2d726a8fe59c3992de7895dd89fadab551a495625fa48e8c5e7`  
		Last Modified: Tue, 04 Jul 2023 16:58:45 GMT  
		Size: 221.0 MB (220991764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd6f861e7cdc6a59484c202dc889a03e05ccea95d4463d5151d5d4d453f418b`  
		Last Modified: Tue, 04 Jul 2023 16:58:21 GMT  
		Size: 2.6 MB (2579607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9919e5999fecf8a9ca11971e06d8a9e2cd6d34b66814734d1133fa1a15c18974`  
		Last Modified: Tue, 04 Jul 2023 16:58:20 GMT  
		Size: 453.8 KB (453840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eef08a146fc9507ef71082bc347f0d29ff21bd404e197c7cd85816682fdde6`  
		Last Modified: Thu, 20 Jul 2023 19:25:27 GMT  
		Size: 319.6 MB (319568024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ea62dc068f265547b7860208d20e6fbf27010604f3d94d82eed9aa042e5670`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66983719352291b41b5df36f2218d5efd6c4bbb9fe710deeeba15b0a3b35d6bd`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a70f8bd79baeba3298dfa5ff82ddc1481896e5c5dc929eada3950a00f23440b`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b229fcd08c4172b87cdd056ecd1905003360746d562a456d2e5091d791418b`  
		Last Modified: Thu, 20 Jul 2023 19:24:51 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
