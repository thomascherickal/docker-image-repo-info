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
$ docker pull odoo@sha256:afc4ac38572d7b4636a8451ba7bd5e9ff96698389abb325b99cb8b41472ab6c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:a322497a7a3e2a2bc7f7a9e6c1c9de7b9b8e59297c68c1db01156a7ff855de12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.8 MB (531759718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0debd08157d3e2d9a905c5c2b411fa31202f4cf2bbe80fd367f16d3ac019e0b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:40:37 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 09 Feb 2023 10:40:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 09 Feb 2023 10:40:38 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:42:07 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 09 Feb 2023 10:42:20 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:42:22 GMT
RUN npm install -g rtlcss
# Thu, 09 Feb 2023 10:42:23 GMT
ENV ODOO_VERSION=14.0
# Fri, 24 Feb 2023 20:25:08 GMT
ARG ODOO_RELEASE=20230224
# Fri, 24 Feb 2023 20:25:08 GMT
ARG ODOO_SHA=a59688f0c2c830f243fec130e3c651d93f188658
# Fri, 24 Feb 2023 20:26:24 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=a59688f0c2c830f243fec130e3c651d93f188658
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 24 Feb 2023 20:26:28 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 24 Feb 2023 20:26:28 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 24 Feb 2023 20:26:28 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=a59688f0c2c830f243fec130e3c651d93f188658
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 24 Feb 2023 20:26:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 24 Feb 2023 20:26:29 GMT
EXPOSE 8069 8071 8072
# Fri, 24 Feb 2023 20:26:29 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 24 Feb 2023 20:26:29 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 24 Feb 2023 20:26:29 GMT
USER odoo
# Fri, 24 Feb 2023 20:26:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:26:29 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:29cd48154c03e9242f1ff4f9895cf886a344fb94c9b71029455e76e11214328f`  
		Last Modified: Thu, 09 Feb 2023 03:25:54 GMT  
		Size: 27.1 MB (27140531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8ec76ccf6adf454aad5923fbc6e5dc07a295b6a788d02bc2a64e3643bb2e04`  
		Last Modified: Thu, 09 Feb 2023 10:46:11 GMT  
		Size: 213.2 MB (213187817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9341ecf4e4d70be43da9a5f4f39e31638f27e9f9c2a51eb1630bf33fd85ee53`  
		Last Modified: Thu, 09 Feb 2023 10:45:49 GMT  
		Size: 13.5 MB (13515275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a76c77ce49e1b0d3c4bf7ad071ad2141f93ac0f42f24dd6bd59ae7c02d56f27`  
		Last Modified: Thu, 09 Feb 2023 10:45:47 GMT  
		Size: 456.5 KB (456451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06746a04ba0963a3764d53b2435a30839aa4b7545e8602346728424c0d8d04ba`  
		Last Modified: Fri, 24 Feb 2023 20:28:41 GMT  
		Size: 277.5 MB (277457179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b113f19acdbf6e5b59c90ecf87d21f861480b8b1874cb3450ffa37e87fb5edb0`  
		Last Modified: Fri, 24 Feb 2023 20:28:10 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7887a5b1b8c364286d64ad8c4d1a25605b8075c713a7ba1e37efc54230b2c3ee`  
		Last Modified: Fri, 24 Feb 2023 20:28:10 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215c5c0035593016961117a66f02485c756b7596f87057fa65e79508c1d31cf4`  
		Last Modified: Fri, 24 Feb 2023 20:28:10 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3689f6bfb1af9982e148bd9dcd528af2f1869d948c0b272b29e65ac254b93fb`  
		Last Modified: Fri, 24 Feb 2023 20:28:10 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:afc4ac38572d7b4636a8451ba7bd5e9ff96698389abb325b99cb8b41472ab6c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:a322497a7a3e2a2bc7f7a9e6c1c9de7b9b8e59297c68c1db01156a7ff855de12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.8 MB (531759718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0debd08157d3e2d9a905c5c2b411fa31202f4cf2bbe80fd367f16d3ac019e0b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:40:37 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 09 Feb 2023 10:40:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 09 Feb 2023 10:40:38 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:42:07 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 09 Feb 2023 10:42:20 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:42:22 GMT
RUN npm install -g rtlcss
# Thu, 09 Feb 2023 10:42:23 GMT
ENV ODOO_VERSION=14.0
# Fri, 24 Feb 2023 20:25:08 GMT
ARG ODOO_RELEASE=20230224
# Fri, 24 Feb 2023 20:25:08 GMT
ARG ODOO_SHA=a59688f0c2c830f243fec130e3c651d93f188658
# Fri, 24 Feb 2023 20:26:24 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=a59688f0c2c830f243fec130e3c651d93f188658
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 24 Feb 2023 20:26:28 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 24 Feb 2023 20:26:28 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 24 Feb 2023 20:26:28 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=a59688f0c2c830f243fec130e3c651d93f188658
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 24 Feb 2023 20:26:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 24 Feb 2023 20:26:29 GMT
EXPOSE 8069 8071 8072
# Fri, 24 Feb 2023 20:26:29 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 24 Feb 2023 20:26:29 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 24 Feb 2023 20:26:29 GMT
USER odoo
# Fri, 24 Feb 2023 20:26:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:26:29 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:29cd48154c03e9242f1ff4f9895cf886a344fb94c9b71029455e76e11214328f`  
		Last Modified: Thu, 09 Feb 2023 03:25:54 GMT  
		Size: 27.1 MB (27140531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8ec76ccf6adf454aad5923fbc6e5dc07a295b6a788d02bc2a64e3643bb2e04`  
		Last Modified: Thu, 09 Feb 2023 10:46:11 GMT  
		Size: 213.2 MB (213187817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9341ecf4e4d70be43da9a5f4f39e31638f27e9f9c2a51eb1630bf33fd85ee53`  
		Last Modified: Thu, 09 Feb 2023 10:45:49 GMT  
		Size: 13.5 MB (13515275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a76c77ce49e1b0d3c4bf7ad071ad2141f93ac0f42f24dd6bd59ae7c02d56f27`  
		Last Modified: Thu, 09 Feb 2023 10:45:47 GMT  
		Size: 456.5 KB (456451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06746a04ba0963a3764d53b2435a30839aa4b7545e8602346728424c0d8d04ba`  
		Last Modified: Fri, 24 Feb 2023 20:28:41 GMT  
		Size: 277.5 MB (277457179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b113f19acdbf6e5b59c90ecf87d21f861480b8b1874cb3450ffa37e87fb5edb0`  
		Last Modified: Fri, 24 Feb 2023 20:28:10 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7887a5b1b8c364286d64ad8c4d1a25605b8075c713a7ba1e37efc54230b2c3ee`  
		Last Modified: Fri, 24 Feb 2023 20:28:10 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215c5c0035593016961117a66f02485c756b7596f87057fa65e79508c1d31cf4`  
		Last Modified: Fri, 24 Feb 2023 20:28:10 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3689f6bfb1af9982e148bd9dcd528af2f1869d948c0b272b29e65ac254b93fb`  
		Last Modified: Fri, 24 Feb 2023 20:28:10 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:1bc24e02cf95b24fad2666fbc64085cf69a2338f5eaae88c968ae0595dd9d81d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:50eeb3a1b54c2ce9d6b17a5bfef91fe0c7b4fc9f322e7f3ecc735908d6203574
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **560.2 MB (560155644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a39fd912306e7ad43a7d10e528b7d174bd46c5596e546fe73df0e82a16ac92`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:35:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 09 Feb 2023 10:35:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 09 Feb 2023 10:35:51 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:37:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 09 Feb 2023 10:37:12 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:37:13 GMT
RUN npm install -g rtlcss
# Thu, 09 Feb 2023 10:38:59 GMT
ENV ODOO_VERSION=15.0
# Fri, 24 Feb 2023 20:23:45 GMT
ARG ODOO_RELEASE=20230224
# Fri, 24 Feb 2023 20:23:45 GMT
ARG ODOO_SHA=44613aceddf8e928ca50fc23979b1141fa4bb7d5
# Fri, 24 Feb 2023 20:24:56 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=44613aceddf8e928ca50fc23979b1141fa4bb7d5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 24 Feb 2023 20:25:00 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 24 Feb 2023 20:25:00 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 24 Feb 2023 20:25:00 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=44613aceddf8e928ca50fc23979b1141fa4bb7d5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 24 Feb 2023 20:25:00 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 24 Feb 2023 20:25:01 GMT
EXPOSE 8069 8071 8072
# Fri, 24 Feb 2023 20:25:01 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 24 Feb 2023 20:25:01 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 24 Feb 2023 20:25:01 GMT
USER odoo
# Fri, 24 Feb 2023 20:25:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:25:01 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58aec9a5b3f5a0ba902eebea63be1021865605f6fa6db9f2440463c989a404d`  
		Last Modified: Thu, 09 Feb 2023 10:44:38 GMT  
		Size: 220.3 MB (220298157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9868f669d922ebb3ec807e24ae5c5586ab504c7f5df9c80fe8148f904c8d878f`  
		Last Modified: Thu, 09 Feb 2023 10:44:12 GMT  
		Size: 2.6 MB (2573943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5eedbe9b213f08a555594fe4e121fda62ee068698f0a84a6b4855d7cd05674`  
		Last Modified: Thu, 09 Feb 2023 10:44:12 GMT  
		Size: 452.0 KB (452028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a9d67b98e3e1453a3ae3b2c633371d440a154fa07488d4f32100779fa2280e`  
		Last Modified: Fri, 24 Feb 2023 20:28:01 GMT  
		Size: 305.4 MB (305417241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3c23b4482a71b0a5029e49638d45a6f0f84bb098aab4688483fc57404ee30a`  
		Last Modified: Fri, 24 Feb 2023 20:27:27 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981980c64f71298cf8a9b52fcbf32714e5b93115f9f412a29f40233457f0a3a6`  
		Last Modified: Fri, 24 Feb 2023 20:27:27 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa758b55a0c38f41600f2e0aa8c9b7d850182dfdce381d486e3fb14c946eb71`  
		Last Modified: Fri, 24 Feb 2023 20:27:27 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f5e731b03bf5710cb96e2ee216eddb4df84aa0d30ee41b88c9a521a0cf04d1`  
		Last Modified: Fri, 24 Feb 2023 20:27:27 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:1bc24e02cf95b24fad2666fbc64085cf69a2338f5eaae88c968ae0595dd9d81d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:50eeb3a1b54c2ce9d6b17a5bfef91fe0c7b4fc9f322e7f3ecc735908d6203574
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **560.2 MB (560155644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a39fd912306e7ad43a7d10e528b7d174bd46c5596e546fe73df0e82a16ac92`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:35:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 09 Feb 2023 10:35:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 09 Feb 2023 10:35:51 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:37:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 09 Feb 2023 10:37:12 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:37:13 GMT
RUN npm install -g rtlcss
# Thu, 09 Feb 2023 10:38:59 GMT
ENV ODOO_VERSION=15.0
# Fri, 24 Feb 2023 20:23:45 GMT
ARG ODOO_RELEASE=20230224
# Fri, 24 Feb 2023 20:23:45 GMT
ARG ODOO_SHA=44613aceddf8e928ca50fc23979b1141fa4bb7d5
# Fri, 24 Feb 2023 20:24:56 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=44613aceddf8e928ca50fc23979b1141fa4bb7d5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 24 Feb 2023 20:25:00 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 24 Feb 2023 20:25:00 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 24 Feb 2023 20:25:00 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=44613aceddf8e928ca50fc23979b1141fa4bb7d5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 24 Feb 2023 20:25:00 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 24 Feb 2023 20:25:01 GMT
EXPOSE 8069 8071 8072
# Fri, 24 Feb 2023 20:25:01 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 24 Feb 2023 20:25:01 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 24 Feb 2023 20:25:01 GMT
USER odoo
# Fri, 24 Feb 2023 20:25:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:25:01 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58aec9a5b3f5a0ba902eebea63be1021865605f6fa6db9f2440463c989a404d`  
		Last Modified: Thu, 09 Feb 2023 10:44:38 GMT  
		Size: 220.3 MB (220298157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9868f669d922ebb3ec807e24ae5c5586ab504c7f5df9c80fe8148f904c8d878f`  
		Last Modified: Thu, 09 Feb 2023 10:44:12 GMT  
		Size: 2.6 MB (2573943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5eedbe9b213f08a555594fe4e121fda62ee068698f0a84a6b4855d7cd05674`  
		Last Modified: Thu, 09 Feb 2023 10:44:12 GMT  
		Size: 452.0 KB (452028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a9d67b98e3e1453a3ae3b2c633371d440a154fa07488d4f32100779fa2280e`  
		Last Modified: Fri, 24 Feb 2023 20:28:01 GMT  
		Size: 305.4 MB (305417241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3c23b4482a71b0a5029e49638d45a6f0f84bb098aab4688483fc57404ee30a`  
		Last Modified: Fri, 24 Feb 2023 20:27:27 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981980c64f71298cf8a9b52fcbf32714e5b93115f9f412a29f40233457f0a3a6`  
		Last Modified: Fri, 24 Feb 2023 20:27:27 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa758b55a0c38f41600f2e0aa8c9b7d850182dfdce381d486e3fb14c946eb71`  
		Last Modified: Fri, 24 Feb 2023 20:27:27 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f5e731b03bf5710cb96e2ee216eddb4df84aa0d30ee41b88c9a521a0cf04d1`  
		Last Modified: Fri, 24 Feb 2023 20:27:27 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:3f22c6e279d68f6f99e7c06127de42dcd49df9091a26905355d42571f1ba397e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:971c643000e012ad8aca71ab2d903f527bdcb13a23a2c5f1c4d9e5a6a4c3367a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **568.6 MB (568642376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d47774edee8f94db3d09c6281f8650fb8d96e8ed0fcbd60dad510bf793e80c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:35:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 09 Feb 2023 10:35:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 09 Feb 2023 10:35:51 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:37:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 09 Feb 2023 10:37:12 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:37:13 GMT
RUN npm install -g rtlcss
# Thu, 09 Feb 2023 10:37:13 GMT
ENV ODOO_VERSION=16.0
# Fri, 24 Feb 2023 20:22:06 GMT
ARG ODOO_RELEASE=20230224
# Fri, 24 Feb 2023 20:22:07 GMT
ARG ODOO_SHA=2a4ed4c36b82a05707b6e709182266672a32ace2
# Fri, 24 Feb 2023 20:23:28 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=2a4ed4c36b82a05707b6e709182266672a32ace2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 24 Feb 2023 20:23:33 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 24 Feb 2023 20:23:34 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 24 Feb 2023 20:23:34 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=2a4ed4c36b82a05707b6e709182266672a32ace2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 24 Feb 2023 20:23:34 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 24 Feb 2023 20:23:34 GMT
EXPOSE 8069 8071 8072
# Fri, 24 Feb 2023 20:23:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 24 Feb 2023 20:23:35 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 24 Feb 2023 20:23:35 GMT
USER odoo
# Fri, 24 Feb 2023 20:23:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:23:35 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58aec9a5b3f5a0ba902eebea63be1021865605f6fa6db9f2440463c989a404d`  
		Last Modified: Thu, 09 Feb 2023 10:44:38 GMT  
		Size: 220.3 MB (220298157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9868f669d922ebb3ec807e24ae5c5586ab504c7f5df9c80fe8148f904c8d878f`  
		Last Modified: Thu, 09 Feb 2023 10:44:12 GMT  
		Size: 2.6 MB (2573943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5eedbe9b213f08a555594fe4e121fda62ee068698f0a84a6b4855d7cd05674`  
		Last Modified: Thu, 09 Feb 2023 10:44:12 GMT  
		Size: 452.0 KB (452028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051a9f5a3ed3d0e5ad6a72f6882280d0e2371a30ea001e3aaf86d724aa85ae41`  
		Last Modified: Fri, 24 Feb 2023 20:27:16 GMT  
		Size: 313.9 MB (313903973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f156b63d2654c37cc880ca06a5c6603f8f2512c214e1940b123f0a5f98de477`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcf456742de08ab92d730c2fcede0f338cffcb9d0cb296b0bc6c32dc6ee3aeb`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f367e40db664c713ee7c434eeb8c14a47745f1dd935fb52c5867994c12923`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fa26a8c3ccf3af00e7a485cd18724370e05e556445b0722922f1195802fa55`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:3f22c6e279d68f6f99e7c06127de42dcd49df9091a26905355d42571f1ba397e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:971c643000e012ad8aca71ab2d903f527bdcb13a23a2c5f1c4d9e5a6a4c3367a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **568.6 MB (568642376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d47774edee8f94db3d09c6281f8650fb8d96e8ed0fcbd60dad510bf793e80c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:35:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 09 Feb 2023 10:35:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 09 Feb 2023 10:35:51 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:37:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 09 Feb 2023 10:37:12 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:37:13 GMT
RUN npm install -g rtlcss
# Thu, 09 Feb 2023 10:37:13 GMT
ENV ODOO_VERSION=16.0
# Fri, 24 Feb 2023 20:22:06 GMT
ARG ODOO_RELEASE=20230224
# Fri, 24 Feb 2023 20:22:07 GMT
ARG ODOO_SHA=2a4ed4c36b82a05707b6e709182266672a32ace2
# Fri, 24 Feb 2023 20:23:28 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=2a4ed4c36b82a05707b6e709182266672a32ace2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 24 Feb 2023 20:23:33 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 24 Feb 2023 20:23:34 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 24 Feb 2023 20:23:34 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=2a4ed4c36b82a05707b6e709182266672a32ace2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 24 Feb 2023 20:23:34 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 24 Feb 2023 20:23:34 GMT
EXPOSE 8069 8071 8072
# Fri, 24 Feb 2023 20:23:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 24 Feb 2023 20:23:35 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 24 Feb 2023 20:23:35 GMT
USER odoo
# Fri, 24 Feb 2023 20:23:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:23:35 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58aec9a5b3f5a0ba902eebea63be1021865605f6fa6db9f2440463c989a404d`  
		Last Modified: Thu, 09 Feb 2023 10:44:38 GMT  
		Size: 220.3 MB (220298157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9868f669d922ebb3ec807e24ae5c5586ab504c7f5df9c80fe8148f904c8d878f`  
		Last Modified: Thu, 09 Feb 2023 10:44:12 GMT  
		Size: 2.6 MB (2573943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5eedbe9b213f08a555594fe4e121fda62ee068698f0a84a6b4855d7cd05674`  
		Last Modified: Thu, 09 Feb 2023 10:44:12 GMT  
		Size: 452.0 KB (452028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051a9f5a3ed3d0e5ad6a72f6882280d0e2371a30ea001e3aaf86d724aa85ae41`  
		Last Modified: Fri, 24 Feb 2023 20:27:16 GMT  
		Size: 313.9 MB (313903973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f156b63d2654c37cc880ca06a5c6603f8f2512c214e1940b123f0a5f98de477`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcf456742de08ab92d730c2fcede0f338cffcb9d0cb296b0bc6c32dc6ee3aeb`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f367e40db664c713ee7c434eeb8c14a47745f1dd935fb52c5867994c12923`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fa26a8c3ccf3af00e7a485cd18724370e05e556445b0722922f1195802fa55`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:3f22c6e279d68f6f99e7c06127de42dcd49df9091a26905355d42571f1ba397e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:971c643000e012ad8aca71ab2d903f527bdcb13a23a2c5f1c4d9e5a6a4c3367a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **568.6 MB (568642376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4d47774edee8f94db3d09c6281f8650fb8d96e8ed0fcbd60dad510bf793e80c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:35:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 09 Feb 2023 10:35:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 09 Feb 2023 10:35:51 GMT
ENV LANG=C.UTF-8
# Thu, 09 Feb 2023 10:37:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 09 Feb 2023 10:37:12 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:37:13 GMT
RUN npm install -g rtlcss
# Thu, 09 Feb 2023 10:37:13 GMT
ENV ODOO_VERSION=16.0
# Fri, 24 Feb 2023 20:22:06 GMT
ARG ODOO_RELEASE=20230224
# Fri, 24 Feb 2023 20:22:07 GMT
ARG ODOO_SHA=2a4ed4c36b82a05707b6e709182266672a32ace2
# Fri, 24 Feb 2023 20:23:28 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=2a4ed4c36b82a05707b6e709182266672a32ace2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 24 Feb 2023 20:23:33 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 24 Feb 2023 20:23:34 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 24 Feb 2023 20:23:34 GMT
# ARGS: ODOO_RELEASE=20230224 ODOO_SHA=2a4ed4c36b82a05707b6e709182266672a32ace2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 24 Feb 2023 20:23:34 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 24 Feb 2023 20:23:34 GMT
EXPOSE 8069 8071 8072
# Fri, 24 Feb 2023 20:23:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 24 Feb 2023 20:23:35 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 24 Feb 2023 20:23:35 GMT
USER odoo
# Fri, 24 Feb 2023 20:23:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:23:35 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58aec9a5b3f5a0ba902eebea63be1021865605f6fa6db9f2440463c989a404d`  
		Last Modified: Thu, 09 Feb 2023 10:44:38 GMT  
		Size: 220.3 MB (220298157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9868f669d922ebb3ec807e24ae5c5586ab504c7f5df9c80fe8148f904c8d878f`  
		Last Modified: Thu, 09 Feb 2023 10:44:12 GMT  
		Size: 2.6 MB (2573943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5eedbe9b213f08a555594fe4e121fda62ee068698f0a84a6b4855d7cd05674`  
		Last Modified: Thu, 09 Feb 2023 10:44:12 GMT  
		Size: 452.0 KB (452028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051a9f5a3ed3d0e5ad6a72f6882280d0e2371a30ea001e3aaf86d724aa85ae41`  
		Last Modified: Fri, 24 Feb 2023 20:27:16 GMT  
		Size: 313.9 MB (313903973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f156b63d2654c37cc880ca06a5c6603f8f2512c214e1940b123f0a5f98de477`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcf456742de08ab92d730c2fcede0f338cffcb9d0cb296b0bc6c32dc6ee3aeb`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f367e40db664c713ee7c434eeb8c14a47745f1dd935fb52c5867994c12923`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fa26a8c3ccf3af00e7a485cd18724370e05e556445b0722922f1195802fa55`  
		Last Modified: Fri, 24 Feb 2023 20:26:42 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
