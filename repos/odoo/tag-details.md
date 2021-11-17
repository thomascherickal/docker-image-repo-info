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
$ docker pull odoo@sha256:a08a9339d3657b7e90b9a8ccf96750582f27c0163e0d6409a3c149977699a6ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:d91482ae3fe95763f89b5889fc8fa23a52d66e30c92ee1a7af8d25612ec6cc31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.5 MB (539542680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3006c41892b4fbfd4173d6b4399b5ba64de10b041af8f7710a347b3d4b12a340`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:13:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 17 Nov 2021 09:13:18 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 17 Nov 2021 09:13:18 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:17:15 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 17 Nov 2021 09:17:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:17:29 GMT
RUN npm install -g rtlcss
# Wed, 17 Nov 2021 09:17:30 GMT
ENV ODOO_VERSION=13.0
# Wed, 17 Nov 2021 09:17:30 GMT
ARG ODOO_RELEASE=20211110
# Wed, 17 Nov 2021 09:17:30 GMT
ARG ODOO_SHA=c4ae69b33bd4353f6023bb57419133de389e0849
# Wed, 17 Nov 2021 09:19:14 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=c4ae69b33bd4353f6023bb57419133de389e0849
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 17 Nov 2021 09:19:18 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 17 Nov 2021 09:19:19 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 17 Nov 2021 09:19:20 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=c4ae69b33bd4353f6023bb57419133de389e0849
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 17 Nov 2021 09:19:20 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 17 Nov 2021 09:19:20 GMT
EXPOSE 8069 8071 8072
# Wed, 17 Nov 2021 09:19:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 17 Nov 2021 09:19:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 17 Nov 2021 09:19:21 GMT
USER odoo
# Wed, 17 Nov 2021 09:19:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 09:19:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8000d6f871a597077bc945f27930d96427d837fb6bc47a4d8322ba718d61a2a0`  
		Last Modified: Wed, 17 Nov 2021 09:22:41 GMT  
		Size: 207.1 MB (207130893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a4e33b7c38be10d731e5a751ee2bdaf14ec8e15f4fe4a5fb4725a2b0545261`  
		Last Modified: Wed, 17 Nov 2021 09:22:12 GMT  
		Size: 13.4 MB (13434039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eca00fd297b3661881f76fa666c3d23fc8c09d8a29fb17f8ad8a11aa94917c9`  
		Last Modified: Wed, 17 Nov 2021 09:22:07 GMT  
		Size: 731.1 KB (731081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed241e681be92359b926b4988de2f1eea29bf2ee22ca01290441e653cc5314`  
		Last Modified: Wed, 17 Nov 2021 09:22:48 GMT  
		Size: 291.1 MB (291090530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73138f241ebe9e34dd7aa7ddfeacc2b3a5a38daff5f6921d4b71db013a14c68`  
		Last Modified: Wed, 17 Nov 2021 09:22:05 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc59a97ed34c9f9c85851a54b5e7ba7f7a73e9cf5818c08ed435001edfd33d`  
		Last Modified: Wed, 17 Nov 2021 09:22:05 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44d73c7fe1034329d49f0e4e86f6fe110e847ab2b5fef4c59431a42e9b1a445`  
		Last Modified: Wed, 17 Nov 2021 09:22:05 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d33af30e89083b124e09aa2da4f1b48ad69a447c8a64f5480d12ff76f3d87a`  
		Last Modified: Wed, 17 Nov 2021 09:22:05 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:a08a9339d3657b7e90b9a8ccf96750582f27c0163e0d6409a3c149977699a6ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:d91482ae3fe95763f89b5889fc8fa23a52d66e30c92ee1a7af8d25612ec6cc31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.5 MB (539542680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3006c41892b4fbfd4173d6b4399b5ba64de10b041af8f7710a347b3d4b12a340`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:13:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 17 Nov 2021 09:13:18 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 17 Nov 2021 09:13:18 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:17:15 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 17 Nov 2021 09:17:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:17:29 GMT
RUN npm install -g rtlcss
# Wed, 17 Nov 2021 09:17:30 GMT
ENV ODOO_VERSION=13.0
# Wed, 17 Nov 2021 09:17:30 GMT
ARG ODOO_RELEASE=20211110
# Wed, 17 Nov 2021 09:17:30 GMT
ARG ODOO_SHA=c4ae69b33bd4353f6023bb57419133de389e0849
# Wed, 17 Nov 2021 09:19:14 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=c4ae69b33bd4353f6023bb57419133de389e0849
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 17 Nov 2021 09:19:18 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 17 Nov 2021 09:19:19 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 17 Nov 2021 09:19:20 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=c4ae69b33bd4353f6023bb57419133de389e0849
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 17 Nov 2021 09:19:20 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 17 Nov 2021 09:19:20 GMT
EXPOSE 8069 8071 8072
# Wed, 17 Nov 2021 09:19:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 17 Nov 2021 09:19:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 17 Nov 2021 09:19:21 GMT
USER odoo
# Wed, 17 Nov 2021 09:19:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 09:19:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8000d6f871a597077bc945f27930d96427d837fb6bc47a4d8322ba718d61a2a0`  
		Last Modified: Wed, 17 Nov 2021 09:22:41 GMT  
		Size: 207.1 MB (207130893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a4e33b7c38be10d731e5a751ee2bdaf14ec8e15f4fe4a5fb4725a2b0545261`  
		Last Modified: Wed, 17 Nov 2021 09:22:12 GMT  
		Size: 13.4 MB (13434039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eca00fd297b3661881f76fa666c3d23fc8c09d8a29fb17f8ad8a11aa94917c9`  
		Last Modified: Wed, 17 Nov 2021 09:22:07 GMT  
		Size: 731.1 KB (731081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bed241e681be92359b926b4988de2f1eea29bf2ee22ca01290441e653cc5314`  
		Last Modified: Wed, 17 Nov 2021 09:22:48 GMT  
		Size: 291.1 MB (291090530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73138f241ebe9e34dd7aa7ddfeacc2b3a5a38daff5f6921d4b71db013a14c68`  
		Last Modified: Wed, 17 Nov 2021 09:22:05 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc59a97ed34c9f9c85851a54b5e7ba7f7a73e9cf5818c08ed435001edfd33d`  
		Last Modified: Wed, 17 Nov 2021 09:22:05 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44d73c7fe1034329d49f0e4e86f6fe110e847ab2b5fef4c59431a42e9b1a445`  
		Last Modified: Wed, 17 Nov 2021 09:22:05 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d33af30e89083b124e09aa2da4f1b48ad69a447c8a64f5480d12ff76f3d87a`  
		Last Modified: Wed, 17 Nov 2021 09:22:05 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:6139451b3f55035f9010eff25f29a083cf7bfdb3403b43eb258e73f7585f89e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:b005ac39f34870e1fdb7b9906fc419bb308214b92dcdc8a939e23abb30ca9198
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.4 MB (528410566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358c9396e1b828ca1e76b234b6912e5bfe5657dd7e0378858bf279faedbbcb42`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:13:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 17 Nov 2021 09:13:18 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 17 Nov 2021 09:13:18 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:14:28 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 17 Nov 2021 09:14:41 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:14:45 GMT
RUN npm install -g rtlcss
# Wed, 17 Nov 2021 09:14:45 GMT
ENV ODOO_VERSION=14.0
# Wed, 17 Nov 2021 09:14:45 GMT
ARG ODOO_RELEASE=20211110
# Wed, 17 Nov 2021 09:14:45 GMT
ARG ODOO_SHA=95a45d67d38de6d81399533b8b4e39fca08c1254
# Wed, 17 Nov 2021 09:16:00 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=95a45d67d38de6d81399533b8b4e39fca08c1254
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 17 Nov 2021 09:16:05 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 17 Nov 2021 09:16:05 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 17 Nov 2021 09:16:06 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=95a45d67d38de6d81399533b8b4e39fca08c1254
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 17 Nov 2021 09:16:06 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 17 Nov 2021 09:16:06 GMT
EXPOSE 8069 8071 8072
# Wed, 17 Nov 2021 09:16:06 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 17 Nov 2021 09:16:07 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 17 Nov 2021 09:16:07 GMT
USER odoo
# Wed, 17 Nov 2021 09:16:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 09:16:07 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9050a25a2e7fc15bfb237c584e249e35ad1a86ce1d54a161a0ff988ac8a05b`  
		Last Modified: Wed, 17 Nov 2021 09:21:44 GMT  
		Size: 213.2 MB (213173458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35caad2bee1ae3832c799d895b217edd464b38ab7eab3b3bd4112a0ac8023dfa`  
		Last Modified: Wed, 17 Nov 2021 09:21:06 GMT  
		Size: 13.4 MB (13436595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e676672899dc5c1f50f0b67069ce37431c5177ff11d52b931dbac889f0792`  
		Last Modified: Wed, 17 Nov 2021 09:21:00 GMT  
		Size: 730.9 KB (730870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a3e802240a801f7ff72cdd618dea95fcb76e1617934bda6ab21543c0a7083a`  
		Last Modified: Wed, 17 Nov 2021 09:21:55 GMT  
		Size: 273.9 MB (273913512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e88d1282e0bb8f269bab117124f33a12906e268ec8184041963c98f03172f8`  
		Last Modified: Wed, 17 Nov 2021 09:20:57 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742adc5b821815e653b33c53357a9a31c1ef3feef4e4ee6d111cb54b1055cfe5`  
		Last Modified: Wed, 17 Nov 2021 09:20:57 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998366f7240c799e2868124d0b73d5e1dc174083241b3c0947878dbaf23f3600`  
		Last Modified: Wed, 17 Nov 2021 09:20:58 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c18aee2d8b386835ff01c1d066d3e546a740a675d122aa1bb1ad46f1ffb758e`  
		Last Modified: Wed, 17 Nov 2021 09:20:57 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:6139451b3f55035f9010eff25f29a083cf7bfdb3403b43eb258e73f7585f89e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:b005ac39f34870e1fdb7b9906fc419bb308214b92dcdc8a939e23abb30ca9198
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.4 MB (528410566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358c9396e1b828ca1e76b234b6912e5bfe5657dd7e0378858bf279faedbbcb42`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 17 Nov 2021 02:21:02 GMT
ADD file:3c54ad257f2e04f7294ce879b884820cf4726c8e93ec548172825963e40c79ad in / 
# Wed, 17 Nov 2021 02:21:02 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:13:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 17 Nov 2021 09:13:18 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 17 Nov 2021 09:13:18 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:14:28 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 17 Nov 2021 09:14:41 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:14:45 GMT
RUN npm install -g rtlcss
# Wed, 17 Nov 2021 09:14:45 GMT
ENV ODOO_VERSION=14.0
# Wed, 17 Nov 2021 09:14:45 GMT
ARG ODOO_RELEASE=20211110
# Wed, 17 Nov 2021 09:14:45 GMT
ARG ODOO_SHA=95a45d67d38de6d81399533b8b4e39fca08c1254
# Wed, 17 Nov 2021 09:16:00 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=95a45d67d38de6d81399533b8b4e39fca08c1254
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 17 Nov 2021 09:16:05 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 17 Nov 2021 09:16:05 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 17 Nov 2021 09:16:06 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=95a45d67d38de6d81399533b8b4e39fca08c1254
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 17 Nov 2021 09:16:06 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 17 Nov 2021 09:16:06 GMT
EXPOSE 8069 8071 8072
# Wed, 17 Nov 2021 09:16:06 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 17 Nov 2021 09:16:07 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 17 Nov 2021 09:16:07 GMT
USER odoo
# Wed, 17 Nov 2021 09:16:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 09:16:07 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a10c77af261312e7c92bcc184f2d1726175ff7f142e44b01c5779cd79348b9fd`  
		Last Modified: Wed, 17 Nov 2021 02:26:31 GMT  
		Size: 27.2 MB (27153675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9050a25a2e7fc15bfb237c584e249e35ad1a86ce1d54a161a0ff988ac8a05b`  
		Last Modified: Wed, 17 Nov 2021 09:21:44 GMT  
		Size: 213.2 MB (213173458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35caad2bee1ae3832c799d895b217edd464b38ab7eab3b3bd4112a0ac8023dfa`  
		Last Modified: Wed, 17 Nov 2021 09:21:06 GMT  
		Size: 13.4 MB (13436595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827e676672899dc5c1f50f0b67069ce37431c5177ff11d52b931dbac889f0792`  
		Last Modified: Wed, 17 Nov 2021 09:21:00 GMT  
		Size: 730.9 KB (730870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a3e802240a801f7ff72cdd618dea95fcb76e1617934bda6ab21543c0a7083a`  
		Last Modified: Wed, 17 Nov 2021 09:21:55 GMT  
		Size: 273.9 MB (273913512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e88d1282e0bb8f269bab117124f33a12906e268ec8184041963c98f03172f8`  
		Last Modified: Wed, 17 Nov 2021 09:20:57 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742adc5b821815e653b33c53357a9a31c1ef3feef4e4ee6d111cb54b1055cfe5`  
		Last Modified: Wed, 17 Nov 2021 09:20:57 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998366f7240c799e2868124d0b73d5e1dc174083241b3c0947878dbaf23f3600`  
		Last Modified: Wed, 17 Nov 2021 09:20:58 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c18aee2d8b386835ff01c1d066d3e546a740a675d122aa1bb1ad46f1ffb758e`  
		Last Modified: Wed, 17 Nov 2021 09:20:57 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:b41814f15b9320b60f867257608e03db75b6f9a445cd16b285dd5ba3038da7aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:702d6422b830b02fda4ee5eefa93bd32bccead17cf6b8f985cc3318a3c39611a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.3 MB (543318115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3849b0d5cca8c2dcb38c9800b9c13cf4c571d0fd460a5627792384ecf9aa052c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:41 GMT
ADD file:a2405ebb9892d98be2eb585f6121864d12b3fd983ebf15e5f0b7486e106a79c6 in / 
# Wed, 17 Nov 2021 02:20:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:10:25 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 17 Nov 2021 09:10:25 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 17 Nov 2021 09:10:25 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:11:27 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 17 Nov 2021 09:11:37 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:11:39 GMT
RUN npm install -g rtlcss
# Wed, 17 Nov 2021 09:11:39 GMT
ENV ODOO_VERSION=15.0
# Wed, 17 Nov 2021 09:11:39 GMT
ARG ODOO_RELEASE=20211110
# Wed, 17 Nov 2021 09:11:40 GMT
ARG ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
# Wed, 17 Nov 2021 09:12:57 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 17 Nov 2021 09:13:01 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 17 Nov 2021 09:13:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 17 Nov 2021 09:13:02 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 17 Nov 2021 09:13:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 17 Nov 2021 09:13:03 GMT
EXPOSE 8069 8071 8072
# Wed, 17 Nov 2021 09:13:03 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 17 Nov 2021 09:13:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 17 Nov 2021 09:13:03 GMT
USER odoo
# Wed, 17 Nov 2021 09:13:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 09:13:04 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:eff15d958d664f0874d16aee393cc44387031ee0a68ef8542d0056c747f378e8`  
		Last Modified: Wed, 17 Nov 2021 02:25:45 GMT  
		Size: 31.4 MB (31370267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9400c757421e2063937e8b190c956fdda2687c92c013b5eff83fe1c61c0c2c8f`  
		Last Modified: Wed, 17 Nov 2021 09:20:38 GMT  
		Size: 220.3 MB (220291328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf19d1a3d79ceb0d2f1f442648da0e6ece72782b8656e052f0867231839dd0b0`  
		Last Modified: Wed, 17 Nov 2021 09:19:52 GMT  
		Size: 2.5 MB (2506093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9605eabe13664e4a62ea8056b48e7547ab78dad77c977652bc44a6e8e1e30d0`  
		Last Modified: Wed, 17 Nov 2021 09:19:51 GMT  
		Size: 724.5 KB (724479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dd0144067b9816daa2e9c5e128284a1ffb2af8ad887060057eec1740a277fc`  
		Last Modified: Wed, 17 Nov 2021 09:20:44 GMT  
		Size: 288.4 MB (288423492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d379ba2c5d0daeee7e64eab4c84ef931722ba3b61f822646e951d3d0387d9d`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acc3388effa209506493f12acfa7790bfd5bace4e945f5ee806d3abfb0e7927`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b516b6485cbad16e360552271b058caf024d336b94a638002401214546365c94`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c921df7aaf8d97bc0c7a7569b14e7078aa5fd5d2a9c7fbcb9766a709a4f676`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:b41814f15b9320b60f867257608e03db75b6f9a445cd16b285dd5ba3038da7aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:702d6422b830b02fda4ee5eefa93bd32bccead17cf6b8f985cc3318a3c39611a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.3 MB (543318115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3849b0d5cca8c2dcb38c9800b9c13cf4c571d0fd460a5627792384ecf9aa052c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:41 GMT
ADD file:a2405ebb9892d98be2eb585f6121864d12b3fd983ebf15e5f0b7486e106a79c6 in / 
# Wed, 17 Nov 2021 02:20:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:10:25 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 17 Nov 2021 09:10:25 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 17 Nov 2021 09:10:25 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:11:27 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 17 Nov 2021 09:11:37 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:11:39 GMT
RUN npm install -g rtlcss
# Wed, 17 Nov 2021 09:11:39 GMT
ENV ODOO_VERSION=15.0
# Wed, 17 Nov 2021 09:11:39 GMT
ARG ODOO_RELEASE=20211110
# Wed, 17 Nov 2021 09:11:40 GMT
ARG ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
# Wed, 17 Nov 2021 09:12:57 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 17 Nov 2021 09:13:01 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 17 Nov 2021 09:13:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 17 Nov 2021 09:13:02 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 17 Nov 2021 09:13:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 17 Nov 2021 09:13:03 GMT
EXPOSE 8069 8071 8072
# Wed, 17 Nov 2021 09:13:03 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 17 Nov 2021 09:13:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 17 Nov 2021 09:13:03 GMT
USER odoo
# Wed, 17 Nov 2021 09:13:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 09:13:04 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:eff15d958d664f0874d16aee393cc44387031ee0a68ef8542d0056c747f378e8`  
		Last Modified: Wed, 17 Nov 2021 02:25:45 GMT  
		Size: 31.4 MB (31370267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9400c757421e2063937e8b190c956fdda2687c92c013b5eff83fe1c61c0c2c8f`  
		Last Modified: Wed, 17 Nov 2021 09:20:38 GMT  
		Size: 220.3 MB (220291328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf19d1a3d79ceb0d2f1f442648da0e6ece72782b8656e052f0867231839dd0b0`  
		Last Modified: Wed, 17 Nov 2021 09:19:52 GMT  
		Size: 2.5 MB (2506093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9605eabe13664e4a62ea8056b48e7547ab78dad77c977652bc44a6e8e1e30d0`  
		Last Modified: Wed, 17 Nov 2021 09:19:51 GMT  
		Size: 724.5 KB (724479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dd0144067b9816daa2e9c5e128284a1ffb2af8ad887060057eec1740a277fc`  
		Last Modified: Wed, 17 Nov 2021 09:20:44 GMT  
		Size: 288.4 MB (288423492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d379ba2c5d0daeee7e64eab4c84ef931722ba3b61f822646e951d3d0387d9d`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acc3388effa209506493f12acfa7790bfd5bace4e945f5ee806d3abfb0e7927`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b516b6485cbad16e360552271b058caf024d336b94a638002401214546365c94`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c921df7aaf8d97bc0c7a7569b14e7078aa5fd5d2a9c7fbcb9766a709a4f676`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:b41814f15b9320b60f867257608e03db75b6f9a445cd16b285dd5ba3038da7aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:702d6422b830b02fda4ee5eefa93bd32bccead17cf6b8f985cc3318a3c39611a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.3 MB (543318115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3849b0d5cca8c2dcb38c9800b9c13cf4c571d0fd460a5627792384ecf9aa052c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:41 GMT
ADD file:a2405ebb9892d98be2eb585f6121864d12b3fd983ebf15e5f0b7486e106a79c6 in / 
# Wed, 17 Nov 2021 02:20:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:10:25 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 17 Nov 2021 09:10:25 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 17 Nov 2021 09:10:25 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:11:27 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 17 Nov 2021 09:11:37 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:11:39 GMT
RUN npm install -g rtlcss
# Wed, 17 Nov 2021 09:11:39 GMT
ENV ODOO_VERSION=15.0
# Wed, 17 Nov 2021 09:11:39 GMT
ARG ODOO_RELEASE=20211110
# Wed, 17 Nov 2021 09:11:40 GMT
ARG ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
# Wed, 17 Nov 2021 09:12:57 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 17 Nov 2021 09:13:01 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 17 Nov 2021 09:13:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 17 Nov 2021 09:13:02 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 17 Nov 2021 09:13:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 17 Nov 2021 09:13:03 GMT
EXPOSE 8069 8071 8072
# Wed, 17 Nov 2021 09:13:03 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 17 Nov 2021 09:13:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 17 Nov 2021 09:13:03 GMT
USER odoo
# Wed, 17 Nov 2021 09:13:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 09:13:04 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:eff15d958d664f0874d16aee393cc44387031ee0a68ef8542d0056c747f378e8`  
		Last Modified: Wed, 17 Nov 2021 02:25:45 GMT  
		Size: 31.4 MB (31370267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9400c757421e2063937e8b190c956fdda2687c92c013b5eff83fe1c61c0c2c8f`  
		Last Modified: Wed, 17 Nov 2021 09:20:38 GMT  
		Size: 220.3 MB (220291328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf19d1a3d79ceb0d2f1f442648da0e6ece72782b8656e052f0867231839dd0b0`  
		Last Modified: Wed, 17 Nov 2021 09:19:52 GMT  
		Size: 2.5 MB (2506093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9605eabe13664e4a62ea8056b48e7547ab78dad77c977652bc44a6e8e1e30d0`  
		Last Modified: Wed, 17 Nov 2021 09:19:51 GMT  
		Size: 724.5 KB (724479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dd0144067b9816daa2e9c5e128284a1ffb2af8ad887060057eec1740a277fc`  
		Last Modified: Wed, 17 Nov 2021 09:20:44 GMT  
		Size: 288.4 MB (288423492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d379ba2c5d0daeee7e64eab4c84ef931722ba3b61f822646e951d3d0387d9d`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acc3388effa209506493f12acfa7790bfd5bace4e945f5ee806d3abfb0e7927`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b516b6485cbad16e360552271b058caf024d336b94a638002401214546365c94`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c921df7aaf8d97bc0c7a7569b14e7078aa5fd5d2a9c7fbcb9766a709a4f676`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
