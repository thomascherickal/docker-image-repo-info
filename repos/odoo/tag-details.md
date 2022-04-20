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
$ docker pull odoo@sha256:aefd57a8d744f24c80cd347a2c7ff95199343df30422cc0d14f72ba10f41a0cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:c8c1d7976417e93d5c3e8ba4605797ed69ea2c209f735db6a3c3186c30b54987
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539670881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:461514f98b2b64a6609d9778ee4fcaa548b4c9b25b92feb896a2c0f13e1b0885`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:46:25 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Apr 2022 12:46:25 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Apr 2022 12:46:25 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:50:29 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Apr 2022 12:50:37 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:50:41 GMT
RUN npm install -g rtlcss
# Wed, 20 Apr 2022 12:50:41 GMT
ENV ODOO_VERSION=13.0
# Wed, 20 Apr 2022 12:50:41 GMT
ARG ODOO_RELEASE=20220401
# Wed, 20 Apr 2022 12:50:41 GMT
ARG ODOO_SHA=2af3333f6048663e921ea49d7dc836d4dcf31cb4
# Wed, 20 Apr 2022 12:51:50 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=2af3333f6048663e921ea49d7dc836d4dcf31cb4
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Apr 2022 12:51:54 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Apr 2022 12:51:54 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Apr 2022 12:51:55 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=2af3333f6048663e921ea49d7dc836d4dcf31cb4
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Apr 2022 12:51:55 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Apr 2022 12:51:55 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Apr 2022 12:51:55 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Apr 2022 12:51:55 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Apr 2022 12:51:55 GMT
USER odoo
# Wed, 20 Apr 2022 12:51:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 12:51:55 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb5c2f3aa8570028e1481e683ce676526f2f383e1d583fc8fe80151c3d75a46`  
		Last Modified: Wed, 20 Apr 2022 12:54:29 GMT  
		Size: 207.1 MB (207144149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ed24c51a5113dc123abfe7c3ae5947e181a730ec5220f51852ce8b7cb296d9`  
		Last Modified: Wed, 20 Apr 2022 12:54:07 GMT  
		Size: 13.4 MB (13438172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2e9a8cb5ff656fd7d11d44d86b540b5429edfa5d9d2ce063061e5f2a027b2b`  
		Last Modified: Wed, 20 Apr 2022 12:54:05 GMT  
		Size: 458.4 KB (458398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403241b9f22e9996e1c2fa95b545d53d9348f6caed3c094e21ea7908f176a7bd`  
		Last Modified: Wed, 20 Apr 2022 12:54:35 GMT  
		Size: 291.5 MB (291487043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eddcee3836d2420aa302a16f8ca502b7a2172fd9b23d106996a2d6339a4386e`  
		Last Modified: Wed, 20 Apr 2022 12:54:02 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9529e56a286ccdf087c550e044d4280c139d678a22a861f4c8afe0fb7e9a4bc4`  
		Last Modified: Wed, 20 Apr 2022 12:54:03 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234dc2ba793d5cb21563d9b2356078770f243caff3e7bd0f3068cd159f455061`  
		Last Modified: Wed, 20 Apr 2022 12:54:02 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cf48d5059eecd1c5cbe666a523a3a2e1e2a4b630da6ab42e1c4d62bb6b6095`  
		Last Modified: Wed, 20 Apr 2022 12:54:02 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:aefd57a8d744f24c80cd347a2c7ff95199343df30422cc0d14f72ba10f41a0cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:c8c1d7976417e93d5c3e8ba4605797ed69ea2c209f735db6a3c3186c30b54987
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539670881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:461514f98b2b64a6609d9778ee4fcaa548b4c9b25b92feb896a2c0f13e1b0885`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:46:25 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Apr 2022 12:46:25 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Apr 2022 12:46:25 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:50:29 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Apr 2022 12:50:37 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:50:41 GMT
RUN npm install -g rtlcss
# Wed, 20 Apr 2022 12:50:41 GMT
ENV ODOO_VERSION=13.0
# Wed, 20 Apr 2022 12:50:41 GMT
ARG ODOO_RELEASE=20220401
# Wed, 20 Apr 2022 12:50:41 GMT
ARG ODOO_SHA=2af3333f6048663e921ea49d7dc836d4dcf31cb4
# Wed, 20 Apr 2022 12:51:50 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=2af3333f6048663e921ea49d7dc836d4dcf31cb4
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Apr 2022 12:51:54 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Apr 2022 12:51:54 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Apr 2022 12:51:55 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=2af3333f6048663e921ea49d7dc836d4dcf31cb4
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Apr 2022 12:51:55 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Apr 2022 12:51:55 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Apr 2022 12:51:55 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Apr 2022 12:51:55 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Apr 2022 12:51:55 GMT
USER odoo
# Wed, 20 Apr 2022 12:51:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 12:51:55 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb5c2f3aa8570028e1481e683ce676526f2f383e1d583fc8fe80151c3d75a46`  
		Last Modified: Wed, 20 Apr 2022 12:54:29 GMT  
		Size: 207.1 MB (207144149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ed24c51a5113dc123abfe7c3ae5947e181a730ec5220f51852ce8b7cb296d9`  
		Last Modified: Wed, 20 Apr 2022 12:54:07 GMT  
		Size: 13.4 MB (13438172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2e9a8cb5ff656fd7d11d44d86b540b5429edfa5d9d2ce063061e5f2a027b2b`  
		Last Modified: Wed, 20 Apr 2022 12:54:05 GMT  
		Size: 458.4 KB (458398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403241b9f22e9996e1c2fa95b545d53d9348f6caed3c094e21ea7908f176a7bd`  
		Last Modified: Wed, 20 Apr 2022 12:54:35 GMT  
		Size: 291.5 MB (291487043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eddcee3836d2420aa302a16f8ca502b7a2172fd9b23d106996a2d6339a4386e`  
		Last Modified: Wed, 20 Apr 2022 12:54:02 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9529e56a286ccdf087c550e044d4280c139d678a22a861f4c8afe0fb7e9a4bc4`  
		Last Modified: Wed, 20 Apr 2022 12:54:03 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234dc2ba793d5cb21563d9b2356078770f243caff3e7bd0f3068cd159f455061`  
		Last Modified: Wed, 20 Apr 2022 12:54:02 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cf48d5059eecd1c5cbe666a523a3a2e1e2a4b630da6ab42e1c4d62bb6b6095`  
		Last Modified: Wed, 20 Apr 2022 12:54:02 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:07efd5e67c10786abf849fb2e85a968b16d835471af8eab269c80144794239bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:bbb22d12833c98b8f2cced11e672c2d582633c96150a9c25f22a6d1449c27406
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.6 MB (529585408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b94de360c386e4634c7df247b98add8f999e3a97e9a78924b15105a6db795c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:46:25 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Apr 2022 12:46:25 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Apr 2022 12:46:25 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:47:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Apr 2022 12:47:52 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:47:55 GMT
RUN npm install -g rtlcss
# Wed, 20 Apr 2022 12:47:56 GMT
ENV ODOO_VERSION=14.0
# Wed, 20 Apr 2022 12:47:56 GMT
ARG ODOO_RELEASE=20220401
# Wed, 20 Apr 2022 12:47:56 GMT
ARG ODOO_SHA=43eabf4f6f55cd2887dc123d955bfaf9c7f27a32
# Wed, 20 Apr 2022 12:49:20 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=43eabf4f6f55cd2887dc123d955bfaf9c7f27a32
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Apr 2022 12:49:24 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Apr 2022 12:49:24 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Apr 2022 12:49:25 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=43eabf4f6f55cd2887dc123d955bfaf9c7f27a32
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Apr 2022 12:49:25 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Apr 2022 12:49:25 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Apr 2022 12:49:25 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Apr 2022 12:49:25 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Apr 2022 12:49:25 GMT
USER odoo
# Wed, 20 Apr 2022 12:49:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 12:49:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef0b3a5b3ccf6bc33961621c8b4217adc5f5ef26d7b92c47c8c39a8820fd58b`  
		Last Modified: Wed, 20 Apr 2022 12:53:38 GMT  
		Size: 213.2 MB (213177837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b2adc658049f20fffa9059922d790f2cc75e2fc5db14b3c1b77043b486b694`  
		Last Modified: Wed, 20 Apr 2022 12:53:16 GMT  
		Size: 13.4 MB (13440548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dafa09d0f12a0ed57ad93fe02efadcc57e517a8c1b2abf6d42c04e6b5031e65`  
		Last Modified: Wed, 20 Apr 2022 12:53:13 GMT  
		Size: 458.5 KB (458493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a3d801afb388ea73dfdcf1c98c4436eb0d013a20fe6e61e0d7a9acc5ce9a1a`  
		Last Modified: Wed, 20 Apr 2022 12:53:45 GMT  
		Size: 275.4 MB (275365415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b2ee8fe90a106f96a5f077118d24536f66e018e9446859e7185530b12180e`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5df638d02c88f9f1e5c6c15b591ad6404172d7cb9b3e1f1680f3f513ae005b2`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b7e5f969acb4c0d5dd7da1fc6683dd4500b2b9d52e08a9473aab7d1dd344cc`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebc2102fa546e7ff4adaf76bf6e0b1624fc5762fdd0f276350ace33eecae970`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:07efd5e67c10786abf849fb2e85a968b16d835471af8eab269c80144794239bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:bbb22d12833c98b8f2cced11e672c2d582633c96150a9c25f22a6d1449c27406
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.6 MB (529585408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b94de360c386e4634c7df247b98add8f999e3a97e9a78924b15105a6db795c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:46:25 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Apr 2022 12:46:25 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Apr 2022 12:46:25 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:47:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Apr 2022 12:47:52 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:47:55 GMT
RUN npm install -g rtlcss
# Wed, 20 Apr 2022 12:47:56 GMT
ENV ODOO_VERSION=14.0
# Wed, 20 Apr 2022 12:47:56 GMT
ARG ODOO_RELEASE=20220401
# Wed, 20 Apr 2022 12:47:56 GMT
ARG ODOO_SHA=43eabf4f6f55cd2887dc123d955bfaf9c7f27a32
# Wed, 20 Apr 2022 12:49:20 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=43eabf4f6f55cd2887dc123d955bfaf9c7f27a32
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Apr 2022 12:49:24 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Apr 2022 12:49:24 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Apr 2022 12:49:25 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=43eabf4f6f55cd2887dc123d955bfaf9c7f27a32
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Apr 2022 12:49:25 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Apr 2022 12:49:25 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Apr 2022 12:49:25 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Apr 2022 12:49:25 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Apr 2022 12:49:25 GMT
USER odoo
# Wed, 20 Apr 2022 12:49:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 12:49:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef0b3a5b3ccf6bc33961621c8b4217adc5f5ef26d7b92c47c8c39a8820fd58b`  
		Last Modified: Wed, 20 Apr 2022 12:53:38 GMT  
		Size: 213.2 MB (213177837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b2adc658049f20fffa9059922d790f2cc75e2fc5db14b3c1b77043b486b694`  
		Last Modified: Wed, 20 Apr 2022 12:53:16 GMT  
		Size: 13.4 MB (13440548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dafa09d0f12a0ed57ad93fe02efadcc57e517a8c1b2abf6d42c04e6b5031e65`  
		Last Modified: Wed, 20 Apr 2022 12:53:13 GMT  
		Size: 458.5 KB (458493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a3d801afb388ea73dfdcf1c98c4436eb0d013a20fe6e61e0d7a9acc5ce9a1a`  
		Last Modified: Wed, 20 Apr 2022 12:53:45 GMT  
		Size: 275.4 MB (275365415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b2ee8fe90a106f96a5f077118d24536f66e018e9446859e7185530b12180e`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5df638d02c88f9f1e5c6c15b591ad6404172d7cb9b3e1f1680f3f513ae005b2`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b7e5f969acb4c0d5dd7da1fc6683dd4500b2b9d52e08a9473aab7d1dd344cc`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebc2102fa546e7ff4adaf76bf6e0b1624fc5762fdd0f276350ace33eecae970`  
		Last Modified: Wed, 20 Apr 2022 12:53:11 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:73759bde823f5e1fdd042d62d75e76a62bfe5abe747c950ff0b317a63daa0619
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:3d8261f3c392aebc8a65c45f4b4efc957b8b0079a6c5a5201c5a3c23c7e2d4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.7 MB (551696432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8977b105a4b8d99ed6f907dcaf23030471c0670412fc30d2f7afc3ffc227f4a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:43:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Apr 2022 12:43:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Apr 2022 12:43:32 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:44:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Apr 2022 12:44:50 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:44:52 GMT
RUN npm install -g rtlcss
# Wed, 20 Apr 2022 12:44:52 GMT
ENV ODOO_VERSION=15.0
# Wed, 20 Apr 2022 12:44:52 GMT
ARG ODOO_RELEASE=20220401
# Wed, 20 Apr 2022 12:44:52 GMT
ARG ODOO_SHA=47f9d71dcfd0c0884969b361bc1bbe5f45fb3ac5
# Wed, 20 Apr 2022 12:46:12 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=47f9d71dcfd0c0884969b361bc1bbe5f45fb3ac5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Apr 2022 12:46:16 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Apr 2022 12:46:16 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Apr 2022 12:46:17 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=47f9d71dcfd0c0884969b361bc1bbe5f45fb3ac5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Apr 2022 12:46:17 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Apr 2022 12:46:17 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Apr 2022 12:46:17 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Apr 2022 12:46:17 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Apr 2022 12:46:17 GMT
USER odoo
# Wed, 20 Apr 2022 12:46:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 12:46:18 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f1aac8f860c1d54f3f94ccc883be166c671639bb052e7754baf4d6032ab4b3`  
		Last Modified: Wed, 20 Apr 2022 12:52:49 GMT  
		Size: 220.3 MB (220300936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875665d357afcc2f5c5593ae40db6baed8f4446ec9b8dca77d5605a49495e0cb`  
		Last Modified: Wed, 20 Apr 2022 12:52:24 GMT  
		Size: 2.5 MB (2510123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9a5928702128a35bd3b53d8a01c591d7884eda973ecebcd3d765abeab07b8`  
		Last Modified: Wed, 20 Apr 2022 12:52:23 GMT  
		Size: 451.8 KB (451820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb3fb341bc0dc23f22449fbbd657ddb79635e399a5e9fe05e6a79708772ee92`  
		Last Modified: Wed, 20 Apr 2022 12:52:56 GMT  
		Size: 297.1 MB (297052117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2389a4ad84d803871e474e3f974682ff21bdd23416ecab02b28e54803b4e82eb`  
		Last Modified: Wed, 20 Apr 2022 12:52:20 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b592d61cebaaddbadbce31a024a8de6156e89f35e7b89e564f387830c85e1c`  
		Last Modified: Wed, 20 Apr 2022 12:52:20 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5a751db86f15b085b7ed04a6c7ce64a4df6d9beffbcec1b95ca93b72e3cb39`  
		Last Modified: Wed, 20 Apr 2022 12:52:21 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79bcab42c989bc38ec6895428158cc1bed467c1c906fb41eb1c5ce8d54d8286`  
		Last Modified: Wed, 20 Apr 2022 12:52:20 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:73759bde823f5e1fdd042d62d75e76a62bfe5abe747c950ff0b317a63daa0619
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:3d8261f3c392aebc8a65c45f4b4efc957b8b0079a6c5a5201c5a3c23c7e2d4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.7 MB (551696432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8977b105a4b8d99ed6f907dcaf23030471c0670412fc30d2f7afc3ffc227f4a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:43:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Apr 2022 12:43:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Apr 2022 12:43:32 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:44:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Apr 2022 12:44:50 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:44:52 GMT
RUN npm install -g rtlcss
# Wed, 20 Apr 2022 12:44:52 GMT
ENV ODOO_VERSION=15.0
# Wed, 20 Apr 2022 12:44:52 GMT
ARG ODOO_RELEASE=20220401
# Wed, 20 Apr 2022 12:44:52 GMT
ARG ODOO_SHA=47f9d71dcfd0c0884969b361bc1bbe5f45fb3ac5
# Wed, 20 Apr 2022 12:46:12 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=47f9d71dcfd0c0884969b361bc1bbe5f45fb3ac5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Apr 2022 12:46:16 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Apr 2022 12:46:16 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Apr 2022 12:46:17 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=47f9d71dcfd0c0884969b361bc1bbe5f45fb3ac5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Apr 2022 12:46:17 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Apr 2022 12:46:17 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Apr 2022 12:46:17 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Apr 2022 12:46:17 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Apr 2022 12:46:17 GMT
USER odoo
# Wed, 20 Apr 2022 12:46:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 12:46:18 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f1aac8f860c1d54f3f94ccc883be166c671639bb052e7754baf4d6032ab4b3`  
		Last Modified: Wed, 20 Apr 2022 12:52:49 GMT  
		Size: 220.3 MB (220300936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875665d357afcc2f5c5593ae40db6baed8f4446ec9b8dca77d5605a49495e0cb`  
		Last Modified: Wed, 20 Apr 2022 12:52:24 GMT  
		Size: 2.5 MB (2510123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9a5928702128a35bd3b53d8a01c591d7884eda973ecebcd3d765abeab07b8`  
		Last Modified: Wed, 20 Apr 2022 12:52:23 GMT  
		Size: 451.8 KB (451820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb3fb341bc0dc23f22449fbbd657ddb79635e399a5e9fe05e6a79708772ee92`  
		Last Modified: Wed, 20 Apr 2022 12:52:56 GMT  
		Size: 297.1 MB (297052117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2389a4ad84d803871e474e3f974682ff21bdd23416ecab02b28e54803b4e82eb`  
		Last Modified: Wed, 20 Apr 2022 12:52:20 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b592d61cebaaddbadbce31a024a8de6156e89f35e7b89e564f387830c85e1c`  
		Last Modified: Wed, 20 Apr 2022 12:52:20 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5a751db86f15b085b7ed04a6c7ce64a4df6d9beffbcec1b95ca93b72e3cb39`  
		Last Modified: Wed, 20 Apr 2022 12:52:21 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79bcab42c989bc38ec6895428158cc1bed467c1c906fb41eb1c5ce8d54d8286`  
		Last Modified: Wed, 20 Apr 2022 12:52:20 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:73759bde823f5e1fdd042d62d75e76a62bfe5abe747c950ff0b317a63daa0619
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:3d8261f3c392aebc8a65c45f4b4efc957b8b0079a6c5a5201c5a3c23c7e2d4fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.7 MB (551696432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8977b105a4b8d99ed6f907dcaf23030471c0670412fc30d2f7afc3ffc227f4a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:43:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Apr 2022 12:43:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Apr 2022 12:43:32 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 12:44:40 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Apr 2022 12:44:50 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:44:52 GMT
RUN npm install -g rtlcss
# Wed, 20 Apr 2022 12:44:52 GMT
ENV ODOO_VERSION=15.0
# Wed, 20 Apr 2022 12:44:52 GMT
ARG ODOO_RELEASE=20220401
# Wed, 20 Apr 2022 12:44:52 GMT
ARG ODOO_SHA=47f9d71dcfd0c0884969b361bc1bbe5f45fb3ac5
# Wed, 20 Apr 2022 12:46:12 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=47f9d71dcfd0c0884969b361bc1bbe5f45fb3ac5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Apr 2022 12:46:16 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Apr 2022 12:46:16 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Apr 2022 12:46:17 GMT
# ARGS: ODOO_RELEASE=20220401 ODOO_SHA=47f9d71dcfd0c0884969b361bc1bbe5f45fb3ac5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Apr 2022 12:46:17 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Apr 2022 12:46:17 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Apr 2022 12:46:17 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Apr 2022 12:46:17 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Apr 2022 12:46:17 GMT
USER odoo
# Wed, 20 Apr 2022 12:46:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Apr 2022 12:46:18 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f1aac8f860c1d54f3f94ccc883be166c671639bb052e7754baf4d6032ab4b3`  
		Last Modified: Wed, 20 Apr 2022 12:52:49 GMT  
		Size: 220.3 MB (220300936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875665d357afcc2f5c5593ae40db6baed8f4446ec9b8dca77d5605a49495e0cb`  
		Last Modified: Wed, 20 Apr 2022 12:52:24 GMT  
		Size: 2.5 MB (2510123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9a5928702128a35bd3b53d8a01c591d7884eda973ecebcd3d765abeab07b8`  
		Last Modified: Wed, 20 Apr 2022 12:52:23 GMT  
		Size: 451.8 KB (451820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb3fb341bc0dc23f22449fbbd657ddb79635e399a5e9fe05e6a79708772ee92`  
		Last Modified: Wed, 20 Apr 2022 12:52:56 GMT  
		Size: 297.1 MB (297052117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2389a4ad84d803871e474e3f974682ff21bdd23416ecab02b28e54803b4e82eb`  
		Last Modified: Wed, 20 Apr 2022 12:52:20 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b592d61cebaaddbadbce31a024a8de6156e89f35e7b89e564f387830c85e1c`  
		Last Modified: Wed, 20 Apr 2022 12:52:20 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5a751db86f15b085b7ed04a6c7ce64a4df6d9beffbcec1b95ca93b72e3cb39`  
		Last Modified: Wed, 20 Apr 2022 12:52:21 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79bcab42c989bc38ec6895428158cc1bed467c1c906fb41eb1c5ce8d54d8286`  
		Last Modified: Wed, 20 Apr 2022 12:52:20 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
