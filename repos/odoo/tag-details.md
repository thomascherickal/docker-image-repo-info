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
$ docker pull odoo@sha256:fe71b6a2aa1aa8bdfa9e59dfbfbbd1113c03c6138db5375a271eb59af3228e92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:ac98f2f1ff8c481c717b9e7b48ed8f38840d0fcb8d6bee73060839151ea15125
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.1 MB (533088300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c713fc7bb48e25013e2cc25c45b2e631599a89086f87e5dbf1dfa6aa3109bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:31 GMT
ADD file:d4315fd7ceb67a5501410e4392ad3fd73642d6e2490f3626ce20a29321fa3682 in / 
# Wed, 16 Aug 2023 01:00:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:21:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 16 Aug 2023 10:21:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 16 Aug 2023 10:21:48 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 10:23:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 16 Aug 2023 10:23:15 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:23:17 GMT
RUN npm install -g rtlcss
# Wed, 16 Aug 2023 10:23:17 GMT
ENV ODOO_VERSION=14.0
# Fri, 01 Sep 2023 19:27:12 GMT
ARG ODOO_RELEASE=20230901
# Fri, 01 Sep 2023 19:27:12 GMT
ARG ODOO_SHA=0777c849049f346bb6f3f0eb7d544e9d2960d8d8
# Fri, 01 Sep 2023 19:28:34 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=0777c849049f346bb6f3f0eb7d544e9d2960d8d8
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 01 Sep 2023 19:28:37 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 01 Sep 2023 19:28:37 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 01 Sep 2023 19:28:38 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=0777c849049f346bb6f3f0eb7d544e9d2960d8d8
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 01 Sep 2023 19:28:38 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 01 Sep 2023 19:28:38 GMT
EXPOSE 8069 8071 8072
# Fri, 01 Sep 2023 19:28:38 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 01 Sep 2023 19:28:38 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 01 Sep 2023 19:28:38 GMT
USER odoo
# Fri, 01 Sep 2023 19:28:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Sep 2023 19:28:38 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ddade83992f922bd9baa0e67dd5f7e8f518b6ed19c67e2ea076c92a8b38416c0`  
		Last Modified: Wed, 16 Aug 2023 01:05:53 GMT  
		Size: 27.2 MB (27187428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f94b5ed49a5ec953e83f40169b949808c407c931aa7085a46846902af681137`  
		Last Modified: Wed, 16 Aug 2023 10:27:04 GMT  
		Size: 213.2 MB (213180563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc841b610acfd62afebf8a7dee73883ec3020b5a503100b4b133df781a3bd04d`  
		Last Modified: Wed, 16 Aug 2023 10:26:44 GMT  
		Size: 13.5 MB (13522678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497179ab34d276ead4cb01db777028bf342b2339f9089021ec71d1791a5da458`  
		Last Modified: Wed, 16 Aug 2023 10:26:42 GMT  
		Size: 458.9 KB (458875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5839d389e44f92ff8ecf63d11fc6a56e544703ea6731502cff968ddb70e433`  
		Last Modified: Fri, 01 Sep 2023 19:30:57 GMT  
		Size: 278.7 MB (278736291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf77173a3a0b65d846b074f565fe06d39c2ab38093f003e2550df4b0617a17d5`  
		Last Modified: Fri, 01 Sep 2023 19:30:26 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04d1d60a925e2fc6b9afbd69625dee5eecc20b6679c738429cd34dcad470d49`  
		Last Modified: Fri, 01 Sep 2023 19:30:26 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d248fe083da032be0e9c6dc7bc5c2f6fbbb225f2e330a211ccaeea836289ba8`  
		Last Modified: Fri, 01 Sep 2023 19:30:26 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b878783775e5d6c91cbec332d7a901fcc319449268bc82e3232956f4993bc85`  
		Last Modified: Fri, 01 Sep 2023 19:30:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:fe71b6a2aa1aa8bdfa9e59dfbfbbd1113c03c6138db5375a271eb59af3228e92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:ac98f2f1ff8c481c717b9e7b48ed8f38840d0fcb8d6bee73060839151ea15125
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.1 MB (533088300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c713fc7bb48e25013e2cc25c45b2e631599a89086f87e5dbf1dfa6aa3109bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:31 GMT
ADD file:d4315fd7ceb67a5501410e4392ad3fd73642d6e2490f3626ce20a29321fa3682 in / 
# Wed, 16 Aug 2023 01:00:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:21:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 16 Aug 2023 10:21:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 16 Aug 2023 10:21:48 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 10:23:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 16 Aug 2023 10:23:15 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:23:17 GMT
RUN npm install -g rtlcss
# Wed, 16 Aug 2023 10:23:17 GMT
ENV ODOO_VERSION=14.0
# Fri, 01 Sep 2023 19:27:12 GMT
ARG ODOO_RELEASE=20230901
# Fri, 01 Sep 2023 19:27:12 GMT
ARG ODOO_SHA=0777c849049f346bb6f3f0eb7d544e9d2960d8d8
# Fri, 01 Sep 2023 19:28:34 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=0777c849049f346bb6f3f0eb7d544e9d2960d8d8
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 01 Sep 2023 19:28:37 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 01 Sep 2023 19:28:37 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 01 Sep 2023 19:28:38 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=0777c849049f346bb6f3f0eb7d544e9d2960d8d8
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 01 Sep 2023 19:28:38 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 01 Sep 2023 19:28:38 GMT
EXPOSE 8069 8071 8072
# Fri, 01 Sep 2023 19:28:38 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 01 Sep 2023 19:28:38 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 01 Sep 2023 19:28:38 GMT
USER odoo
# Fri, 01 Sep 2023 19:28:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Sep 2023 19:28:38 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ddade83992f922bd9baa0e67dd5f7e8f518b6ed19c67e2ea076c92a8b38416c0`  
		Last Modified: Wed, 16 Aug 2023 01:05:53 GMT  
		Size: 27.2 MB (27187428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f94b5ed49a5ec953e83f40169b949808c407c931aa7085a46846902af681137`  
		Last Modified: Wed, 16 Aug 2023 10:27:04 GMT  
		Size: 213.2 MB (213180563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc841b610acfd62afebf8a7dee73883ec3020b5a503100b4b133df781a3bd04d`  
		Last Modified: Wed, 16 Aug 2023 10:26:44 GMT  
		Size: 13.5 MB (13522678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497179ab34d276ead4cb01db777028bf342b2339f9089021ec71d1791a5da458`  
		Last Modified: Wed, 16 Aug 2023 10:26:42 GMT  
		Size: 458.9 KB (458875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5839d389e44f92ff8ecf63d11fc6a56e544703ea6731502cff968ddb70e433`  
		Last Modified: Fri, 01 Sep 2023 19:30:57 GMT  
		Size: 278.7 MB (278736291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf77173a3a0b65d846b074f565fe06d39c2ab38093f003e2550df4b0617a17d5`  
		Last Modified: Fri, 01 Sep 2023 19:30:26 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04d1d60a925e2fc6b9afbd69625dee5eecc20b6679c738429cd34dcad470d49`  
		Last Modified: Fri, 01 Sep 2023 19:30:26 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d248fe083da032be0e9c6dc7bc5c2f6fbbb225f2e330a211ccaeea836289ba8`  
		Last Modified: Fri, 01 Sep 2023 19:30:26 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b878783775e5d6c91cbec332d7a901fcc319449268bc82e3232956f4993bc85`  
		Last Modified: Fri, 01 Sep 2023 19:30:26 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:f6dc10955ff8d1f76ef7b52ce7f63aa6310bd992ef4e45d5f8f2e0d16310d1fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:5cf57d8c0c02767e4edc677565af5aea893bbd51def54c35c8432663d860159c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.2 MB (562175249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a70c181c01528523156993f23bf66e7cbf1618f9d3420145cb0a2ce2ba841ffa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:16:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 16 Aug 2023 10:16:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 16 Aug 2023 10:16:30 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 10:20:15 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 16 Aug 2023 10:20:22 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:20:23 GMT
RUN npm install -g rtlcss
# Wed, 16 Aug 2023 10:20:24 GMT
ENV ODOO_VERSION=15.0
# Fri, 01 Sep 2023 19:25:48 GMT
ARG ODOO_RELEASE=20230901
# Fri, 01 Sep 2023 19:25:48 GMT
ARG ODOO_SHA=22553b2cb576c94801b6b1180c55e6d6d29de338
# Fri, 01 Sep 2023 19:27:03 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=22553b2cb576c94801b6b1180c55e6d6d29de338
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 01 Sep 2023 19:27:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 01 Sep 2023 19:27:07 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 01 Sep 2023 19:27:08 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=22553b2cb576c94801b6b1180c55e6d6d29de338
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 01 Sep 2023 19:27:08 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 01 Sep 2023 19:27:08 GMT
EXPOSE 8069 8071 8072
# Fri, 01 Sep 2023 19:27:08 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 01 Sep 2023 19:27:08 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 01 Sep 2023 19:27:08 GMT
USER odoo
# Fri, 01 Sep 2023 19:27:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Sep 2023 19:27:09 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18e6ccd242f394f129dfb1542a55693c092efc01323daf560f2cea9f7c93f9d`  
		Last Modified: Wed, 16 Aug 2023 10:26:21 GMT  
		Size: 220.3 MB (220302753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8225239de85406993faad4ed5848d1f01aadf58ffcb88de9ba6cbee36f6eff`  
		Last Modified: Wed, 16 Aug 2023 10:25:57 GMT  
		Size: 2.6 MB (2576533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf486b5a74cf8335fb645fe6c165ce01e7422386abffef6f5874c9353e969af6`  
		Last Modified: Wed, 16 Aug 2023 10:25:57 GMT  
		Size: 454.4 KB (454433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc107a2fae9d8b3925c149de7e67e6511d8291d2458bf1b934c38c733141d8`  
		Last Modified: Fri, 01 Sep 2023 19:30:17 GMT  
		Size: 307.4 MB (307421387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed41e70fd7d470c8ce4cf56e38a55f6176c356347c75125670e78fd38e2b0eb9`  
		Last Modified: Fri, 01 Sep 2023 19:29:44 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a34a11248960f4a02adea2210e8a0e4ee3bdc285b3ecd99828d680e0a3594b`  
		Last Modified: Fri, 01 Sep 2023 19:29:44 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2314dea4e178b49849832f6ccf0356ab85c630cb783fdc2a0e48b8a5bc660b11`  
		Last Modified: Fri, 01 Sep 2023 19:29:44 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18e628fc3ad46ef4ffca0a3103c053968bc842940d50bcb5459de3c774ce54b`  
		Last Modified: Fri, 01 Sep 2023 19:29:44 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:f6dc10955ff8d1f76ef7b52ce7f63aa6310bd992ef4e45d5f8f2e0d16310d1fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:5cf57d8c0c02767e4edc677565af5aea893bbd51def54c35c8432663d860159c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.2 MB (562175249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a70c181c01528523156993f23bf66e7cbf1618f9d3420145cb0a2ce2ba841ffa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:16:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 16 Aug 2023 10:16:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 16 Aug 2023 10:16:30 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 10:20:15 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 16 Aug 2023 10:20:22 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:20:23 GMT
RUN npm install -g rtlcss
# Wed, 16 Aug 2023 10:20:24 GMT
ENV ODOO_VERSION=15.0
# Fri, 01 Sep 2023 19:25:48 GMT
ARG ODOO_RELEASE=20230901
# Fri, 01 Sep 2023 19:25:48 GMT
ARG ODOO_SHA=22553b2cb576c94801b6b1180c55e6d6d29de338
# Fri, 01 Sep 2023 19:27:03 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=22553b2cb576c94801b6b1180c55e6d6d29de338
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 01 Sep 2023 19:27:07 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 01 Sep 2023 19:27:07 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 01 Sep 2023 19:27:08 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=22553b2cb576c94801b6b1180c55e6d6d29de338
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 01 Sep 2023 19:27:08 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 01 Sep 2023 19:27:08 GMT
EXPOSE 8069 8071 8072
# Fri, 01 Sep 2023 19:27:08 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 01 Sep 2023 19:27:08 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 01 Sep 2023 19:27:08 GMT
USER odoo
# Fri, 01 Sep 2023 19:27:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Sep 2023 19:27:09 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18e6ccd242f394f129dfb1542a55693c092efc01323daf560f2cea9f7c93f9d`  
		Last Modified: Wed, 16 Aug 2023 10:26:21 GMT  
		Size: 220.3 MB (220302753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8225239de85406993faad4ed5848d1f01aadf58ffcb88de9ba6cbee36f6eff`  
		Last Modified: Wed, 16 Aug 2023 10:25:57 GMT  
		Size: 2.6 MB (2576533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf486b5a74cf8335fb645fe6c165ce01e7422386abffef6f5874c9353e969af6`  
		Last Modified: Wed, 16 Aug 2023 10:25:57 GMT  
		Size: 454.4 KB (454433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc107a2fae9d8b3925c149de7e67e6511d8291d2458bf1b934c38c733141d8`  
		Last Modified: Fri, 01 Sep 2023 19:30:17 GMT  
		Size: 307.4 MB (307421387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed41e70fd7d470c8ce4cf56e38a55f6176c356347c75125670e78fd38e2b0eb9`  
		Last Modified: Fri, 01 Sep 2023 19:29:44 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a34a11248960f4a02adea2210e8a0e4ee3bdc285b3ecd99828d680e0a3594b`  
		Last Modified: Fri, 01 Sep 2023 19:29:44 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2314dea4e178b49849832f6ccf0356ab85c630cb783fdc2a0e48b8a5bc660b11`  
		Last Modified: Fri, 01 Sep 2023 19:29:44 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18e628fc3ad46ef4ffca0a3103c053968bc842940d50bcb5459de3c774ce54b`  
		Last Modified: Fri, 01 Sep 2023 19:29:44 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:156744992a8b7fca37ac120a78885b3375fe757f3262a1c76496b96f84b658ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:5f4f87d99eb68f6487dfccfc59ea130378dcdd7d52b42e8f6f00031db09ab037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.3 MB (576261332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a8eadb505e031fc9c95ac7ce211683f3f2568e81aa20be7df2c95fb8155f23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:16:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 16 Aug 2023 10:16:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 16 Aug 2023 10:16:30 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 10:17:35 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 16 Aug 2023 10:17:43 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:17:44 GMT
RUN npm install -g rtlcss
# Wed, 16 Aug 2023 10:17:44 GMT
ENV ODOO_VERSION=16.0
# Fri, 01 Sep 2023 19:24:10 GMT
ARG ODOO_RELEASE=20230901
# Fri, 01 Sep 2023 19:24:10 GMT
ARG ODOO_SHA=2287a32457f8d26405b7203820c54dc112a4537d
# Fri, 01 Sep 2023 19:25:33 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=2287a32457f8d26405b7203820c54dc112a4537d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 01 Sep 2023 19:25:38 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 01 Sep 2023 19:25:38 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 01 Sep 2023 19:25:38 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=2287a32457f8d26405b7203820c54dc112a4537d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 01 Sep 2023 19:25:38 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 01 Sep 2023 19:25:39 GMT
EXPOSE 8069 8071 8072
# Fri, 01 Sep 2023 19:25:39 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 01 Sep 2023 19:25:39 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 01 Sep 2023 19:25:39 GMT
USER odoo
# Fri, 01 Sep 2023 19:25:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Sep 2023 19:25:39 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38faf7b926f64bb75adbf63bb8f9cf962e9fe7240f1b77f975713e522fb38f2f`  
		Last Modified: Wed, 16 Aug 2023 10:25:32 GMT  
		Size: 221.0 MB (220992472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f422a2822ff3c0ddcb0feae90917ad16bfadc792ed6120bb85ec478c192fc14`  
		Last Modified: Wed, 16 Aug 2023 10:25:08 GMT  
		Size: 2.6 MB (2579930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e455fdc49a2fa9b84da301d6cacd3ac952037699a291e871cd86ab33ff34b4`  
		Last Modified: Wed, 16 Aug 2023 10:25:08 GMT  
		Size: 454.4 KB (454421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48fd8a9318858cec18a1a03898de2d5aba0be2d4504f8eab870997bfef32931`  
		Last Modified: Fri, 01 Sep 2023 19:29:33 GMT  
		Size: 320.8 MB (320814369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cb9474d7f3df483b5799c91399dd2248b68ee421ad0e5c5c086488c62b2eb1`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1332ca861c89763f99cdda917a3ae85bccfa3b616e919c1fe90fa5c18cecc3`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a14024af035aff7dcecde6f32f22598d01ff8001a1e67caec94834e1e848d9`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50853cb11cd6692fba52c2b6c17e07b49cb5982cafa5e8f0af594b6f25416032`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:156744992a8b7fca37ac120a78885b3375fe757f3262a1c76496b96f84b658ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:5f4f87d99eb68f6487dfccfc59ea130378dcdd7d52b42e8f6f00031db09ab037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.3 MB (576261332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a8eadb505e031fc9c95ac7ce211683f3f2568e81aa20be7df2c95fb8155f23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:16:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 16 Aug 2023 10:16:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 16 Aug 2023 10:16:30 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 10:17:35 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 16 Aug 2023 10:17:43 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:17:44 GMT
RUN npm install -g rtlcss
# Wed, 16 Aug 2023 10:17:44 GMT
ENV ODOO_VERSION=16.0
# Fri, 01 Sep 2023 19:24:10 GMT
ARG ODOO_RELEASE=20230901
# Fri, 01 Sep 2023 19:24:10 GMT
ARG ODOO_SHA=2287a32457f8d26405b7203820c54dc112a4537d
# Fri, 01 Sep 2023 19:25:33 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=2287a32457f8d26405b7203820c54dc112a4537d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 01 Sep 2023 19:25:38 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 01 Sep 2023 19:25:38 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 01 Sep 2023 19:25:38 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=2287a32457f8d26405b7203820c54dc112a4537d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 01 Sep 2023 19:25:38 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 01 Sep 2023 19:25:39 GMT
EXPOSE 8069 8071 8072
# Fri, 01 Sep 2023 19:25:39 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 01 Sep 2023 19:25:39 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 01 Sep 2023 19:25:39 GMT
USER odoo
# Fri, 01 Sep 2023 19:25:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Sep 2023 19:25:39 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38faf7b926f64bb75adbf63bb8f9cf962e9fe7240f1b77f975713e522fb38f2f`  
		Last Modified: Wed, 16 Aug 2023 10:25:32 GMT  
		Size: 221.0 MB (220992472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f422a2822ff3c0ddcb0feae90917ad16bfadc792ed6120bb85ec478c192fc14`  
		Last Modified: Wed, 16 Aug 2023 10:25:08 GMT  
		Size: 2.6 MB (2579930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e455fdc49a2fa9b84da301d6cacd3ac952037699a291e871cd86ab33ff34b4`  
		Last Modified: Wed, 16 Aug 2023 10:25:08 GMT  
		Size: 454.4 KB (454421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48fd8a9318858cec18a1a03898de2d5aba0be2d4504f8eab870997bfef32931`  
		Last Modified: Fri, 01 Sep 2023 19:29:33 GMT  
		Size: 320.8 MB (320814369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cb9474d7f3df483b5799c91399dd2248b68ee421ad0e5c5c086488c62b2eb1`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1332ca861c89763f99cdda917a3ae85bccfa3b616e919c1fe90fa5c18cecc3`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a14024af035aff7dcecde6f32f22598d01ff8001a1e67caec94834e1e848d9`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50853cb11cd6692fba52c2b6c17e07b49cb5982cafa5e8f0af594b6f25416032`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:156744992a8b7fca37ac120a78885b3375fe757f3262a1c76496b96f84b658ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:5f4f87d99eb68f6487dfccfc59ea130378dcdd7d52b42e8f6f00031db09ab037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.3 MB (576261332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a8eadb505e031fc9c95ac7ce211683f3f2568e81aa20be7df2c95fb8155f23`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:16:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 16 Aug 2023 10:16:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 16 Aug 2023 10:16:30 GMT
ENV LANG=C.UTF-8
# Wed, 16 Aug 2023 10:17:35 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 16 Aug 2023 10:17:43 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:17:44 GMT
RUN npm install -g rtlcss
# Wed, 16 Aug 2023 10:17:44 GMT
ENV ODOO_VERSION=16.0
# Fri, 01 Sep 2023 19:24:10 GMT
ARG ODOO_RELEASE=20230901
# Fri, 01 Sep 2023 19:24:10 GMT
ARG ODOO_SHA=2287a32457f8d26405b7203820c54dc112a4537d
# Fri, 01 Sep 2023 19:25:33 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=2287a32457f8d26405b7203820c54dc112a4537d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 01 Sep 2023 19:25:38 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 01 Sep 2023 19:25:38 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 01 Sep 2023 19:25:38 GMT
# ARGS: ODOO_RELEASE=20230901 ODOO_SHA=2287a32457f8d26405b7203820c54dc112a4537d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 01 Sep 2023 19:25:38 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 01 Sep 2023 19:25:39 GMT
EXPOSE 8069 8071 8072
# Fri, 01 Sep 2023 19:25:39 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 01 Sep 2023 19:25:39 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 01 Sep 2023 19:25:39 GMT
USER odoo
# Fri, 01 Sep 2023 19:25:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Sep 2023 19:25:39 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38faf7b926f64bb75adbf63bb8f9cf962e9fe7240f1b77f975713e522fb38f2f`  
		Last Modified: Wed, 16 Aug 2023 10:25:32 GMT  
		Size: 221.0 MB (220992472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f422a2822ff3c0ddcb0feae90917ad16bfadc792ed6120bb85ec478c192fc14`  
		Last Modified: Wed, 16 Aug 2023 10:25:08 GMT  
		Size: 2.6 MB (2579930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e455fdc49a2fa9b84da301d6cacd3ac952037699a291e871cd86ab33ff34b4`  
		Last Modified: Wed, 16 Aug 2023 10:25:08 GMT  
		Size: 454.4 KB (454421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48fd8a9318858cec18a1a03898de2d5aba0be2d4504f8eab870997bfef32931`  
		Last Modified: Fri, 01 Sep 2023 19:29:33 GMT  
		Size: 320.8 MB (320814369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cb9474d7f3df483b5799c91399dd2248b68ee421ad0e5c5c086488c62b2eb1`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1332ca861c89763f99cdda917a3ae85bccfa3b616e919c1fe90fa5c18cecc3`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a14024af035aff7dcecde6f32f22598d01ff8001a1e67caec94834e1e848d9`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50853cb11cd6692fba52c2b6c17e07b49cb5982cafa5e8f0af594b6f25416032`  
		Last Modified: Fri, 01 Sep 2023 19:28:57 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
