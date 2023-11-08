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
$ docker pull odoo@sha256:e94c0b591de2e07d09164b750372ec223a7c57402e937f7adb0197b3b37eaebd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:17655905194de67d7ee52f5ade0e71505fc36683d88891c2836e8b25a2a258ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533313457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13641e055fc94151b855f2ed3e833316090545eb3e5817fcda26cb13f8a20ce8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 12:05:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Nov 2023 12:05:29 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Nov 2023 12:05:29 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 12:06:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Nov 2023 12:06:57 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 12:06:59 GMT
RUN npm install -g rtlcss
# Wed, 01 Nov 2023 12:07:00 GMT
ENV ODOO_VERSION=14.0
# Wed, 01 Nov 2023 12:07:00 GMT
ARG ODOO_RELEASE=20230925
# Wed, 01 Nov 2023 12:07:00 GMT
ARG ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
# Wed, 01 Nov 2023 12:08:12 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 01 Nov 2023 12:08:16 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 01 Nov 2023 12:08:16 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 01 Nov 2023 12:08:16 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 01 Nov 2023 12:08:16 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 01 Nov 2023 12:08:17 GMT
EXPOSE 8069 8071 8072
# Wed, 01 Nov 2023 12:08:17 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 01 Nov 2023 12:08:17 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 01 Nov 2023 12:08:17 GMT
USER odoo
# Wed, 01 Nov 2023 12:08:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 12:08:17 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd6f2282b1528e9d19460586cc68e865fa113c5ff1cee997d8372cb2b6b45ca`  
		Last Modified: Wed, 01 Nov 2023 12:10:27 GMT  
		Size: 213.2 MB (213188996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9cd6f7f6861851c66bd7a47e0676762a3c7c0ae1a878bbfdb3a170a606af3`  
		Last Modified: Wed, 01 Nov 2023 12:10:06 GMT  
		Size: 13.6 MB (13567547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764a49934ac4fe6676c13cd02961d560d2e536a4a119b84c928597a50463e30f`  
		Last Modified: Wed, 01 Nov 2023 12:10:05 GMT  
		Size: 462.2 KB (462244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7731caac676ae8854a21c713a0baf7470ac21137ff9b6d38812584d9c25f7f97`  
		Last Modified: Wed, 01 Nov 2023 12:10:33 GMT  
		Size: 278.9 MB (278904792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ce56eb8830b6b1cc0cac5d5b8daa5a88b13e596cd9b37c9d082f340a439711`  
		Last Modified: Wed, 01 Nov 2023 12:10:01 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6485e8a937cc7fee3469f3047251627888ea033567d63f1f9286beda268f00`  
		Last Modified: Wed, 01 Nov 2023 12:10:01 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3798ecdf27e46fa3f909f28c4fd195cab4dbcca02e480823d7e35e2d3be7a7`  
		Last Modified: Wed, 01 Nov 2023 12:10:01 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4b191f59e8e7e7e10e9d4c76ceb7f734763a6d6f99d4dd984aef64916d5dd`  
		Last Modified: Wed, 01 Nov 2023 12:10:01 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:e94c0b591de2e07d09164b750372ec223a7c57402e937f7adb0197b3b37eaebd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:17655905194de67d7ee52f5ade0e71505fc36683d88891c2836e8b25a2a258ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533313457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13641e055fc94151b855f2ed3e833316090545eb3e5817fcda26cb13f8a20ce8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 12:05:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Nov 2023 12:05:29 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Nov 2023 12:05:29 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 12:06:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Nov 2023 12:06:57 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 12:06:59 GMT
RUN npm install -g rtlcss
# Wed, 01 Nov 2023 12:07:00 GMT
ENV ODOO_VERSION=14.0
# Wed, 01 Nov 2023 12:07:00 GMT
ARG ODOO_RELEASE=20230925
# Wed, 01 Nov 2023 12:07:00 GMT
ARG ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
# Wed, 01 Nov 2023 12:08:12 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 01 Nov 2023 12:08:16 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 01 Nov 2023 12:08:16 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 01 Nov 2023 12:08:16 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 01 Nov 2023 12:08:16 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 01 Nov 2023 12:08:17 GMT
EXPOSE 8069 8071 8072
# Wed, 01 Nov 2023 12:08:17 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 01 Nov 2023 12:08:17 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 01 Nov 2023 12:08:17 GMT
USER odoo
# Wed, 01 Nov 2023 12:08:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 12:08:17 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd6f2282b1528e9d19460586cc68e865fa113c5ff1cee997d8372cb2b6b45ca`  
		Last Modified: Wed, 01 Nov 2023 12:10:27 GMT  
		Size: 213.2 MB (213188996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9cd6f7f6861851c66bd7a47e0676762a3c7c0ae1a878bbfdb3a170a606af3`  
		Last Modified: Wed, 01 Nov 2023 12:10:06 GMT  
		Size: 13.6 MB (13567547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764a49934ac4fe6676c13cd02961d560d2e536a4a119b84c928597a50463e30f`  
		Last Modified: Wed, 01 Nov 2023 12:10:05 GMT  
		Size: 462.2 KB (462244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7731caac676ae8854a21c713a0baf7470ac21137ff9b6d38812584d9c25f7f97`  
		Last Modified: Wed, 01 Nov 2023 12:10:33 GMT  
		Size: 278.9 MB (278904792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ce56eb8830b6b1cc0cac5d5b8daa5a88b13e596cd9b37c9d082f340a439711`  
		Last Modified: Wed, 01 Nov 2023 12:10:01 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6485e8a937cc7fee3469f3047251627888ea033567d63f1f9286beda268f00`  
		Last Modified: Wed, 01 Nov 2023 12:10:01 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3798ecdf27e46fa3f909f28c4fd195cab4dbcca02e480823d7e35e2d3be7a7`  
		Last Modified: Wed, 01 Nov 2023 12:10:01 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4b191f59e8e7e7e10e9d4c76ceb7f734763a6d6f99d4dd984aef64916d5dd`  
		Last Modified: Wed, 01 Nov 2023 12:10:01 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:6d79e2c97383fe610d28ce81c66294f8acf5bc0f8ec0c60396dab0eb4f55ff5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:5914c7794e2b287d274c65b25a96bdebf396b591e436b15958bd7f6bd29905b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.5 MB (562475380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a4db52d5a016704c90ea5d02e37339b9c27975d2f4df42206a6430aadd24b0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 11:59:56 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Nov 2023 11:59:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Nov 2023 11:59:56 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 12:03:56 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Nov 2023 12:04:02 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 12:04:04 GMT
RUN npm install -g rtlcss
# Wed, 01 Nov 2023 12:04:04 GMT
ENV ODOO_VERSION=15.0
# Wed, 01 Nov 2023 12:04:04 GMT
ARG ODOO_RELEASE=20230925
# Wed, 01 Nov 2023 12:04:04 GMT
ARG ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
# Wed, 01 Nov 2023 12:05:13 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 01 Nov 2023 12:05:18 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 01 Nov 2023 12:05:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 01 Nov 2023 12:05:18 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 01 Nov 2023 12:05:18 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 01 Nov 2023 12:05:18 GMT
EXPOSE 8069 8071 8072
# Wed, 01 Nov 2023 12:05:18 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 01 Nov 2023 12:05:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 01 Nov 2023 12:05:19 GMT
USER odoo
# Wed, 01 Nov 2023 12:05:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 12:05:19 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae4769061fca067a25d337753a857c225301a3391d70dc9c355ec401a1666f9`  
		Last Modified: Wed, 01 Nov 2023 12:09:44 GMT  
		Size: 220.3 MB (220298628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f037b076bdf88bd13eb93037e412a84af9179318c033537325a2abb0e21f3437`  
		Last Modified: Wed, 01 Nov 2023 12:09:20 GMT  
		Size: 2.6 MB (2624848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09c8bae1e450f33859e0454685d8e83ce199230cdf0487f7b3bca45bccd8a66`  
		Last Modified: Wed, 01 Nov 2023 12:09:20 GMT  
		Size: 457.9 KB (457875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadeb02c722625f8938cdd3226da78a5e65f03b88e67ef6a48baf10890ef6a8a`  
		Last Modified: Wed, 01 Nov 2023 12:09:52 GMT  
		Size: 307.7 MB (307673653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836783f7494ee06aeda6556c0e8d9221dc818f2ff37709a2179015c651e65ed`  
		Last Modified: Wed, 01 Nov 2023 12:09:18 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dbb62fd009c14dc3a96a874071ae596e6f131bfaaa4a3fd4dee506ba6ad99`  
		Last Modified: Wed, 01 Nov 2023 12:09:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4f465d2dd5c17cb04650850524eeedf7a4642aa0351429199ef7fffdda9f72`  
		Last Modified: Wed, 01 Nov 2023 12:09:18 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d3d0eab7e25d65587082ac90586132af3418b08ea526095c9cdb0d2e2854c7`  
		Last Modified: Wed, 01 Nov 2023 12:09:18 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:6d79e2c97383fe610d28ce81c66294f8acf5bc0f8ec0c60396dab0eb4f55ff5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:5914c7794e2b287d274c65b25a96bdebf396b591e436b15958bd7f6bd29905b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.5 MB (562475380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a4db52d5a016704c90ea5d02e37339b9c27975d2f4df42206a6430aadd24b0a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 11:59:56 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Nov 2023 11:59:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Nov 2023 11:59:56 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 12:03:56 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Nov 2023 12:04:02 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 12:04:04 GMT
RUN npm install -g rtlcss
# Wed, 01 Nov 2023 12:04:04 GMT
ENV ODOO_VERSION=15.0
# Wed, 01 Nov 2023 12:04:04 GMT
ARG ODOO_RELEASE=20230925
# Wed, 01 Nov 2023 12:04:04 GMT
ARG ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
# Wed, 01 Nov 2023 12:05:13 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 01 Nov 2023 12:05:18 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 01 Nov 2023 12:05:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 01 Nov 2023 12:05:18 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 01 Nov 2023 12:05:18 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 01 Nov 2023 12:05:18 GMT
EXPOSE 8069 8071 8072
# Wed, 01 Nov 2023 12:05:18 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 01 Nov 2023 12:05:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 01 Nov 2023 12:05:19 GMT
USER odoo
# Wed, 01 Nov 2023 12:05:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 12:05:19 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae4769061fca067a25d337753a857c225301a3391d70dc9c355ec401a1666f9`  
		Last Modified: Wed, 01 Nov 2023 12:09:44 GMT  
		Size: 220.3 MB (220298628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f037b076bdf88bd13eb93037e412a84af9179318c033537325a2abb0e21f3437`  
		Last Modified: Wed, 01 Nov 2023 12:09:20 GMT  
		Size: 2.6 MB (2624848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09c8bae1e450f33859e0454685d8e83ce199230cdf0487f7b3bca45bccd8a66`  
		Last Modified: Wed, 01 Nov 2023 12:09:20 GMT  
		Size: 457.9 KB (457875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadeb02c722625f8938cdd3226da78a5e65f03b88e67ef6a48baf10890ef6a8a`  
		Last Modified: Wed, 01 Nov 2023 12:09:52 GMT  
		Size: 307.7 MB (307673653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e836783f7494ee06aeda6556c0e8d9221dc818f2ff37709a2179015c651e65ed`  
		Last Modified: Wed, 01 Nov 2023 12:09:18 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dbb62fd009c14dc3a96a874071ae596e6f131bfaaa4a3fd4dee506ba6ad99`  
		Last Modified: Wed, 01 Nov 2023 12:09:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4f465d2dd5c17cb04650850524eeedf7a4642aa0351429199ef7fffdda9f72`  
		Last Modified: Wed, 01 Nov 2023 12:09:18 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d3d0eab7e25d65587082ac90586132af3418b08ea526095c9cdb0d2e2854c7`  
		Last Modified: Wed, 01 Nov 2023 12:09:18 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:bd63911f1819f24b3b9ea5b11002f30e5560cc12519c41cdbfc7b5781d451bfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:5865fb20279fea1e44bb3539bd7fca37970ad22cdd520401973c4ddec1af470c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.8 MB (576802332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6566b405046872be3fdc6deb1c554ab0a4b10c21415953356d8e3c455d70f71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 11:59:56 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Nov 2023 11:59:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Nov 2023 11:59:56 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 12:01:06 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Nov 2023 12:01:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 12:01:18 GMT
RUN npm install -g rtlcss
# Wed, 01 Nov 2023 12:01:18 GMT
ENV ODOO_VERSION=16.0
# Wed, 01 Nov 2023 12:01:18 GMT
ARG ODOO_RELEASE=20230925
# Wed, 01 Nov 2023 12:01:18 GMT
ARG ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
# Wed, 01 Nov 2023 12:02:43 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 01 Nov 2023 12:02:46 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 01 Nov 2023 12:02:46 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 01 Nov 2023 12:02:47 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 01 Nov 2023 12:02:47 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 01 Nov 2023 12:02:47 GMT
EXPOSE 8069 8071 8072
# Wed, 01 Nov 2023 12:02:47 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 01 Nov 2023 12:02:47 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 01 Nov 2023 12:02:47 GMT
USER odoo
# Wed, 01 Nov 2023 12:02:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 12:02:48 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b776214855ac38a27d7439aa4917671493c6da45ebfca393acf978c6ef7e3315`  
		Last Modified: Wed, 01 Nov 2023 12:08:55 GMT  
		Size: 221.0 MB (220990382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d33471fdaa7ac2a6ef985ab7601d9eb66512db62c63858eca047cdb0eb07039`  
		Last Modified: Wed, 01 Nov 2023 12:08:32 GMT  
		Size: 2.6 MB (2628090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2362017507d95df530e38a737eab9f281058ba57e46068e0614ae884b6df0f`  
		Last Modified: Wed, 01 Nov 2023 12:08:31 GMT  
		Size: 457.9 KB (457911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380c6382db69193728b2c0ca2ef3d3c0a95fa9d0bb1fa3fa1431cb89d3f5b394`  
		Last Modified: Wed, 01 Nov 2023 12:09:06 GMT  
		Size: 321.3 MB (321305564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3f5299e7c95478133a079523c19f07ca84dc02e25d7a221a6a2685fd639b4c`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef93d32506d5bbd9f4667c59bcf133fd0da03d9f7f7af09aa848424527eb8b62`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5022648e2bb5bb382e428a9e06e60d60b4e1064c6f5b205b2b7492d3ac3ce5`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7442bfdbfef0d55dfc5515cf2369a41544fbd9c079ad181cd60864ba51560c7f`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:8f6eedc129b5b3fcb29f2cd2b1a9ad32c524929b493c9d2adc2a8a87e2aa7651
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.8 MB (572758883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c1566cee291601a50b7b337b36cde5aae59862c8f99c9feddbb63fda1144c08`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Tue, 07 Nov 2023 23:48:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 07 Nov 2023 23:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 07 Nov 2023 23:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 07 Nov 2023 23:48:30 GMT
ARG TARGETARCH
# Tue, 07 Nov 2023 23:49:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 07 Nov 2023 23:49:46 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Nov 2023 23:49:48 GMT
RUN npm install -g rtlcss
# Tue, 07 Nov 2023 23:49:48 GMT
ENV ODOO_VERSION=16.0
# Tue, 07 Nov 2023 23:49:48 GMT
ARG ODOO_RELEASE=20231106
# Tue, 07 Nov 2023 23:49:48 GMT
ARG ODOO_SHA=ef0fa4f34bbb1af69733a8df1a19d2756de7916b
# Tue, 07 Nov 2023 23:51:03 GMT
# ARGS: ODOO_RELEASE=20231106 ODOO_SHA=ef0fa4f34bbb1af69733a8df1a19d2756de7916b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 07 Nov 2023 23:51:11 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 07 Nov 2023 23:51:11 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 07 Nov 2023 23:51:12 GMT
# ARGS: ODOO_RELEASE=20231106 ODOO_SHA=ef0fa4f34bbb1af69733a8df1a19d2756de7916b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 07 Nov 2023 23:51:12 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 07 Nov 2023 23:51:12 GMT
EXPOSE 8069 8071 8072
# Tue, 07 Nov 2023 23:51:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 07 Nov 2023 23:51:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 07 Nov 2023 23:51:12 GMT
USER odoo
# Tue, 07 Nov 2023 23:51:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Nov 2023 23:51:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5812a002d612ea362d56834609da19cbf53fb331e9f92b0b4b8d1cdd3b8aa9`  
		Last Modified: Tue, 07 Nov 2023 23:51:50 GMT  
		Size: 216.9 MB (216907690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59eaf6b2e981344b7a4bf54a869a293a9e69d429da23202eed603c8f1f41835`  
		Last Modified: Tue, 07 Nov 2023 23:51:32 GMT  
		Size: 2.6 MB (2634000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd2aeeb4414cf9678f9200a368d1873d1290880b10ec32b5a9264ae836d479b`  
		Last Modified: Tue, 07 Nov 2023 23:51:32 GMT  
		Size: 459.4 KB (459450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6432fc1af8295bd2885e33af1ed29b63dfedfa95bd638318ef031a3149020f65`  
		Last Modified: Tue, 07 Nov 2023 23:51:59 GMT  
		Size: 322.7 MB (322691375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe67fd3464d0eb156b296d671af3c33c269b79421cb53e285946720fad365f1`  
		Last Modified: Tue, 07 Nov 2023 23:51:30 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c1da646860f489d84029b167a63ae78951477fea9b760f6395a78ccfa8e22a`  
		Last Modified: Tue, 07 Nov 2023 23:51:29 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139c616c540ed904f9dd0938081c0e5b3b571369f2a5135756a0e732d7bffc1d`  
		Last Modified: Tue, 07 Nov 2023 23:51:30 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753c5cd5597c8c95c1b91ff13d8463e6804519c8a55179b0e6dd2af3b75fa7a2`  
		Last Modified: Tue, 07 Nov 2023 23:51:30 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:bd63911f1819f24b3b9ea5b11002f30e5560cc12519c41cdbfc7b5781d451bfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:5865fb20279fea1e44bb3539bd7fca37970ad22cdd520401973c4ddec1af470c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.8 MB (576802332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6566b405046872be3fdc6deb1c554ab0a4b10c21415953356d8e3c455d70f71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 11:59:56 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Nov 2023 11:59:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Nov 2023 11:59:56 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 12:01:06 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Nov 2023 12:01:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 12:01:18 GMT
RUN npm install -g rtlcss
# Wed, 01 Nov 2023 12:01:18 GMT
ENV ODOO_VERSION=16.0
# Wed, 01 Nov 2023 12:01:18 GMT
ARG ODOO_RELEASE=20230925
# Wed, 01 Nov 2023 12:01:18 GMT
ARG ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
# Wed, 01 Nov 2023 12:02:43 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 01 Nov 2023 12:02:46 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 01 Nov 2023 12:02:46 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 01 Nov 2023 12:02:47 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 01 Nov 2023 12:02:47 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 01 Nov 2023 12:02:47 GMT
EXPOSE 8069 8071 8072
# Wed, 01 Nov 2023 12:02:47 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 01 Nov 2023 12:02:47 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 01 Nov 2023 12:02:47 GMT
USER odoo
# Wed, 01 Nov 2023 12:02:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 12:02:48 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b776214855ac38a27d7439aa4917671493c6da45ebfca393acf978c6ef7e3315`  
		Last Modified: Wed, 01 Nov 2023 12:08:55 GMT  
		Size: 221.0 MB (220990382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d33471fdaa7ac2a6ef985ab7601d9eb66512db62c63858eca047cdb0eb07039`  
		Last Modified: Wed, 01 Nov 2023 12:08:32 GMT  
		Size: 2.6 MB (2628090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2362017507d95df530e38a737eab9f281058ba57e46068e0614ae884b6df0f`  
		Last Modified: Wed, 01 Nov 2023 12:08:31 GMT  
		Size: 457.9 KB (457911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380c6382db69193728b2c0ca2ef3d3c0a95fa9d0bb1fa3fa1431cb89d3f5b394`  
		Last Modified: Wed, 01 Nov 2023 12:09:06 GMT  
		Size: 321.3 MB (321305564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3f5299e7c95478133a079523c19f07ca84dc02e25d7a221a6a2685fd639b4c`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef93d32506d5bbd9f4667c59bcf133fd0da03d9f7f7af09aa848424527eb8b62`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5022648e2bb5bb382e428a9e06e60d60b4e1064c6f5b205b2b7492d3ac3ce5`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7442bfdbfef0d55dfc5515cf2369a41544fbd9c079ad181cd60864ba51560c7f`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:16.0` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:8f6eedc129b5b3fcb29f2cd2b1a9ad32c524929b493c9d2adc2a8a87e2aa7651
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.8 MB (572758883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c1566cee291601a50b7b337b36cde5aae59862c8f99c9feddbb63fda1144c08`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Tue, 07 Nov 2023 23:48:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 07 Nov 2023 23:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 07 Nov 2023 23:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 07 Nov 2023 23:48:30 GMT
ARG TARGETARCH
# Tue, 07 Nov 2023 23:49:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 07 Nov 2023 23:49:46 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Nov 2023 23:49:48 GMT
RUN npm install -g rtlcss
# Tue, 07 Nov 2023 23:49:48 GMT
ENV ODOO_VERSION=16.0
# Tue, 07 Nov 2023 23:49:48 GMT
ARG ODOO_RELEASE=20231106
# Tue, 07 Nov 2023 23:49:48 GMT
ARG ODOO_SHA=ef0fa4f34bbb1af69733a8df1a19d2756de7916b
# Tue, 07 Nov 2023 23:51:03 GMT
# ARGS: ODOO_RELEASE=20231106 ODOO_SHA=ef0fa4f34bbb1af69733a8df1a19d2756de7916b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 07 Nov 2023 23:51:11 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 07 Nov 2023 23:51:11 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 07 Nov 2023 23:51:12 GMT
# ARGS: ODOO_RELEASE=20231106 ODOO_SHA=ef0fa4f34bbb1af69733a8df1a19d2756de7916b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 07 Nov 2023 23:51:12 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 07 Nov 2023 23:51:12 GMT
EXPOSE 8069 8071 8072
# Tue, 07 Nov 2023 23:51:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 07 Nov 2023 23:51:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 07 Nov 2023 23:51:12 GMT
USER odoo
# Tue, 07 Nov 2023 23:51:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Nov 2023 23:51:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5812a002d612ea362d56834609da19cbf53fb331e9f92b0b4b8d1cdd3b8aa9`  
		Last Modified: Tue, 07 Nov 2023 23:51:50 GMT  
		Size: 216.9 MB (216907690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59eaf6b2e981344b7a4bf54a869a293a9e69d429da23202eed603c8f1f41835`  
		Last Modified: Tue, 07 Nov 2023 23:51:32 GMT  
		Size: 2.6 MB (2634000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd2aeeb4414cf9678f9200a368d1873d1290880b10ec32b5a9264ae836d479b`  
		Last Modified: Tue, 07 Nov 2023 23:51:32 GMT  
		Size: 459.4 KB (459450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6432fc1af8295bd2885e33af1ed29b63dfedfa95bd638318ef031a3149020f65`  
		Last Modified: Tue, 07 Nov 2023 23:51:59 GMT  
		Size: 322.7 MB (322691375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe67fd3464d0eb156b296d671af3c33c269b79421cb53e285946720fad365f1`  
		Last Modified: Tue, 07 Nov 2023 23:51:30 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c1da646860f489d84029b167a63ae78951477fea9b760f6395a78ccfa8e22a`  
		Last Modified: Tue, 07 Nov 2023 23:51:29 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139c616c540ed904f9dd0938081c0e5b3b571369f2a5135756a0e732d7bffc1d`  
		Last Modified: Tue, 07 Nov 2023 23:51:30 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753c5cd5597c8c95c1b91ff13d8463e6804519c8a55179b0e6dd2af3b75fa7a2`  
		Last Modified: Tue, 07 Nov 2023 23:51:30 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:bd63911f1819f24b3b9ea5b11002f30e5560cc12519c41cdbfc7b5781d451bfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:5865fb20279fea1e44bb3539bd7fca37970ad22cdd520401973c4ddec1af470c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.8 MB (576802332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6566b405046872be3fdc6deb1c554ab0a4b10c21415953356d8e3c455d70f71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 11:59:56 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Nov 2023 11:59:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Nov 2023 11:59:56 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 12:01:06 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Nov 2023 12:01:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 12:01:18 GMT
RUN npm install -g rtlcss
# Wed, 01 Nov 2023 12:01:18 GMT
ENV ODOO_VERSION=16.0
# Wed, 01 Nov 2023 12:01:18 GMT
ARG ODOO_RELEASE=20230925
# Wed, 01 Nov 2023 12:01:18 GMT
ARG ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
# Wed, 01 Nov 2023 12:02:43 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 01 Nov 2023 12:02:46 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 01 Nov 2023 12:02:46 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 01 Nov 2023 12:02:47 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 01 Nov 2023 12:02:47 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 01 Nov 2023 12:02:47 GMT
EXPOSE 8069 8071 8072
# Wed, 01 Nov 2023 12:02:47 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 01 Nov 2023 12:02:47 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 01 Nov 2023 12:02:47 GMT
USER odoo
# Wed, 01 Nov 2023 12:02:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Nov 2023 12:02:48 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b776214855ac38a27d7439aa4917671493c6da45ebfca393acf978c6ef7e3315`  
		Last Modified: Wed, 01 Nov 2023 12:08:55 GMT  
		Size: 221.0 MB (220990382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d33471fdaa7ac2a6ef985ab7601d9eb66512db62c63858eca047cdb0eb07039`  
		Last Modified: Wed, 01 Nov 2023 12:08:32 GMT  
		Size: 2.6 MB (2628090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2362017507d95df530e38a737eab9f281058ba57e46068e0614ae884b6df0f`  
		Last Modified: Wed, 01 Nov 2023 12:08:31 GMT  
		Size: 457.9 KB (457911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380c6382db69193728b2c0ca2ef3d3c0a95fa9d0bb1fa3fa1431cb89d3f5b394`  
		Last Modified: Wed, 01 Nov 2023 12:09:06 GMT  
		Size: 321.3 MB (321305564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3f5299e7c95478133a079523c19f07ca84dc02e25d7a221a6a2685fd639b4c`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef93d32506d5bbd9f4667c59bcf133fd0da03d9f7f7af09aa848424527eb8b62`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5022648e2bb5bb382e428a9e06e60d60b4e1064c6f5b205b2b7492d3ac3ce5`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7442bfdbfef0d55dfc5515cf2369a41544fbd9c079ad181cd60864ba51560c7f`  
		Last Modified: Wed, 01 Nov 2023 12:08:29 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:latest` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:8f6eedc129b5b3fcb29f2cd2b1a9ad32c524929b493c9d2adc2a8a87e2aa7651
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.8 MB (572758883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c1566cee291601a50b7b337b36cde5aae59862c8f99c9feddbb63fda1144c08`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Tue, 07 Nov 2023 23:48:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 07 Nov 2023 23:48:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 07 Nov 2023 23:48:30 GMT
ENV LANG=C.UTF-8
# Tue, 07 Nov 2023 23:48:30 GMT
ARG TARGETARCH
# Tue, 07 Nov 2023 23:49:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=9df8dd7b1e99782f1cfa19aca665969bbd9cc159  ;;     "arm64")  WKHTMLTOPDF_SHA=58c84db46b11ba0e14abb77a32324b1c257f1f22  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=7ed8f6dcedf5345a3dd4eeb58dc89704d862f9cd  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.bullseye_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 07 Nov 2023 23:49:46 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Nov 2023 23:49:48 GMT
RUN npm install -g rtlcss
# Tue, 07 Nov 2023 23:49:48 GMT
ENV ODOO_VERSION=16.0
# Tue, 07 Nov 2023 23:49:48 GMT
ARG ODOO_RELEASE=20231106
# Tue, 07 Nov 2023 23:49:48 GMT
ARG ODOO_SHA=ef0fa4f34bbb1af69733a8df1a19d2756de7916b
# Tue, 07 Nov 2023 23:51:03 GMT
# ARGS: ODOO_RELEASE=20231106 ODOO_SHA=ef0fa4f34bbb1af69733a8df1a19d2756de7916b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 07 Nov 2023 23:51:11 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 07 Nov 2023 23:51:11 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 07 Nov 2023 23:51:12 GMT
# ARGS: ODOO_RELEASE=20231106 ODOO_SHA=ef0fa4f34bbb1af69733a8df1a19d2756de7916b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 07 Nov 2023 23:51:12 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 07 Nov 2023 23:51:12 GMT
EXPOSE 8069 8071 8072
# Tue, 07 Nov 2023 23:51:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 07 Nov 2023 23:51:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 07 Nov 2023 23:51:12 GMT
USER odoo
# Tue, 07 Nov 2023 23:51:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 07 Nov 2023 23:51:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5812a002d612ea362d56834609da19cbf53fb331e9f92b0b4b8d1cdd3b8aa9`  
		Last Modified: Tue, 07 Nov 2023 23:51:50 GMT  
		Size: 216.9 MB (216907690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59eaf6b2e981344b7a4bf54a869a293a9e69d429da23202eed603c8f1f41835`  
		Last Modified: Tue, 07 Nov 2023 23:51:32 GMT  
		Size: 2.6 MB (2634000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd2aeeb4414cf9678f9200a368d1873d1290880b10ec32b5a9264ae836d479b`  
		Last Modified: Tue, 07 Nov 2023 23:51:32 GMT  
		Size: 459.4 KB (459450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6432fc1af8295bd2885e33af1ed29b63dfedfa95bd638318ef031a3149020f65`  
		Last Modified: Tue, 07 Nov 2023 23:51:59 GMT  
		Size: 322.7 MB (322691375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe67fd3464d0eb156b296d671af3c33c269b79421cb53e285946720fad365f1`  
		Last Modified: Tue, 07 Nov 2023 23:51:30 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c1da646860f489d84029b167a63ae78951477fea9b760f6395a78ccfa8e22a`  
		Last Modified: Tue, 07 Nov 2023 23:51:29 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139c616c540ed904f9dd0938081c0e5b3b571369f2a5135756a0e732d7bffc1d`  
		Last Modified: Tue, 07 Nov 2023 23:51:30 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753c5cd5597c8c95c1b91ff13d8463e6804519c8a55179b0e6dd2af3b75fa7a2`  
		Last Modified: Tue, 07 Nov 2023 23:51:30 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
