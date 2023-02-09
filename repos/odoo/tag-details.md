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
$ docker pull odoo@sha256:fe4f15e2bba69c227c872284515179671e8ae3bd5198cf872e0fd45305496282
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:2521a8e96553a995b3378c60c65ee165337fe81985d3ad78b84900c7f9f720ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.5 MB (531527305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f05dbae37f938f464c6b5e7189e61a000af05f913ca8657f3a2ddc4975575e5`
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
# Thu, 09 Feb 2023 10:42:23 GMT
ARG ODOO_RELEASE=20230109
# Thu, 09 Feb 2023 10:42:23 GMT
ARG ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
# Thu, 09 Feb 2023 10:43:38 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 09 Feb 2023 10:43:43 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 09 Feb 2023 10:43:43 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 09 Feb 2023 10:43:43 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 09 Feb 2023 10:43:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 09 Feb 2023 10:43:43 GMT
EXPOSE 8069 8071 8072
# Thu, 09 Feb 2023 10:43:44 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 09 Feb 2023 10:43:44 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 09 Feb 2023 10:43:44 GMT
USER odoo
# Thu, 09 Feb 2023 10:43:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 10:43:44 GMT
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
	-	`sha256:b8d2d5aec219580ed8a3bf6e2d891eace357256cbdb16fb0475530b1bf4fdbee`  
		Last Modified: Thu, 09 Feb 2023 10:46:18 GMT  
		Size: 277.2 MB (277224767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7236da96300ca2f0e1da6a36a531e796d5f10682818131d6e019069de4394bab`  
		Last Modified: Thu, 09 Feb 2023 10:45:45 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4210cca1277eaa6828c16a2cae9fb2f1a4680bc2927a2bd7874b2110d9cae14`  
		Last Modified: Thu, 09 Feb 2023 10:45:45 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481a4ee9a6f25e485faa6624a61eb0dcdfe2cbbe5c2f78ab05b13867f740b131`  
		Last Modified: Thu, 09 Feb 2023 10:45:45 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae4cb27023048fde60476174b689ad9a2b91e7a14100650af4191a9435b0d9c`  
		Last Modified: Thu, 09 Feb 2023 10:45:45 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:fe4f15e2bba69c227c872284515179671e8ae3bd5198cf872e0fd45305496282
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:2521a8e96553a995b3378c60c65ee165337fe81985d3ad78b84900c7f9f720ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.5 MB (531527305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f05dbae37f938f464c6b5e7189e61a000af05f913ca8657f3a2ddc4975575e5`
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
# Thu, 09 Feb 2023 10:42:23 GMT
ARG ODOO_RELEASE=20230109
# Thu, 09 Feb 2023 10:42:23 GMT
ARG ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
# Thu, 09 Feb 2023 10:43:38 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 09 Feb 2023 10:43:43 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 09 Feb 2023 10:43:43 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 09 Feb 2023 10:43:43 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 09 Feb 2023 10:43:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 09 Feb 2023 10:43:43 GMT
EXPOSE 8069 8071 8072
# Thu, 09 Feb 2023 10:43:44 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 09 Feb 2023 10:43:44 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 09 Feb 2023 10:43:44 GMT
USER odoo
# Thu, 09 Feb 2023 10:43:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 10:43:44 GMT
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
	-	`sha256:b8d2d5aec219580ed8a3bf6e2d891eace357256cbdb16fb0475530b1bf4fdbee`  
		Last Modified: Thu, 09 Feb 2023 10:46:18 GMT  
		Size: 277.2 MB (277224767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7236da96300ca2f0e1da6a36a531e796d5f10682818131d6e019069de4394bab`  
		Last Modified: Thu, 09 Feb 2023 10:45:45 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4210cca1277eaa6828c16a2cae9fb2f1a4680bc2927a2bd7874b2110d9cae14`  
		Last Modified: Thu, 09 Feb 2023 10:45:45 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481a4ee9a6f25e485faa6624a61eb0dcdfe2cbbe5c2f78ab05b13867f740b131`  
		Last Modified: Thu, 09 Feb 2023 10:45:45 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae4cb27023048fde60476174b689ad9a2b91e7a14100650af4191a9435b0d9c`  
		Last Modified: Thu, 09 Feb 2023 10:45:45 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:f6fd4411afbe1f6a62555b29d0f940d52a0ee5ab80bc0a6279b7ba9b82e862b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:1e916bf6e3402a62407dca2dad87b8ea0a1ec699be7c56dc554606222e614a42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **559.7 MB (559730755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41364dc0a6d9eb9193eae6d3c5ac75d813c4910ddf6e986afce14ed926332309`
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
# Thu, 09 Feb 2023 10:38:59 GMT
ARG ODOO_RELEASE=20230109
# Thu, 09 Feb 2023 10:38:59 GMT
ARG ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
# Thu, 09 Feb 2023 10:40:15 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 09 Feb 2023 10:40:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 09 Feb 2023 10:40:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 09 Feb 2023 10:40:20 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 09 Feb 2023 10:40:20 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 09 Feb 2023 10:40:21 GMT
EXPOSE 8069 8071 8072
# Thu, 09 Feb 2023 10:40:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 09 Feb 2023 10:40:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 09 Feb 2023 10:40:21 GMT
USER odoo
# Thu, 09 Feb 2023 10:40:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 10:40:21 GMT
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
	-	`sha256:583619e9986aef51d909adce03f8f9c55ece4be41d2a81476d299bc9ae36061e`  
		Last Modified: Thu, 09 Feb 2023 10:45:36 GMT  
		Size: 305.0 MB (304992351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b5e1ec9460aec5ec7800aded676c7687711e7f625c3e4915d64755ad02fdc0`  
		Last Modified: Thu, 09 Feb 2023 10:45:00 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f8c30f6376a3107fb39894da05de718d9f3b672b6eb9080b1126c12bd09f38`  
		Last Modified: Thu, 09 Feb 2023 10:44:59 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37169ce3aa175f3167216bc2291bf24ea1a33607fb8657b28dfabc51bddfeaf6`  
		Last Modified: Thu, 09 Feb 2023 10:44:59 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bac53fa97aa9c37d5e7b513d8235c7fbedaadd2b6053d7d3a4c69d94c55bb3`  
		Last Modified: Thu, 09 Feb 2023 10:44:59 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:f6fd4411afbe1f6a62555b29d0f940d52a0ee5ab80bc0a6279b7ba9b82e862b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:1e916bf6e3402a62407dca2dad87b8ea0a1ec699be7c56dc554606222e614a42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **559.7 MB (559730755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41364dc0a6d9eb9193eae6d3c5ac75d813c4910ddf6e986afce14ed926332309`
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
# Thu, 09 Feb 2023 10:38:59 GMT
ARG ODOO_RELEASE=20230109
# Thu, 09 Feb 2023 10:38:59 GMT
ARG ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
# Thu, 09 Feb 2023 10:40:15 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 09 Feb 2023 10:40:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 09 Feb 2023 10:40:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 09 Feb 2023 10:40:20 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 09 Feb 2023 10:40:20 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 09 Feb 2023 10:40:21 GMT
EXPOSE 8069 8071 8072
# Thu, 09 Feb 2023 10:40:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 09 Feb 2023 10:40:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 09 Feb 2023 10:40:21 GMT
USER odoo
# Thu, 09 Feb 2023 10:40:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 10:40:21 GMT
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
	-	`sha256:583619e9986aef51d909adce03f8f9c55ece4be41d2a81476d299bc9ae36061e`  
		Last Modified: Thu, 09 Feb 2023 10:45:36 GMT  
		Size: 305.0 MB (304992351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b5e1ec9460aec5ec7800aded676c7687711e7f625c3e4915d64755ad02fdc0`  
		Last Modified: Thu, 09 Feb 2023 10:45:00 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f8c30f6376a3107fb39894da05de718d9f3b672b6eb9080b1126c12bd09f38`  
		Last Modified: Thu, 09 Feb 2023 10:44:59 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37169ce3aa175f3167216bc2291bf24ea1a33607fb8657b28dfabc51bddfeaf6`  
		Last Modified: Thu, 09 Feb 2023 10:44:59 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bac53fa97aa9c37d5e7b513d8235c7fbedaadd2b6053d7d3a4c69d94c55bb3`  
		Last Modified: Thu, 09 Feb 2023 10:44:59 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:9d1bb6c4ebc5daada8de0ed8dea65312003db8f3441907fbe6ca8ee562cf4371
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:5b8119506fba61848557bfbbfa8bd8dc5e25a6df2e83750dcef199148e9b25f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566195651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b43d3875c61ab18c2a6716ef549140ab2a4b9ea3b36ae6093f1e53a058eacd`
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
# Thu, 09 Feb 2023 10:37:13 GMT
ARG ODOO_RELEASE=20230109
# Thu, 09 Feb 2023 10:37:14 GMT
ARG ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
# Thu, 09 Feb 2023 10:38:36 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 09 Feb 2023 10:38:41 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 09 Feb 2023 10:38:41 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 09 Feb 2023 10:38:42 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 09 Feb 2023 10:38:42 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 09 Feb 2023 10:38:42 GMT
EXPOSE 8069 8071 8072
# Thu, 09 Feb 2023 10:38:42 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 09 Feb 2023 10:38:42 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 09 Feb 2023 10:38:43 GMT
USER odoo
# Thu, 09 Feb 2023 10:38:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 10:38:43 GMT
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
	-	`sha256:3013f4ea4a3a548afd0fdb650252e9c1a23ee34abd8aa59200863dc4a588b0ea`  
		Last Modified: Thu, 09 Feb 2023 10:44:48 GMT  
		Size: 311.5 MB (311457245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841bdc15b53e6c1278a0bb88ba0564e4cf06ab1492349e7c5dccbdd2ed44333d`  
		Last Modified: Thu, 09 Feb 2023 10:44:10 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991294a9d78b1eb2f59372bf7d3cee2308eadf478b3c3120b448ed3a23310aa`  
		Last Modified: Thu, 09 Feb 2023 10:44:11 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832b4c5de816f150e6ace83d48a416356d672e26d9d098bd4f2c1b162379cce2`  
		Last Modified: Thu, 09 Feb 2023 10:44:10 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b78f7c7070d5844d2d1f71912fe9f527086711fefe1164b82ba1c5af476ae97`  
		Last Modified: Thu, 09 Feb 2023 10:44:10 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:9d1bb6c4ebc5daada8de0ed8dea65312003db8f3441907fbe6ca8ee562cf4371
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:5b8119506fba61848557bfbbfa8bd8dc5e25a6df2e83750dcef199148e9b25f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566195651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b43d3875c61ab18c2a6716ef549140ab2a4b9ea3b36ae6093f1e53a058eacd`
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
# Thu, 09 Feb 2023 10:37:13 GMT
ARG ODOO_RELEASE=20230109
# Thu, 09 Feb 2023 10:37:14 GMT
ARG ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
# Thu, 09 Feb 2023 10:38:36 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 09 Feb 2023 10:38:41 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 09 Feb 2023 10:38:41 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 09 Feb 2023 10:38:42 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 09 Feb 2023 10:38:42 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 09 Feb 2023 10:38:42 GMT
EXPOSE 8069 8071 8072
# Thu, 09 Feb 2023 10:38:42 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 09 Feb 2023 10:38:42 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 09 Feb 2023 10:38:43 GMT
USER odoo
# Thu, 09 Feb 2023 10:38:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 10:38:43 GMT
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
	-	`sha256:3013f4ea4a3a548afd0fdb650252e9c1a23ee34abd8aa59200863dc4a588b0ea`  
		Last Modified: Thu, 09 Feb 2023 10:44:48 GMT  
		Size: 311.5 MB (311457245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841bdc15b53e6c1278a0bb88ba0564e4cf06ab1492349e7c5dccbdd2ed44333d`  
		Last Modified: Thu, 09 Feb 2023 10:44:10 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991294a9d78b1eb2f59372bf7d3cee2308eadf478b3c3120b448ed3a23310aa`  
		Last Modified: Thu, 09 Feb 2023 10:44:11 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832b4c5de816f150e6ace83d48a416356d672e26d9d098bd4f2c1b162379cce2`  
		Last Modified: Thu, 09 Feb 2023 10:44:10 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b78f7c7070d5844d2d1f71912fe9f527086711fefe1164b82ba1c5af476ae97`  
		Last Modified: Thu, 09 Feb 2023 10:44:10 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:9d1bb6c4ebc5daada8de0ed8dea65312003db8f3441907fbe6ca8ee562cf4371
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:5b8119506fba61848557bfbbfa8bd8dc5e25a6df2e83750dcef199148e9b25f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566195651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b43d3875c61ab18c2a6716ef549140ab2a4b9ea3b36ae6093f1e53a058eacd`
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
# Thu, 09 Feb 2023 10:37:13 GMT
ARG ODOO_RELEASE=20230109
# Thu, 09 Feb 2023 10:37:14 GMT
ARG ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
# Thu, 09 Feb 2023 10:38:36 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 09 Feb 2023 10:38:41 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 09 Feb 2023 10:38:41 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 09 Feb 2023 10:38:42 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 09 Feb 2023 10:38:42 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 09 Feb 2023 10:38:42 GMT
EXPOSE 8069 8071 8072
# Thu, 09 Feb 2023 10:38:42 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 09 Feb 2023 10:38:42 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 09 Feb 2023 10:38:43 GMT
USER odoo
# Thu, 09 Feb 2023 10:38:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 10:38:43 GMT
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
	-	`sha256:3013f4ea4a3a548afd0fdb650252e9c1a23ee34abd8aa59200863dc4a588b0ea`  
		Last Modified: Thu, 09 Feb 2023 10:44:48 GMT  
		Size: 311.5 MB (311457245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841bdc15b53e6c1278a0bb88ba0564e4cf06ab1492349e7c5dccbdd2ed44333d`  
		Last Modified: Thu, 09 Feb 2023 10:44:10 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991294a9d78b1eb2f59372bf7d3cee2308eadf478b3c3120b448ed3a23310aa`  
		Last Modified: Thu, 09 Feb 2023 10:44:11 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832b4c5de816f150e6ace83d48a416356d672e26d9d098bd4f2c1b162379cce2`  
		Last Modified: Thu, 09 Feb 2023 10:44:10 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b78f7c7070d5844d2d1f71912fe9f527086711fefe1164b82ba1c5af476ae97`  
		Last Modified: Thu, 09 Feb 2023 10:44:10 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
