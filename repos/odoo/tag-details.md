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
$ docker pull odoo@sha256:896819f8c49cc1df3d03efd0ce63827c5e1a395a9301c0a1845327070ac152e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:f9c46a1b8ab52a0896a2303aedbc1cf05e394781644420bb618b597395a9df9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533313268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eace01d4a567fe9dabf8c8990a269aac9a169787414241d094169dd0c5322fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:35 GMT
ADD file:04482e1456288a566d216ed1cea383eabd946f66656da78e1e151056edf936d1 in / 
# Wed, 11 Oct 2023 18:35:35 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:25:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 12 Oct 2023 00:25:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 12 Oct 2023 00:25:30 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 00:27:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 12 Oct 2023 00:27:15 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:27:18 GMT
RUN npm install -g rtlcss
# Thu, 12 Oct 2023 00:27:18 GMT
ENV ODOO_VERSION=14.0
# Thu, 12 Oct 2023 00:27:18 GMT
ARG ODOO_RELEASE=20230925
# Thu, 12 Oct 2023 00:27:18 GMT
ARG ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
# Thu, 12 Oct 2023 00:28:32 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Oct 2023 00:28:34 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 12 Oct 2023 00:28:34 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Oct 2023 00:28:35 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Oct 2023 00:28:35 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Oct 2023 00:28:35 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Oct 2023 00:28:35 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Oct 2023 00:28:35 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Oct 2023 00:28:35 GMT
USER odoo
# Thu, 12 Oct 2023 00:28:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 00:28:35 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b70638ed4228556f5f57f76a636b1668fe301e86662437141774e61963da1b4f`  
		Last Modified: Wed, 11 Oct 2023 18:41:01 GMT  
		Size: 27.2 MB (27187490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb284015af4ddb6cbb27184a7a73ab1a8b8d8997be2c0239caa534a868b0ead3`  
		Last Modified: Thu, 12 Oct 2023 00:30:47 GMT  
		Size: 213.2 MB (213188800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b62e7888c226bc7f97419e538838b0471841298058d05c8a4b80bcb1a2d70`  
		Last Modified: Thu, 12 Oct 2023 00:30:26 GMT  
		Size: 13.6 MB (13567548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2667852297377b81ef81fc2e1c7b4fbd28be1dde5ddbc6b87c076b13d959f36`  
		Last Modified: Thu, 12 Oct 2023 00:30:24 GMT  
		Size: 461.5 KB (461516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b2d75b3ca298b7ff07d03ed1c694c37dd8c2bd3c3ae88a8b28c822c60430dc`  
		Last Modified: Thu, 12 Oct 2023 00:30:54 GMT  
		Size: 278.9 MB (278905449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb45187e5c55668318fb27d30aee4705e16223cc5c0d0e888c93aa8de1609c17`  
		Last Modified: Thu, 12 Oct 2023 00:30:22 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e33f7629c3a21374659d86d389feadf617274dc53bb8dff2db0f14c56b3a79`  
		Last Modified: Thu, 12 Oct 2023 00:30:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1928e7e90b7077ee0a7cf89a0a6851e46beadd632b95d386b84b775bfd2e9e8f`  
		Last Modified: Thu, 12 Oct 2023 00:30:21 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1450dbe232194b47e94376301cb93964a3df513a0c831227a9cdcfd91f02befd`  
		Last Modified: Thu, 12 Oct 2023 00:30:21 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:896819f8c49cc1df3d03efd0ce63827c5e1a395a9301c0a1845327070ac152e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:f9c46a1b8ab52a0896a2303aedbc1cf05e394781644420bb618b597395a9df9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **533.3 MB (533313268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eace01d4a567fe9dabf8c8990a269aac9a169787414241d094169dd0c5322fe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:35 GMT
ADD file:04482e1456288a566d216ed1cea383eabd946f66656da78e1e151056edf936d1 in / 
# Wed, 11 Oct 2023 18:35:35 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:25:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 12 Oct 2023 00:25:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 12 Oct 2023 00:25:30 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 00:27:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 12 Oct 2023 00:27:15 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:27:18 GMT
RUN npm install -g rtlcss
# Thu, 12 Oct 2023 00:27:18 GMT
ENV ODOO_VERSION=14.0
# Thu, 12 Oct 2023 00:27:18 GMT
ARG ODOO_RELEASE=20230925
# Thu, 12 Oct 2023 00:27:18 GMT
ARG ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
# Thu, 12 Oct 2023 00:28:32 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Oct 2023 00:28:34 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 12 Oct 2023 00:28:34 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Oct 2023 00:28:35 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=b7622d939c7135e693d498aec22a21638616bfee
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Oct 2023 00:28:35 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Oct 2023 00:28:35 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Oct 2023 00:28:35 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Oct 2023 00:28:35 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Oct 2023 00:28:35 GMT
USER odoo
# Thu, 12 Oct 2023 00:28:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 00:28:35 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b70638ed4228556f5f57f76a636b1668fe301e86662437141774e61963da1b4f`  
		Last Modified: Wed, 11 Oct 2023 18:41:01 GMT  
		Size: 27.2 MB (27187490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb284015af4ddb6cbb27184a7a73ab1a8b8d8997be2c0239caa534a868b0ead3`  
		Last Modified: Thu, 12 Oct 2023 00:30:47 GMT  
		Size: 213.2 MB (213188800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b62e7888c226bc7f97419e538838b0471841298058d05c8a4b80bcb1a2d70`  
		Last Modified: Thu, 12 Oct 2023 00:30:26 GMT  
		Size: 13.6 MB (13567548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2667852297377b81ef81fc2e1c7b4fbd28be1dde5ddbc6b87c076b13d959f36`  
		Last Modified: Thu, 12 Oct 2023 00:30:24 GMT  
		Size: 461.5 KB (461516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b2d75b3ca298b7ff07d03ed1c694c37dd8c2bd3c3ae88a8b28c822c60430dc`  
		Last Modified: Thu, 12 Oct 2023 00:30:54 GMT  
		Size: 278.9 MB (278905449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb45187e5c55668318fb27d30aee4705e16223cc5c0d0e888c93aa8de1609c17`  
		Last Modified: Thu, 12 Oct 2023 00:30:22 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e33f7629c3a21374659d86d389feadf617274dc53bb8dff2db0f14c56b3a79`  
		Last Modified: Thu, 12 Oct 2023 00:30:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1928e7e90b7077ee0a7cf89a0a6851e46beadd632b95d386b84b775bfd2e9e8f`  
		Last Modified: Thu, 12 Oct 2023 00:30:21 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1450dbe232194b47e94376301cb93964a3df513a0c831227a9cdcfd91f02befd`  
		Last Modified: Thu, 12 Oct 2023 00:30:21 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:4517adf1539f8cbdeca3ed0a42b76e365528c412206b19530a6fe00541399d42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:0478a0f3ee305515067afbc234b00e8602f2e990ff36ab07855da4d7bfd9955c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.5 MB (562481475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64b664a48f442ba79656320ad7325bcc1acebec9123ab5eb6e9f56f9355dcc24`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:19:57 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 12 Oct 2023 00:19:57 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 12 Oct 2023 00:19:57 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 00:23:57 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 12 Oct 2023 00:24:04 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:24:05 GMT
RUN npm install -g rtlcss
# Thu, 12 Oct 2023 00:24:05 GMT
ENV ODOO_VERSION=15.0
# Thu, 12 Oct 2023 00:24:05 GMT
ARG ODOO_RELEASE=20230925
# Thu, 12 Oct 2023 00:24:05 GMT
ARG ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
# Thu, 12 Oct 2023 00:25:17 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Oct 2023 00:25:21 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 12 Oct 2023 00:25:21 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Oct 2023 00:25:21 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Oct 2023 00:25:22 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Oct 2023 00:25:22 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Oct 2023 00:25:22 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Oct 2023 00:25:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Oct 2023 00:25:22 GMT
USER odoo
# Thu, 12 Oct 2023 00:25:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 00:25:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284e9c0342cd55845407b5a692d66b21c0ddf6b5417a3b86f88e1a7e0c716784`  
		Last Modified: Thu, 12 Oct 2023 00:30:04 GMT  
		Size: 220.3 MB (220297549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a95d741728c5091c421e238edb845f3ccc737f180c0aa0a00a06035f74dffd`  
		Last Modified: Thu, 12 Oct 2023 00:29:39 GMT  
		Size: 2.6 MB (2624799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c58c1a43fe65513d327e8a2552e62287456178ff05ee53f215093fe0af87b8`  
		Last Modified: Thu, 12 Oct 2023 00:29:39 GMT  
		Size: 457.2 KB (457244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61751bd77bc3dbde33c42058ee60254b1fad43241a6197e95ed62c689a7d08a`  
		Last Modified: Thu, 12 Oct 2023 00:30:12 GMT  
		Size: 307.7 MB (307681559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2501db6efdaf01b9640d67067d4af3e3145f75140239157ce9f0780b978cfcf4`  
		Last Modified: Thu, 12 Oct 2023 00:29:37 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceea80e97de4dedf133beeb8e2a23ffe1a4cd9699019f61d094e3937a655f187`  
		Last Modified: Thu, 12 Oct 2023 00:29:37 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cebfd656496743da0f7c59cdb44e08b2379964f47133d95d8d9882c5050d5a`  
		Last Modified: Thu, 12 Oct 2023 00:29:37 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1759103d3aca833681692c6124e0ae234d3e2bdbc57eeeecc2935ffb44ceaaf`  
		Last Modified: Thu, 12 Oct 2023 00:29:37 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:4517adf1539f8cbdeca3ed0a42b76e365528c412206b19530a6fe00541399d42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:0478a0f3ee305515067afbc234b00e8602f2e990ff36ab07855da4d7bfd9955c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.5 MB (562481475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64b664a48f442ba79656320ad7325bcc1acebec9123ab5eb6e9f56f9355dcc24`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:19:57 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 12 Oct 2023 00:19:57 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 12 Oct 2023 00:19:57 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 00:23:57 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 12 Oct 2023 00:24:04 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:24:05 GMT
RUN npm install -g rtlcss
# Thu, 12 Oct 2023 00:24:05 GMT
ENV ODOO_VERSION=15.0
# Thu, 12 Oct 2023 00:24:05 GMT
ARG ODOO_RELEASE=20230925
# Thu, 12 Oct 2023 00:24:05 GMT
ARG ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
# Thu, 12 Oct 2023 00:25:17 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Oct 2023 00:25:21 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 12 Oct 2023 00:25:21 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Oct 2023 00:25:21 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=e10abf8d0b57917d198d8185aa893fd44ce65c9c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Oct 2023 00:25:22 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Oct 2023 00:25:22 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Oct 2023 00:25:22 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Oct 2023 00:25:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Oct 2023 00:25:22 GMT
USER odoo
# Thu, 12 Oct 2023 00:25:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 00:25:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284e9c0342cd55845407b5a692d66b21c0ddf6b5417a3b86f88e1a7e0c716784`  
		Last Modified: Thu, 12 Oct 2023 00:30:04 GMT  
		Size: 220.3 MB (220297549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a95d741728c5091c421e238edb845f3ccc737f180c0aa0a00a06035f74dffd`  
		Last Modified: Thu, 12 Oct 2023 00:29:39 GMT  
		Size: 2.6 MB (2624799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c58c1a43fe65513d327e8a2552e62287456178ff05ee53f215093fe0af87b8`  
		Last Modified: Thu, 12 Oct 2023 00:29:39 GMT  
		Size: 457.2 KB (457244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61751bd77bc3dbde33c42058ee60254b1fad43241a6197e95ed62c689a7d08a`  
		Last Modified: Thu, 12 Oct 2023 00:30:12 GMT  
		Size: 307.7 MB (307681559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2501db6efdaf01b9640d67067d4af3e3145f75140239157ce9f0780b978cfcf4`  
		Last Modified: Thu, 12 Oct 2023 00:29:37 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceea80e97de4dedf133beeb8e2a23ffe1a4cd9699019f61d094e3937a655f187`  
		Last Modified: Thu, 12 Oct 2023 00:29:37 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cebfd656496743da0f7c59cdb44e08b2379964f47133d95d8d9882c5050d5a`  
		Last Modified: Thu, 12 Oct 2023 00:29:37 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1759103d3aca833681692c6124e0ae234d3e2bdbc57eeeecc2935ffb44ceaaf`  
		Last Modified: Thu, 12 Oct 2023 00:29:37 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:01697e5fbab426474004fa6b8c49f0af7554b1fafe2d5c10d68f52461fccf490
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:d84d0d713e8fc33126f97f0706df092f67f8d5e32bc7fb88083003cc40bf64f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.8 MB (576806934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f6ec0d61e8b356ed4c1422c3263ce2743dbc67a9973af9dd417ad90a8be6c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:19:57 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 12 Oct 2023 00:19:57 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 12 Oct 2023 00:19:57 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 00:21:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 12 Oct 2023 00:21:15 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:21:16 GMT
RUN npm install -g rtlcss
# Thu, 12 Oct 2023 00:21:16 GMT
ENV ODOO_VERSION=16.0
# Thu, 12 Oct 2023 00:21:17 GMT
ARG ODOO_RELEASE=20230925
# Thu, 12 Oct 2023 00:21:17 GMT
ARG ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
# Thu, 12 Oct 2023 00:22:49 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Oct 2023 00:22:54 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 12 Oct 2023 00:22:54 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Oct 2023 00:22:54 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Oct 2023 00:22:54 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Oct 2023 00:22:54 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Oct 2023 00:22:54 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Oct 2023 00:22:55 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Oct 2023 00:22:55 GMT
USER odoo
# Thu, 12 Oct 2023 00:22:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 00:22:55 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d361645e6e1ccf35842cd5eecba0ebc49b323a1b5620e333fcc753bae4d5fbc3`  
		Last Modified: Thu, 12 Oct 2023 00:29:13 GMT  
		Size: 221.0 MB (220990725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5302d28554bbcd79d6bf767cc6e8b48a0c1339264f4448085ff4cc3417f501f`  
		Last Modified: Thu, 12 Oct 2023 00:28:49 GMT  
		Size: 2.6 MB (2628048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d21d45cc4a63b48a65b85f9c014fd7d7af6a43a3571071f582c2bc334ad175`  
		Last Modified: Thu, 12 Oct 2023 00:28:49 GMT  
		Size: 457.2 KB (457194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef9674e55780baea497534673da1655f08144b64a962d71dd05909b03d673ec`  
		Last Modified: Thu, 12 Oct 2023 00:29:24 GMT  
		Size: 321.3 MB (321310642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89b0de0a7ef60c87a76e0d30dcc4ebf776d7050ca3f31dc56f3bd6f92460c1c`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2f302451ec2da5f3f57cf9a2370f276f5d0f43711d1ab57914828866f7f3ac`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0c51ea4877caa63c5e0e87e3d6da150114ba3fb4fb7bd2aebc49bc57985b35`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc2566bf1e44b6707a1ffb37669b2b252eb8bf4fa9e3b738cec1bd7469f5cf8`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:01697e5fbab426474004fa6b8c49f0af7554b1fafe2d5c10d68f52461fccf490
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:d84d0d713e8fc33126f97f0706df092f67f8d5e32bc7fb88083003cc40bf64f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.8 MB (576806934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f6ec0d61e8b356ed4c1422c3263ce2743dbc67a9973af9dd417ad90a8be6c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:19:57 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 12 Oct 2023 00:19:57 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 12 Oct 2023 00:19:57 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 00:21:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 12 Oct 2023 00:21:15 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:21:16 GMT
RUN npm install -g rtlcss
# Thu, 12 Oct 2023 00:21:16 GMT
ENV ODOO_VERSION=16.0
# Thu, 12 Oct 2023 00:21:17 GMT
ARG ODOO_RELEASE=20230925
# Thu, 12 Oct 2023 00:21:17 GMT
ARG ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
# Thu, 12 Oct 2023 00:22:49 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Oct 2023 00:22:54 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 12 Oct 2023 00:22:54 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Oct 2023 00:22:54 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Oct 2023 00:22:54 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Oct 2023 00:22:54 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Oct 2023 00:22:54 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Oct 2023 00:22:55 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Oct 2023 00:22:55 GMT
USER odoo
# Thu, 12 Oct 2023 00:22:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 00:22:55 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d361645e6e1ccf35842cd5eecba0ebc49b323a1b5620e333fcc753bae4d5fbc3`  
		Last Modified: Thu, 12 Oct 2023 00:29:13 GMT  
		Size: 221.0 MB (220990725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5302d28554bbcd79d6bf767cc6e8b48a0c1339264f4448085ff4cc3417f501f`  
		Last Modified: Thu, 12 Oct 2023 00:28:49 GMT  
		Size: 2.6 MB (2628048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d21d45cc4a63b48a65b85f9c014fd7d7af6a43a3571071f582c2bc334ad175`  
		Last Modified: Thu, 12 Oct 2023 00:28:49 GMT  
		Size: 457.2 KB (457194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef9674e55780baea497534673da1655f08144b64a962d71dd05909b03d673ec`  
		Last Modified: Thu, 12 Oct 2023 00:29:24 GMT  
		Size: 321.3 MB (321310642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89b0de0a7ef60c87a76e0d30dcc4ebf776d7050ca3f31dc56f3bd6f92460c1c`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2f302451ec2da5f3f57cf9a2370f276f5d0f43711d1ab57914828866f7f3ac`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0c51ea4877caa63c5e0e87e3d6da150114ba3fb4fb7bd2aebc49bc57985b35`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc2566bf1e44b6707a1ffb37669b2b252eb8bf4fa9e3b738cec1bd7469f5cf8`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:01697e5fbab426474004fa6b8c49f0af7554b1fafe2d5c10d68f52461fccf490
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:d84d0d713e8fc33126f97f0706df092f67f8d5e32bc7fb88083003cc40bf64f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.8 MB (576806934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f6ec0d61e8b356ed4c1422c3263ce2743dbc67a9973af9dd417ad90a8be6c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:19:57 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 12 Oct 2023 00:19:57 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 12 Oct 2023 00:19:57 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 00:21:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 12 Oct 2023 00:21:15 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:21:16 GMT
RUN npm install -g rtlcss
# Thu, 12 Oct 2023 00:21:16 GMT
ENV ODOO_VERSION=16.0
# Thu, 12 Oct 2023 00:21:17 GMT
ARG ODOO_RELEASE=20230925
# Thu, 12 Oct 2023 00:21:17 GMT
ARG ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
# Thu, 12 Oct 2023 00:22:49 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Oct 2023 00:22:54 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 12 Oct 2023 00:22:54 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Oct 2023 00:22:54 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Oct 2023 00:22:54 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Oct 2023 00:22:54 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Oct 2023 00:22:54 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Oct 2023 00:22:55 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Oct 2023 00:22:55 GMT
USER odoo
# Thu, 12 Oct 2023 00:22:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 00:22:55 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d361645e6e1ccf35842cd5eecba0ebc49b323a1b5620e333fcc753bae4d5fbc3`  
		Last Modified: Thu, 12 Oct 2023 00:29:13 GMT  
		Size: 221.0 MB (220990725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5302d28554bbcd79d6bf767cc6e8b48a0c1339264f4448085ff4cc3417f501f`  
		Last Modified: Thu, 12 Oct 2023 00:28:49 GMT  
		Size: 2.6 MB (2628048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d21d45cc4a63b48a65b85f9c014fd7d7af6a43a3571071f582c2bc334ad175`  
		Last Modified: Thu, 12 Oct 2023 00:28:49 GMT  
		Size: 457.2 KB (457194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef9674e55780baea497534673da1655f08144b64a962d71dd05909b03d673ec`  
		Last Modified: Thu, 12 Oct 2023 00:29:24 GMT  
		Size: 321.3 MB (321310642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89b0de0a7ef60c87a76e0d30dcc4ebf776d7050ca3f31dc56f3bd6f92460c1c`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2f302451ec2da5f3f57cf9a2370f276f5d0f43711d1ab57914828866f7f3ac`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0c51ea4877caa63c5e0e87e3d6da150114ba3fb4fb7bd2aebc49bc57985b35`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc2566bf1e44b6707a1ffb37669b2b252eb8bf4fa9e3b738cec1bd7469f5cf8`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
