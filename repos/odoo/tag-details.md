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
$ docker pull odoo@sha256:86b6340c8bcc8b915ea5a3c145aff0f40f3d541677b7ab8b4189b097653f31c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:e97afd1156c4958a442d91a0910ffa78f7520d7fc9fa2edc3f1e09447e2fa9bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.6 MB (539583868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e780753cd733b317f366239e83a1818faf476b325ed1f35538e7c4669cf991ce`
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
# Fri, 18 Feb 2022 00:52:40 GMT
ARG ODOO_RELEASE=20220217
# Fri, 18 Feb 2022 00:52:40 GMT
ARG ODOO_SHA=37c5e4abedbad70199f9588225a9c35f2d960d13
# Fri, 18 Feb 2022 00:53:56 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=37c5e4abedbad70199f9588225a9c35f2d960d13
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Feb 2022 00:54:00 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Feb 2022 00:54:00 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Feb 2022 00:54:01 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=37c5e4abedbad70199f9588225a9c35f2d960d13
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Feb 2022 00:54:01 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Feb 2022 00:54:01 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Feb 2022 00:54:01 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Feb 2022 00:54:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Feb 2022 00:54:02 GMT
USER odoo
# Fri, 18 Feb 2022 00:54:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Feb 2022 00:54:02 GMT
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
	-	`sha256:ad805f7bca04293a8e450333893acf932d5f01abcda7aff0399b5aa5e15c58f7`  
		Last Modified: Fri, 18 Feb 2022 00:56:43 GMT  
		Size: 291.4 MB (291415557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa08b101aa5475b9efb5d651589aa4760f93011ce0b4da49baa135e793ca3ccf`  
		Last Modified: Fri, 18 Feb 2022 00:56:09 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6055f201c639405e4b49ea1ba24fa22110c35d651ed897a3e6c2329d9491e5`  
		Last Modified: Fri, 18 Feb 2022 00:56:09 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8754dd994e0c50b0558714399b7a9faf40e5c79706d13bd75d007c881f4efff5`  
		Last Modified: Fri, 18 Feb 2022 00:56:10 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882d4a9585129e51069ece37cddc2944e82794fe8a5673ebfe80d7a4f64985cf`  
		Last Modified: Fri, 18 Feb 2022 00:56:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:86b6340c8bcc8b915ea5a3c145aff0f40f3d541677b7ab8b4189b097653f31c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:e97afd1156c4958a442d91a0910ffa78f7520d7fc9fa2edc3f1e09447e2fa9bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.6 MB (539583868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e780753cd733b317f366239e83a1818faf476b325ed1f35538e7c4669cf991ce`
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
# Fri, 18 Feb 2022 00:52:40 GMT
ARG ODOO_RELEASE=20220217
# Fri, 18 Feb 2022 00:52:40 GMT
ARG ODOO_SHA=37c5e4abedbad70199f9588225a9c35f2d960d13
# Fri, 18 Feb 2022 00:53:56 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=37c5e4abedbad70199f9588225a9c35f2d960d13
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Feb 2022 00:54:00 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Feb 2022 00:54:00 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Feb 2022 00:54:01 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=37c5e4abedbad70199f9588225a9c35f2d960d13
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Feb 2022 00:54:01 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Feb 2022 00:54:01 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Feb 2022 00:54:01 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Feb 2022 00:54:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Feb 2022 00:54:02 GMT
USER odoo
# Fri, 18 Feb 2022 00:54:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Feb 2022 00:54:02 GMT
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
	-	`sha256:ad805f7bca04293a8e450333893acf932d5f01abcda7aff0399b5aa5e15c58f7`  
		Last Modified: Fri, 18 Feb 2022 00:56:43 GMT  
		Size: 291.4 MB (291415557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa08b101aa5475b9efb5d651589aa4760f93011ce0b4da49baa135e793ca3ccf`  
		Last Modified: Fri, 18 Feb 2022 00:56:09 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6055f201c639405e4b49ea1ba24fa22110c35d651ed897a3e6c2329d9491e5`  
		Last Modified: Fri, 18 Feb 2022 00:56:09 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8754dd994e0c50b0558714399b7a9faf40e5c79706d13bd75d007c881f4efff5`  
		Last Modified: Fri, 18 Feb 2022 00:56:10 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882d4a9585129e51069ece37cddc2944e82794fe8a5673ebfe80d7a4f64985cf`  
		Last Modified: Fri, 18 Feb 2022 00:56:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:cd76bc867cf9ffee2260032686cee29fc4aa3287581c9c9f8d5644602e364dad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:fb26036e812edaff5539ee8a404cd4670da6a187c12697d18add42c7265bd5fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.4 MB (529386852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ba73aacd429c84d80d286455901bf4e63dc20656c01b0e2248bd56006a548a`
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
# Fri, 18 Feb 2022 00:51:02 GMT
ARG ODOO_RELEASE=20220217
# Fri, 18 Feb 2022 00:51:03 GMT
ARG ODOO_SHA=b7a4ab618dc5144ebf02ff91d8c151dca30080d7
# Fri, 18 Feb 2022 00:52:25 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=b7a4ab618dc5144ebf02ff91d8c151dca30080d7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Feb 2022 00:52:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Feb 2022 00:52:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Feb 2022 00:52:30 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=b7a4ab618dc5144ebf02ff91d8c151dca30080d7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Feb 2022 00:52:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Feb 2022 00:52:30 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Feb 2022 00:52:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Feb 2022 00:52:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Feb 2022 00:52:31 GMT
USER odoo
# Fri, 18 Feb 2022 00:52:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Feb 2022 00:52:31 GMT
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
	-	`sha256:a1beb6c82f285df49a16954ca3714db8724e0bb03a11df5c30578bf3e3fe10eb`  
		Last Modified: Fri, 18 Feb 2022 00:56:00 GMT  
		Size: 275.2 MB (275174010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691550dcf09a72f5e6775ecda918dd6085d4e9e907f403f7fac338ee3b3df0d6`  
		Last Modified: Fri, 18 Feb 2022 00:55:25 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf51771edae9b5694d711bf7787b863c04514eee3446edbf907367ca6db715e4`  
		Last Modified: Fri, 18 Feb 2022 00:55:25 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f65bb023652b60dd49c7d39e537fd86fe9b9ca48d3ca490e19ff3a5221f9d5`  
		Last Modified: Fri, 18 Feb 2022 00:55:25 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3aa912426ad79afafaf22738f9db3c3a8f8362b209da4d3fe4ff9873f9eaa2`  
		Last Modified: Fri, 18 Feb 2022 00:55:25 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:cd76bc867cf9ffee2260032686cee29fc4aa3287581c9c9f8d5644602e364dad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:fb26036e812edaff5539ee8a404cd4670da6a187c12697d18add42c7265bd5fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.4 MB (529386852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ba73aacd429c84d80d286455901bf4e63dc20656c01b0e2248bd56006a548a`
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
# Fri, 18 Feb 2022 00:51:02 GMT
ARG ODOO_RELEASE=20220217
# Fri, 18 Feb 2022 00:51:03 GMT
ARG ODOO_SHA=b7a4ab618dc5144ebf02ff91d8c151dca30080d7
# Fri, 18 Feb 2022 00:52:25 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=b7a4ab618dc5144ebf02ff91d8c151dca30080d7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Feb 2022 00:52:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Feb 2022 00:52:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Feb 2022 00:52:30 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=b7a4ab618dc5144ebf02ff91d8c151dca30080d7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Feb 2022 00:52:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Feb 2022 00:52:30 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Feb 2022 00:52:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Feb 2022 00:52:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Feb 2022 00:52:31 GMT
USER odoo
# Fri, 18 Feb 2022 00:52:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Feb 2022 00:52:31 GMT
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
	-	`sha256:a1beb6c82f285df49a16954ca3714db8724e0bb03a11df5c30578bf3e3fe10eb`  
		Last Modified: Fri, 18 Feb 2022 00:56:00 GMT  
		Size: 275.2 MB (275174010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691550dcf09a72f5e6775ecda918dd6085d4e9e907f403f7fac338ee3b3df0d6`  
		Last Modified: Fri, 18 Feb 2022 00:55:25 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf51771edae9b5694d711bf7787b863c04514eee3446edbf907367ca6db715e4`  
		Last Modified: Fri, 18 Feb 2022 00:55:25 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f65bb023652b60dd49c7d39e537fd86fe9b9ca48d3ca490e19ff3a5221f9d5`  
		Last Modified: Fri, 18 Feb 2022 00:55:25 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3aa912426ad79afafaf22738f9db3c3a8f8362b209da4d3fe4ff9873f9eaa2`  
		Last Modified: Fri, 18 Feb 2022 00:55:25 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:788506e9b7c50ef258a7dc936e120ee92e140d40bc78d89850be6cd24cc0fdef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:d79ed77fb63231aec6937c5dcb49b948f6cc6cea20e3a5307d62cc9563814f4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **548.9 MB (548899376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddaf343ae4ef9899c0031c8b9eae585d4e2c6255a5dac38a55fa56ba27302bae`
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
# Fri, 18 Feb 2022 00:48:53 GMT
ARG ODOO_RELEASE=20220217
# Fri, 18 Feb 2022 00:48:54 GMT
ARG ODOO_SHA=1cd3850c04e63652b2c66b73d8e8d7e013777e2f
# Fri, 18 Feb 2022 00:50:40 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=1cd3850c04e63652b2c66b73d8e8d7e013777e2f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Feb 2022 00:50:43 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Feb 2022 00:50:43 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Feb 2022 00:50:44 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=1cd3850c04e63652b2c66b73d8e8d7e013777e2f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Feb 2022 00:50:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Feb 2022 00:50:45 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Feb 2022 00:50:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Feb 2022 00:50:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Feb 2022 00:50:46 GMT
USER odoo
# Fri, 18 Feb 2022 00:50:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Feb 2022 00:50:46 GMT
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
	-	`sha256:e2855f887d0ff580e6137174b71fa9750d9eaf2eb7619c3725225eb0f903f126`  
		Last Modified: Fri, 18 Feb 2022 00:55:13 GMT  
		Size: 294.3 MB (294293228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c303c99e22e31ce38b0f55c9deba242e520868bc5dd622060d3dcc873b9fdf2`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148bc3cc0a30a6e659f28cabf4e41e5506260e9165a2ce6b4c72e8afc75ff921`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b17eb6ce6a781d7e9950c5654b19f48dd07a388000cb41ced175eae3f4863`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c795a72ad1eff0f27fad400f91cbdab798d0eb4fff5846100881ab6a8dd0711`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:788506e9b7c50ef258a7dc936e120ee92e140d40bc78d89850be6cd24cc0fdef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:d79ed77fb63231aec6937c5dcb49b948f6cc6cea20e3a5307d62cc9563814f4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **548.9 MB (548899376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddaf343ae4ef9899c0031c8b9eae585d4e2c6255a5dac38a55fa56ba27302bae`
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
# Fri, 18 Feb 2022 00:48:53 GMT
ARG ODOO_RELEASE=20220217
# Fri, 18 Feb 2022 00:48:54 GMT
ARG ODOO_SHA=1cd3850c04e63652b2c66b73d8e8d7e013777e2f
# Fri, 18 Feb 2022 00:50:40 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=1cd3850c04e63652b2c66b73d8e8d7e013777e2f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Feb 2022 00:50:43 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Feb 2022 00:50:43 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Feb 2022 00:50:44 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=1cd3850c04e63652b2c66b73d8e8d7e013777e2f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Feb 2022 00:50:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Feb 2022 00:50:45 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Feb 2022 00:50:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Feb 2022 00:50:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Feb 2022 00:50:46 GMT
USER odoo
# Fri, 18 Feb 2022 00:50:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Feb 2022 00:50:46 GMT
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
	-	`sha256:e2855f887d0ff580e6137174b71fa9750d9eaf2eb7619c3725225eb0f903f126`  
		Last Modified: Fri, 18 Feb 2022 00:55:13 GMT  
		Size: 294.3 MB (294293228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c303c99e22e31ce38b0f55c9deba242e520868bc5dd622060d3dcc873b9fdf2`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148bc3cc0a30a6e659f28cabf4e41e5506260e9165a2ce6b4c72e8afc75ff921`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b17eb6ce6a781d7e9950c5654b19f48dd07a388000cb41ced175eae3f4863`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c795a72ad1eff0f27fad400f91cbdab798d0eb4fff5846100881ab6a8dd0711`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:788506e9b7c50ef258a7dc936e120ee92e140d40bc78d89850be6cd24cc0fdef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:d79ed77fb63231aec6937c5dcb49b948f6cc6cea20e3a5307d62cc9563814f4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **548.9 MB (548899376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddaf343ae4ef9899c0031c8b9eae585d4e2c6255a5dac38a55fa56ba27302bae`
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
# Fri, 18 Feb 2022 00:48:53 GMT
ARG ODOO_RELEASE=20220217
# Fri, 18 Feb 2022 00:48:54 GMT
ARG ODOO_SHA=1cd3850c04e63652b2c66b73d8e8d7e013777e2f
# Fri, 18 Feb 2022 00:50:40 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=1cd3850c04e63652b2c66b73d8e8d7e013777e2f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Feb 2022 00:50:43 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Feb 2022 00:50:43 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Feb 2022 00:50:44 GMT
# ARGS: ODOO_RELEASE=20220217 ODOO_SHA=1cd3850c04e63652b2c66b73d8e8d7e013777e2f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Feb 2022 00:50:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Feb 2022 00:50:45 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Feb 2022 00:50:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Feb 2022 00:50:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Feb 2022 00:50:46 GMT
USER odoo
# Fri, 18 Feb 2022 00:50:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Feb 2022 00:50:46 GMT
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
	-	`sha256:e2855f887d0ff580e6137174b71fa9750d9eaf2eb7619c3725225eb0f903f126`  
		Last Modified: Fri, 18 Feb 2022 00:55:13 GMT  
		Size: 294.3 MB (294293228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c303c99e22e31ce38b0f55c9deba242e520868bc5dd622060d3dcc873b9fdf2`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148bc3cc0a30a6e659f28cabf4e41e5506260e9165a2ce6b4c72e8afc75ff921`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921b17eb6ce6a781d7e9950c5654b19f48dd07a388000cb41ced175eae3f4863`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c795a72ad1eff0f27fad400f91cbdab798d0eb4fff5846100881ab6a8dd0711`  
		Last Modified: Fri, 18 Feb 2022 00:54:29 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
