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
$ docker pull odoo@sha256:ec817358882df7697834e17eb85c2a38fd7825d6d61380aa0190322445a21985
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:b7bcd007415f90d46160c6f060fadbfb641082a0a502a6733da663f2e9a2d451
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.5 MB (531523300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65ca0bd69d371ce80297f2d01b257d4c1c7bc655cb2fd200d5ed2f2be664309`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 04 Feb 2023 06:52:07 GMT
ADD file:4fbe1e3712cf37c85529cc81e0d03c82085203de00d64b0d669b5996e975925a in / 
# Sat, 04 Feb 2023 06:52:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:58:38 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 04 Feb 2023 14:58:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 04 Feb 2023 14:58:39 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 15:00:19 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 04 Feb 2023 15:00:31 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 15:00:34 GMT
RUN npm install -g rtlcss
# Sat, 04 Feb 2023 15:00:34 GMT
ENV ODOO_VERSION=14.0
# Sat, 04 Feb 2023 15:00:34 GMT
ARG ODOO_RELEASE=20230109
# Sat, 04 Feb 2023 15:00:34 GMT
ARG ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
# Sat, 04 Feb 2023 15:01:58 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 04 Feb 2023 15:02:02 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 04 Feb 2023 15:02:02 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 04 Feb 2023 15:02:03 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 04 Feb 2023 15:02:03 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 04 Feb 2023 15:02:03 GMT
EXPOSE 8069 8071 8072
# Sat, 04 Feb 2023 15:02:03 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 04 Feb 2023 15:02:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 04 Feb 2023 15:02:03 GMT
USER odoo
# Sat, 04 Feb 2023 15:02:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Feb 2023 15:02:04 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:0cf508b37688dca559387b506062329202aaf08b48be5f55f9278b2a818ad2c9`  
		Last Modified: Sat, 04 Feb 2023 06:56:58 GMT  
		Size: 27.1 MB (27140353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46875ca8f91d165cb74fdf5cd5302cbc7d0caa3f716c144b7fc138a9a6fd8e6`  
		Last Modified: Sat, 04 Feb 2023 15:04:29 GMT  
		Size: 213.2 MB (213188139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce146016e360d9bef7360580d5a2c0cb8a04f3c586c3d20cd2e952e36ee7c6d6`  
		Last Modified: Sat, 04 Feb 2023 15:04:07 GMT  
		Size: 13.5 MB (13515278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679f0464b415f1e41cdc975dba69941802cf353f77e10e16a8114069b928f025`  
		Last Modified: Sat, 04 Feb 2023 15:04:04 GMT  
		Size: 456.7 KB (456707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f5dfdf6edba0828b165568f39693daeaebbad7348ae8e9a5ab77ba3be7f3a6`  
		Last Modified: Sat, 04 Feb 2023 15:04:36 GMT  
		Size: 277.2 MB (277220357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6e1c9e612b37b3183a944d4a890f6843800e727c7955bbb06a22d643cbbf63`  
		Last Modified: Sat, 04 Feb 2023 15:04:02 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a09fc9db5bca1615a6f6ad938bee226d919b76c46636c87697d10dcb7da85`  
		Last Modified: Sat, 04 Feb 2023 15:04:02 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60b4fc48ccedb78060904eaf8cc469417a922b025fedb31f1ba43c66fb868b`  
		Last Modified: Sat, 04 Feb 2023 15:04:02 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4780cc3c6b9312fb8a63e2f3cec0085b35f704d7da7c544d6b6e22977646a6`  
		Last Modified: Sat, 04 Feb 2023 15:04:02 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:ec817358882df7697834e17eb85c2a38fd7825d6d61380aa0190322445a21985
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:b7bcd007415f90d46160c6f060fadbfb641082a0a502a6733da663f2e9a2d451
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.5 MB (531523300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65ca0bd69d371ce80297f2d01b257d4c1c7bc655cb2fd200d5ed2f2be664309`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 04 Feb 2023 06:52:07 GMT
ADD file:4fbe1e3712cf37c85529cc81e0d03c82085203de00d64b0d669b5996e975925a in / 
# Sat, 04 Feb 2023 06:52:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:58:38 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 04 Feb 2023 14:58:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 04 Feb 2023 14:58:39 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 15:00:19 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 04 Feb 2023 15:00:31 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 15:00:34 GMT
RUN npm install -g rtlcss
# Sat, 04 Feb 2023 15:00:34 GMT
ENV ODOO_VERSION=14.0
# Sat, 04 Feb 2023 15:00:34 GMT
ARG ODOO_RELEASE=20230109
# Sat, 04 Feb 2023 15:00:34 GMT
ARG ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
# Sat, 04 Feb 2023 15:01:58 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 04 Feb 2023 15:02:02 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 04 Feb 2023 15:02:02 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 04 Feb 2023 15:02:03 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=ef9eef9a5e5bbeb455ac7d1c05cc675e74876609
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 04 Feb 2023 15:02:03 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 04 Feb 2023 15:02:03 GMT
EXPOSE 8069 8071 8072
# Sat, 04 Feb 2023 15:02:03 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 04 Feb 2023 15:02:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 04 Feb 2023 15:02:03 GMT
USER odoo
# Sat, 04 Feb 2023 15:02:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Feb 2023 15:02:04 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:0cf508b37688dca559387b506062329202aaf08b48be5f55f9278b2a818ad2c9`  
		Last Modified: Sat, 04 Feb 2023 06:56:58 GMT  
		Size: 27.1 MB (27140353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46875ca8f91d165cb74fdf5cd5302cbc7d0caa3f716c144b7fc138a9a6fd8e6`  
		Last Modified: Sat, 04 Feb 2023 15:04:29 GMT  
		Size: 213.2 MB (213188139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce146016e360d9bef7360580d5a2c0cb8a04f3c586c3d20cd2e952e36ee7c6d6`  
		Last Modified: Sat, 04 Feb 2023 15:04:07 GMT  
		Size: 13.5 MB (13515278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679f0464b415f1e41cdc975dba69941802cf353f77e10e16a8114069b928f025`  
		Last Modified: Sat, 04 Feb 2023 15:04:04 GMT  
		Size: 456.7 KB (456707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f5dfdf6edba0828b165568f39693daeaebbad7348ae8e9a5ab77ba3be7f3a6`  
		Last Modified: Sat, 04 Feb 2023 15:04:36 GMT  
		Size: 277.2 MB (277220357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6e1c9e612b37b3183a944d4a890f6843800e727c7955bbb06a22d643cbbf63`  
		Last Modified: Sat, 04 Feb 2023 15:04:02 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a09fc9db5bca1615a6f6ad938bee226d919b76c46636c87697d10dcb7da85`  
		Last Modified: Sat, 04 Feb 2023 15:04:02 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60b4fc48ccedb78060904eaf8cc469417a922b025fedb31f1ba43c66fb868b`  
		Last Modified: Sat, 04 Feb 2023 15:04:02 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4780cc3c6b9312fb8a63e2f3cec0085b35f704d7da7c544d6b6e22977646a6`  
		Last Modified: Sat, 04 Feb 2023 15:04:02 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:cedb15e82f428cd2e26d4a086c7c01efc78fe0b7d0eae9462631418714d7f5da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:34102f01c5e70fa5174ad7c4e8350728e707fd185e58ce2b2c1ff799e8450a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **559.7 MB (559720018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:698249fb6ebf50ae36be3378038a14dd42260bd3311cf96ba3a71e8e2e48fd87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:53:52 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 04 Feb 2023 14:53:52 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 04 Feb 2023 14:53:52 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 14:55:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 04 Feb 2023 14:55:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:55:15 GMT
RUN npm install -g rtlcss
# Sat, 04 Feb 2023 14:57:00 GMT
ENV ODOO_VERSION=15.0
# Sat, 04 Feb 2023 14:57:00 GMT
ARG ODOO_RELEASE=20230109
# Sat, 04 Feb 2023 14:57:00 GMT
ARG ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
# Sat, 04 Feb 2023 14:58:16 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 04 Feb 2023 14:58:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 04 Feb 2023 14:58:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 04 Feb 2023 14:58:21 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 04 Feb 2023 14:58:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 04 Feb 2023 14:58:21 GMT
EXPOSE 8069 8071 8072
# Sat, 04 Feb 2023 14:58:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 04 Feb 2023 14:58:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 04 Feb 2023 14:58:21 GMT
USER odoo
# Sat, 04 Feb 2023 14:58:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Feb 2023 14:58:21 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad657314e8b53b0a613039a17caa7f1f3071a8c4baba7938cae0f1f89d15be92`  
		Last Modified: Sat, 04 Feb 2023 15:02:55 GMT  
		Size: 220.3 MB (220301510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd8b86b19f6ff9f32a13fce6026c4775fcc428e4a3bead195007db14444bc31`  
		Last Modified: Sat, 04 Feb 2023 15:02:28 GMT  
		Size: 2.6 MB (2573962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2bacefcbedf6e986430ebc769f05d9878b3c9514a84c0b59c50afd03feba34`  
		Last Modified: Sat, 04 Feb 2023 15:02:28 GMT  
		Size: 452.2 KB (452232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c561e1fcf7e302c4bc7ade9d79884bff4bbe33876d802c64c8d6e7d0487640c0`  
		Last Modified: Sat, 04 Feb 2023 15:03:52 GMT  
		Size: 305.0 MB (304992934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bf7c7305c1f862573d000dbfea4ae531e801b8b7a919fb848f4fc17fd96ff3`  
		Last Modified: Sat, 04 Feb 2023 15:03:16 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5467cf41784fb9bd813eae010b40a8f0df96b8574dd4ffab5844de4df028fe63`  
		Last Modified: Sat, 04 Feb 2023 15:03:17 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b388130d5039415b569aeb6bf2ee26f08748f32581d97e3400152bfa8c8ab1`  
		Last Modified: Sat, 04 Feb 2023 15:03:16 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3377cf7348fe34a3e618b87002d46f5f9f69fa272b965a76dcd592c2106929d9`  
		Last Modified: Sat, 04 Feb 2023 15:03:17 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:cedb15e82f428cd2e26d4a086c7c01efc78fe0b7d0eae9462631418714d7f5da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:34102f01c5e70fa5174ad7c4e8350728e707fd185e58ce2b2c1ff799e8450a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **559.7 MB (559720018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:698249fb6ebf50ae36be3378038a14dd42260bd3311cf96ba3a71e8e2e48fd87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:53:52 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 04 Feb 2023 14:53:52 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 04 Feb 2023 14:53:52 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 14:55:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 04 Feb 2023 14:55:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:55:15 GMT
RUN npm install -g rtlcss
# Sat, 04 Feb 2023 14:57:00 GMT
ENV ODOO_VERSION=15.0
# Sat, 04 Feb 2023 14:57:00 GMT
ARG ODOO_RELEASE=20230109
# Sat, 04 Feb 2023 14:57:00 GMT
ARG ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
# Sat, 04 Feb 2023 14:58:16 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 04 Feb 2023 14:58:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 04 Feb 2023 14:58:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 04 Feb 2023 14:58:21 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=618e45490616f63dfb68077523c2971cbb6cdda7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 04 Feb 2023 14:58:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 04 Feb 2023 14:58:21 GMT
EXPOSE 8069 8071 8072
# Sat, 04 Feb 2023 14:58:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 04 Feb 2023 14:58:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 04 Feb 2023 14:58:21 GMT
USER odoo
# Sat, 04 Feb 2023 14:58:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Feb 2023 14:58:21 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad657314e8b53b0a613039a17caa7f1f3071a8c4baba7938cae0f1f89d15be92`  
		Last Modified: Sat, 04 Feb 2023 15:02:55 GMT  
		Size: 220.3 MB (220301510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd8b86b19f6ff9f32a13fce6026c4775fcc428e4a3bead195007db14444bc31`  
		Last Modified: Sat, 04 Feb 2023 15:02:28 GMT  
		Size: 2.6 MB (2573962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2bacefcbedf6e986430ebc769f05d9878b3c9514a84c0b59c50afd03feba34`  
		Last Modified: Sat, 04 Feb 2023 15:02:28 GMT  
		Size: 452.2 KB (452232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c561e1fcf7e302c4bc7ade9d79884bff4bbe33876d802c64c8d6e7d0487640c0`  
		Last Modified: Sat, 04 Feb 2023 15:03:52 GMT  
		Size: 305.0 MB (304992934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88bf7c7305c1f862573d000dbfea4ae531e801b8b7a919fb848f4fc17fd96ff3`  
		Last Modified: Sat, 04 Feb 2023 15:03:16 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5467cf41784fb9bd813eae010b40a8f0df96b8574dd4ffab5844de4df028fe63`  
		Last Modified: Sat, 04 Feb 2023 15:03:17 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b388130d5039415b569aeb6bf2ee26f08748f32581d97e3400152bfa8c8ab1`  
		Last Modified: Sat, 04 Feb 2023 15:03:16 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3377cf7348fe34a3e618b87002d46f5f9f69fa272b965a76dcd592c2106929d9`  
		Last Modified: Sat, 04 Feb 2023 15:03:17 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:b4147b40da31ac4a2df8be2b28dd639b2e00bff079837c55e35864d0aa7ab186
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:4ac878f5df6ad228f2c98e7ebdffa0634de5f9a8971a545404562d1fa589b933
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566183830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9bcd3f05e245d506d4d4c56f85bbe934123cf8ec014d99111b8fe9e28dbcb90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:53:52 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 04 Feb 2023 14:53:52 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 04 Feb 2023 14:53:52 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 14:55:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 04 Feb 2023 14:55:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:55:15 GMT
RUN npm install -g rtlcss
# Sat, 04 Feb 2023 14:55:15 GMT
ENV ODOO_VERSION=16.0
# Sat, 04 Feb 2023 14:55:15 GMT
ARG ODOO_RELEASE=20230109
# Sat, 04 Feb 2023 14:55:15 GMT
ARG ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
# Sat, 04 Feb 2023 14:56:41 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 04 Feb 2023 14:56:46 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 04 Feb 2023 14:56:46 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 04 Feb 2023 14:56:46 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 04 Feb 2023 14:56:46 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 04 Feb 2023 14:56:46 GMT
EXPOSE 8069 8071 8072
# Sat, 04 Feb 2023 14:56:47 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 04 Feb 2023 14:56:47 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 04 Feb 2023 14:56:47 GMT
USER odoo
# Sat, 04 Feb 2023 14:56:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Feb 2023 14:56:47 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad657314e8b53b0a613039a17caa7f1f3071a8c4baba7938cae0f1f89d15be92`  
		Last Modified: Sat, 04 Feb 2023 15:02:55 GMT  
		Size: 220.3 MB (220301510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd8b86b19f6ff9f32a13fce6026c4775fcc428e4a3bead195007db14444bc31`  
		Last Modified: Sat, 04 Feb 2023 15:02:28 GMT  
		Size: 2.6 MB (2573962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2bacefcbedf6e986430ebc769f05d9878b3c9514a84c0b59c50afd03feba34`  
		Last Modified: Sat, 04 Feb 2023 15:02:28 GMT  
		Size: 452.2 KB (452232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d48c44e58c91addfa074531c297de637159348e9d2b173445047c9056c91bbb`  
		Last Modified: Sat, 04 Feb 2023 15:03:04 GMT  
		Size: 311.5 MB (311456747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da7e9d4a8047843fb3437a87819de562fde0fcaa42b4de186b8026c3635f729`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc30ac6dd37b0186fb8b9023b21943ecc24a21cae7a53bea241a55b5697aea9`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491f760c366d63ff2e63a4bb9328beb3cde85c9a6f80efb3829a2b7d901d43d2`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cf82a0d9eeb10feab350c3c8a42b91cb53d2e7f69128e1bb0097e176f250c2`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:b4147b40da31ac4a2df8be2b28dd639b2e00bff079837c55e35864d0aa7ab186
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:4ac878f5df6ad228f2c98e7ebdffa0634de5f9a8971a545404562d1fa589b933
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566183830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9bcd3f05e245d506d4d4c56f85bbe934123cf8ec014d99111b8fe9e28dbcb90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:53:52 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 04 Feb 2023 14:53:52 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 04 Feb 2023 14:53:52 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 14:55:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 04 Feb 2023 14:55:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:55:15 GMT
RUN npm install -g rtlcss
# Sat, 04 Feb 2023 14:55:15 GMT
ENV ODOO_VERSION=16.0
# Sat, 04 Feb 2023 14:55:15 GMT
ARG ODOO_RELEASE=20230109
# Sat, 04 Feb 2023 14:55:15 GMT
ARG ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
# Sat, 04 Feb 2023 14:56:41 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 04 Feb 2023 14:56:46 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 04 Feb 2023 14:56:46 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 04 Feb 2023 14:56:46 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 04 Feb 2023 14:56:46 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 04 Feb 2023 14:56:46 GMT
EXPOSE 8069 8071 8072
# Sat, 04 Feb 2023 14:56:47 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 04 Feb 2023 14:56:47 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 04 Feb 2023 14:56:47 GMT
USER odoo
# Sat, 04 Feb 2023 14:56:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Feb 2023 14:56:47 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad657314e8b53b0a613039a17caa7f1f3071a8c4baba7938cae0f1f89d15be92`  
		Last Modified: Sat, 04 Feb 2023 15:02:55 GMT  
		Size: 220.3 MB (220301510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd8b86b19f6ff9f32a13fce6026c4775fcc428e4a3bead195007db14444bc31`  
		Last Modified: Sat, 04 Feb 2023 15:02:28 GMT  
		Size: 2.6 MB (2573962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2bacefcbedf6e986430ebc769f05d9878b3c9514a84c0b59c50afd03feba34`  
		Last Modified: Sat, 04 Feb 2023 15:02:28 GMT  
		Size: 452.2 KB (452232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d48c44e58c91addfa074531c297de637159348e9d2b173445047c9056c91bbb`  
		Last Modified: Sat, 04 Feb 2023 15:03:04 GMT  
		Size: 311.5 MB (311456747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da7e9d4a8047843fb3437a87819de562fde0fcaa42b4de186b8026c3635f729`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc30ac6dd37b0186fb8b9023b21943ecc24a21cae7a53bea241a55b5697aea9`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491f760c366d63ff2e63a4bb9328beb3cde85c9a6f80efb3829a2b7d901d43d2`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cf82a0d9eeb10feab350c3c8a42b91cb53d2e7f69128e1bb0097e176f250c2`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:b4147b40da31ac4a2df8be2b28dd639b2e00bff079837c55e35864d0aa7ab186
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:4ac878f5df6ad228f2c98e7ebdffa0634de5f9a8971a545404562d1fa589b933
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.2 MB (566183830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9bcd3f05e245d506d4d4c56f85bbe934123cf8ec014d99111b8fe9e28dbcb90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:53:52 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 04 Feb 2023 14:53:52 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 04 Feb 2023 14:53:52 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 14:55:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 04 Feb 2023 14:55:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:55:15 GMT
RUN npm install -g rtlcss
# Sat, 04 Feb 2023 14:55:15 GMT
ENV ODOO_VERSION=16.0
# Sat, 04 Feb 2023 14:55:15 GMT
ARG ODOO_RELEASE=20230109
# Sat, 04 Feb 2023 14:55:15 GMT
ARG ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
# Sat, 04 Feb 2023 14:56:41 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 04 Feb 2023 14:56:46 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Sat, 04 Feb 2023 14:56:46 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 04 Feb 2023 14:56:46 GMT
# ARGS: ODOO_RELEASE=20230109 ODOO_SHA=884bf72c7318835b9ac56be2594032cbba7b8c7b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 04 Feb 2023 14:56:46 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 04 Feb 2023 14:56:46 GMT
EXPOSE 8069 8071 8072
# Sat, 04 Feb 2023 14:56:47 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 04 Feb 2023 14:56:47 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 04 Feb 2023 14:56:47 GMT
USER odoo
# Sat, 04 Feb 2023 14:56:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Feb 2023 14:56:47 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad657314e8b53b0a613039a17caa7f1f3071a8c4baba7938cae0f1f89d15be92`  
		Last Modified: Sat, 04 Feb 2023 15:02:55 GMT  
		Size: 220.3 MB (220301510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd8b86b19f6ff9f32a13fce6026c4775fcc428e4a3bead195007db14444bc31`  
		Last Modified: Sat, 04 Feb 2023 15:02:28 GMT  
		Size: 2.6 MB (2573962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2bacefcbedf6e986430ebc769f05d9878b3c9514a84c0b59c50afd03feba34`  
		Last Modified: Sat, 04 Feb 2023 15:02:28 GMT  
		Size: 452.2 KB (452232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d48c44e58c91addfa074531c297de637159348e9d2b173445047c9056c91bbb`  
		Last Modified: Sat, 04 Feb 2023 15:03:04 GMT  
		Size: 311.5 MB (311456747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da7e9d4a8047843fb3437a87819de562fde0fcaa42b4de186b8026c3635f729`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc30ac6dd37b0186fb8b9023b21943ecc24a21cae7a53bea241a55b5697aea9`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491f760c366d63ff2e63a4bb9328beb3cde85c9a6f80efb3829a2b7d901d43d2`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cf82a0d9eeb10feab350c3c8a42b91cb53d2e7f69128e1bb0097e176f250c2`  
		Last Modified: Sat, 04 Feb 2023 15:02:26 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
