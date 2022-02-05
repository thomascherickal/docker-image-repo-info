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
$ docker pull odoo@sha256:215f4de85c10617f3a5feb200f8b4ef61f7c53ea506fb81d423961b563ee759a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:81a82ebc115ea0f424e4876cf17a56e81d01485e3bbae757a39627b03042e3a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.5 MB (539508777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2c839c5a3f834e3d1bddc77cb57370e2990e89b02e10c5dc2646a6d314b19e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:06:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Jan 2022 09:06:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 26 Jan 2022 09:06:22 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 09:10:31 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Jan 2022 09:11:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:11:19 GMT
RUN npm install -g rtlcss
# Wed, 26 Jan 2022 09:11:19 GMT
ENV ODOO_VERSION=13.0
# Sat, 05 Feb 2022 01:48:43 GMT
ARG ODOO_RELEASE=20220204
# Sat, 05 Feb 2022 01:48:44 GMT
ARG ODOO_SHA=bc23629b326a00db91e31a8a6735946519b78dd7
# Sat, 05 Feb 2022 01:49:57 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=bc23629b326a00db91e31a8a6735946519b78dd7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 05 Feb 2022 01:50:00 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 05 Feb 2022 01:50:00 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 05 Feb 2022 01:50:01 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=bc23629b326a00db91e31a8a6735946519b78dd7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 05 Feb 2022 01:50:01 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 05 Feb 2022 01:50:02 GMT
EXPOSE 8069 8071 8072
# Sat, 05 Feb 2022 01:50:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 05 Feb 2022 01:50:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 05 Feb 2022 01:50:03 GMT
USER odoo
# Sat, 05 Feb 2022 01:50:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Feb 2022 01:50:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1643683a10820c31ffd26f415c4c5a3d8da779af7f087d7c33939c40597425a`  
		Last Modified: Wed, 26 Jan 2022 09:16:15 GMT  
		Size: 207.1 MB (207131191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebec2e1c27f1ac41a1fde98e797a9891f5dc8db95df82fc8e43e3717d5bcb7f8`  
		Last Modified: Wed, 26 Jan 2022 09:15:39 GMT  
		Size: 13.4 MB (13433899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426af2fe5b1c6cfebdb4e8ec73348b9d2c5b12fc783ac4d7daa8e515c42f80f8`  
		Last Modified: Wed, 26 Jan 2022 09:15:35 GMT  
		Size: 447.0 KB (447023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f550fefc3bc262c9c3358a2f076139484829d7ea3ce0484a345d04f2f0acfd`  
		Last Modified: Sat, 05 Feb 2022 01:53:08 GMT  
		Size: 291.3 MB (291340468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904c6abf9f9bf1bfae9d1c90c71f264e373b9a7bd2f613f5c6b5845bb1017e2a`  
		Last Modified: Sat, 05 Feb 2022 01:52:22 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b9bb6ee7b8489dff73a28e4056daccdf9386946fb5c37bd7c833e6149c21f8`  
		Last Modified: Sat, 05 Feb 2022 01:52:30 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4a96e89c436a700bee8b1e7ee85890db1ba02d7b89d6808cefd3de229711f9`  
		Last Modified: Sat, 05 Feb 2022 01:52:22 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf271d72a38b7916e3223ab5719ad0ba314d90e8f5b9283cb9a28f942bd136`  
		Last Modified: Sat, 05 Feb 2022 01:52:22 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:215f4de85c10617f3a5feb200f8b4ef61f7c53ea506fb81d423961b563ee759a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:81a82ebc115ea0f424e4876cf17a56e81d01485e3bbae757a39627b03042e3a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.5 MB (539508777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2c839c5a3f834e3d1bddc77cb57370e2990e89b02e10c5dc2646a6d314b19e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:06:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Jan 2022 09:06:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 26 Jan 2022 09:06:22 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 09:10:31 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Jan 2022 09:11:16 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:11:19 GMT
RUN npm install -g rtlcss
# Wed, 26 Jan 2022 09:11:19 GMT
ENV ODOO_VERSION=13.0
# Sat, 05 Feb 2022 01:48:43 GMT
ARG ODOO_RELEASE=20220204
# Sat, 05 Feb 2022 01:48:44 GMT
ARG ODOO_SHA=bc23629b326a00db91e31a8a6735946519b78dd7
# Sat, 05 Feb 2022 01:49:57 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=bc23629b326a00db91e31a8a6735946519b78dd7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 05 Feb 2022 01:50:00 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 05 Feb 2022 01:50:00 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 05 Feb 2022 01:50:01 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=bc23629b326a00db91e31a8a6735946519b78dd7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 05 Feb 2022 01:50:01 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 05 Feb 2022 01:50:02 GMT
EXPOSE 8069 8071 8072
# Sat, 05 Feb 2022 01:50:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 05 Feb 2022 01:50:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 05 Feb 2022 01:50:03 GMT
USER odoo
# Sat, 05 Feb 2022 01:50:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Feb 2022 01:50:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1643683a10820c31ffd26f415c4c5a3d8da779af7f087d7c33939c40597425a`  
		Last Modified: Wed, 26 Jan 2022 09:16:15 GMT  
		Size: 207.1 MB (207131191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebec2e1c27f1ac41a1fde98e797a9891f5dc8db95df82fc8e43e3717d5bcb7f8`  
		Last Modified: Wed, 26 Jan 2022 09:15:39 GMT  
		Size: 13.4 MB (13433899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426af2fe5b1c6cfebdb4e8ec73348b9d2c5b12fc783ac4d7daa8e515c42f80f8`  
		Last Modified: Wed, 26 Jan 2022 09:15:35 GMT  
		Size: 447.0 KB (447023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f550fefc3bc262c9c3358a2f076139484829d7ea3ce0484a345d04f2f0acfd`  
		Last Modified: Sat, 05 Feb 2022 01:53:08 GMT  
		Size: 291.3 MB (291340468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904c6abf9f9bf1bfae9d1c90c71f264e373b9a7bd2f613f5c6b5845bb1017e2a`  
		Last Modified: Sat, 05 Feb 2022 01:52:22 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b9bb6ee7b8489dff73a28e4056daccdf9386946fb5c37bd7c833e6149c21f8`  
		Last Modified: Sat, 05 Feb 2022 01:52:30 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4a96e89c436a700bee8b1e7ee85890db1ba02d7b89d6808cefd3de229711f9`  
		Last Modified: Sat, 05 Feb 2022 01:52:22 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf271d72a38b7916e3223ab5719ad0ba314d90e8f5b9283cb9a28f942bd136`  
		Last Modified: Sat, 05 Feb 2022 01:52:22 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:22a7c8d3b5592746b22d7ee217a008e5f3d2ed316b506df141aa44148b295a51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:f5a911320ed7ef65ef12dcab134d5838bac680d25a75329cedba2859e5ea0da1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.3 MB (529319412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d169f39a095ad407fffaedc4f1781bcc8aa3f8acb67610c4a9d4f28eda40f8b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:06:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Jan 2022 09:06:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 26 Jan 2022 09:06:22 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 09:07:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Jan 2022 09:07:48 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:07:52 GMT
RUN npm install -g rtlcss
# Wed, 26 Jan 2022 09:07:52 GMT
ENV ODOO_VERSION=14.0
# Sat, 05 Feb 2022 01:47:06 GMT
ARG ODOO_RELEASE=20220204
# Sat, 05 Feb 2022 01:47:06 GMT
ARG ODOO_SHA=8af8029ab9176ac00776c7aa464af691dfa10547
# Sat, 05 Feb 2022 01:48:24 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=8af8029ab9176ac00776c7aa464af691dfa10547
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 05 Feb 2022 01:48:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 05 Feb 2022 01:48:30 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 05 Feb 2022 01:48:30 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=8af8029ab9176ac00776c7aa464af691dfa10547
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 05 Feb 2022 01:48:31 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 05 Feb 2022 01:48:31 GMT
EXPOSE 8069 8071 8072
# Sat, 05 Feb 2022 01:48:31 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 05 Feb 2022 01:48:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 05 Feb 2022 01:48:31 GMT
USER odoo
# Sat, 05 Feb 2022 01:48:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Feb 2022 01:48:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158787f79b5bbd45592d744836bf9bab3a8f9ffc1fc9d765e0a69828fba80f7a`  
		Last Modified: Wed, 26 Jan 2022 09:15:11 GMT  
		Size: 213.2 MB (213173094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c04dc7402806cf6edd8c86d43be59a3f35cc2abdeb069509b0b8089ff88d8c`  
		Last Modified: Wed, 26 Jan 2022 09:14:42 GMT  
		Size: 13.4 MB (13436578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b98a5866acaabb48e508494ade5b4cd13f3c3225e581cd1ea045e283d0602c`  
		Last Modified: Wed, 26 Jan 2022 09:14:38 GMT  
		Size: 447.0 KB (446976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb19b232c81bf09ba450111d4043c8f6b50521e3311a2b16b234193fb5a14c71`  
		Last Modified: Sat, 05 Feb 2022 01:52:00 GMT  
		Size: 275.1 MB (275106565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212038a5b112e8acce82dc6a1a2ffd377282bc25deef1947a77788a619a6fbb5`  
		Last Modified: Sat, 05 Feb 2022 01:51:16 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28578d5a1c944b4e889cb3e0368aaa005ae8d7a1ad7ceab19c88cdb3c6a11694`  
		Last Modified: Sat, 05 Feb 2022 01:51:15 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e29aa111e83af87aa0df569a06b628b33e593db081042480d5236c88c096b7`  
		Last Modified: Sat, 05 Feb 2022 01:51:16 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6733d15209f7df53d7993113c59d230ab7cf649fc1e1485e7729172f1b6857`  
		Last Modified: Sat, 05 Feb 2022 01:51:15 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:22a7c8d3b5592746b22d7ee217a008e5f3d2ed316b506df141aa44148b295a51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:f5a911320ed7ef65ef12dcab134d5838bac680d25a75329cedba2859e5ea0da1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.3 MB (529319412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d169f39a095ad407fffaedc4f1781bcc8aa3f8acb67610c4a9d4f28eda40f8b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:06:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Jan 2022 09:06:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 26 Jan 2022 09:06:22 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 09:07:36 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Jan 2022 09:07:48 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:07:52 GMT
RUN npm install -g rtlcss
# Wed, 26 Jan 2022 09:07:52 GMT
ENV ODOO_VERSION=14.0
# Sat, 05 Feb 2022 01:47:06 GMT
ARG ODOO_RELEASE=20220204
# Sat, 05 Feb 2022 01:47:06 GMT
ARG ODOO_SHA=8af8029ab9176ac00776c7aa464af691dfa10547
# Sat, 05 Feb 2022 01:48:24 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=8af8029ab9176ac00776c7aa464af691dfa10547
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 05 Feb 2022 01:48:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 05 Feb 2022 01:48:30 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 05 Feb 2022 01:48:30 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=8af8029ab9176ac00776c7aa464af691dfa10547
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 05 Feb 2022 01:48:31 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 05 Feb 2022 01:48:31 GMT
EXPOSE 8069 8071 8072
# Sat, 05 Feb 2022 01:48:31 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 05 Feb 2022 01:48:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 05 Feb 2022 01:48:31 GMT
USER odoo
# Sat, 05 Feb 2022 01:48:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Feb 2022 01:48:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158787f79b5bbd45592d744836bf9bab3a8f9ffc1fc9d765e0a69828fba80f7a`  
		Last Modified: Wed, 26 Jan 2022 09:15:11 GMT  
		Size: 213.2 MB (213173094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c04dc7402806cf6edd8c86d43be59a3f35cc2abdeb069509b0b8089ff88d8c`  
		Last Modified: Wed, 26 Jan 2022 09:14:42 GMT  
		Size: 13.4 MB (13436578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b98a5866acaabb48e508494ade5b4cd13f3c3225e581cd1ea045e283d0602c`  
		Last Modified: Wed, 26 Jan 2022 09:14:38 GMT  
		Size: 447.0 KB (446976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb19b232c81bf09ba450111d4043c8f6b50521e3311a2b16b234193fb5a14c71`  
		Last Modified: Sat, 05 Feb 2022 01:52:00 GMT  
		Size: 275.1 MB (275106565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212038a5b112e8acce82dc6a1a2ffd377282bc25deef1947a77788a619a6fbb5`  
		Last Modified: Sat, 05 Feb 2022 01:51:16 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28578d5a1c944b4e889cb3e0368aaa005ae8d7a1ad7ceab19c88cdb3c6a11694`  
		Last Modified: Sat, 05 Feb 2022 01:51:15 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e29aa111e83af87aa0df569a06b628b33e593db081042480d5236c88c096b7`  
		Last Modified: Sat, 05 Feb 2022 01:51:16 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6733d15209f7df53d7993113c59d230ab7cf649fc1e1485e7729172f1b6857`  
		Last Modified: Sat, 05 Feb 2022 01:51:15 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:a66a69926529b87b28dad918a37f5fa03c0c9a3aa7e5222c556a9e08a900a1fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:d5309469826d4737e37b93aba92c9a0f2638221042ec6092eac85daf6b76b0d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **548.6 MB (548565313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f132b1fdff36281346aaa1d2b8e944adb113ad4f5ec69ce962eb05113e41c56`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:02:43 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Jan 2022 09:02:43 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 26 Jan 2022 09:02:43 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 09:04:06 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Jan 2022 09:04:44 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:04:46 GMT
RUN npm install -g rtlcss
# Wed, 26 Jan 2022 09:04:46 GMT
ENV ODOO_VERSION=15.0
# Sat, 05 Feb 2022 01:44:42 GMT
ARG ODOO_RELEASE=20220204
# Sat, 05 Feb 2022 01:44:42 GMT
ARG ODOO_SHA=6f7f4163fb5c73a24df365ca392fad120c9973df
# Sat, 05 Feb 2022 01:46:42 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=6f7f4163fb5c73a24df365ca392fad120c9973df
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 05 Feb 2022 01:46:47 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 05 Feb 2022 01:46:47 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 05 Feb 2022 01:46:49 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=6f7f4163fb5c73a24df365ca392fad120c9973df
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 05 Feb 2022 01:46:49 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 05 Feb 2022 01:46:50 GMT
EXPOSE 8069 8071 8072
# Sat, 05 Feb 2022 01:46:50 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 05 Feb 2022 01:46:50 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 05 Feb 2022 01:46:51 GMT
USER odoo
# Sat, 05 Feb 2022 01:46:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Feb 2022 01:46:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9293b96c918352418f9470373a3ccf1788a2b957d28fcb51b99beab26e73f974`  
		Last Modified: Wed, 26 Jan 2022 09:14:12 GMT  
		Size: 220.3 MB (220291077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfb4ef07b63f082d87ab75156c6ae62bcaf11e1ac37595986d8fd97b5dd5c80`  
		Last Modified: Wed, 26 Jan 2022 09:13:41 GMT  
		Size: 2.5 MB (2506147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2f8d17d4fa74bd599ba34671d44d6da384f629a1bda0e322208540e26ae8ee`  
		Last Modified: Wed, 26 Jan 2022 09:13:41 GMT  
		Size: 440.2 KB (440201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa61b81c71995de6d01df900b02700fc3a79394ffd3d5c48cbd455e254fd68b`  
		Last Modified: Sat, 05 Feb 2022 01:51:02 GMT  
		Size: 294.0 MB (293959165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ac710a95508d1c9d8c04ad10b5f595d52db343dcc19523aa709b8d74e7c4d5`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27288a7a8091fdab37f15cf0a64765913cd0b7e1cf633a2c1aefd910cf796d3`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d47098a3f6e7588e7ec9dffdbb3a052c50b6d99b70b339c05735aa81274ddf4`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4357ba915e49860b1a6fb6b0e747fa555e6cfadcc9dab79c67fa0b2c54048c46`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:a66a69926529b87b28dad918a37f5fa03c0c9a3aa7e5222c556a9e08a900a1fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:d5309469826d4737e37b93aba92c9a0f2638221042ec6092eac85daf6b76b0d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **548.6 MB (548565313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f132b1fdff36281346aaa1d2b8e944adb113ad4f5ec69ce962eb05113e41c56`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:02:43 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Jan 2022 09:02:43 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 26 Jan 2022 09:02:43 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 09:04:06 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Jan 2022 09:04:44 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:04:46 GMT
RUN npm install -g rtlcss
# Wed, 26 Jan 2022 09:04:46 GMT
ENV ODOO_VERSION=15.0
# Sat, 05 Feb 2022 01:44:42 GMT
ARG ODOO_RELEASE=20220204
# Sat, 05 Feb 2022 01:44:42 GMT
ARG ODOO_SHA=6f7f4163fb5c73a24df365ca392fad120c9973df
# Sat, 05 Feb 2022 01:46:42 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=6f7f4163fb5c73a24df365ca392fad120c9973df
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 05 Feb 2022 01:46:47 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 05 Feb 2022 01:46:47 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 05 Feb 2022 01:46:49 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=6f7f4163fb5c73a24df365ca392fad120c9973df
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 05 Feb 2022 01:46:49 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 05 Feb 2022 01:46:50 GMT
EXPOSE 8069 8071 8072
# Sat, 05 Feb 2022 01:46:50 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 05 Feb 2022 01:46:50 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 05 Feb 2022 01:46:51 GMT
USER odoo
# Sat, 05 Feb 2022 01:46:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Feb 2022 01:46:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9293b96c918352418f9470373a3ccf1788a2b957d28fcb51b99beab26e73f974`  
		Last Modified: Wed, 26 Jan 2022 09:14:12 GMT  
		Size: 220.3 MB (220291077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfb4ef07b63f082d87ab75156c6ae62bcaf11e1ac37595986d8fd97b5dd5c80`  
		Last Modified: Wed, 26 Jan 2022 09:13:41 GMT  
		Size: 2.5 MB (2506147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2f8d17d4fa74bd599ba34671d44d6da384f629a1bda0e322208540e26ae8ee`  
		Last Modified: Wed, 26 Jan 2022 09:13:41 GMT  
		Size: 440.2 KB (440201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa61b81c71995de6d01df900b02700fc3a79394ffd3d5c48cbd455e254fd68b`  
		Last Modified: Sat, 05 Feb 2022 01:51:02 GMT  
		Size: 294.0 MB (293959165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ac710a95508d1c9d8c04ad10b5f595d52db343dcc19523aa709b8d74e7c4d5`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27288a7a8091fdab37f15cf0a64765913cd0b7e1cf633a2c1aefd910cf796d3`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d47098a3f6e7588e7ec9dffdbb3a052c50b6d99b70b339c05735aa81274ddf4`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4357ba915e49860b1a6fb6b0e747fa555e6cfadcc9dab79c67fa0b2c54048c46`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:a66a69926529b87b28dad918a37f5fa03c0c9a3aa7e5222c556a9e08a900a1fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:d5309469826d4737e37b93aba92c9a0f2638221042ec6092eac85daf6b76b0d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **548.6 MB (548565313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f132b1fdff36281346aaa1d2b8e944adb113ad4f5ec69ce962eb05113e41c56`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:02:43 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Jan 2022 09:02:43 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 26 Jan 2022 09:02:43 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 09:04:06 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Jan 2022 09:04:44 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:04:46 GMT
RUN npm install -g rtlcss
# Wed, 26 Jan 2022 09:04:46 GMT
ENV ODOO_VERSION=15.0
# Sat, 05 Feb 2022 01:44:42 GMT
ARG ODOO_RELEASE=20220204
# Sat, 05 Feb 2022 01:44:42 GMT
ARG ODOO_SHA=6f7f4163fb5c73a24df365ca392fad120c9973df
# Sat, 05 Feb 2022 01:46:42 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=6f7f4163fb5c73a24df365ca392fad120c9973df
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 05 Feb 2022 01:46:47 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 05 Feb 2022 01:46:47 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 05 Feb 2022 01:46:49 GMT
# ARGS: ODOO_RELEASE=20220204 ODOO_SHA=6f7f4163fb5c73a24df365ca392fad120c9973df
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 05 Feb 2022 01:46:49 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 05 Feb 2022 01:46:50 GMT
EXPOSE 8069 8071 8072
# Sat, 05 Feb 2022 01:46:50 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 05 Feb 2022 01:46:50 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 05 Feb 2022 01:46:51 GMT
USER odoo
# Sat, 05 Feb 2022 01:46:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 05 Feb 2022 01:46:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9293b96c918352418f9470373a3ccf1788a2b957d28fcb51b99beab26e73f974`  
		Last Modified: Wed, 26 Jan 2022 09:14:12 GMT  
		Size: 220.3 MB (220291077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfb4ef07b63f082d87ab75156c6ae62bcaf11e1ac37595986d8fd97b5dd5c80`  
		Last Modified: Wed, 26 Jan 2022 09:13:41 GMT  
		Size: 2.5 MB (2506147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2f8d17d4fa74bd599ba34671d44d6da384f629a1bda0e322208540e26ae8ee`  
		Last Modified: Wed, 26 Jan 2022 09:13:41 GMT  
		Size: 440.2 KB (440201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa61b81c71995de6d01df900b02700fc3a79394ffd3d5c48cbd455e254fd68b`  
		Last Modified: Sat, 05 Feb 2022 01:51:02 GMT  
		Size: 294.0 MB (293959165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ac710a95508d1c9d8c04ad10b5f595d52db343dcc19523aa709b8d74e7c4d5`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27288a7a8091fdab37f15cf0a64765913cd0b7e1cf633a2c1aefd910cf796d3`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d47098a3f6e7588e7ec9dffdbb3a052c50b6d99b70b339c05735aa81274ddf4`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4357ba915e49860b1a6fb6b0e747fa555e6cfadcc9dab79c67fa0b2c54048c46`  
		Last Modified: Sat, 05 Feb 2022 01:50:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
