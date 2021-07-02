<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `odoo`

-	[`odoo:12`](#odoo12)
-	[`odoo:12.0`](#odoo120)
-	[`odoo:13`](#odoo13)
-	[`odoo:13.0`](#odoo130)
-	[`odoo:14`](#odoo14)
-	[`odoo:14.0`](#odoo140)
-	[`odoo:latest`](#odoolatest)

## `odoo:12`

```console
$ docker pull odoo@sha256:dbd38f35dba73528969f82e1f2ed92f64990440767f7d4c5120c5456f1b9713b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:7e4790c5cfd870b4048e4a927dbdfdee5ae4f9e2e41e083be85aaa2c57ece1a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538359265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bde895eb56b3ffa410d02567bd3841f07a8aa9bbf1d8d1f87886b9f41de19ec4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:51:50 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 23 Jun 2021 07:51:50 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 23 Jun 2021 07:51:50 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 07:51:52 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 23 Jun 2021 07:53:47 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 23 Jun 2021 07:54:01 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:54:13 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:54:14 GMT
ENV ODOO_VERSION=12.0
# Fri, 02 Jul 2021 18:24:53 GMT
ARG ODOO_RELEASE=20210702
# Fri, 02 Jul 2021 18:24:54 GMT
ARG ODOO_SHA=5c07ed019be6158129e974eced0ee26967b8767f
# Fri, 02 Jul 2021 18:25:59 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=5c07ed019be6158129e974eced0ee26967b8767f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Jul 2021 18:26:02 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 02 Jul 2021 18:26:02 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Jul 2021 18:26:03 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=5c07ed019be6158129e974eced0ee26967b8767f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Jul 2021 18:26:03 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Jul 2021 18:26:03 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Jul 2021 18:26:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Jul 2021 18:26:04 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Jul 2021 18:26:04 GMT
USER odoo
# Fri, 02 Jul 2021 18:26:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jul 2021 18:26:04 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f8f66a1ee8d03d029b9e9fd4fab492aae82ab75ecc939a565a9ed63bd81f8`  
		Last Modified: Wed, 23 Jun 2021 07:57:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef6f54374b12d423468b84b7b20816bca30d69f0367e06c3fcc78a58990776d`  
		Last Modified: Wed, 23 Jun 2021 07:58:33 GMT  
		Size: 219.7 MB (219658352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc0f9e42ea609c4a44d52d51b1be4eb6a509244b5ff23b7ce9cc26e2d31f4d9`  
		Last Modified: Wed, 23 Jun 2021 07:57:59 GMT  
		Size: 2.2 MB (2224626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47480c9939297e4d6a19caeef3f46a6554712b96da0972a4b1630a6d1a39808f`  
		Last Modified: Wed, 23 Jun 2021 07:58:05 GMT  
		Size: 22.0 MB (22023550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4742e00f66f1e83ef4e246be39aad8a1ef6dc7bf0e67e3438068f27b3eb7890`  
		Last Modified: Fri, 02 Jul 2021 18:28:27 GMT  
		Size: 271.9 MB (271921898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64f99f379ac6237d7c7b72b913a7f8547c6f896ccfb8b982001de1a44c6115`  
		Last Modified: Fri, 02 Jul 2021 18:27:59 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3db1289de4b69c89f5f3b0c1dfb36bee38f0a82de39b78b0538f8e20418ba1`  
		Last Modified: Fri, 02 Jul 2021 18:27:59 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8caed96a6be3c172115011f596f7d7940d074c52a049a1b79ffa995953fb34`  
		Last Modified: Fri, 02 Jul 2021 18:27:59 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304a22a25bcd8be19bce284abb63c53ae814b923274b0298061ac8f6a04b483e`  
		Last Modified: Fri, 02 Jul 2021 18:27:59 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:dbd38f35dba73528969f82e1f2ed92f64990440767f7d4c5120c5456f1b9713b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:7e4790c5cfd870b4048e4a927dbdfdee5ae4f9e2e41e083be85aaa2c57ece1a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538359265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bde895eb56b3ffa410d02567bd3841f07a8aa9bbf1d8d1f87886b9f41de19ec4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:51:50 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 23 Jun 2021 07:51:50 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 23 Jun 2021 07:51:50 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 07:51:52 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 23 Jun 2021 07:53:47 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 23 Jun 2021 07:54:01 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:54:13 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:54:14 GMT
ENV ODOO_VERSION=12.0
# Fri, 02 Jul 2021 18:24:53 GMT
ARG ODOO_RELEASE=20210702
# Fri, 02 Jul 2021 18:24:54 GMT
ARG ODOO_SHA=5c07ed019be6158129e974eced0ee26967b8767f
# Fri, 02 Jul 2021 18:25:59 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=5c07ed019be6158129e974eced0ee26967b8767f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Jul 2021 18:26:02 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 02 Jul 2021 18:26:02 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Jul 2021 18:26:03 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=5c07ed019be6158129e974eced0ee26967b8767f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Jul 2021 18:26:03 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Jul 2021 18:26:03 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Jul 2021 18:26:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Jul 2021 18:26:04 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Jul 2021 18:26:04 GMT
USER odoo
# Fri, 02 Jul 2021 18:26:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jul 2021 18:26:04 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f8f66a1ee8d03d029b9e9fd4fab492aae82ab75ecc939a565a9ed63bd81f8`  
		Last Modified: Wed, 23 Jun 2021 07:57:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef6f54374b12d423468b84b7b20816bca30d69f0367e06c3fcc78a58990776d`  
		Last Modified: Wed, 23 Jun 2021 07:58:33 GMT  
		Size: 219.7 MB (219658352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc0f9e42ea609c4a44d52d51b1be4eb6a509244b5ff23b7ce9cc26e2d31f4d9`  
		Last Modified: Wed, 23 Jun 2021 07:57:59 GMT  
		Size: 2.2 MB (2224626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47480c9939297e4d6a19caeef3f46a6554712b96da0972a4b1630a6d1a39808f`  
		Last Modified: Wed, 23 Jun 2021 07:58:05 GMT  
		Size: 22.0 MB (22023550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4742e00f66f1e83ef4e246be39aad8a1ef6dc7bf0e67e3438068f27b3eb7890`  
		Last Modified: Fri, 02 Jul 2021 18:28:27 GMT  
		Size: 271.9 MB (271921898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b64f99f379ac6237d7c7b72b913a7f8547c6f896ccfb8b982001de1a44c6115`  
		Last Modified: Fri, 02 Jul 2021 18:27:59 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3db1289de4b69c89f5f3b0c1dfb36bee38f0a82de39b78b0538f8e20418ba1`  
		Last Modified: Fri, 02 Jul 2021 18:27:59 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8caed96a6be3c172115011f596f7d7940d074c52a049a1b79ffa995953fb34`  
		Last Modified: Fri, 02 Jul 2021 18:27:59 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304a22a25bcd8be19bce284abb63c53ae814b923274b0298061ac8f6a04b483e`  
		Last Modified: Fri, 02 Jul 2021 18:27:59 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:6fe99f172dad16f7701074c9232640dc7ccb5083508e229731d5068299645147
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:0d1f2ede153f34957e158c47bfd7d0c3aab1cdd0db709bf90c8bce7890466282
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.3 MB (528271232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bbb9f8970e15b39cac5395ad493514827e7fb8b2eb0cf51d5a5a93c0fcfd55f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:44:56 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 23 Jun 2021 07:44:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 23 Jun 2021 07:44:57 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 07:49:38 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 23 Jun 2021 07:49:48 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:49:53 GMT
RUN npm install -g rtlcss
# Wed, 23 Jun 2021 07:49:53 GMT
ENV ODOO_VERSION=13.0
# Fri, 02 Jul 2021 18:23:28 GMT
ARG ODOO_RELEASE=20210702
# Fri, 02 Jul 2021 18:23:28 GMT
ARG ODOO_SHA=f135b9d4967ef9221ff6aba58b1c4a3ea8334202
# Fri, 02 Jul 2021 18:24:37 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=f135b9d4967ef9221ff6aba58b1c4a3ea8334202
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Jul 2021 18:24:40 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 02 Jul 2021 18:24:40 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Jul 2021 18:24:42 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=f135b9d4967ef9221ff6aba58b1c4a3ea8334202
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Jul 2021 18:24:42 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Jul 2021 18:24:42 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Jul 2021 18:24:42 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Jul 2021 18:24:42 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Jul 2021 18:24:43 GMT
USER odoo
# Fri, 02 Jul 2021 18:24:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jul 2021 18:24:43 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d760ec83e05549c1bafe40d795ed53c471a0208b2e5a5fe29f1f4575e4277ed`  
		Last Modified: Wed, 23 Jun 2021 07:57:34 GMT  
		Size: 207.1 MB (207122080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6f5407abbe57f2c624e00f8226cb3f74567fc177824c08838c437a8d05fba`  
		Last Modified: Wed, 23 Jun 2021 07:57:03 GMT  
		Size: 2.3 MB (2346852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7db6376102b543b53d50ab5ed822526c9569bbee49c030740510ed71465072`  
		Last Modified: Wed, 23 Jun 2021 07:57:03 GMT  
		Size: 885.8 KB (885845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e888c31054e38d42e49d9a9300e407418f68a9fd57c0939631eeb16590441d55`  
		Last Modified: Fri, 02 Jul 2021 18:27:48 GMT  
		Size: 290.8 MB (290768175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228f78f5139b87d9245dc560367248cdb4cd9c4e3adc6eaf6c4c2924996d6142`  
		Last Modified: Fri, 02 Jul 2021 18:27:16 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a027bd1452b83ce7460764b07ebb6630a972887e1cdf2f0c0c4c448de66bbd2`  
		Last Modified: Fri, 02 Jul 2021 18:27:17 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2febbd7f55a9f3feb53bcdeb1707b9b752f173240e7232979353ca79ea4ddfc`  
		Last Modified: Fri, 02 Jul 2021 18:27:16 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9665050c95eea8f5c3179897ebdc4c2b6f55731e68a3a2651e74b9bab90eefc9`  
		Last Modified: Fri, 02 Jul 2021 18:27:16 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:6fe99f172dad16f7701074c9232640dc7ccb5083508e229731d5068299645147
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:0d1f2ede153f34957e158c47bfd7d0c3aab1cdd0db709bf90c8bce7890466282
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.3 MB (528271232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bbb9f8970e15b39cac5395ad493514827e7fb8b2eb0cf51d5a5a93c0fcfd55f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:44:56 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 23 Jun 2021 07:44:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 23 Jun 2021 07:44:57 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 07:49:38 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 23 Jun 2021 07:49:48 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:49:53 GMT
RUN npm install -g rtlcss
# Wed, 23 Jun 2021 07:49:53 GMT
ENV ODOO_VERSION=13.0
# Fri, 02 Jul 2021 18:23:28 GMT
ARG ODOO_RELEASE=20210702
# Fri, 02 Jul 2021 18:23:28 GMT
ARG ODOO_SHA=f135b9d4967ef9221ff6aba58b1c4a3ea8334202
# Fri, 02 Jul 2021 18:24:37 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=f135b9d4967ef9221ff6aba58b1c4a3ea8334202
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Jul 2021 18:24:40 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 02 Jul 2021 18:24:40 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Jul 2021 18:24:42 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=f135b9d4967ef9221ff6aba58b1c4a3ea8334202
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Jul 2021 18:24:42 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Jul 2021 18:24:42 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Jul 2021 18:24:42 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Jul 2021 18:24:42 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Jul 2021 18:24:43 GMT
USER odoo
# Fri, 02 Jul 2021 18:24:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jul 2021 18:24:43 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d760ec83e05549c1bafe40d795ed53c471a0208b2e5a5fe29f1f4575e4277ed`  
		Last Modified: Wed, 23 Jun 2021 07:57:34 GMT  
		Size: 207.1 MB (207122080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a6f5407abbe57f2c624e00f8226cb3f74567fc177824c08838c437a8d05fba`  
		Last Modified: Wed, 23 Jun 2021 07:57:03 GMT  
		Size: 2.3 MB (2346852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7db6376102b543b53d50ab5ed822526c9569bbee49c030740510ed71465072`  
		Last Modified: Wed, 23 Jun 2021 07:57:03 GMT  
		Size: 885.8 KB (885845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e888c31054e38d42e49d9a9300e407418f68a9fd57c0939631eeb16590441d55`  
		Last Modified: Fri, 02 Jul 2021 18:27:48 GMT  
		Size: 290.8 MB (290768175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228f78f5139b87d9245dc560367248cdb4cd9c4e3adc6eaf6c4c2924996d6142`  
		Last Modified: Fri, 02 Jul 2021 18:27:16 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a027bd1452b83ce7460764b07ebb6630a972887e1cdf2f0c0c4c448de66bbd2`  
		Last Modified: Fri, 02 Jul 2021 18:27:17 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2febbd7f55a9f3feb53bcdeb1707b9b752f173240e7232979353ca79ea4ddfc`  
		Last Modified: Fri, 02 Jul 2021 18:27:16 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9665050c95eea8f5c3179897ebdc4c2b6f55731e68a3a2651e74b9bab90eefc9`  
		Last Modified: Fri, 02 Jul 2021 18:27:16 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:684f2f2ce756074a0012244defd69d0a57520b14056f338de96423981d8d4ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:3a12a390e066e2b699310e3a5567f44272bbc665d76d184f6acfb353b6e4e2cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.6 MB (515643184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8010c7f4b40de9630e61bb5d26097c0f288290770fce8345f8c030fefa9e6b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:44:56 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 23 Jun 2021 07:44:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 23 Jun 2021 07:44:57 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 07:46:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 23 Jun 2021 07:46:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:46:34 GMT
RUN npm install -g rtlcss
# Wed, 23 Jun 2021 07:46:34 GMT
ENV ODOO_VERSION=14.0
# Fri, 02 Jul 2021 18:22:03 GMT
ARG ODOO_RELEASE=20210702
# Fri, 02 Jul 2021 18:22:03 GMT
ARG ODOO_SHA=03c63a0e755fc4895eeefc97ba7a136bc8d8cde9
# Fri, 02 Jul 2021 18:23:12 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=03c63a0e755fc4895eeefc97ba7a136bc8d8cde9
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Jul 2021 18:23:15 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 02 Jul 2021 18:23:16 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Jul 2021 18:23:17 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=03c63a0e755fc4895eeefc97ba7a136bc8d8cde9
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Jul 2021 18:23:17 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Jul 2021 18:23:17 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Jul 2021 18:23:17 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Jul 2021 18:23:18 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Jul 2021 18:23:18 GMT
USER odoo
# Fri, 02 Jul 2021 18:23:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jul 2021 18:23:18 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80704698691bf3031da85fe60e94cb6d4b0debc3ac2359dd2d707eb4e5681e78`  
		Last Modified: Wed, 23 Jun 2021 07:56:36 GMT  
		Size: 213.2 MB (213171040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc9af296bc1aa9b42af1b6d402cffc8e0ba56cc15906dbf0e7e73b86f00952`  
		Last Modified: Wed, 23 Jun 2021 07:55:49 GMT  
		Size: 2.3 MB (2349730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65481a06fbb9368a1fb401461f0fdeb3a19ce0ef7a7b427d12f614c55ac2527b`  
		Last Modified: Wed, 23 Jun 2021 07:55:49 GMT  
		Size: 885.9 KB (885943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fa3f954253d6924c5ade3613a4146fa9a2f172777e6ab5ad0d953e76620d15`  
		Last Modified: Fri, 02 Jul 2021 18:27:03 GMT  
		Size: 272.1 MB (272088191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df065d4e0f0c0652004835f1a405c73d1f2c7565cf1f70dd20c4e34f531e15e`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b37590a408335014d5be6ebe2f216e9795b9a2d16536aab632adfc6d4e679b65`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c5eb0e450d374263193bbf43220929af579272dbff7411effa58189751bd7`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2b5c697264c418fae0c6519f79098c4ce135286ec3449f616403b5c2c1e17b`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:684f2f2ce756074a0012244defd69d0a57520b14056f338de96423981d8d4ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:3a12a390e066e2b699310e3a5567f44272bbc665d76d184f6acfb353b6e4e2cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.6 MB (515643184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8010c7f4b40de9630e61bb5d26097c0f288290770fce8345f8c030fefa9e6b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:44:56 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 23 Jun 2021 07:44:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 23 Jun 2021 07:44:57 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 07:46:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 23 Jun 2021 07:46:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:46:34 GMT
RUN npm install -g rtlcss
# Wed, 23 Jun 2021 07:46:34 GMT
ENV ODOO_VERSION=14.0
# Fri, 02 Jul 2021 18:22:03 GMT
ARG ODOO_RELEASE=20210702
# Fri, 02 Jul 2021 18:22:03 GMT
ARG ODOO_SHA=03c63a0e755fc4895eeefc97ba7a136bc8d8cde9
# Fri, 02 Jul 2021 18:23:12 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=03c63a0e755fc4895eeefc97ba7a136bc8d8cde9
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Jul 2021 18:23:15 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 02 Jul 2021 18:23:16 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Jul 2021 18:23:17 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=03c63a0e755fc4895eeefc97ba7a136bc8d8cde9
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Jul 2021 18:23:17 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Jul 2021 18:23:17 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Jul 2021 18:23:17 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Jul 2021 18:23:18 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Jul 2021 18:23:18 GMT
USER odoo
# Fri, 02 Jul 2021 18:23:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jul 2021 18:23:18 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80704698691bf3031da85fe60e94cb6d4b0debc3ac2359dd2d707eb4e5681e78`  
		Last Modified: Wed, 23 Jun 2021 07:56:36 GMT  
		Size: 213.2 MB (213171040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc9af296bc1aa9b42af1b6d402cffc8e0ba56cc15906dbf0e7e73b86f00952`  
		Last Modified: Wed, 23 Jun 2021 07:55:49 GMT  
		Size: 2.3 MB (2349730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65481a06fbb9368a1fb401461f0fdeb3a19ce0ef7a7b427d12f614c55ac2527b`  
		Last Modified: Wed, 23 Jun 2021 07:55:49 GMT  
		Size: 885.9 KB (885943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fa3f954253d6924c5ade3613a4146fa9a2f172777e6ab5ad0d953e76620d15`  
		Last Modified: Fri, 02 Jul 2021 18:27:03 GMT  
		Size: 272.1 MB (272088191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df065d4e0f0c0652004835f1a405c73d1f2c7565cf1f70dd20c4e34f531e15e`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b37590a408335014d5be6ebe2f216e9795b9a2d16536aab632adfc6d4e679b65`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c5eb0e450d374263193bbf43220929af579272dbff7411effa58189751bd7`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2b5c697264c418fae0c6519f79098c4ce135286ec3449f616403b5c2c1e17b`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:684f2f2ce756074a0012244defd69d0a57520b14056f338de96423981d8d4ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:3a12a390e066e2b699310e3a5567f44272bbc665d76d184f6acfb353b6e4e2cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.6 MB (515643184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8010c7f4b40de9630e61bb5d26097c0f288290770fce8345f8c030fefa9e6b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:44:56 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 23 Jun 2021 07:44:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 23 Jun 2021 07:44:57 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 07:46:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 23 Jun 2021 07:46:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:46:34 GMT
RUN npm install -g rtlcss
# Wed, 23 Jun 2021 07:46:34 GMT
ENV ODOO_VERSION=14.0
# Fri, 02 Jul 2021 18:22:03 GMT
ARG ODOO_RELEASE=20210702
# Fri, 02 Jul 2021 18:22:03 GMT
ARG ODOO_SHA=03c63a0e755fc4895eeefc97ba7a136bc8d8cde9
# Fri, 02 Jul 2021 18:23:12 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=03c63a0e755fc4895eeefc97ba7a136bc8d8cde9
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Jul 2021 18:23:15 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 02 Jul 2021 18:23:16 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Jul 2021 18:23:17 GMT
# ARGS: ODOO_RELEASE=20210702 ODOO_SHA=03c63a0e755fc4895eeefc97ba7a136bc8d8cde9
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Jul 2021 18:23:17 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Jul 2021 18:23:17 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Jul 2021 18:23:17 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Jul 2021 18:23:18 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Jul 2021 18:23:18 GMT
USER odoo
# Fri, 02 Jul 2021 18:23:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Jul 2021 18:23:18 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80704698691bf3031da85fe60e94cb6d4b0debc3ac2359dd2d707eb4e5681e78`  
		Last Modified: Wed, 23 Jun 2021 07:56:36 GMT  
		Size: 213.2 MB (213171040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc9af296bc1aa9b42af1b6d402cffc8e0ba56cc15906dbf0e7e73b86f00952`  
		Last Modified: Wed, 23 Jun 2021 07:55:49 GMT  
		Size: 2.3 MB (2349730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65481a06fbb9368a1fb401461f0fdeb3a19ce0ef7a7b427d12f614c55ac2527b`  
		Last Modified: Wed, 23 Jun 2021 07:55:49 GMT  
		Size: 885.9 KB (885943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fa3f954253d6924c5ade3613a4146fa9a2f172777e6ab5ad0d953e76620d15`  
		Last Modified: Fri, 02 Jul 2021 18:27:03 GMT  
		Size: 272.1 MB (272088191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df065d4e0f0c0652004835f1a405c73d1f2c7565cf1f70dd20c4e34f531e15e`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b37590a408335014d5be6ebe2f216e9795b9a2d16536aab632adfc6d4e679b65`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c5eb0e450d374263193bbf43220929af579272dbff7411effa58189751bd7`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2b5c697264c418fae0c6519f79098c4ce135286ec3449f616403b5c2c1e17b`  
		Last Modified: Fri, 02 Jul 2021 18:26:31 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
