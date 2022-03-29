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
$ docker pull odoo@sha256:6db9db2bc9f3ac548242fc103243ae699793ec2447adc3c603abc97035b11619
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:9ec42a56614eb11a84c49ae7cfa6078066bbda0dadfcc036d0d8194588660ea4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539678620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7686ecdc3f9fb5ea5796b79f406c823b6376f2d4ef776513382e5ebfc31b80ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 19:02:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 29 Mar 2022 19:02:29 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 29 Mar 2022 19:02:29 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 19:06:03 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 29 Mar 2022 19:06:12 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 19:06:15 GMT
RUN npm install -g rtlcss
# Tue, 29 Mar 2022 19:06:15 GMT
ENV ODOO_VERSION=13.0
# Tue, 29 Mar 2022 19:06:15 GMT
ARG ODOO_RELEASE=20220325
# Tue, 29 Mar 2022 19:06:15 GMT
ARG ODOO_SHA=93b53403ec8f09103d6c2cb70dc4901756bc58d2
# Tue, 29 Mar 2022 19:07:26 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=93b53403ec8f09103d6c2cb70dc4901756bc58d2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 29 Mar 2022 19:07:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 29 Mar 2022 19:07:30 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 29 Mar 2022 19:07:30 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=93b53403ec8f09103d6c2cb70dc4901756bc58d2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 29 Mar 2022 19:07:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 29 Mar 2022 19:07:30 GMT
EXPOSE 8069 8071 8072
# Tue, 29 Mar 2022 19:07:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 29 Mar 2022 19:07:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 29 Mar 2022 19:07:31 GMT
USER odoo
# Tue, 29 Mar 2022 19:07:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 19:07:31 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a511858723517facee7b2235b79b364ee6ebcf20153dc49f3c226d6d4e39e363`  
		Last Modified: Tue, 29 Mar 2022 19:10:01 GMT  
		Size: 207.1 MB (207143257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fead8ec7541d6642b89ca7e91985366ae38f95e593cea160b9edb52516a5598`  
		Last Modified: Tue, 29 Mar 2022 19:09:38 GMT  
		Size: 13.4 MB (13438585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396d3da3445e859d637b818783f718c773ee45472a72a96f4a29bc61e2726e4e`  
		Last Modified: Tue, 29 Mar 2022 19:09:35 GMT  
		Size: 457.2 KB (457185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e94e4f308d6ed0abd5c938cd57381d91483f97eb9f5e622b5ed6ddbcc1d180c`  
		Last Modified: Tue, 29 Mar 2022 19:10:07 GMT  
		Size: 291.5 MB (291485162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00bc6c1ff1d653ce507f3526151051d3ac712ff746cc7904d0113ac069714ae1`  
		Last Modified: Tue, 29 Mar 2022 19:09:33 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f13002ba65ce11d855a462fe1c3b33bdb1da77b8f3113fdc38b64a2984829d4`  
		Last Modified: Tue, 29 Mar 2022 19:09:33 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b7023a675a94302558dcc60ea9f142cbc42c125b199071e139926a92759755`  
		Last Modified: Tue, 29 Mar 2022 19:09:32 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e17869c2cee9e9e793f2e0b7d41cfe30722ba7511584801e3a8505bc796d41`  
		Last Modified: Tue, 29 Mar 2022 19:09:32 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:6db9db2bc9f3ac548242fc103243ae699793ec2447adc3c603abc97035b11619
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:9ec42a56614eb11a84c49ae7cfa6078066bbda0dadfcc036d0d8194588660ea4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539678620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7686ecdc3f9fb5ea5796b79f406c823b6376f2d4ef776513382e5ebfc31b80ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 19:02:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 29 Mar 2022 19:02:29 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 29 Mar 2022 19:02:29 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 19:06:03 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 29 Mar 2022 19:06:12 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 19:06:15 GMT
RUN npm install -g rtlcss
# Tue, 29 Mar 2022 19:06:15 GMT
ENV ODOO_VERSION=13.0
# Tue, 29 Mar 2022 19:06:15 GMT
ARG ODOO_RELEASE=20220325
# Tue, 29 Mar 2022 19:06:15 GMT
ARG ODOO_SHA=93b53403ec8f09103d6c2cb70dc4901756bc58d2
# Tue, 29 Mar 2022 19:07:26 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=93b53403ec8f09103d6c2cb70dc4901756bc58d2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 29 Mar 2022 19:07:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 29 Mar 2022 19:07:30 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 29 Mar 2022 19:07:30 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=93b53403ec8f09103d6c2cb70dc4901756bc58d2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 29 Mar 2022 19:07:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 29 Mar 2022 19:07:30 GMT
EXPOSE 8069 8071 8072
# Tue, 29 Mar 2022 19:07:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 29 Mar 2022 19:07:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 29 Mar 2022 19:07:31 GMT
USER odoo
# Tue, 29 Mar 2022 19:07:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 19:07:31 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a511858723517facee7b2235b79b364ee6ebcf20153dc49f3c226d6d4e39e363`  
		Last Modified: Tue, 29 Mar 2022 19:10:01 GMT  
		Size: 207.1 MB (207143257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fead8ec7541d6642b89ca7e91985366ae38f95e593cea160b9edb52516a5598`  
		Last Modified: Tue, 29 Mar 2022 19:09:38 GMT  
		Size: 13.4 MB (13438585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396d3da3445e859d637b818783f718c773ee45472a72a96f4a29bc61e2726e4e`  
		Last Modified: Tue, 29 Mar 2022 19:09:35 GMT  
		Size: 457.2 KB (457185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e94e4f308d6ed0abd5c938cd57381d91483f97eb9f5e622b5ed6ddbcc1d180c`  
		Last Modified: Tue, 29 Mar 2022 19:10:07 GMT  
		Size: 291.5 MB (291485162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00bc6c1ff1d653ce507f3526151051d3ac712ff746cc7904d0113ac069714ae1`  
		Last Modified: Tue, 29 Mar 2022 19:09:33 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f13002ba65ce11d855a462fe1c3b33bdb1da77b8f3113fdc38b64a2984829d4`  
		Last Modified: Tue, 29 Mar 2022 19:09:33 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b7023a675a94302558dcc60ea9f142cbc42c125b199071e139926a92759755`  
		Last Modified: Tue, 29 Mar 2022 19:09:32 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e17869c2cee9e9e793f2e0b7d41cfe30722ba7511584801e3a8505bc796d41`  
		Last Modified: Tue, 29 Mar 2022 19:09:32 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:8d159d83d33a5e7e1b799adcef52f26203744d2430c36d1002bd0f657203d204
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:647d9981604b8fc8c0773f3346908e7b8b0a43eb64941d2455effecef06780f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.5 MB (529540866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba95c862a87233f1a0dc9ec658f166847c59f18389ace89741d2a6f679a66d3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 19:02:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 29 Mar 2022 19:02:29 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 29 Mar 2022 19:02:29 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 19:03:32 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 29 Mar 2022 19:03:44 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 19:03:47 GMT
RUN npm install -g rtlcss
# Tue, 29 Mar 2022 19:03:47 GMT
ENV ODOO_VERSION=14.0
# Tue, 29 Mar 2022 19:03:47 GMT
ARG ODOO_RELEASE=20220325
# Tue, 29 Mar 2022 19:03:48 GMT
ARG ODOO_SHA=eabfcf757b772782f11db1ea484e9319be58c3c5
# Tue, 29 Mar 2022 19:04:59 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=eabfcf757b772782f11db1ea484e9319be58c3c5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 29 Mar 2022 19:05:03 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 29 Mar 2022 19:05:03 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 29 Mar 2022 19:05:04 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=eabfcf757b772782f11db1ea484e9319be58c3c5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 29 Mar 2022 19:05:04 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 29 Mar 2022 19:05:04 GMT
EXPOSE 8069 8071 8072
# Tue, 29 Mar 2022 19:05:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 29 Mar 2022 19:05:04 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 29 Mar 2022 19:05:05 GMT
USER odoo
# Tue, 29 Mar 2022 19:05:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 19:05:05 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d71810975b7f42c776c1f507c47736d2bd6904ab77b06df0c936554750b0dc`  
		Last Modified: Tue, 29 Mar 2022 19:09:15 GMT  
		Size: 213.2 MB (213182657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e598731bdf8c71ef7ba2ee42f6fc6b4a739285b74bf7d60a63db66774b1d65`  
		Last Modified: Tue, 29 Mar 2022 19:08:51 GMT  
		Size: 13.4 MB (13440807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843965b80de19e5d7d522b083ee79b394c9969e157265dfbc5fb3718943f877d`  
		Last Modified: Tue, 29 Mar 2022 19:08:48 GMT  
		Size: 457.2 KB (457156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b1e84beaf76256d7c1959545d1054429ee2460f82964ad33286a8cf5a98809`  
		Last Modified: Tue, 29 Mar 2022 19:09:21 GMT  
		Size: 275.3 MB (275305810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed8228da289351ace8010a6ab4e7b28a3e680b010743bce000d6e1d68e2f51d`  
		Last Modified: Tue, 29 Mar 2022 19:08:46 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abb36b18dfa33a3a1fc56f772a7486a7063d000646f6e1dd134b210dabd44cd`  
		Last Modified: Tue, 29 Mar 2022 19:08:46 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4408ec40e2859f6ba6158e402e619c4a683ea68c07b9dc44db7bee7fdb41db3f`  
		Last Modified: Tue, 29 Mar 2022 19:08:46 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790b8d488b0703d68c5ff9938a9eda7cf9832ca1cae8e727d1e5b89d66a7cddc`  
		Last Modified: Tue, 29 Mar 2022 19:08:46 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:8d159d83d33a5e7e1b799adcef52f26203744d2430c36d1002bd0f657203d204
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:647d9981604b8fc8c0773f3346908e7b8b0a43eb64941d2455effecef06780f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.5 MB (529540866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba95c862a87233f1a0dc9ec658f166847c59f18389ace89741d2a6f679a66d3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 19:02:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 29 Mar 2022 19:02:29 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 29 Mar 2022 19:02:29 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 19:03:32 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 29 Mar 2022 19:03:44 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 19:03:47 GMT
RUN npm install -g rtlcss
# Tue, 29 Mar 2022 19:03:47 GMT
ENV ODOO_VERSION=14.0
# Tue, 29 Mar 2022 19:03:47 GMT
ARG ODOO_RELEASE=20220325
# Tue, 29 Mar 2022 19:03:48 GMT
ARG ODOO_SHA=eabfcf757b772782f11db1ea484e9319be58c3c5
# Tue, 29 Mar 2022 19:04:59 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=eabfcf757b772782f11db1ea484e9319be58c3c5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 29 Mar 2022 19:05:03 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 29 Mar 2022 19:05:03 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 29 Mar 2022 19:05:04 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=eabfcf757b772782f11db1ea484e9319be58c3c5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 29 Mar 2022 19:05:04 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 29 Mar 2022 19:05:04 GMT
EXPOSE 8069 8071 8072
# Tue, 29 Mar 2022 19:05:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 29 Mar 2022 19:05:04 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 29 Mar 2022 19:05:05 GMT
USER odoo
# Tue, 29 Mar 2022 19:05:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 19:05:05 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d71810975b7f42c776c1f507c47736d2bd6904ab77b06df0c936554750b0dc`  
		Last Modified: Tue, 29 Mar 2022 19:09:15 GMT  
		Size: 213.2 MB (213182657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e598731bdf8c71ef7ba2ee42f6fc6b4a739285b74bf7d60a63db66774b1d65`  
		Last Modified: Tue, 29 Mar 2022 19:08:51 GMT  
		Size: 13.4 MB (13440807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843965b80de19e5d7d522b083ee79b394c9969e157265dfbc5fb3718943f877d`  
		Last Modified: Tue, 29 Mar 2022 19:08:48 GMT  
		Size: 457.2 KB (457156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b1e84beaf76256d7c1959545d1054429ee2460f82964ad33286a8cf5a98809`  
		Last Modified: Tue, 29 Mar 2022 19:09:21 GMT  
		Size: 275.3 MB (275305810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed8228da289351ace8010a6ab4e7b28a3e680b010743bce000d6e1d68e2f51d`  
		Last Modified: Tue, 29 Mar 2022 19:08:46 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abb36b18dfa33a3a1fc56f772a7486a7063d000646f6e1dd134b210dabd44cd`  
		Last Modified: Tue, 29 Mar 2022 19:08:46 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4408ec40e2859f6ba6158e402e619c4a683ea68c07b9dc44db7bee7fdb41db3f`  
		Last Modified: Tue, 29 Mar 2022 19:08:46 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790b8d488b0703d68c5ff9938a9eda7cf9832ca1cae8e727d1e5b89d66a7cddc`  
		Last Modified: Tue, 29 Mar 2022 19:08:46 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:8c2881cd6f13eb85e0086d237b8c39b1ac9c23a4b592d132714308cac651439b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:cae06b02083470ecc8814c739263b951faff8762cb8121d82454b44b3f5939bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.5 MB (551544020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03dbbe9108c28ef2cc4ff02c8f3eeaa5cd70613b0f7630e6bcd1055965095ce1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:59:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 29 Mar 2022 18:59:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 29 Mar 2022 18:59:21 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 19:00:20 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 29 Mar 2022 19:00:31 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 19:00:32 GMT
RUN npm install -g rtlcss
# Tue, 29 Mar 2022 19:00:32 GMT
ENV ODOO_VERSION=15.0
# Tue, 29 Mar 2022 19:00:33 GMT
ARG ODOO_RELEASE=20220325
# Tue, 29 Mar 2022 19:00:33 GMT
ARG ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
# Tue, 29 Mar 2022 19:02:19 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 29 Mar 2022 19:02:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 29 Mar 2022 19:02:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 29 Mar 2022 19:02:23 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 29 Mar 2022 19:02:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 29 Mar 2022 19:02:23 GMT
EXPOSE 8069 8071 8072
# Tue, 29 Mar 2022 19:02:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 29 Mar 2022 19:02:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 29 Mar 2022 19:02:24 GMT
USER odoo
# Tue, 29 Mar 2022 19:02:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 19:02:24 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c747a1fa386d9308d1e2f9baef9efced0ce497e52e37fa9688ddc2a83779205`  
		Last Modified: Tue, 29 Mar 2022 19:08:26 GMT  
		Size: 220.3 MB (220306192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26df123c00088a4376eaafc17e8c006c7c47cc1dfa794ff5663dd160dba57157`  
		Last Modified: Tue, 29 Mar 2022 19:07:59 GMT  
		Size: 2.5 MB (2510070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff3bdf6129a4fe206bdf15ab252ebd5569b0f3efff6f8c7e2be9a0e0479b1cc`  
		Last Modified: Tue, 29 Mar 2022 19:07:58 GMT  
		Size: 450.8 KB (450767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01aec3f70f62afe7b3b91a5ffed9b81566e20857fa753e1f8fca00c2d8a76d5b`  
		Last Modified: Tue, 29 Mar 2022 19:08:32 GMT  
		Size: 296.9 MB (296896072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50e8b4b5551815104a61e8c9c95c7725ed5f2183a3b2d64dda20557595e6399`  
		Last Modified: Tue, 29 Mar 2022 19:07:57 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bfc2abf2008b8b202a10511cf9d03ccc2e2343a207f8a37f9d42e29c5f28d8`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf54e7361a0a8e603c294cd65b5257820b5bfe537a9f3898aa8a11bb2887ef1c`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52e6f0a41f3ba62d5cb85b997e04aa6a02aa721736275a8bbe9d772ce125df7`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:8c2881cd6f13eb85e0086d237b8c39b1ac9c23a4b592d132714308cac651439b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:cae06b02083470ecc8814c739263b951faff8762cb8121d82454b44b3f5939bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.5 MB (551544020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03dbbe9108c28ef2cc4ff02c8f3eeaa5cd70613b0f7630e6bcd1055965095ce1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:59:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 29 Mar 2022 18:59:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 29 Mar 2022 18:59:21 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 19:00:20 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 29 Mar 2022 19:00:31 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 19:00:32 GMT
RUN npm install -g rtlcss
# Tue, 29 Mar 2022 19:00:32 GMT
ENV ODOO_VERSION=15.0
# Tue, 29 Mar 2022 19:00:33 GMT
ARG ODOO_RELEASE=20220325
# Tue, 29 Mar 2022 19:00:33 GMT
ARG ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
# Tue, 29 Mar 2022 19:02:19 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 29 Mar 2022 19:02:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 29 Mar 2022 19:02:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 29 Mar 2022 19:02:23 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 29 Mar 2022 19:02:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 29 Mar 2022 19:02:23 GMT
EXPOSE 8069 8071 8072
# Tue, 29 Mar 2022 19:02:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 29 Mar 2022 19:02:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 29 Mar 2022 19:02:24 GMT
USER odoo
# Tue, 29 Mar 2022 19:02:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 19:02:24 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c747a1fa386d9308d1e2f9baef9efced0ce497e52e37fa9688ddc2a83779205`  
		Last Modified: Tue, 29 Mar 2022 19:08:26 GMT  
		Size: 220.3 MB (220306192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26df123c00088a4376eaafc17e8c006c7c47cc1dfa794ff5663dd160dba57157`  
		Last Modified: Tue, 29 Mar 2022 19:07:59 GMT  
		Size: 2.5 MB (2510070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff3bdf6129a4fe206bdf15ab252ebd5569b0f3efff6f8c7e2be9a0e0479b1cc`  
		Last Modified: Tue, 29 Mar 2022 19:07:58 GMT  
		Size: 450.8 KB (450767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01aec3f70f62afe7b3b91a5ffed9b81566e20857fa753e1f8fca00c2d8a76d5b`  
		Last Modified: Tue, 29 Mar 2022 19:08:32 GMT  
		Size: 296.9 MB (296896072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50e8b4b5551815104a61e8c9c95c7725ed5f2183a3b2d64dda20557595e6399`  
		Last Modified: Tue, 29 Mar 2022 19:07:57 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bfc2abf2008b8b202a10511cf9d03ccc2e2343a207f8a37f9d42e29c5f28d8`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf54e7361a0a8e603c294cd65b5257820b5bfe537a9f3898aa8a11bb2887ef1c`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52e6f0a41f3ba62d5cb85b997e04aa6a02aa721736275a8bbe9d772ce125df7`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:8c2881cd6f13eb85e0086d237b8c39b1ac9c23a4b592d132714308cac651439b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:cae06b02083470ecc8814c739263b951faff8762cb8121d82454b44b3f5939bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.5 MB (551544020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03dbbe9108c28ef2cc4ff02c8f3eeaa5cd70613b0f7630e6bcd1055965095ce1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:59:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 29 Mar 2022 18:59:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 29 Mar 2022 18:59:21 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 19:00:20 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 29 Mar 2022 19:00:31 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 19:00:32 GMT
RUN npm install -g rtlcss
# Tue, 29 Mar 2022 19:00:32 GMT
ENV ODOO_VERSION=15.0
# Tue, 29 Mar 2022 19:00:33 GMT
ARG ODOO_RELEASE=20220325
# Tue, 29 Mar 2022 19:00:33 GMT
ARG ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
# Tue, 29 Mar 2022 19:02:19 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 29 Mar 2022 19:02:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 29 Mar 2022 19:02:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 29 Mar 2022 19:02:23 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 29 Mar 2022 19:02:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 29 Mar 2022 19:02:23 GMT
EXPOSE 8069 8071 8072
# Tue, 29 Mar 2022 19:02:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 29 Mar 2022 19:02:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 29 Mar 2022 19:02:24 GMT
USER odoo
# Tue, 29 Mar 2022 19:02:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 19:02:24 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c747a1fa386d9308d1e2f9baef9efced0ce497e52e37fa9688ddc2a83779205`  
		Last Modified: Tue, 29 Mar 2022 19:08:26 GMT  
		Size: 220.3 MB (220306192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26df123c00088a4376eaafc17e8c006c7c47cc1dfa794ff5663dd160dba57157`  
		Last Modified: Tue, 29 Mar 2022 19:07:59 GMT  
		Size: 2.5 MB (2510070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff3bdf6129a4fe206bdf15ab252ebd5569b0f3efff6f8c7e2be9a0e0479b1cc`  
		Last Modified: Tue, 29 Mar 2022 19:07:58 GMT  
		Size: 450.8 KB (450767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01aec3f70f62afe7b3b91a5ffed9b81566e20857fa753e1f8fca00c2d8a76d5b`  
		Last Modified: Tue, 29 Mar 2022 19:08:32 GMT  
		Size: 296.9 MB (296896072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50e8b4b5551815104a61e8c9c95c7725ed5f2183a3b2d64dda20557595e6399`  
		Last Modified: Tue, 29 Mar 2022 19:07:57 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bfc2abf2008b8b202a10511cf9d03ccc2e2343a207f8a37f9d42e29c5f28d8`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf54e7361a0a8e603c294cd65b5257820b5bfe537a9f3898aa8a11bb2887ef1c`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52e6f0a41f3ba62d5cb85b997e04aa6a02aa721736275a8bbe9d772ce125df7`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
