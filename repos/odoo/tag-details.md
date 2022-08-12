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
$ docker pull odoo@sha256:56a5f4ce5564ccc63556e52d191c783a5c8dde4966dcc9bf81a92cc7d97689c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:4360ddf883d9266a8f2052bfeb0fd4ea031940d48ad6bad037b3eaab7ae07c2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.4 MB (540384892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98766d6a36ddc074d60968d8ddaed2a2196f39b4fc318eb475f8506877a7ad5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:24 GMT
ADD file:81dbfe4f9df4d280f7580380c0c5c93ba71fedba17b3072d2b7b4bce127f88a9 in / 
# Tue, 02 Aug 2022 01:20:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:38:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 02 Aug 2022 05:38:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 02 Aug 2022 05:38:48 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 05:42:38 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 02 Aug 2022 05:42:47 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:42:50 GMT
RUN npm install -g rtlcss
# Tue, 02 Aug 2022 05:42:50 GMT
ENV ODOO_VERSION=13.0
# Fri, 12 Aug 2022 21:01:02 GMT
ARG ODOO_RELEASE=20220812
# Fri, 12 Aug 2022 21:01:02 GMT
ARG ODOO_SHA=cde4183434f9004943b5ed5792c4d899e1901d06
# Fri, 12 Aug 2022 21:02:17 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=cde4183434f9004943b5ed5792c4d899e1901d06
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 12 Aug 2022 21:02:21 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 12 Aug 2022 21:02:21 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 12 Aug 2022 21:02:22 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=cde4183434f9004943b5ed5792c4d899e1901d06
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 12 Aug 2022 21:02:22 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 12 Aug 2022 21:02:22 GMT
EXPOSE 8069 8071 8072
# Fri, 12 Aug 2022 21:02:22 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 12 Aug 2022 21:02:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 12 Aug 2022 21:02:22 GMT
USER odoo
# Fri, 12 Aug 2022 21:02:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Aug 2022 21:02:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:751ef25978b2971e15496369695ba51ed5b1b9aaca7e37b18a173d754d1ca820`  
		Last Modified: Tue, 02 Aug 2022 01:25:00 GMT  
		Size: 27.1 MB (27140083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5718371f43c618dd7c037dc9e6f276d3bdfb4242e47d30ede3d8e797f7e6f78a`  
		Last Modified: Tue, 02 Aug 2022 05:46:33 GMT  
		Size: 207.1 MB (207143577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b563a78258fd2c7c9ee449d16fdd0f86d7c54d1784ca7c103dd02900afc29168`  
		Last Modified: Tue, 02 Aug 2022 05:46:13 GMT  
		Size: 13.4 MB (13442945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b350b162f7b9f79c7d63f4e71229b205d9070f98f801cf71ad2b9211e8ede686`  
		Last Modified: Tue, 02 Aug 2022 05:46:09 GMT  
		Size: 508.4 KB (508417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4368c3a76f1e858322bbb3ae0430272da7ab90ea11413c123bed7619c1e0f1`  
		Last Modified: Fri, 12 Aug 2022 21:04:40 GMT  
		Size: 292.1 MB (292147405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7196053602655444e2eefafcad77f70b0613a699589d7fdd8eb578b48f6a9d4d`  
		Last Modified: Fri, 12 Aug 2022 21:04:07 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff85f81e4d2f4eb14f0981456d969e813e7a82e40f080b8c20a1411f9a49b4b0`  
		Last Modified: Fri, 12 Aug 2022 21:04:07 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd8e0eedbf40dd364bf75ffe4afa133b8faa66efab173ecd6f62fab54ddd797`  
		Last Modified: Fri, 12 Aug 2022 21:04:07 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df40a7b31cbc232a30b6e3117c63c455b5ffb824e70151cae32cc5ea57555e9`  
		Last Modified: Fri, 12 Aug 2022 21:04:07 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:56a5f4ce5564ccc63556e52d191c783a5c8dde4966dcc9bf81a92cc7d97689c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:4360ddf883d9266a8f2052bfeb0fd4ea031940d48ad6bad037b3eaab7ae07c2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.4 MB (540384892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98766d6a36ddc074d60968d8ddaed2a2196f39b4fc318eb475f8506877a7ad5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:24 GMT
ADD file:81dbfe4f9df4d280f7580380c0c5c93ba71fedba17b3072d2b7b4bce127f88a9 in / 
# Tue, 02 Aug 2022 01:20:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:38:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 02 Aug 2022 05:38:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 02 Aug 2022 05:38:48 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 05:42:38 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 02 Aug 2022 05:42:47 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:42:50 GMT
RUN npm install -g rtlcss
# Tue, 02 Aug 2022 05:42:50 GMT
ENV ODOO_VERSION=13.0
# Fri, 12 Aug 2022 21:01:02 GMT
ARG ODOO_RELEASE=20220812
# Fri, 12 Aug 2022 21:01:02 GMT
ARG ODOO_SHA=cde4183434f9004943b5ed5792c4d899e1901d06
# Fri, 12 Aug 2022 21:02:17 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=cde4183434f9004943b5ed5792c4d899e1901d06
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 12 Aug 2022 21:02:21 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 12 Aug 2022 21:02:21 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 12 Aug 2022 21:02:22 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=cde4183434f9004943b5ed5792c4d899e1901d06
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 12 Aug 2022 21:02:22 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 12 Aug 2022 21:02:22 GMT
EXPOSE 8069 8071 8072
# Fri, 12 Aug 2022 21:02:22 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 12 Aug 2022 21:02:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 12 Aug 2022 21:02:22 GMT
USER odoo
# Fri, 12 Aug 2022 21:02:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Aug 2022 21:02:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:751ef25978b2971e15496369695ba51ed5b1b9aaca7e37b18a173d754d1ca820`  
		Last Modified: Tue, 02 Aug 2022 01:25:00 GMT  
		Size: 27.1 MB (27140083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5718371f43c618dd7c037dc9e6f276d3bdfb4242e47d30ede3d8e797f7e6f78a`  
		Last Modified: Tue, 02 Aug 2022 05:46:33 GMT  
		Size: 207.1 MB (207143577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b563a78258fd2c7c9ee449d16fdd0f86d7c54d1784ca7c103dd02900afc29168`  
		Last Modified: Tue, 02 Aug 2022 05:46:13 GMT  
		Size: 13.4 MB (13442945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b350b162f7b9f79c7d63f4e71229b205d9070f98f801cf71ad2b9211e8ede686`  
		Last Modified: Tue, 02 Aug 2022 05:46:09 GMT  
		Size: 508.4 KB (508417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4368c3a76f1e858322bbb3ae0430272da7ab90ea11413c123bed7619c1e0f1`  
		Last Modified: Fri, 12 Aug 2022 21:04:40 GMT  
		Size: 292.1 MB (292147405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7196053602655444e2eefafcad77f70b0613a699589d7fdd8eb578b48f6a9d4d`  
		Last Modified: Fri, 12 Aug 2022 21:04:07 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff85f81e4d2f4eb14f0981456d969e813e7a82e40f080b8c20a1411f9a49b4b0`  
		Last Modified: Fri, 12 Aug 2022 21:04:07 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd8e0eedbf40dd364bf75ffe4afa133b8faa66efab173ecd6f62fab54ddd797`  
		Last Modified: Fri, 12 Aug 2022 21:04:07 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df40a7b31cbc232a30b6e3117c63c455b5ffb824e70151cae32cc5ea57555e9`  
		Last Modified: Fri, 12 Aug 2022 21:04:07 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:479987d26b4795a456dc1bd6b8114102af2a79fa47adc6e6393f038f7de8602d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:ea8a155713b7cbe033a6da8f14c368403b81b1aa24261d5fc8994607f927ddcf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.9 MB (530852761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683bac9d379b8a52d0d0c9170b2a2875898217fc8690d38e9afbc1f8e38315d1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:24 GMT
ADD file:81dbfe4f9df4d280f7580380c0c5c93ba71fedba17b3072d2b7b4bce127f88a9 in / 
# Tue, 02 Aug 2022 01:20:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:38:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 02 Aug 2022 05:38:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 02 Aug 2022 05:38:48 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 05:39:53 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 02 Aug 2022 05:40:06 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:40:09 GMT
RUN npm install -g rtlcss
# Tue, 02 Aug 2022 05:40:09 GMT
ENV ODOO_VERSION=14.0
# Fri, 12 Aug 2022 20:59:39 GMT
ARG ODOO_RELEASE=20220812
# Fri, 12 Aug 2022 20:59:39 GMT
ARG ODOO_SHA=91048a02688e4d22aa188db7802e2eb6c07cb081
# Fri, 12 Aug 2022 21:00:52 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=91048a02688e4d22aa188db7802e2eb6c07cb081
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 12 Aug 2022 21:00:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 12 Aug 2022 21:00:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 12 Aug 2022 21:00:56 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=91048a02688e4d22aa188db7802e2eb6c07cb081
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 12 Aug 2022 21:00:57 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 12 Aug 2022 21:00:57 GMT
EXPOSE 8069 8071 8072
# Fri, 12 Aug 2022 21:00:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 12 Aug 2022 21:00:57 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 12 Aug 2022 21:00:57 GMT
USER odoo
# Fri, 12 Aug 2022 21:00:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Aug 2022 21:00:57 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:751ef25978b2971e15496369695ba51ed5b1b9aaca7e37b18a173d754d1ca820`  
		Last Modified: Tue, 02 Aug 2022 01:25:00 GMT  
		Size: 27.1 MB (27140083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2a9029ee3604b9372e42d87384e5e066e9148be333e0dc03e9c8f855e427b`  
		Last Modified: Tue, 02 Aug 2022 05:45:48 GMT  
		Size: 213.2 MB (213182454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d65776201572904d097cfdcb3376d445b11bfc305826f497d3cafee088aeb73`  
		Last Modified: Tue, 02 Aug 2022 05:45:26 GMT  
		Size: 13.4 MB (13444602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470b77fa97db81c4c7ed1ba15b82f7fd432abb5d20e2953a06898a889d44ca6b`  
		Last Modified: Tue, 02 Aug 2022 05:45:23 GMT  
		Size: 508.2 KB (508239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b049d7aa7544b7b977d0b84f0a9c0fd98ce74f1ceed9dc5f237ea4db0be131`  
		Last Modified: Fri, 12 Aug 2022 21:03:57 GMT  
		Size: 276.6 MB (276574921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a9a0ba92c6e21efbac691c6b8da5e60f4357a3c3ea1bcf029d7dc4605b45b7`  
		Last Modified: Fri, 12 Aug 2022 21:03:25 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fb2b2332ab27074d4ab1efbf561c30d89ad7efe7d02f3f1c09c6934e4e0b6a`  
		Last Modified: Fri, 12 Aug 2022 21:03:25 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1e284632d0fc22dbdb6b51cea2b54eaff8abd8d8e4a4d750903c50daecfb32`  
		Last Modified: Fri, 12 Aug 2022 21:03:24 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb3db2587dca9ac7989a2f118ef3d9dd31e0a38811105b0b721139bf5c8a13d`  
		Last Modified: Fri, 12 Aug 2022 21:03:25 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:479987d26b4795a456dc1bd6b8114102af2a79fa47adc6e6393f038f7de8602d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:ea8a155713b7cbe033a6da8f14c368403b81b1aa24261d5fc8994607f927ddcf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.9 MB (530852761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683bac9d379b8a52d0d0c9170b2a2875898217fc8690d38e9afbc1f8e38315d1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:24 GMT
ADD file:81dbfe4f9df4d280f7580380c0c5c93ba71fedba17b3072d2b7b4bce127f88a9 in / 
# Tue, 02 Aug 2022 01:20:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:38:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 02 Aug 2022 05:38:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 02 Aug 2022 05:38:48 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 05:39:53 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 02 Aug 2022 05:40:06 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:40:09 GMT
RUN npm install -g rtlcss
# Tue, 02 Aug 2022 05:40:09 GMT
ENV ODOO_VERSION=14.0
# Fri, 12 Aug 2022 20:59:39 GMT
ARG ODOO_RELEASE=20220812
# Fri, 12 Aug 2022 20:59:39 GMT
ARG ODOO_SHA=91048a02688e4d22aa188db7802e2eb6c07cb081
# Fri, 12 Aug 2022 21:00:52 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=91048a02688e4d22aa188db7802e2eb6c07cb081
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 12 Aug 2022 21:00:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 12 Aug 2022 21:00:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 12 Aug 2022 21:00:56 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=91048a02688e4d22aa188db7802e2eb6c07cb081
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 12 Aug 2022 21:00:57 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 12 Aug 2022 21:00:57 GMT
EXPOSE 8069 8071 8072
# Fri, 12 Aug 2022 21:00:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 12 Aug 2022 21:00:57 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 12 Aug 2022 21:00:57 GMT
USER odoo
# Fri, 12 Aug 2022 21:00:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Aug 2022 21:00:57 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:751ef25978b2971e15496369695ba51ed5b1b9aaca7e37b18a173d754d1ca820`  
		Last Modified: Tue, 02 Aug 2022 01:25:00 GMT  
		Size: 27.1 MB (27140083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2a9029ee3604b9372e42d87384e5e066e9148be333e0dc03e9c8f855e427b`  
		Last Modified: Tue, 02 Aug 2022 05:45:48 GMT  
		Size: 213.2 MB (213182454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d65776201572904d097cfdcb3376d445b11bfc305826f497d3cafee088aeb73`  
		Last Modified: Tue, 02 Aug 2022 05:45:26 GMT  
		Size: 13.4 MB (13444602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470b77fa97db81c4c7ed1ba15b82f7fd432abb5d20e2953a06898a889d44ca6b`  
		Last Modified: Tue, 02 Aug 2022 05:45:23 GMT  
		Size: 508.2 KB (508239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b049d7aa7544b7b977d0b84f0a9c0fd98ce74f1ceed9dc5f237ea4db0be131`  
		Last Modified: Fri, 12 Aug 2022 21:03:57 GMT  
		Size: 276.6 MB (276574921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a9a0ba92c6e21efbac691c6b8da5e60f4357a3c3ea1bcf029d7dc4605b45b7`  
		Last Modified: Fri, 12 Aug 2022 21:03:25 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fb2b2332ab27074d4ab1efbf561c30d89ad7efe7d02f3f1c09c6934e4e0b6a`  
		Last Modified: Fri, 12 Aug 2022 21:03:25 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1e284632d0fc22dbdb6b51cea2b54eaff8abd8d8e4a4d750903c50daecfb32`  
		Last Modified: Fri, 12 Aug 2022 21:03:24 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb3db2587dca9ac7989a2f118ef3d9dd31e0a38811105b0b721139bf5c8a13d`  
		Last Modified: Fri, 12 Aug 2022 21:03:25 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:c00026af75004041f4d0000c8dd40c5b991c8964ef73d628e0a217df918ddbef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:b8ed5a50552cf2731678668e3af69dd6e1ed55a97daae21f4cc08596e8b920bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.8 MB (557764760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf8b38c6e36f039b4c5dd882b94f262e9ed1d7c213984a60bfd0f35523328a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:36:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 02 Aug 2022 05:36:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 02 Aug 2022 05:36:10 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 05:37:09 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 02 Aug 2022 05:37:19 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:37:21 GMT
RUN npm install -g rtlcss
# Tue, 02 Aug 2022 05:37:21 GMT
ENV ODOO_VERSION=15.0
# Fri, 12 Aug 2022 20:58:01 GMT
ARG ODOO_RELEASE=20220812
# Fri, 12 Aug 2022 20:58:01 GMT
ARG ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
# Fri, 12 Aug 2022 20:59:20 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 12 Aug 2022 20:59:25 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 12 Aug 2022 20:59:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 12 Aug 2022 20:59:25 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 12 Aug 2022 20:59:25 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 12 Aug 2022 20:59:26 GMT
EXPOSE 8069 8071 8072
# Fri, 12 Aug 2022 20:59:26 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 12 Aug 2022 20:59:26 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 12 Aug 2022 20:59:26 GMT
USER odoo
# Fri, 12 Aug 2022 20:59:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Aug 2022 20:59:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc04a644bed3d89143e2aa316af36b00716f4554c4f513da256351fe8cce70aa`  
		Last Modified: Tue, 02 Aug 2022 05:45:00 GMT  
		Size: 220.3 MB (220296597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad4934bbcf7f8f118d6cb4c9dee0e952084f336902f9279646ba728e05729cb`  
		Last Modified: Tue, 02 Aug 2022 05:44:34 GMT  
		Size: 2.5 MB (2513325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77946ee2a1b368dc2efeb7362de7ab48b80331ab4549032ab68486f60bc166ba`  
		Last Modified: Tue, 02 Aug 2022 05:44:33 GMT  
		Size: 502.0 KB (501982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2efed753a3cd370ba3d137eac4c8ccc248091d59b667ddc71801411bf4c559`  
		Last Modified: Fri, 12 Aug 2022 21:03:11 GMT  
		Size: 303.1 MB (303083638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55215f540a300038e579642dcf31d6ec9b159c715e96bd352b71318a3616ec7a`  
		Last Modified: Fri, 12 Aug 2022 21:02:40 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a970400473ae4cf1a239965d63dcf0c2c5e5cb38ccd6d21e9b8dea01219eadb`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5cd72681947ff93f98358119c7f9b078248c9c0f75efd61137874ae26d2a97`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6996b3f50e0e9ee247af79d077cbe84b012b933334c959fb1ce6d3358c6d8f6`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:c00026af75004041f4d0000c8dd40c5b991c8964ef73d628e0a217df918ddbef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:b8ed5a50552cf2731678668e3af69dd6e1ed55a97daae21f4cc08596e8b920bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.8 MB (557764760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf8b38c6e36f039b4c5dd882b94f262e9ed1d7c213984a60bfd0f35523328a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:36:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 02 Aug 2022 05:36:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 02 Aug 2022 05:36:10 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 05:37:09 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 02 Aug 2022 05:37:19 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:37:21 GMT
RUN npm install -g rtlcss
# Tue, 02 Aug 2022 05:37:21 GMT
ENV ODOO_VERSION=15.0
# Fri, 12 Aug 2022 20:58:01 GMT
ARG ODOO_RELEASE=20220812
# Fri, 12 Aug 2022 20:58:01 GMT
ARG ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
# Fri, 12 Aug 2022 20:59:20 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 12 Aug 2022 20:59:25 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 12 Aug 2022 20:59:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 12 Aug 2022 20:59:25 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 12 Aug 2022 20:59:25 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 12 Aug 2022 20:59:26 GMT
EXPOSE 8069 8071 8072
# Fri, 12 Aug 2022 20:59:26 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 12 Aug 2022 20:59:26 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 12 Aug 2022 20:59:26 GMT
USER odoo
# Fri, 12 Aug 2022 20:59:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Aug 2022 20:59:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc04a644bed3d89143e2aa316af36b00716f4554c4f513da256351fe8cce70aa`  
		Last Modified: Tue, 02 Aug 2022 05:45:00 GMT  
		Size: 220.3 MB (220296597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad4934bbcf7f8f118d6cb4c9dee0e952084f336902f9279646ba728e05729cb`  
		Last Modified: Tue, 02 Aug 2022 05:44:34 GMT  
		Size: 2.5 MB (2513325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77946ee2a1b368dc2efeb7362de7ab48b80331ab4549032ab68486f60bc166ba`  
		Last Modified: Tue, 02 Aug 2022 05:44:33 GMT  
		Size: 502.0 KB (501982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2efed753a3cd370ba3d137eac4c8ccc248091d59b667ddc71801411bf4c559`  
		Last Modified: Fri, 12 Aug 2022 21:03:11 GMT  
		Size: 303.1 MB (303083638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55215f540a300038e579642dcf31d6ec9b159c715e96bd352b71318a3616ec7a`  
		Last Modified: Fri, 12 Aug 2022 21:02:40 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a970400473ae4cf1a239965d63dcf0c2c5e5cb38ccd6d21e9b8dea01219eadb`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5cd72681947ff93f98358119c7f9b078248c9c0f75efd61137874ae26d2a97`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6996b3f50e0e9ee247af79d077cbe84b012b933334c959fb1ce6d3358c6d8f6`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:c00026af75004041f4d0000c8dd40c5b991c8964ef73d628e0a217df918ddbef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:b8ed5a50552cf2731678668e3af69dd6e1ed55a97daae21f4cc08596e8b920bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.8 MB (557764760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf8b38c6e36f039b4c5dd882b94f262e9ed1d7c213984a60bfd0f35523328a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:36:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 02 Aug 2022 05:36:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 02 Aug 2022 05:36:10 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 05:37:09 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 02 Aug 2022 05:37:19 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:37:21 GMT
RUN npm install -g rtlcss
# Tue, 02 Aug 2022 05:37:21 GMT
ENV ODOO_VERSION=15.0
# Fri, 12 Aug 2022 20:58:01 GMT
ARG ODOO_RELEASE=20220812
# Fri, 12 Aug 2022 20:58:01 GMT
ARG ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
# Fri, 12 Aug 2022 20:59:20 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 12 Aug 2022 20:59:25 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 12 Aug 2022 20:59:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 12 Aug 2022 20:59:25 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 12 Aug 2022 20:59:25 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 12 Aug 2022 20:59:26 GMT
EXPOSE 8069 8071 8072
# Fri, 12 Aug 2022 20:59:26 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 12 Aug 2022 20:59:26 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 12 Aug 2022 20:59:26 GMT
USER odoo
# Fri, 12 Aug 2022 20:59:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Aug 2022 20:59:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc04a644bed3d89143e2aa316af36b00716f4554c4f513da256351fe8cce70aa`  
		Last Modified: Tue, 02 Aug 2022 05:45:00 GMT  
		Size: 220.3 MB (220296597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad4934bbcf7f8f118d6cb4c9dee0e952084f336902f9279646ba728e05729cb`  
		Last Modified: Tue, 02 Aug 2022 05:44:34 GMT  
		Size: 2.5 MB (2513325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77946ee2a1b368dc2efeb7362de7ab48b80331ab4549032ab68486f60bc166ba`  
		Last Modified: Tue, 02 Aug 2022 05:44:33 GMT  
		Size: 502.0 KB (501982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2efed753a3cd370ba3d137eac4c8ccc248091d59b667ddc71801411bf4c559`  
		Last Modified: Fri, 12 Aug 2022 21:03:11 GMT  
		Size: 303.1 MB (303083638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55215f540a300038e579642dcf31d6ec9b159c715e96bd352b71318a3616ec7a`  
		Last Modified: Fri, 12 Aug 2022 21:02:40 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a970400473ae4cf1a239965d63dcf0c2c5e5cb38ccd6d21e9b8dea01219eadb`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5cd72681947ff93f98358119c7f9b078248c9c0f75efd61137874ae26d2a97`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6996b3f50e0e9ee247af79d077cbe84b012b933334c959fb1ce6d3358c6d8f6`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
