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
$ docker pull odoo@sha256:eaec4815e3ea1af9dfa2ba4e492c4c97fd9f513f7ed52dddf683a0e3dab7df5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:6977e211b5cf9913c11386517e09a02cd15ca0ed907d7c94585d8fa59e54af2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.0 MB (532028491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a57ac4169d3cfc4b5ec33f4d1a52dc279346b3103e2f494f57cf4b8f20901e30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 18:28:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Mar 2023 18:28:55 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Mar 2023 18:28:55 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 18:30:22 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Mar 2023 18:30:34 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 18:30:37 GMT
RUN npm install -g rtlcss
# Wed, 01 Mar 2023 18:30:37 GMT
ENV ODOO_VERSION=14.0
# Mon, 20 Mar 2023 22:47:26 GMT
ARG ODOO_RELEASE=20230317
# Mon, 20 Mar 2023 22:47:26 GMT
ARG ODOO_SHA=4b677e345f13d6421d78f6a3f3dce4ccf6bd2a99
# Mon, 20 Mar 2023 22:48:48 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=4b677e345f13d6421d78f6a3f3dce4ccf6bd2a99
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Mar 2023 22:48:52 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 20 Mar 2023 22:48:52 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Mar 2023 22:48:53 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=4b677e345f13d6421d78f6a3f3dce4ccf6bd2a99
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Mar 2023 22:48:53 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Mar 2023 22:48:53 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Mar 2023 22:48:53 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Mar 2023 22:48:53 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Mar 2023 22:48:53 GMT
USER odoo
# Mon, 20 Mar 2023 22:48:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Mar 2023 22:48:53 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098558a773310761d275e903e5c82ae82e62aeca797d7d0ef00b03572bacee38`  
		Last Modified: Wed, 01 Mar 2023 18:34:10 GMT  
		Size: 213.2 MB (213201748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41b0353de2b48785e5a3ca2e802fc194ffe1afca628efde22ee6692794f2b0f`  
		Last Modified: Wed, 01 Mar 2023 18:33:49 GMT  
		Size: 13.5 MB (13517762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5562db7956eed4ba9670c33d418977feff13172f8d3c302618dc6c4c8201c0`  
		Last Modified: Wed, 01 Mar 2023 18:33:46 GMT  
		Size: 456.4 KB (456438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a364d36c131accdc3862af151023b2f92bc10f55b5839e0083e402c4c41281ab`  
		Last Modified: Mon, 20 Mar 2023 22:51:16 GMT  
		Size: 277.7 MB (277710195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c3dd04334c56d1916e87db758a871c022c406060f34f6f869a82a07783bb5e`  
		Last Modified: Mon, 20 Mar 2023 22:50:45 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f08c81c0bcbd0981dc0acc0a42f36171b1c248f19fbd58a81ee50eb7bcbd5b`  
		Last Modified: Mon, 20 Mar 2023 22:50:45 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181871290e8283296f47366f385aef543a1762498bd6cc22a14df8a557127a09`  
		Last Modified: Mon, 20 Mar 2023 22:50:45 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e291e4c92765326c6f148b0cf36d7c5717bd164520b4e1e3e423eb9193ea9`  
		Last Modified: Mon, 20 Mar 2023 22:50:45 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:eaec4815e3ea1af9dfa2ba4e492c4c97fd9f513f7ed52dddf683a0e3dab7df5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:6977e211b5cf9913c11386517e09a02cd15ca0ed907d7c94585d8fa59e54af2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.0 MB (532028491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a57ac4169d3cfc4b5ec33f4d1a52dc279346b3103e2f494f57cf4b8f20901e30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 18:28:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Mar 2023 18:28:55 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Mar 2023 18:28:55 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 18:30:22 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Mar 2023 18:30:34 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 18:30:37 GMT
RUN npm install -g rtlcss
# Wed, 01 Mar 2023 18:30:37 GMT
ENV ODOO_VERSION=14.0
# Mon, 20 Mar 2023 22:47:26 GMT
ARG ODOO_RELEASE=20230317
# Mon, 20 Mar 2023 22:47:26 GMT
ARG ODOO_SHA=4b677e345f13d6421d78f6a3f3dce4ccf6bd2a99
# Mon, 20 Mar 2023 22:48:48 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=4b677e345f13d6421d78f6a3f3dce4ccf6bd2a99
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Mar 2023 22:48:52 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 20 Mar 2023 22:48:52 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Mar 2023 22:48:53 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=4b677e345f13d6421d78f6a3f3dce4ccf6bd2a99
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Mar 2023 22:48:53 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Mar 2023 22:48:53 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Mar 2023 22:48:53 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Mar 2023 22:48:53 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Mar 2023 22:48:53 GMT
USER odoo
# Mon, 20 Mar 2023 22:48:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Mar 2023 22:48:53 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098558a773310761d275e903e5c82ae82e62aeca797d7d0ef00b03572bacee38`  
		Last Modified: Wed, 01 Mar 2023 18:34:10 GMT  
		Size: 213.2 MB (213201748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41b0353de2b48785e5a3ca2e802fc194ffe1afca628efde22ee6692794f2b0f`  
		Last Modified: Wed, 01 Mar 2023 18:33:49 GMT  
		Size: 13.5 MB (13517762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5562db7956eed4ba9670c33d418977feff13172f8d3c302618dc6c4c8201c0`  
		Last Modified: Wed, 01 Mar 2023 18:33:46 GMT  
		Size: 456.4 KB (456438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a364d36c131accdc3862af151023b2f92bc10f55b5839e0083e402c4c41281ab`  
		Last Modified: Mon, 20 Mar 2023 22:51:16 GMT  
		Size: 277.7 MB (277710195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c3dd04334c56d1916e87db758a871c022c406060f34f6f869a82a07783bb5e`  
		Last Modified: Mon, 20 Mar 2023 22:50:45 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f08c81c0bcbd0981dc0acc0a42f36171b1c248f19fbd58a81ee50eb7bcbd5b`  
		Last Modified: Mon, 20 Mar 2023 22:50:45 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181871290e8283296f47366f385aef543a1762498bd6cc22a14df8a557127a09`  
		Last Modified: Mon, 20 Mar 2023 22:50:45 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e291e4c92765326c6f148b0cf36d7c5717bd164520b4e1e3e423eb9193ea9`  
		Last Modified: Mon, 20 Mar 2023 22:50:45 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:5ce2a1c0c137dcffb3f2b6be8b07f9e06779dbc72dde7a56b29110402a894900
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:b46e471cab7c73bfe334877b35909cdb8282e42aa49875f6bb1e613c72aab4c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **560.3 MB (560302384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6a2c196e7952f3657bec3f1e1a7456de7b659f3f04896d3bdf448d7963ffc57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 18:24:38 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Mar 2023 18:24:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Mar 2023 18:24:38 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 18:25:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Mar 2023 18:25:55 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 18:25:57 GMT
RUN npm install -g rtlcss
# Wed, 01 Mar 2023 18:27:31 GMT
ENV ODOO_VERSION=15.0
# Mon, 20 Mar 2023 22:46:03 GMT
ARG ODOO_RELEASE=20230317
# Mon, 20 Mar 2023 22:46:03 GMT
ARG ODOO_SHA=2ebd7a6c36e415ed18a19148d2a1d8958d140bef
# Mon, 20 Mar 2023 22:47:15 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=2ebd7a6c36e415ed18a19148d2a1d8958d140bef
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Mar 2023 22:47:19 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 20 Mar 2023 22:47:19 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Mar 2023 22:47:20 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=2ebd7a6c36e415ed18a19148d2a1d8958d140bef
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Mar 2023 22:47:20 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Mar 2023 22:47:20 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Mar 2023 22:47:20 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Mar 2023 22:47:20 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Mar 2023 22:47:20 GMT
USER odoo
# Mon, 20 Mar 2023 22:47:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Mar 2023 22:47:21 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0ec9a41360fcaaa5f19bb2439c6b467cf4a33a0b0eaf74839a228bf1723d08`  
		Last Modified: Wed, 01 Mar 2023 18:32:40 GMT  
		Size: 220.3 MB (220298372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cf54990bd6ba63bd5db241053550b76696f1e581799de07562f631fcad34a5`  
		Last Modified: Wed, 01 Mar 2023 18:32:15 GMT  
		Size: 2.6 MB (2575211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d0db56a607542f664eb62978c779afe3f2c828db31f16594b723c048ba1b53`  
		Last Modified: Wed, 01 Mar 2023 18:32:15 GMT  
		Size: 452.0 KB (452031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c2841239c63ad4551d9a1abbd4064e7a79c9d93c7d2137e599076662494365`  
		Last Modified: Mon, 20 Mar 2023 22:50:36 GMT  
		Size: 305.6 MB (305562902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f01e48eee6843a989c9d13fa979b2152ca95652e9298a156f231cf3c0c0e5f`  
		Last Modified: Mon, 20 Mar 2023 22:50:03 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0376bd8f22a78df4079b38328a77696c2a2d251dc1c0aa04e32270eaf77144`  
		Last Modified: Mon, 20 Mar 2023 22:50:02 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc79c28e46777bba0a63473db35204946c6d012848b8db66bfd430401ee39746`  
		Last Modified: Mon, 20 Mar 2023 22:50:02 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d84741385ac1c17a2c14d524a92f14bfead88d6b9108e53e3320fe609f56299`  
		Last Modified: Mon, 20 Mar 2023 22:50:02 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:5ce2a1c0c137dcffb3f2b6be8b07f9e06779dbc72dde7a56b29110402a894900
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:b46e471cab7c73bfe334877b35909cdb8282e42aa49875f6bb1e613c72aab4c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **560.3 MB (560302384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6a2c196e7952f3657bec3f1e1a7456de7b659f3f04896d3bdf448d7963ffc57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 18:24:38 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Mar 2023 18:24:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Mar 2023 18:24:38 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 18:25:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Mar 2023 18:25:55 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 18:25:57 GMT
RUN npm install -g rtlcss
# Wed, 01 Mar 2023 18:27:31 GMT
ENV ODOO_VERSION=15.0
# Mon, 20 Mar 2023 22:46:03 GMT
ARG ODOO_RELEASE=20230317
# Mon, 20 Mar 2023 22:46:03 GMT
ARG ODOO_SHA=2ebd7a6c36e415ed18a19148d2a1d8958d140bef
# Mon, 20 Mar 2023 22:47:15 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=2ebd7a6c36e415ed18a19148d2a1d8958d140bef
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Mar 2023 22:47:19 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 20 Mar 2023 22:47:19 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Mar 2023 22:47:20 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=2ebd7a6c36e415ed18a19148d2a1d8958d140bef
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Mar 2023 22:47:20 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Mar 2023 22:47:20 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Mar 2023 22:47:20 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Mar 2023 22:47:20 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Mar 2023 22:47:20 GMT
USER odoo
# Mon, 20 Mar 2023 22:47:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Mar 2023 22:47:21 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0ec9a41360fcaaa5f19bb2439c6b467cf4a33a0b0eaf74839a228bf1723d08`  
		Last Modified: Wed, 01 Mar 2023 18:32:40 GMT  
		Size: 220.3 MB (220298372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cf54990bd6ba63bd5db241053550b76696f1e581799de07562f631fcad34a5`  
		Last Modified: Wed, 01 Mar 2023 18:32:15 GMT  
		Size: 2.6 MB (2575211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d0db56a607542f664eb62978c779afe3f2c828db31f16594b723c048ba1b53`  
		Last Modified: Wed, 01 Mar 2023 18:32:15 GMT  
		Size: 452.0 KB (452031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c2841239c63ad4551d9a1abbd4064e7a79c9d93c7d2137e599076662494365`  
		Last Modified: Mon, 20 Mar 2023 22:50:36 GMT  
		Size: 305.6 MB (305562902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f01e48eee6843a989c9d13fa979b2152ca95652e9298a156f231cf3c0c0e5f`  
		Last Modified: Mon, 20 Mar 2023 22:50:03 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0376bd8f22a78df4079b38328a77696c2a2d251dc1c0aa04e32270eaf77144`  
		Last Modified: Mon, 20 Mar 2023 22:50:02 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc79c28e46777bba0a63473db35204946c6d012848b8db66bfd430401ee39746`  
		Last Modified: Mon, 20 Mar 2023 22:50:02 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d84741385ac1c17a2c14d524a92f14bfead88d6b9108e53e3320fe609f56299`  
		Last Modified: Mon, 20 Mar 2023 22:50:02 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:f83fdd14325af3849c183d26826c9d1904791ee2e9f2238949bb58c17417771d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:f1d613c60af0dc28cdaeadb135fbf8eda21934e931831862be97defed419c0f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.1 MB (569077385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12168a286d985abc8766f8baccbf2926da8b61e45006308b8c1d9fc750fe0bde`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 18:24:38 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Mar 2023 18:24:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Mar 2023 18:24:38 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 18:25:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Mar 2023 18:25:55 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 18:25:57 GMT
RUN npm install -g rtlcss
# Wed, 01 Mar 2023 18:25:57 GMT
ENV ODOO_VERSION=16.0
# Mon, 20 Mar 2023 22:44:24 GMT
ARG ODOO_RELEASE=20230317
# Mon, 20 Mar 2023 22:44:24 GMT
ARG ODOO_SHA=13d351efd1263e2db7788a7c4995935752eab898
# Mon, 20 Mar 2023 22:45:53 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=13d351efd1263e2db7788a7c4995935752eab898
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Mar 2023 22:45:57 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 20 Mar 2023 22:45:57 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Mar 2023 22:45:58 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=13d351efd1263e2db7788a7c4995935752eab898
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Mar 2023 22:45:58 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Mar 2023 22:45:58 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Mar 2023 22:45:58 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Mar 2023 22:45:58 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Mar 2023 22:45:58 GMT
USER odoo
# Mon, 20 Mar 2023 22:45:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Mar 2023 22:45:58 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0ec9a41360fcaaa5f19bb2439c6b467cf4a33a0b0eaf74839a228bf1723d08`  
		Last Modified: Wed, 01 Mar 2023 18:32:40 GMT  
		Size: 220.3 MB (220298372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cf54990bd6ba63bd5db241053550b76696f1e581799de07562f631fcad34a5`  
		Last Modified: Wed, 01 Mar 2023 18:32:15 GMT  
		Size: 2.6 MB (2575211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d0db56a607542f664eb62978c779afe3f2c828db31f16594b723c048ba1b53`  
		Last Modified: Wed, 01 Mar 2023 18:32:15 GMT  
		Size: 452.0 KB (452031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47bc5e250a5039906e4fbc02e17c1b27bf898e5f4f30b1b8f99bffa7ec82784`  
		Last Modified: Mon, 20 Mar 2023 22:49:51 GMT  
		Size: 314.3 MB (314337902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28723d913216936cf9b1b4fe6cf06cda853046dff8f25149d0d10f2ab64dbe69`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75628ef57bfb16e3e60e4e48e0a8ece3a8767bf045eb3a6857f762c7c359fb90`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28051c5bc5e85964dca1e47a7714fa6d54c377b80ffe02e5ca0586dd4a50d5c`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2372b5d80b4ffaad0922d1568d9ebcd0c395fbe7098a9d4f35b8202fb7620c98`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:f83fdd14325af3849c183d26826c9d1904791ee2e9f2238949bb58c17417771d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:f1d613c60af0dc28cdaeadb135fbf8eda21934e931831862be97defed419c0f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.1 MB (569077385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12168a286d985abc8766f8baccbf2926da8b61e45006308b8c1d9fc750fe0bde`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 18:24:38 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Mar 2023 18:24:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Mar 2023 18:24:38 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 18:25:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Mar 2023 18:25:55 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 18:25:57 GMT
RUN npm install -g rtlcss
# Wed, 01 Mar 2023 18:25:57 GMT
ENV ODOO_VERSION=16.0
# Mon, 20 Mar 2023 22:44:24 GMT
ARG ODOO_RELEASE=20230317
# Mon, 20 Mar 2023 22:44:24 GMT
ARG ODOO_SHA=13d351efd1263e2db7788a7c4995935752eab898
# Mon, 20 Mar 2023 22:45:53 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=13d351efd1263e2db7788a7c4995935752eab898
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Mar 2023 22:45:57 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 20 Mar 2023 22:45:57 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Mar 2023 22:45:58 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=13d351efd1263e2db7788a7c4995935752eab898
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Mar 2023 22:45:58 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Mar 2023 22:45:58 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Mar 2023 22:45:58 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Mar 2023 22:45:58 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Mar 2023 22:45:58 GMT
USER odoo
# Mon, 20 Mar 2023 22:45:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Mar 2023 22:45:58 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0ec9a41360fcaaa5f19bb2439c6b467cf4a33a0b0eaf74839a228bf1723d08`  
		Last Modified: Wed, 01 Mar 2023 18:32:40 GMT  
		Size: 220.3 MB (220298372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cf54990bd6ba63bd5db241053550b76696f1e581799de07562f631fcad34a5`  
		Last Modified: Wed, 01 Mar 2023 18:32:15 GMT  
		Size: 2.6 MB (2575211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d0db56a607542f664eb62978c779afe3f2c828db31f16594b723c048ba1b53`  
		Last Modified: Wed, 01 Mar 2023 18:32:15 GMT  
		Size: 452.0 KB (452031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47bc5e250a5039906e4fbc02e17c1b27bf898e5f4f30b1b8f99bffa7ec82784`  
		Last Modified: Mon, 20 Mar 2023 22:49:51 GMT  
		Size: 314.3 MB (314337902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28723d913216936cf9b1b4fe6cf06cda853046dff8f25149d0d10f2ab64dbe69`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75628ef57bfb16e3e60e4e48e0a8ece3a8767bf045eb3a6857f762c7c359fb90`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28051c5bc5e85964dca1e47a7714fa6d54c377b80ffe02e5ca0586dd4a50d5c`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2372b5d80b4ffaad0922d1568d9ebcd0c395fbe7098a9d4f35b8202fb7620c98`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:f83fdd14325af3849c183d26826c9d1904791ee2e9f2238949bb58c17417771d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:f1d613c60af0dc28cdaeadb135fbf8eda21934e931831862be97defed419c0f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.1 MB (569077385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12168a286d985abc8766f8baccbf2926da8b61e45006308b8c1d9fc750fe0bde`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 18:24:38 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 01 Mar 2023 18:24:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 01 Mar 2023 18:24:38 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 18:25:45 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 01 Mar 2023 18:25:55 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 18:25:57 GMT
RUN npm install -g rtlcss
# Wed, 01 Mar 2023 18:25:57 GMT
ENV ODOO_VERSION=16.0
# Mon, 20 Mar 2023 22:44:24 GMT
ARG ODOO_RELEASE=20230317
# Mon, 20 Mar 2023 22:44:24 GMT
ARG ODOO_SHA=13d351efd1263e2db7788a7c4995935752eab898
# Mon, 20 Mar 2023 22:45:53 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=13d351efd1263e2db7788a7c4995935752eab898
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Mar 2023 22:45:57 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 20 Mar 2023 22:45:57 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Mar 2023 22:45:58 GMT
# ARGS: ODOO_RELEASE=20230317 ODOO_SHA=13d351efd1263e2db7788a7c4995935752eab898
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Mar 2023 22:45:58 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Mar 2023 22:45:58 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Mar 2023 22:45:58 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Mar 2023 22:45:58 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Mar 2023 22:45:58 GMT
USER odoo
# Mon, 20 Mar 2023 22:45:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Mar 2023 22:45:58 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0ec9a41360fcaaa5f19bb2439c6b467cf4a33a0b0eaf74839a228bf1723d08`  
		Last Modified: Wed, 01 Mar 2023 18:32:40 GMT  
		Size: 220.3 MB (220298372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cf54990bd6ba63bd5db241053550b76696f1e581799de07562f631fcad34a5`  
		Last Modified: Wed, 01 Mar 2023 18:32:15 GMT  
		Size: 2.6 MB (2575211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d0db56a607542f664eb62978c779afe3f2c828db31f16594b723c048ba1b53`  
		Last Modified: Wed, 01 Mar 2023 18:32:15 GMT  
		Size: 452.0 KB (452031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47bc5e250a5039906e4fbc02e17c1b27bf898e5f4f30b1b8f99bffa7ec82784`  
		Last Modified: Mon, 20 Mar 2023 22:49:51 GMT  
		Size: 314.3 MB (314337902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28723d913216936cf9b1b4fe6cf06cda853046dff8f25149d0d10f2ab64dbe69`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75628ef57bfb16e3e60e4e48e0a8ece3a8767bf045eb3a6857f762c7c359fb90`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28051c5bc5e85964dca1e47a7714fa6d54c377b80ffe02e5ca0586dd4a50d5c`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2372b5d80b4ffaad0922d1568d9ebcd0c395fbe7098a9d4f35b8202fb7620c98`  
		Last Modified: Mon, 20 Mar 2023 22:49:15 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
