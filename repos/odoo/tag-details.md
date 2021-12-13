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
$ docker pull odoo@sha256:10730b186e2854c680893495201f1cce31b7f49cda4073f1d0b53ea1e564f31b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:f264e50369280b3ec9b4540bdab2b5955a96f1f81ac097f78fb60e1b973e52dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.4 MB (539395462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d964cd058eb4e42dd39bc26439e8fc356d195658058443d89b38458102e7df4b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:24:44 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 02 Dec 2021 03:24:45 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 02 Dec 2021 03:24:45 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 03:29:05 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 02 Dec 2021 03:29:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:29:34 GMT
RUN npm install -g rtlcss
# Thu, 02 Dec 2021 03:29:34 GMT
ENV ODOO_VERSION=13.0
# Mon, 13 Dec 2021 19:40:11 GMT
ARG ODOO_RELEASE=20211213
# Mon, 13 Dec 2021 19:40:11 GMT
ARG ODOO_SHA=acbb9ee40e8998751d9eb632444c1fc1e105766d
# Mon, 13 Dec 2021 19:41:39 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=acbb9ee40e8998751d9eb632444c1fc1e105766d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Dec 2021 19:41:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Dec 2021 19:41:43 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Dec 2021 19:41:44 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=acbb9ee40e8998751d9eb632444c1fc1e105766d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Dec 2021 19:41:44 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Dec 2021 19:41:44 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Dec 2021 19:41:44 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Dec 2021 19:41:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Dec 2021 19:41:45 GMT
USER odoo
# Mon, 13 Dec 2021 19:41:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Dec 2021 19:41:45 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8988f86f949d08f5ea393c3cb9d4016acd45699f4fb9c3b6a78c8b107d9be55`  
		Last Modified: Thu, 02 Dec 2021 03:34:31 GMT  
		Size: 207.1 MB (207130653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78dd91afcfb205b31d583947328c09101f9c1a292ee4ab5357b9cc5c12a691c`  
		Last Modified: Thu, 02 Dec 2021 03:33:57 GMT  
		Size: 13.4 MB (13434259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c875e5005d33be86db39c7b664080d0b957d3d88521bd5d30b592382eddeea0e`  
		Last Modified: Thu, 02 Dec 2021 03:33:52 GMT  
		Size: 425.0 KB (424962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4991968f744bc2ab83923ee017198a2af22a14039ce5ee18b7b332992414299e`  
		Last Modified: Mon, 13 Dec 2021 19:44:07 GMT  
		Size: 291.2 MB (291249393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40092472066a216884270be267a54c3faab88f6060865fb2daab32e8c3a6879e`  
		Last Modified: Mon, 13 Dec 2021 19:43:33 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676c87f3451a8e360980612151b66f2ec9534787ae3bebe793eee33858a147c0`  
		Last Modified: Mon, 13 Dec 2021 19:43:33 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47459f85fd00e4d3c5a1e8ccceded8edd1b8a3ed61a5c4f47c10700323cc3fbd`  
		Last Modified: Mon, 13 Dec 2021 19:43:33 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab2e45b355cfda5e686b4e65fa5b1e6e38a51fabc1a7aec9de0cead3cbce676`  
		Last Modified: Mon, 13 Dec 2021 19:43:33 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:10730b186e2854c680893495201f1cce31b7f49cda4073f1d0b53ea1e564f31b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:f264e50369280b3ec9b4540bdab2b5955a96f1f81ac097f78fb60e1b973e52dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.4 MB (539395462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d964cd058eb4e42dd39bc26439e8fc356d195658058443d89b38458102e7df4b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:24:44 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 02 Dec 2021 03:24:45 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 02 Dec 2021 03:24:45 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 03:29:05 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 02 Dec 2021 03:29:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:29:34 GMT
RUN npm install -g rtlcss
# Thu, 02 Dec 2021 03:29:34 GMT
ENV ODOO_VERSION=13.0
# Mon, 13 Dec 2021 19:40:11 GMT
ARG ODOO_RELEASE=20211213
# Mon, 13 Dec 2021 19:40:11 GMT
ARG ODOO_SHA=acbb9ee40e8998751d9eb632444c1fc1e105766d
# Mon, 13 Dec 2021 19:41:39 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=acbb9ee40e8998751d9eb632444c1fc1e105766d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Dec 2021 19:41:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Dec 2021 19:41:43 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Dec 2021 19:41:44 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=acbb9ee40e8998751d9eb632444c1fc1e105766d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Dec 2021 19:41:44 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Dec 2021 19:41:44 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Dec 2021 19:41:44 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Dec 2021 19:41:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Dec 2021 19:41:45 GMT
USER odoo
# Mon, 13 Dec 2021 19:41:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Dec 2021 19:41:45 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8988f86f949d08f5ea393c3cb9d4016acd45699f4fb9c3b6a78c8b107d9be55`  
		Last Modified: Thu, 02 Dec 2021 03:34:31 GMT  
		Size: 207.1 MB (207130653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78dd91afcfb205b31d583947328c09101f9c1a292ee4ab5357b9cc5c12a691c`  
		Last Modified: Thu, 02 Dec 2021 03:33:57 GMT  
		Size: 13.4 MB (13434259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c875e5005d33be86db39c7b664080d0b957d3d88521bd5d30b592382eddeea0e`  
		Last Modified: Thu, 02 Dec 2021 03:33:52 GMT  
		Size: 425.0 KB (424962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4991968f744bc2ab83923ee017198a2af22a14039ce5ee18b7b332992414299e`  
		Last Modified: Mon, 13 Dec 2021 19:44:07 GMT  
		Size: 291.2 MB (291249393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40092472066a216884270be267a54c3faab88f6060865fb2daab32e8c3a6879e`  
		Last Modified: Mon, 13 Dec 2021 19:43:33 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676c87f3451a8e360980612151b66f2ec9534787ae3bebe793eee33858a147c0`  
		Last Modified: Mon, 13 Dec 2021 19:43:33 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47459f85fd00e4d3c5a1e8ccceded8edd1b8a3ed61a5c4f47c10700323cc3fbd`  
		Last Modified: Mon, 13 Dec 2021 19:43:33 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab2e45b355cfda5e686b4e65fa5b1e6e38a51fabc1a7aec9de0cead3cbce676`  
		Last Modified: Mon, 13 Dec 2021 19:43:33 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:16194b4d8ff41721ee1a1da22641ae2f9fd1aa4ad96f51cc5957d155ff1eeded
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:d11e2af3e97d5767c13cadb37d415dc4806a47484c2d55013e851c4ac1ed59aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.1 MB (529103461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac9a2565ea509b7e2acc70d360394b92b1775b1a00dd749464865b8c874a462f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:24:44 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 02 Dec 2021 03:24:45 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 02 Dec 2021 03:24:45 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 03:26:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 02 Dec 2021 03:26:23 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:26:27 GMT
RUN npm install -g rtlcss
# Thu, 02 Dec 2021 03:26:27 GMT
ENV ODOO_VERSION=14.0
# Mon, 13 Dec 2021 19:38:33 GMT
ARG ODOO_RELEASE=20211213
# Mon, 13 Dec 2021 19:38:33 GMT
ARG ODOO_SHA=fbd8ce32d2949e11f83453759c5f41ba89ed8f2c
# Mon, 13 Dec 2021 19:39:54 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=fbd8ce32d2949e11f83453759c5f41ba89ed8f2c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Dec 2021 19:39:58 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Dec 2021 19:39:59 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Dec 2021 19:40:00 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=fbd8ce32d2949e11f83453759c5f41ba89ed8f2c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Dec 2021 19:40:00 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Dec 2021 19:40:00 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Dec 2021 19:40:00 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Dec 2021 19:40:00 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Dec 2021 19:40:01 GMT
USER odoo
# Mon, 13 Dec 2021 19:40:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Dec 2021 19:40:01 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc20adace522abb201c7423e22fd72bcb79776eea50c16f27d7304e0ef69a17`  
		Last Modified: Thu, 02 Dec 2021 03:33:31 GMT  
		Size: 213.2 MB (213172687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864e4021f806774779a9ca1a51ef676584c0ebfe979b016930caa5019dbebe2`  
		Last Modified: Thu, 02 Dec 2021 03:32:56 GMT  
		Size: 13.4 MB (13436533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c504b4f0face0abb0105469a79f865565c73340c11e0eb38cf2f615bd7f3ff60`  
		Last Modified: Thu, 02 Dec 2021 03:32:52 GMT  
		Size: 424.9 KB (424854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be485a85f8634dd287d7403d5780442c32dceae599c14ce506f9622cf23ec292`  
		Last Modified: Mon, 13 Dec 2021 19:43:22 GMT  
		Size: 274.9 MB (274913197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97288879706f7e522cee94afbdfa8f8950ffc2b6f4837faedaee26d04a616c5d`  
		Last Modified: Mon, 13 Dec 2021 19:42:48 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57fd906b1d05fbfc8999bcdfe0eff5983502a3db62ba73111d510f6601c23db`  
		Last Modified: Mon, 13 Dec 2021 19:42:48 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13566163a4155255293ba8269155324e5dbde73566f87493827b106c04a5b13`  
		Last Modified: Mon, 13 Dec 2021 19:42:48 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669097fb8418498b860d6a9976bf18044c6075d5e256c86e328d7d48203cbf46`  
		Last Modified: Mon, 13 Dec 2021 19:42:48 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:16194b4d8ff41721ee1a1da22641ae2f9fd1aa4ad96f51cc5957d155ff1eeded
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:d11e2af3e97d5767c13cadb37d415dc4806a47484c2d55013e851c4ac1ed59aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.1 MB (529103461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac9a2565ea509b7e2acc70d360394b92b1775b1a00dd749464865b8c874a462f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:24:44 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 02 Dec 2021 03:24:45 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 02 Dec 2021 03:24:45 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 03:26:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 02 Dec 2021 03:26:23 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:26:27 GMT
RUN npm install -g rtlcss
# Thu, 02 Dec 2021 03:26:27 GMT
ENV ODOO_VERSION=14.0
# Mon, 13 Dec 2021 19:38:33 GMT
ARG ODOO_RELEASE=20211213
# Mon, 13 Dec 2021 19:38:33 GMT
ARG ODOO_SHA=fbd8ce32d2949e11f83453759c5f41ba89ed8f2c
# Mon, 13 Dec 2021 19:39:54 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=fbd8ce32d2949e11f83453759c5f41ba89ed8f2c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Dec 2021 19:39:58 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Dec 2021 19:39:59 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Dec 2021 19:40:00 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=fbd8ce32d2949e11f83453759c5f41ba89ed8f2c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Dec 2021 19:40:00 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Dec 2021 19:40:00 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Dec 2021 19:40:00 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Dec 2021 19:40:00 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Dec 2021 19:40:01 GMT
USER odoo
# Mon, 13 Dec 2021 19:40:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Dec 2021 19:40:01 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc20adace522abb201c7423e22fd72bcb79776eea50c16f27d7304e0ef69a17`  
		Last Modified: Thu, 02 Dec 2021 03:33:31 GMT  
		Size: 213.2 MB (213172687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864e4021f806774779a9ca1a51ef676584c0ebfe979b016930caa5019dbebe2`  
		Last Modified: Thu, 02 Dec 2021 03:32:56 GMT  
		Size: 13.4 MB (13436533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c504b4f0face0abb0105469a79f865565c73340c11e0eb38cf2f615bd7f3ff60`  
		Last Modified: Thu, 02 Dec 2021 03:32:52 GMT  
		Size: 424.9 KB (424854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be485a85f8634dd287d7403d5780442c32dceae599c14ce506f9622cf23ec292`  
		Last Modified: Mon, 13 Dec 2021 19:43:22 GMT  
		Size: 274.9 MB (274913197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97288879706f7e522cee94afbdfa8f8950ffc2b6f4837faedaee26d04a616c5d`  
		Last Modified: Mon, 13 Dec 2021 19:42:48 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57fd906b1d05fbfc8999bcdfe0eff5983502a3db62ba73111d510f6601c23db`  
		Last Modified: Mon, 13 Dec 2021 19:42:48 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13566163a4155255293ba8269155324e5dbde73566f87493827b106c04a5b13`  
		Last Modified: Mon, 13 Dec 2021 19:42:48 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669097fb8418498b860d6a9976bf18044c6075d5e256c86e328d7d48203cbf46`  
		Last Modified: Mon, 13 Dec 2021 19:42:48 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:8062c21adb0a4e3200cf8e42408cf961201048f5ae088cf47b628a8274226db0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:5cce551c5487110902e55a7755f52a59e42bb518fd8a82a78f1dac5f2bf2c8e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **546.2 MB (546212190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0cf722c9692cc9b9a43016f6eca636640254a1138b05c516c22e60246e6df06`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:21:36 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 02 Dec 2021 03:21:37 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 02 Dec 2021 03:21:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 03:22:43 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 02 Dec 2021 03:23:01 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:23:04 GMT
RUN npm install -g rtlcss
# Thu, 02 Dec 2021 03:23:04 GMT
ENV ODOO_VERSION=15.0
# Mon, 13 Dec 2021 19:36:55 GMT
ARG ODOO_RELEASE=20211213
# Mon, 13 Dec 2021 19:36:55 GMT
ARG ODOO_SHA=b95ff701609710b8d11a63a7feca2129c01193c0
# Mon, 13 Dec 2021 19:38:11 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=b95ff701609710b8d11a63a7feca2129c01193c0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Dec 2021 19:38:15 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Dec 2021 19:38:15 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Dec 2021 19:38:16 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=b95ff701609710b8d11a63a7feca2129c01193c0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Dec 2021 19:38:16 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Dec 2021 19:38:16 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Dec 2021 19:38:17 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Dec 2021 19:38:17 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Dec 2021 19:38:17 GMT
USER odoo
# Mon, 13 Dec 2021 19:38:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Dec 2021 19:38:17 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8928362baaf188d2d35b07907f7df5a83838f416511d7c90d1001f0f69b22d`  
		Last Modified: Thu, 02 Dec 2021 03:32:31 GMT  
		Size: 220.3 MB (220290298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1196c36b7759c2bc3f823f01785a679ef74915d5281b24e23220cfac4fb643c`  
		Last Modified: Thu, 02 Dec 2021 03:31:45 GMT  
		Size: 2.5 MB (2506050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014833e3ecaf723c362d63385e2ff1ece9d0f33f6818690c2ffb8acbbc320186`  
		Last Modified: Thu, 02 Dec 2021 03:31:45 GMT  
		Size: 417.8 KB (417795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47ba6bcf217c53bb47d74cd3b7d658bef87942db4626cf2e9f387cb3f530719`  
		Last Modified: Mon, 13 Dec 2021 19:42:34 GMT  
		Size: 291.6 MB (291625365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2cb6d340eb30e83ae63c6eca61b5f2b867e7ca4c9604af18c0e40b9546263c`  
		Last Modified: Mon, 13 Dec 2021 19:42:00 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:929ffb6475af451c610194953dea2840ce8fdfc019b8ce5d4abed12caceab3d2`  
		Last Modified: Mon, 13 Dec 2021 19:42:01 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dce199b6b093ee9c82d891f20b52bfb1f40cebbdca994a70564eacc795fe2b0`  
		Last Modified: Mon, 13 Dec 2021 19:42:00 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1a3c709fb69fd910bad9716caf7fd17bef03d4bad8347c0f59f5ea4ba70937`  
		Last Modified: Mon, 13 Dec 2021 19:42:00 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:8062c21adb0a4e3200cf8e42408cf961201048f5ae088cf47b628a8274226db0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:5cce551c5487110902e55a7755f52a59e42bb518fd8a82a78f1dac5f2bf2c8e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **546.2 MB (546212190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0cf722c9692cc9b9a43016f6eca636640254a1138b05c516c22e60246e6df06`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:21:36 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 02 Dec 2021 03:21:37 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 02 Dec 2021 03:21:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 03:22:43 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 02 Dec 2021 03:23:01 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:23:04 GMT
RUN npm install -g rtlcss
# Thu, 02 Dec 2021 03:23:04 GMT
ENV ODOO_VERSION=15.0
# Mon, 13 Dec 2021 19:36:55 GMT
ARG ODOO_RELEASE=20211213
# Mon, 13 Dec 2021 19:36:55 GMT
ARG ODOO_SHA=b95ff701609710b8d11a63a7feca2129c01193c0
# Mon, 13 Dec 2021 19:38:11 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=b95ff701609710b8d11a63a7feca2129c01193c0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Dec 2021 19:38:15 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Dec 2021 19:38:15 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Dec 2021 19:38:16 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=b95ff701609710b8d11a63a7feca2129c01193c0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Dec 2021 19:38:16 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Dec 2021 19:38:16 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Dec 2021 19:38:17 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Dec 2021 19:38:17 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Dec 2021 19:38:17 GMT
USER odoo
# Mon, 13 Dec 2021 19:38:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Dec 2021 19:38:17 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8928362baaf188d2d35b07907f7df5a83838f416511d7c90d1001f0f69b22d`  
		Last Modified: Thu, 02 Dec 2021 03:32:31 GMT  
		Size: 220.3 MB (220290298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1196c36b7759c2bc3f823f01785a679ef74915d5281b24e23220cfac4fb643c`  
		Last Modified: Thu, 02 Dec 2021 03:31:45 GMT  
		Size: 2.5 MB (2506050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014833e3ecaf723c362d63385e2ff1ece9d0f33f6818690c2ffb8acbbc320186`  
		Last Modified: Thu, 02 Dec 2021 03:31:45 GMT  
		Size: 417.8 KB (417795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47ba6bcf217c53bb47d74cd3b7d658bef87942db4626cf2e9f387cb3f530719`  
		Last Modified: Mon, 13 Dec 2021 19:42:34 GMT  
		Size: 291.6 MB (291625365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2cb6d340eb30e83ae63c6eca61b5f2b867e7ca4c9604af18c0e40b9546263c`  
		Last Modified: Mon, 13 Dec 2021 19:42:00 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:929ffb6475af451c610194953dea2840ce8fdfc019b8ce5d4abed12caceab3d2`  
		Last Modified: Mon, 13 Dec 2021 19:42:01 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dce199b6b093ee9c82d891f20b52bfb1f40cebbdca994a70564eacc795fe2b0`  
		Last Modified: Mon, 13 Dec 2021 19:42:00 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1a3c709fb69fd910bad9716caf7fd17bef03d4bad8347c0f59f5ea4ba70937`  
		Last Modified: Mon, 13 Dec 2021 19:42:00 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:8062c21adb0a4e3200cf8e42408cf961201048f5ae088cf47b628a8274226db0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:5cce551c5487110902e55a7755f52a59e42bb518fd8a82a78f1dac5f2bf2c8e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **546.2 MB (546212190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0cf722c9692cc9b9a43016f6eca636640254a1138b05c516c22e60246e6df06`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:21:36 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 02 Dec 2021 03:21:37 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 02 Dec 2021 03:21:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 03:22:43 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 02 Dec 2021 03:23:01 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:23:04 GMT
RUN npm install -g rtlcss
# Thu, 02 Dec 2021 03:23:04 GMT
ENV ODOO_VERSION=15.0
# Mon, 13 Dec 2021 19:36:55 GMT
ARG ODOO_RELEASE=20211213
# Mon, 13 Dec 2021 19:36:55 GMT
ARG ODOO_SHA=b95ff701609710b8d11a63a7feca2129c01193c0
# Mon, 13 Dec 2021 19:38:11 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=b95ff701609710b8d11a63a7feca2129c01193c0
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Dec 2021 19:38:15 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Dec 2021 19:38:15 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Dec 2021 19:38:16 GMT
# ARGS: ODOO_RELEASE=20211213 ODOO_SHA=b95ff701609710b8d11a63a7feca2129c01193c0
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Dec 2021 19:38:16 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Dec 2021 19:38:16 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Dec 2021 19:38:17 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Dec 2021 19:38:17 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Dec 2021 19:38:17 GMT
USER odoo
# Mon, 13 Dec 2021 19:38:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Dec 2021 19:38:17 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8928362baaf188d2d35b07907f7df5a83838f416511d7c90d1001f0f69b22d`  
		Last Modified: Thu, 02 Dec 2021 03:32:31 GMT  
		Size: 220.3 MB (220290298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1196c36b7759c2bc3f823f01785a679ef74915d5281b24e23220cfac4fb643c`  
		Last Modified: Thu, 02 Dec 2021 03:31:45 GMT  
		Size: 2.5 MB (2506050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014833e3ecaf723c362d63385e2ff1ece9d0f33f6818690c2ffb8acbbc320186`  
		Last Modified: Thu, 02 Dec 2021 03:31:45 GMT  
		Size: 417.8 KB (417795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47ba6bcf217c53bb47d74cd3b7d658bef87942db4626cf2e9f387cb3f530719`  
		Last Modified: Mon, 13 Dec 2021 19:42:34 GMT  
		Size: 291.6 MB (291625365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2cb6d340eb30e83ae63c6eca61b5f2b867e7ca4c9604af18c0e40b9546263c`  
		Last Modified: Mon, 13 Dec 2021 19:42:00 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:929ffb6475af451c610194953dea2840ce8fdfc019b8ce5d4abed12caceab3d2`  
		Last Modified: Mon, 13 Dec 2021 19:42:01 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dce199b6b093ee9c82d891f20b52bfb1f40cebbdca994a70564eacc795fe2b0`  
		Last Modified: Mon, 13 Dec 2021 19:42:00 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1a3c709fb69fd910bad9716caf7fd17bef03d4bad8347c0f59f5ea4ba70937`  
		Last Modified: Mon, 13 Dec 2021 19:42:00 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
