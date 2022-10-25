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
$ docker pull odoo@sha256:78b19636b37997b10d52603252b8d14b51742ac1066dc216a04f6aeb7f6183db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:97f1628eeb514e332642b53035121bde2eba850a6480e2565bce596362bbcd5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.1 MB (531077768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f8f7dd35345fb5fcb98b5cb84f33f03cfa2447d468fb048fb719695ca656d4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:22:13 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 25 Oct 2022 04:22:13 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 25 Oct 2022 04:22:13 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:23:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 25 Oct 2022 04:23:56 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:23:58 GMT
RUN npm install -g rtlcss
# Tue, 25 Oct 2022 04:23:58 GMT
ENV ODOO_VERSION=14.0
# Tue, 25 Oct 2022 04:23:59 GMT
ARG ODOO_RELEASE=20221012
# Tue, 25 Oct 2022 04:23:59 GMT
ARG ODOO_SHA=f938f53b8c9de5bb941bffbca1eb4d6bf44fa314
# Tue, 25 Oct 2022 04:25:18 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f938f53b8c9de5bb941bffbca1eb4d6bf44fa314
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 25 Oct 2022 04:25:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 25 Oct 2022 04:25:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 25 Oct 2022 04:25:23 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f938f53b8c9de5bb941bffbca1eb4d6bf44fa314
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 25 Oct 2022 04:25:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 25 Oct 2022 04:25:23 GMT
EXPOSE 8069 8071 8072
# Tue, 25 Oct 2022 04:25:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 25 Oct 2022 04:25:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 25 Oct 2022 04:25:24 GMT
USER odoo
# Tue, 25 Oct 2022 04:25:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 04:25:24 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faac7a4e46b306b96418e8946e9ba17e1fb320a1ae730c993241aafaf249b5d1`  
		Last Modified: Tue, 25 Oct 2022 04:27:49 GMT  
		Size: 213.2 MB (213185702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7011c07b6707d10ea804fe3b27f6772b3cea5b67c0ebb2933a79d1b4b7e123`  
		Last Modified: Tue, 25 Oct 2022 04:27:27 GMT  
		Size: 13.5 MB (13528969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254861bde8dbcd4ddf95d713137dde2c44d43eb2c907ea71665ee05060d6071`  
		Last Modified: Tue, 25 Oct 2022 04:27:24 GMT  
		Size: 453.8 KB (453804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c176e9c7d77dbfb3cd68d45e1490b65d5eadc20e8ea1a4e0fbc69b39d5e55c`  
		Last Modified: Tue, 25 Oct 2022 04:27:57 GMT  
		Size: 276.8 MB (276765996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dab81a9bbe1e9e7a88d757474d68a04c437ace3d76bec163861b842668bd43`  
		Last Modified: Tue, 25 Oct 2022 04:27:22 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecfac8163728506a21003797f38de54e5e609bce965c852a39578f017118759`  
		Last Modified: Tue, 25 Oct 2022 04:27:22 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcb4fc092fa1230d6c82b5b208839f176b243e30bf8967d75a5f4946c2749e5`  
		Last Modified: Tue, 25 Oct 2022 04:27:22 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f465b1b47947c8d6a5278cef4fa2a8f8985afff8a5822ffeedb5082f06ad84`  
		Last Modified: Tue, 25 Oct 2022 04:27:22 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:78b19636b37997b10d52603252b8d14b51742ac1066dc216a04f6aeb7f6183db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:97f1628eeb514e332642b53035121bde2eba850a6480e2565bce596362bbcd5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.1 MB (531077768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f8f7dd35345fb5fcb98b5cb84f33f03cfa2447d468fb048fb719695ca656d4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:22:13 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 25 Oct 2022 04:22:13 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 25 Oct 2022 04:22:13 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:23:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 25 Oct 2022 04:23:56 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:23:58 GMT
RUN npm install -g rtlcss
# Tue, 25 Oct 2022 04:23:58 GMT
ENV ODOO_VERSION=14.0
# Tue, 25 Oct 2022 04:23:59 GMT
ARG ODOO_RELEASE=20221012
# Tue, 25 Oct 2022 04:23:59 GMT
ARG ODOO_SHA=f938f53b8c9de5bb941bffbca1eb4d6bf44fa314
# Tue, 25 Oct 2022 04:25:18 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f938f53b8c9de5bb941bffbca1eb4d6bf44fa314
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 25 Oct 2022 04:25:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 25 Oct 2022 04:25:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 25 Oct 2022 04:25:23 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f938f53b8c9de5bb941bffbca1eb4d6bf44fa314
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 25 Oct 2022 04:25:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 25 Oct 2022 04:25:23 GMT
EXPOSE 8069 8071 8072
# Tue, 25 Oct 2022 04:25:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 25 Oct 2022 04:25:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 25 Oct 2022 04:25:24 GMT
USER odoo
# Tue, 25 Oct 2022 04:25:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 04:25:24 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faac7a4e46b306b96418e8946e9ba17e1fb320a1ae730c993241aafaf249b5d1`  
		Last Modified: Tue, 25 Oct 2022 04:27:49 GMT  
		Size: 213.2 MB (213185702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7011c07b6707d10ea804fe3b27f6772b3cea5b67c0ebb2933a79d1b4b7e123`  
		Last Modified: Tue, 25 Oct 2022 04:27:27 GMT  
		Size: 13.5 MB (13528969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254861bde8dbcd4ddf95d713137dde2c44d43eb2c907ea71665ee05060d6071`  
		Last Modified: Tue, 25 Oct 2022 04:27:24 GMT  
		Size: 453.8 KB (453804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c176e9c7d77dbfb3cd68d45e1490b65d5eadc20e8ea1a4e0fbc69b39d5e55c`  
		Last Modified: Tue, 25 Oct 2022 04:27:57 GMT  
		Size: 276.8 MB (276765996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dab81a9bbe1e9e7a88d757474d68a04c437ace3d76bec163861b842668bd43`  
		Last Modified: Tue, 25 Oct 2022 04:27:22 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecfac8163728506a21003797f38de54e5e609bce965c852a39578f017118759`  
		Last Modified: Tue, 25 Oct 2022 04:27:22 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcb4fc092fa1230d6c82b5b208839f176b243e30bf8967d75a5f4946c2749e5`  
		Last Modified: Tue, 25 Oct 2022 04:27:22 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f465b1b47947c8d6a5278cef4fa2a8f8985afff8a5822ffeedb5082f06ad84`  
		Last Modified: Tue, 25 Oct 2022 04:27:22 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:fba3fe4462f1facf18dbca150ddd38c31beae33e08bcdd65b17efecf75a424a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:b46fd82879e17ed06391d44e69fb2a13f10ced4c9451e42a2ae49fae82bb11c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **558.8 MB (558777226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3575bf5ebd38e05b7fb8f9365d0f1527b06f4006e3fdff7cf0d795e75f6e92fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:17:27 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 25 Oct 2022 04:17:27 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 25 Oct 2022 04:17:27 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:18:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 25 Oct 2022 04:18:52 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:18:54 GMT
RUN npm install -g rtlcss
# Tue, 25 Oct 2022 04:20:35 GMT
ENV ODOO_VERSION=15.0
# Tue, 25 Oct 2022 04:20:35 GMT
ARG ODOO_RELEASE=20221012
# Tue, 25 Oct 2022 04:20:35 GMT
ARG ODOO_SHA=55bf57fd9544ba5ea4033507eaf424cbbf1e95dc
# Tue, 25 Oct 2022 04:21:51 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=55bf57fd9544ba5ea4033507eaf424cbbf1e95dc
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 25 Oct 2022 04:21:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 25 Oct 2022 04:21:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 25 Oct 2022 04:21:56 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=55bf57fd9544ba5ea4033507eaf424cbbf1e95dc
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 25 Oct 2022 04:21:56 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 25 Oct 2022 04:21:57 GMT
EXPOSE 8069 8071 8072
# Tue, 25 Oct 2022 04:21:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 25 Oct 2022 04:21:57 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 25 Oct 2022 04:21:57 GMT
USER odoo
# Tue, 25 Oct 2022 04:21:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 04:21:57 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f207492967abb893017aed63de26947bc26869c41cb3ae43d047964a3f68abbe`  
		Last Modified: Tue, 25 Oct 2022 04:26:18 GMT  
		Size: 220.3 MB (220299448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034ca3be8a4120921abf777d526b8d64a15bfde37777c39a62f8c4934362a209`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 2.6 MB (2582213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260a86372800d03191e4df8077b594ccd6ea0f53bbc9f7f306cd191796d9f641`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 449.8 KB (449767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e694353540c4c2610407e2b024bbe77397f7af36f46e500965a2901d3139a514`  
		Last Modified: Tue, 25 Oct 2022 04:27:12 GMT  
		Size: 304.0 MB (304023301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddcd1da658249f6138a5bbd30b9eb3ccf85d8c6db4418eceb320631a526d07fa`  
		Last Modified: Tue, 25 Oct 2022 04:26:37 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9b144ab49709b3d1f861a7cc65b2b9031147bd7ccdf2508ce2e222f9ee86a6`  
		Last Modified: Tue, 25 Oct 2022 04:26:37 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c687076bc1cbb219e0c89bce6ae018337bcc103d5a5af1797275167318fc13a`  
		Last Modified: Tue, 25 Oct 2022 04:26:37 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dcd705f514196d8aed31cb849f1e95d1e5282c2bafd3ed79aba7eeb05e32d6`  
		Last Modified: Tue, 25 Oct 2022 04:26:37 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:fba3fe4462f1facf18dbca150ddd38c31beae33e08bcdd65b17efecf75a424a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:b46fd82879e17ed06391d44e69fb2a13f10ced4c9451e42a2ae49fae82bb11c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **558.8 MB (558777226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3575bf5ebd38e05b7fb8f9365d0f1527b06f4006e3fdff7cf0d795e75f6e92fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:17:27 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 25 Oct 2022 04:17:27 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 25 Oct 2022 04:17:27 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:18:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 25 Oct 2022 04:18:52 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:18:54 GMT
RUN npm install -g rtlcss
# Tue, 25 Oct 2022 04:20:35 GMT
ENV ODOO_VERSION=15.0
# Tue, 25 Oct 2022 04:20:35 GMT
ARG ODOO_RELEASE=20221012
# Tue, 25 Oct 2022 04:20:35 GMT
ARG ODOO_SHA=55bf57fd9544ba5ea4033507eaf424cbbf1e95dc
# Tue, 25 Oct 2022 04:21:51 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=55bf57fd9544ba5ea4033507eaf424cbbf1e95dc
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 25 Oct 2022 04:21:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 25 Oct 2022 04:21:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 25 Oct 2022 04:21:56 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=55bf57fd9544ba5ea4033507eaf424cbbf1e95dc
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 25 Oct 2022 04:21:56 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 25 Oct 2022 04:21:57 GMT
EXPOSE 8069 8071 8072
# Tue, 25 Oct 2022 04:21:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 25 Oct 2022 04:21:57 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 25 Oct 2022 04:21:57 GMT
USER odoo
# Tue, 25 Oct 2022 04:21:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 04:21:57 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f207492967abb893017aed63de26947bc26869c41cb3ae43d047964a3f68abbe`  
		Last Modified: Tue, 25 Oct 2022 04:26:18 GMT  
		Size: 220.3 MB (220299448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034ca3be8a4120921abf777d526b8d64a15bfde37777c39a62f8c4934362a209`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 2.6 MB (2582213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260a86372800d03191e4df8077b594ccd6ea0f53bbc9f7f306cd191796d9f641`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 449.8 KB (449767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e694353540c4c2610407e2b024bbe77397f7af36f46e500965a2901d3139a514`  
		Last Modified: Tue, 25 Oct 2022 04:27:12 GMT  
		Size: 304.0 MB (304023301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddcd1da658249f6138a5bbd30b9eb3ccf85d8c6db4418eceb320631a526d07fa`  
		Last Modified: Tue, 25 Oct 2022 04:26:37 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9b144ab49709b3d1f861a7cc65b2b9031147bd7ccdf2508ce2e222f9ee86a6`  
		Last Modified: Tue, 25 Oct 2022 04:26:37 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c687076bc1cbb219e0c89bce6ae018337bcc103d5a5af1797275167318fc13a`  
		Last Modified: Tue, 25 Oct 2022 04:26:37 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dcd705f514196d8aed31cb849f1e95d1e5282c2bafd3ed79aba7eeb05e32d6`  
		Last Modified: Tue, 25 Oct 2022 04:26:37 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:debb8b4ec6741a3a0e986b819557de0b9e8f9c4de16908b317e34838bf43dee2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:4110198fd60c6cd326c532ce27ad431b063476933da7610139264d76c6177ab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.0 MB (548958774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d82a3f7d3864c1046e5967342796f9e92ae7171e363f6baf239765ebb1ae9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:17:27 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 25 Oct 2022 04:17:27 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 25 Oct 2022 04:17:27 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:18:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 25 Oct 2022 04:18:52 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:18:54 GMT
RUN npm install -g rtlcss
# Tue, 25 Oct 2022 04:18:54 GMT
ENV ODOO_VERSION=16.0
# Tue, 25 Oct 2022 04:18:54 GMT
ARG ODOO_RELEASE=20221012
# Tue, 25 Oct 2022 04:18:54 GMT
ARG ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
# Tue, 25 Oct 2022 04:20:19 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 25 Oct 2022 04:20:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 25 Oct 2022 04:20:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 25 Oct 2022 04:20:23 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 25 Oct 2022 04:20:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 25 Oct 2022 04:20:24 GMT
EXPOSE 8069 8071 8072
# Tue, 25 Oct 2022 04:20:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 25 Oct 2022 04:20:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 25 Oct 2022 04:20:24 GMT
USER odoo
# Tue, 25 Oct 2022 04:20:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 04:20:24 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f207492967abb893017aed63de26947bc26869c41cb3ae43d047964a3f68abbe`  
		Last Modified: Tue, 25 Oct 2022 04:26:18 GMT  
		Size: 220.3 MB (220299448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034ca3be8a4120921abf777d526b8d64a15bfde37777c39a62f8c4934362a209`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 2.6 MB (2582213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260a86372800d03191e4df8077b594ccd6ea0f53bbc9f7f306cd191796d9f641`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 449.8 KB (449767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caa33c4d9d34d3a1e72d460dd6b8bd8be65cc719f5a02804d1af4e98574057c`  
		Last Modified: Tue, 25 Oct 2022 04:26:24 GMT  
		Size: 294.2 MB (294204843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6358514a760e4cc3729bac9a4cc44e967c069888c1a866cd427aed6503874a6e`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6e9d3885e34085b18fefbb2a05774dcdfa809089a9284d3761b480fc6814a`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475015701f8f26b0872f8e93222391d601d1419113047f71266cfc6c525f48ca`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f872f3bdb2d2e38d871218c914ca1b81c885636aa66f098e5531929878facb`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:debb8b4ec6741a3a0e986b819557de0b9e8f9c4de16908b317e34838bf43dee2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:4110198fd60c6cd326c532ce27ad431b063476933da7610139264d76c6177ab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.0 MB (548958774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d82a3f7d3864c1046e5967342796f9e92ae7171e363f6baf239765ebb1ae9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:17:27 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 25 Oct 2022 04:17:27 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 25 Oct 2022 04:17:27 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:18:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 25 Oct 2022 04:18:52 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:18:54 GMT
RUN npm install -g rtlcss
# Tue, 25 Oct 2022 04:18:54 GMT
ENV ODOO_VERSION=16.0
# Tue, 25 Oct 2022 04:18:54 GMT
ARG ODOO_RELEASE=20221012
# Tue, 25 Oct 2022 04:18:54 GMT
ARG ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
# Tue, 25 Oct 2022 04:20:19 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 25 Oct 2022 04:20:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 25 Oct 2022 04:20:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 25 Oct 2022 04:20:23 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 25 Oct 2022 04:20:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 25 Oct 2022 04:20:24 GMT
EXPOSE 8069 8071 8072
# Tue, 25 Oct 2022 04:20:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 25 Oct 2022 04:20:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 25 Oct 2022 04:20:24 GMT
USER odoo
# Tue, 25 Oct 2022 04:20:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 04:20:24 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f207492967abb893017aed63de26947bc26869c41cb3ae43d047964a3f68abbe`  
		Last Modified: Tue, 25 Oct 2022 04:26:18 GMT  
		Size: 220.3 MB (220299448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034ca3be8a4120921abf777d526b8d64a15bfde37777c39a62f8c4934362a209`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 2.6 MB (2582213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260a86372800d03191e4df8077b594ccd6ea0f53bbc9f7f306cd191796d9f641`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 449.8 KB (449767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caa33c4d9d34d3a1e72d460dd6b8bd8be65cc719f5a02804d1af4e98574057c`  
		Last Modified: Tue, 25 Oct 2022 04:26:24 GMT  
		Size: 294.2 MB (294204843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6358514a760e4cc3729bac9a4cc44e967c069888c1a866cd427aed6503874a6e`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6e9d3885e34085b18fefbb2a05774dcdfa809089a9284d3761b480fc6814a`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475015701f8f26b0872f8e93222391d601d1419113047f71266cfc6c525f48ca`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f872f3bdb2d2e38d871218c914ca1b81c885636aa66f098e5531929878facb`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:debb8b4ec6741a3a0e986b819557de0b9e8f9c4de16908b317e34838bf43dee2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:4110198fd60c6cd326c532ce27ad431b063476933da7610139264d76c6177ab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.0 MB (548958774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d82a3f7d3864c1046e5967342796f9e92ae7171e363f6baf239765ebb1ae9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:17:27 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 25 Oct 2022 04:17:27 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 25 Oct 2022 04:17:27 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:18:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 25 Oct 2022 04:18:52 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:18:54 GMT
RUN npm install -g rtlcss
# Tue, 25 Oct 2022 04:18:54 GMT
ENV ODOO_VERSION=16.0
# Tue, 25 Oct 2022 04:18:54 GMT
ARG ODOO_RELEASE=20221012
# Tue, 25 Oct 2022 04:18:54 GMT
ARG ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
# Tue, 25 Oct 2022 04:20:19 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 25 Oct 2022 04:20:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 25 Oct 2022 04:20:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 25 Oct 2022 04:20:23 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 25 Oct 2022 04:20:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 25 Oct 2022 04:20:24 GMT
EXPOSE 8069 8071 8072
# Tue, 25 Oct 2022 04:20:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 25 Oct 2022 04:20:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 25 Oct 2022 04:20:24 GMT
USER odoo
# Tue, 25 Oct 2022 04:20:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 04:20:24 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f207492967abb893017aed63de26947bc26869c41cb3ae43d047964a3f68abbe`  
		Last Modified: Tue, 25 Oct 2022 04:26:18 GMT  
		Size: 220.3 MB (220299448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034ca3be8a4120921abf777d526b8d64a15bfde37777c39a62f8c4934362a209`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 2.6 MB (2582213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260a86372800d03191e4df8077b594ccd6ea0f53bbc9f7f306cd191796d9f641`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 449.8 KB (449767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caa33c4d9d34d3a1e72d460dd6b8bd8be65cc719f5a02804d1af4e98574057c`  
		Last Modified: Tue, 25 Oct 2022 04:26:24 GMT  
		Size: 294.2 MB (294204843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6358514a760e4cc3729bac9a4cc44e967c069888c1a866cd427aed6503874a6e`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6e9d3885e34085b18fefbb2a05774dcdfa809089a9284d3761b480fc6814a`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475015701f8f26b0872f8e93222391d601d1419113047f71266cfc6c525f48ca`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f872f3bdb2d2e38d871218c914ca1b81c885636aa66f098e5531929878facb`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
