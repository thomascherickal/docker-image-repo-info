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
$ docker pull odoo@sha256:ba3ea6a5e13bcca82f597d91e67cc178721b4408ee21da7867edadd1e7f9f4dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:657019990b26a8c7c6db13a8667767b08e0e25f4a956bac637e55fb9faccc78f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.7 MB (532682186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9cf6e394d9d50e29eacb45b172c3623793e57ebdee5c7ed1464ae8741c89bca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:32 GMT
ADD file:2818e508d01da2188fb234b38fb19aa1ea9eeeae92d361ecdf49318d949f51a9 in / 
# Mon, 12 Jun 2023 23:21:32 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:31:42 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Jun 2023 07:31:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Jun 2023 07:31:42 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 07:33:35 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 13 Jun 2023 07:33:47 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:33:50 GMT
RUN npm install -g rtlcss
# Tue, 13 Jun 2023 07:33:50 GMT
ENV ODOO_VERSION=14.0
# Wed, 14 Jun 2023 04:30:47 GMT
ARG ODOO_RELEASE=20230613
# Wed, 14 Jun 2023 04:30:47 GMT
ARG ODOO_SHA=e73fbeab19595d52e7ebae3081d3989ee415f43f
# Wed, 14 Jun 2023 04:32:13 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=e73fbeab19595d52e7ebae3081d3989ee415f43f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 14 Jun 2023 04:32:17 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 14 Jun 2023 04:32:17 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 14 Jun 2023 04:32:18 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=e73fbeab19595d52e7ebae3081d3989ee415f43f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 14 Jun 2023 04:32:18 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 14 Jun 2023 04:32:18 GMT
EXPOSE 8069 8071 8072
# Wed, 14 Jun 2023 04:32:18 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 14 Jun 2023 04:32:18 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 14 Jun 2023 04:32:18 GMT
USER odoo
# Wed, 14 Jun 2023 04:32:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 04:32:18 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:8b91b88d557765cd8c6802668755a3f6dc4337b6ce15a17e4857139e5fc964f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:09 GMT  
		Size: 27.1 MB (27138450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e5002b5ea775e66bb8ed13a29d4cb4211ed8997ba6bdc303fd9a85fe503599`  
		Last Modified: Tue, 13 Jun 2023 07:37:35 GMT  
		Size: 213.2 MB (213199216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3b8791ab67afd61cac80a3091c7249ff248213ce957875bef3f0b1b1590263`  
		Last Modified: Tue, 13 Jun 2023 07:37:15 GMT  
		Size: 13.5 MB (13520946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9871a097e610176015bafb017a7f44fec2052f3d38de96814509597f53e2448`  
		Last Modified: Tue, 13 Jun 2023 07:37:12 GMT  
		Size: 458.8 KB (458750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02455a4a3298728a93d50cc36bb3ca4ec0bcf4e685f768c273bcb221c643fd94`  
		Last Modified: Wed, 14 Jun 2023 04:34:32 GMT  
		Size: 278.4 MB (278362367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed08837acf63be58398dcade1686b3941e37be8640d6f55bc1c35250600bd75`  
		Last Modified: Wed, 14 Jun 2023 04:34:02 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb2e0494654c67e6295be90c281793672ab593d1797f03e56b1c1b102a4f3a5`  
		Last Modified: Wed, 14 Jun 2023 04:34:02 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb30e067881f66ed4104ad0f6a5a70f0492e97a77485f389cfc8d2ee769c7ec`  
		Last Modified: Wed, 14 Jun 2023 04:34:02 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b308bd6ae5172d9ba23bda2795799acb56d598af551e92675188aab3d00924`  
		Last Modified: Wed, 14 Jun 2023 04:34:02 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:ba3ea6a5e13bcca82f597d91e67cc178721b4408ee21da7867edadd1e7f9f4dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:657019990b26a8c7c6db13a8667767b08e0e25f4a956bac637e55fb9faccc78f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.7 MB (532682186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9cf6e394d9d50e29eacb45b172c3623793e57ebdee5c7ed1464ae8741c89bca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:32 GMT
ADD file:2818e508d01da2188fb234b38fb19aa1ea9eeeae92d361ecdf49318d949f51a9 in / 
# Mon, 12 Jun 2023 23:21:32 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:31:42 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Jun 2023 07:31:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Jun 2023 07:31:42 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 07:33:35 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 13 Jun 2023 07:33:47 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:33:50 GMT
RUN npm install -g rtlcss
# Tue, 13 Jun 2023 07:33:50 GMT
ENV ODOO_VERSION=14.0
# Wed, 14 Jun 2023 04:30:47 GMT
ARG ODOO_RELEASE=20230613
# Wed, 14 Jun 2023 04:30:47 GMT
ARG ODOO_SHA=e73fbeab19595d52e7ebae3081d3989ee415f43f
# Wed, 14 Jun 2023 04:32:13 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=e73fbeab19595d52e7ebae3081d3989ee415f43f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 14 Jun 2023 04:32:17 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 14 Jun 2023 04:32:17 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 14 Jun 2023 04:32:18 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=e73fbeab19595d52e7ebae3081d3989ee415f43f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 14 Jun 2023 04:32:18 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 14 Jun 2023 04:32:18 GMT
EXPOSE 8069 8071 8072
# Wed, 14 Jun 2023 04:32:18 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 14 Jun 2023 04:32:18 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 14 Jun 2023 04:32:18 GMT
USER odoo
# Wed, 14 Jun 2023 04:32:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 04:32:18 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:8b91b88d557765cd8c6802668755a3f6dc4337b6ce15a17e4857139e5fc964f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:09 GMT  
		Size: 27.1 MB (27138450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e5002b5ea775e66bb8ed13a29d4cb4211ed8997ba6bdc303fd9a85fe503599`  
		Last Modified: Tue, 13 Jun 2023 07:37:35 GMT  
		Size: 213.2 MB (213199216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3b8791ab67afd61cac80a3091c7249ff248213ce957875bef3f0b1b1590263`  
		Last Modified: Tue, 13 Jun 2023 07:37:15 GMT  
		Size: 13.5 MB (13520946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9871a097e610176015bafb017a7f44fec2052f3d38de96814509597f53e2448`  
		Last Modified: Tue, 13 Jun 2023 07:37:12 GMT  
		Size: 458.8 KB (458750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02455a4a3298728a93d50cc36bb3ca4ec0bcf4e685f768c273bcb221c643fd94`  
		Last Modified: Wed, 14 Jun 2023 04:34:32 GMT  
		Size: 278.4 MB (278362367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed08837acf63be58398dcade1686b3941e37be8640d6f55bc1c35250600bd75`  
		Last Modified: Wed, 14 Jun 2023 04:34:02 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb2e0494654c67e6295be90c281793672ab593d1797f03e56b1c1b102a4f3a5`  
		Last Modified: Wed, 14 Jun 2023 04:34:02 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb30e067881f66ed4104ad0f6a5a70f0492e97a77485f389cfc8d2ee769c7ec`  
		Last Modified: Wed, 14 Jun 2023 04:34:02 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b308bd6ae5172d9ba23bda2795799acb56d598af551e92675188aab3d00924`  
		Last Modified: Wed, 14 Jun 2023 04:34:02 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:9b84f60f6f817094717d4b6b8c98e2b9874f136ef6d07ef81a972fb0f1a9d6e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:0bb78119fde699e29d8ac4497bd929dadc5de4453b8ca0dd63aaaa9ea5c1234a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561351415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1635437d83096ab553272d49f77cc798ea138b3d87fdcfb5ead4f70843746aae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:26:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Jun 2023 07:26:55 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Jun 2023 07:26:55 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 07:28:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 13 Jun 2023 07:28:36 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:28:38 GMT
RUN npm install -g rtlcss
# Tue, 13 Jun 2023 07:30:19 GMT
ENV ODOO_VERSION=15.0
# Wed, 14 Jun 2023 04:29:22 GMT
ARG ODOO_RELEASE=20230613
# Wed, 14 Jun 2023 04:29:22 GMT
ARG ODOO_SHA=069b72fbdce8c39278961f659a16b244c94ea83b
# Wed, 14 Jun 2023 04:30:36 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=069b72fbdce8c39278961f659a16b244c94ea83b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 14 Jun 2023 04:30:40 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 14 Jun 2023 04:30:40 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 14 Jun 2023 04:30:40 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=069b72fbdce8c39278961f659a16b244c94ea83b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 14 Jun 2023 04:30:40 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 14 Jun 2023 04:30:40 GMT
EXPOSE 8069 8071 8072
# Wed, 14 Jun 2023 04:30:41 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 14 Jun 2023 04:30:41 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 14 Jun 2023 04:30:41 GMT
USER odoo
# Wed, 14 Jun 2023 04:30:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 04:30:41 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd64d7ca73c2e93c76513d56030613b9b9cf0e27efdb3a253d1591507005e0cd`  
		Last Modified: Tue, 13 Jun 2023 07:36:08 GMT  
		Size: 220.3 MB (220302623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377e8b4bd092ea25a9ae903dc284787bd0503e212e6d227300943cb1f2e8fe9b`  
		Last Modified: Tue, 13 Jun 2023 07:35:44 GMT  
		Size: 2.6 MB (2576153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c886eafab424bce7b46782d3222cd1432beb940d583b9b559df7de7dfc41943`  
		Last Modified: Tue, 13 Jun 2023 07:35:44 GMT  
		Size: 454.3 KB (454307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a36ae9206728a1f7d582b0d3f11e341bff4efdcc20fe1bdafdb2ed034ea74b8`  
		Last Modified: Wed, 14 Jun 2023 04:33:53 GMT  
		Size: 306.6 MB (306598464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c797d2631196ce57018e6ed1151e102c1b498369dcd4d2e3cfb7f86ea3fa796`  
		Last Modified: Wed, 14 Jun 2023 04:33:20 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d01e7fdf5622ad67c30d2ddc0cdba4a990f3bb4c5c55c30f1dba53a610452b`  
		Last Modified: Wed, 14 Jun 2023 04:33:20 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec3fbde404d8fcfd0a64ea630ece215186773fbe611d762aaac60cbae8e3d58`  
		Last Modified: Wed, 14 Jun 2023 04:33:20 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce141ad1599ae2532e524b84b867da7a00022574016bf15c56011aff2d02089a`  
		Last Modified: Wed, 14 Jun 2023 04:33:20 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:9b84f60f6f817094717d4b6b8c98e2b9874f136ef6d07ef81a972fb0f1a9d6e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:0bb78119fde699e29d8ac4497bd929dadc5de4453b8ca0dd63aaaa9ea5c1234a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561351415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1635437d83096ab553272d49f77cc798ea138b3d87fdcfb5ead4f70843746aae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:26:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Jun 2023 07:26:55 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Jun 2023 07:26:55 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 07:28:26 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 13 Jun 2023 07:28:36 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:28:38 GMT
RUN npm install -g rtlcss
# Tue, 13 Jun 2023 07:30:19 GMT
ENV ODOO_VERSION=15.0
# Wed, 14 Jun 2023 04:29:22 GMT
ARG ODOO_RELEASE=20230613
# Wed, 14 Jun 2023 04:29:22 GMT
ARG ODOO_SHA=069b72fbdce8c39278961f659a16b244c94ea83b
# Wed, 14 Jun 2023 04:30:36 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=069b72fbdce8c39278961f659a16b244c94ea83b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 14 Jun 2023 04:30:40 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 14 Jun 2023 04:30:40 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 14 Jun 2023 04:30:40 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=069b72fbdce8c39278961f659a16b244c94ea83b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 14 Jun 2023 04:30:40 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 14 Jun 2023 04:30:40 GMT
EXPOSE 8069 8071 8072
# Wed, 14 Jun 2023 04:30:41 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 14 Jun 2023 04:30:41 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 14 Jun 2023 04:30:41 GMT
USER odoo
# Wed, 14 Jun 2023 04:30:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 04:30:41 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd64d7ca73c2e93c76513d56030613b9b9cf0e27efdb3a253d1591507005e0cd`  
		Last Modified: Tue, 13 Jun 2023 07:36:08 GMT  
		Size: 220.3 MB (220302623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377e8b4bd092ea25a9ae903dc284787bd0503e212e6d227300943cb1f2e8fe9b`  
		Last Modified: Tue, 13 Jun 2023 07:35:44 GMT  
		Size: 2.6 MB (2576153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c886eafab424bce7b46782d3222cd1432beb940d583b9b559df7de7dfc41943`  
		Last Modified: Tue, 13 Jun 2023 07:35:44 GMT  
		Size: 454.3 KB (454307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a36ae9206728a1f7d582b0d3f11e341bff4efdcc20fe1bdafdb2ed034ea74b8`  
		Last Modified: Wed, 14 Jun 2023 04:33:53 GMT  
		Size: 306.6 MB (306598464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c797d2631196ce57018e6ed1151e102c1b498369dcd4d2e3cfb7f86ea3fa796`  
		Last Modified: Wed, 14 Jun 2023 04:33:20 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d01e7fdf5622ad67c30d2ddc0cdba4a990f3bb4c5c55c30f1dba53a610452b`  
		Last Modified: Wed, 14 Jun 2023 04:33:20 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec3fbde404d8fcfd0a64ea630ece215186773fbe611d762aaac60cbae8e3d58`  
		Last Modified: Wed, 14 Jun 2023 04:33:20 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce141ad1599ae2532e524b84b867da7a00022574016bf15c56011aff2d02089a`  
		Last Modified: Wed, 14 Jun 2023 04:33:20 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:38d7cc5986fc76f091dd7294c08ff43b7d12eea9baa22dc6905f157676c8dc83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:df0276cdb0ff8bb7883058071daf898d90fdbf13045ae96d131584660878da84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.6 MB (572555134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7751cf537987c6c7cfc02d948dc60780524386d8b8cd18b8c9c46c37773892b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:26:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Jun 2023 07:26:55 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Jun 2023 07:26:55 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 04:27:24 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 14 Jun 2023 04:27:35 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 04:27:37 GMT
RUN npm install -g rtlcss
# Wed, 14 Jun 2023 04:27:37 GMT
ENV ODOO_VERSION=16.0
# Wed, 14 Jun 2023 04:27:37 GMT
ARG ODOO_RELEASE=20230613
# Wed, 14 Jun 2023 04:27:37 GMT
ARG ODOO_SHA=5cd43e65a2c3836894e14fc902a935bf84c64877
# Wed, 14 Jun 2023 04:29:11 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=5cd43e65a2c3836894e14fc902a935bf84c64877
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 14 Jun 2023 04:29:15 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 14 Jun 2023 04:29:15 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 14 Jun 2023 04:29:16 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=5cd43e65a2c3836894e14fc902a935bf84c64877
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 14 Jun 2023 04:29:16 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 14 Jun 2023 04:29:16 GMT
EXPOSE 8069 8071 8072
# Wed, 14 Jun 2023 04:29:16 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 14 Jun 2023 04:29:16 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 14 Jun 2023 04:29:16 GMT
USER odoo
# Wed, 14 Jun 2023 04:29:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 04:29:16 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0150bee3cf7fd565f38365a92baed4868a70bda3097098238210c9059af7204`  
		Last Modified: Wed, 14 Jun 2023 04:32:59 GMT  
		Size: 221.0 MB (220992456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4009085967d4272bf851a9728ec147d197d9ae6a1f8df3f47bebffd2ab1a4360`  
		Last Modified: Wed, 14 Jun 2023 04:32:35 GMT  
		Size: 2.6 MB (2579555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525116348075279c320d804574bf4ecb000e0141c6da9e43d183af7422dd459e`  
		Last Modified: Wed, 14 Jun 2023 04:32:35 GMT  
		Size: 454.4 KB (454369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6355c29c4d7f0c0372efd04cec7ca19385a0c4bf585dc4dcd675d27c673fb19`  
		Last Modified: Wed, 14 Jun 2023 04:33:09 GMT  
		Size: 317.1 MB (317108880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4745f0afa6faee3c5513f33029f9677e9217cfc6ce8024f831010b8a7f8025f5`  
		Last Modified: Wed, 14 Jun 2023 04:32:32 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf2a3fe15e4a78d88cdbc47ce8843e668f11f544a62ce9ec865993f6026823c`  
		Last Modified: Wed, 14 Jun 2023 04:32:33 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e535b6c2af211353b3caa7e66fa1e53623fd5bb892f6ee8bf678f1b4bb120e3f`  
		Last Modified: Wed, 14 Jun 2023 04:32:32 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0a5cc69a89d34f6ee37bd23327656f797846766536a52434b9cff3037517bd`  
		Last Modified: Wed, 14 Jun 2023 04:32:32 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:38d7cc5986fc76f091dd7294c08ff43b7d12eea9baa22dc6905f157676c8dc83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:df0276cdb0ff8bb7883058071daf898d90fdbf13045ae96d131584660878da84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.6 MB (572555134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7751cf537987c6c7cfc02d948dc60780524386d8b8cd18b8c9c46c37773892b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:26:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Jun 2023 07:26:55 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Jun 2023 07:26:55 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 04:27:24 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 14 Jun 2023 04:27:35 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 04:27:37 GMT
RUN npm install -g rtlcss
# Wed, 14 Jun 2023 04:27:37 GMT
ENV ODOO_VERSION=16.0
# Wed, 14 Jun 2023 04:27:37 GMT
ARG ODOO_RELEASE=20230613
# Wed, 14 Jun 2023 04:27:37 GMT
ARG ODOO_SHA=5cd43e65a2c3836894e14fc902a935bf84c64877
# Wed, 14 Jun 2023 04:29:11 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=5cd43e65a2c3836894e14fc902a935bf84c64877
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 14 Jun 2023 04:29:15 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 14 Jun 2023 04:29:15 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 14 Jun 2023 04:29:16 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=5cd43e65a2c3836894e14fc902a935bf84c64877
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 14 Jun 2023 04:29:16 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 14 Jun 2023 04:29:16 GMT
EXPOSE 8069 8071 8072
# Wed, 14 Jun 2023 04:29:16 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 14 Jun 2023 04:29:16 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 14 Jun 2023 04:29:16 GMT
USER odoo
# Wed, 14 Jun 2023 04:29:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 04:29:16 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0150bee3cf7fd565f38365a92baed4868a70bda3097098238210c9059af7204`  
		Last Modified: Wed, 14 Jun 2023 04:32:59 GMT  
		Size: 221.0 MB (220992456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4009085967d4272bf851a9728ec147d197d9ae6a1f8df3f47bebffd2ab1a4360`  
		Last Modified: Wed, 14 Jun 2023 04:32:35 GMT  
		Size: 2.6 MB (2579555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525116348075279c320d804574bf4ecb000e0141c6da9e43d183af7422dd459e`  
		Last Modified: Wed, 14 Jun 2023 04:32:35 GMT  
		Size: 454.4 KB (454369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6355c29c4d7f0c0372efd04cec7ca19385a0c4bf585dc4dcd675d27c673fb19`  
		Last Modified: Wed, 14 Jun 2023 04:33:09 GMT  
		Size: 317.1 MB (317108880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4745f0afa6faee3c5513f33029f9677e9217cfc6ce8024f831010b8a7f8025f5`  
		Last Modified: Wed, 14 Jun 2023 04:32:32 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf2a3fe15e4a78d88cdbc47ce8843e668f11f544a62ce9ec865993f6026823c`  
		Last Modified: Wed, 14 Jun 2023 04:32:33 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e535b6c2af211353b3caa7e66fa1e53623fd5bb892f6ee8bf678f1b4bb120e3f`  
		Last Modified: Wed, 14 Jun 2023 04:32:32 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0a5cc69a89d34f6ee37bd23327656f797846766536a52434b9cff3037517bd`  
		Last Modified: Wed, 14 Jun 2023 04:32:32 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:38d7cc5986fc76f091dd7294c08ff43b7d12eea9baa22dc6905f157676c8dc83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:df0276cdb0ff8bb7883058071daf898d90fdbf13045ae96d131584660878da84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **572.6 MB (572555134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7751cf537987c6c7cfc02d948dc60780524386d8b8cd18b8c9c46c37773892b4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:26:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Jun 2023 07:26:55 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Jun 2023 07:26:55 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 04:27:24 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 14 Jun 2023 04:27:35 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 04:27:37 GMT
RUN npm install -g rtlcss
# Wed, 14 Jun 2023 04:27:37 GMT
ENV ODOO_VERSION=16.0
# Wed, 14 Jun 2023 04:27:37 GMT
ARG ODOO_RELEASE=20230613
# Wed, 14 Jun 2023 04:27:37 GMT
ARG ODOO_SHA=5cd43e65a2c3836894e14fc902a935bf84c64877
# Wed, 14 Jun 2023 04:29:11 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=5cd43e65a2c3836894e14fc902a935bf84c64877
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 14 Jun 2023 04:29:15 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 14 Jun 2023 04:29:15 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 14 Jun 2023 04:29:16 GMT
# ARGS: ODOO_RELEASE=20230613 ODOO_SHA=5cd43e65a2c3836894e14fc902a935bf84c64877
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 14 Jun 2023 04:29:16 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 14 Jun 2023 04:29:16 GMT
EXPOSE 8069 8071 8072
# Wed, 14 Jun 2023 04:29:16 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 14 Jun 2023 04:29:16 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 14 Jun 2023 04:29:16 GMT
USER odoo
# Wed, 14 Jun 2023 04:29:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 04:29:16 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0150bee3cf7fd565f38365a92baed4868a70bda3097098238210c9059af7204`  
		Last Modified: Wed, 14 Jun 2023 04:32:59 GMT  
		Size: 221.0 MB (220992456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4009085967d4272bf851a9728ec147d197d9ae6a1f8df3f47bebffd2ab1a4360`  
		Last Modified: Wed, 14 Jun 2023 04:32:35 GMT  
		Size: 2.6 MB (2579555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525116348075279c320d804574bf4ecb000e0141c6da9e43d183af7422dd459e`  
		Last Modified: Wed, 14 Jun 2023 04:32:35 GMT  
		Size: 454.4 KB (454369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6355c29c4d7f0c0372efd04cec7ca19385a0c4bf585dc4dcd675d27c673fb19`  
		Last Modified: Wed, 14 Jun 2023 04:33:09 GMT  
		Size: 317.1 MB (317108880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4745f0afa6faee3c5513f33029f9677e9217cfc6ce8024f831010b8a7f8025f5`  
		Last Modified: Wed, 14 Jun 2023 04:32:32 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf2a3fe15e4a78d88cdbc47ce8843e668f11f544a62ce9ec865993f6026823c`  
		Last Modified: Wed, 14 Jun 2023 04:32:33 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e535b6c2af211353b3caa7e66fa1e53623fd5bb892f6ee8bf678f1b4bb120e3f`  
		Last Modified: Wed, 14 Jun 2023 04:32:32 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0a5cc69a89d34f6ee37bd23327656f797846766536a52434b9cff3037517bd`  
		Last Modified: Wed, 14 Jun 2023 04:32:32 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
