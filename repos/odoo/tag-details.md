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
$ docker pull odoo@sha256:84247e36a322e9a875f5b4855453ac0bd7caf171a19c16a4e7a95e57de2732c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:4e0b89b8f6425639d02925b67beb6dc5da8d8c924ef64a8d1c817a6ece84ef3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.4 MB (531441053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a43eaf8697b219857e0d68f9a19e04cae7ffbe7fb57d2c2b63cc98f12426dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:52 GMT
ADD file:660e0093a3da49e4ca41260d09d585754ccb1eff8974c4b0dd4456b76ddbbc9a in / 
# Wed, 21 Dec 2022 01:20:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:04:03 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 21 Dec 2022 12:04:03 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 21 Dec 2022 12:04:03 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:05:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 21 Dec 2022 12:05:40 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:05:43 GMT
RUN npm install -g rtlcss
# Wed, 21 Dec 2022 12:05:43 GMT
ENV ODOO_VERSION=14.0
# Tue, 27 Dec 2022 18:01:36 GMT
ARG ODOO_RELEASE=20221226
# Tue, 27 Dec 2022 18:01:36 GMT
ARG ODOO_SHA=ec385462138e5027be4cf452844a3df3a8ef3573
# Tue, 27 Dec 2022 18:03:01 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=ec385462138e5027be4cf452844a3df3a8ef3573
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Dec 2022 18:03:05 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 27 Dec 2022 18:03:05 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Dec 2022 18:03:06 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=ec385462138e5027be4cf452844a3df3a8ef3573
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Dec 2022 18:03:06 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Dec 2022 18:03:06 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Dec 2022 18:03:06 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Dec 2022 18:03:06 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Dec 2022 18:03:06 GMT
USER odoo
# Tue, 27 Dec 2022 18:03:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Dec 2022 18:03:06 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b52ebda398ed2c4602ea06056f78d45a59474ee4e2a020967251ba082424e7e2`  
		Last Modified: Wed, 21 Dec 2022 01:25:17 GMT  
		Size: 27.1 MB (27140331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd809e7e6338e9ff619aa861a2c83ea5794e2e9f1e27208941b0cb0830d586`  
		Last Modified: Wed, 21 Dec 2022 12:09:24 GMT  
		Size: 213.2 MB (213188652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7447a10d2ac09f77c91f4405dd22b28022ae50b65e4a89bd2b93bc773c1a76f`  
		Last Modified: Wed, 21 Dec 2022 12:09:01 GMT  
		Size: 13.5 MB (13515235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2a982470c9023112777135e16db2722d58d0e80637be6f6512ed77e73a0e45`  
		Last Modified: Wed, 21 Dec 2022 12:08:58 GMT  
		Size: 457.1 KB (457118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65cdb588c681f94113f521c0f28431c5de472bc7ff6784c9335567da66d3f7`  
		Last Modified: Tue, 27 Dec 2022 18:05:29 GMT  
		Size: 277.1 MB (277137254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461a77cb6390c035984eed1a65b7e3da3e5a03f4302fed0095fabd83bb5d7953`  
		Last Modified: Tue, 27 Dec 2022 18:04:56 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f884bab9414953aa12f5133c82dfca14f7e59e2344ad5f37cf102fe1ecb1a115`  
		Last Modified: Tue, 27 Dec 2022 18:04:56 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6658d04cd4fbd2a673381901cf7f14fa3621a5ebf4241703805cb02342cb711`  
		Last Modified: Tue, 27 Dec 2022 18:04:56 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25933233c7917cc3b2fc9e8e050bc8fe6af9ef31d1a2850605d27c5824040318`  
		Last Modified: Tue, 27 Dec 2022 18:04:56 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:84247e36a322e9a875f5b4855453ac0bd7caf171a19c16a4e7a95e57de2732c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:4e0b89b8f6425639d02925b67beb6dc5da8d8c924ef64a8d1c817a6ece84ef3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.4 MB (531441053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a43eaf8697b219857e0d68f9a19e04cae7ffbe7fb57d2c2b63cc98f12426dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:52 GMT
ADD file:660e0093a3da49e4ca41260d09d585754ccb1eff8974c4b0dd4456b76ddbbc9a in / 
# Wed, 21 Dec 2022 01:20:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:04:03 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 21 Dec 2022 12:04:03 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 21 Dec 2022 12:04:03 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:05:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 21 Dec 2022 12:05:40 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:05:43 GMT
RUN npm install -g rtlcss
# Wed, 21 Dec 2022 12:05:43 GMT
ENV ODOO_VERSION=14.0
# Tue, 27 Dec 2022 18:01:36 GMT
ARG ODOO_RELEASE=20221226
# Tue, 27 Dec 2022 18:01:36 GMT
ARG ODOO_SHA=ec385462138e5027be4cf452844a3df3a8ef3573
# Tue, 27 Dec 2022 18:03:01 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=ec385462138e5027be4cf452844a3df3a8ef3573
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Dec 2022 18:03:05 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 27 Dec 2022 18:03:05 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Dec 2022 18:03:06 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=ec385462138e5027be4cf452844a3df3a8ef3573
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Dec 2022 18:03:06 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Dec 2022 18:03:06 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Dec 2022 18:03:06 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Dec 2022 18:03:06 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Dec 2022 18:03:06 GMT
USER odoo
# Tue, 27 Dec 2022 18:03:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Dec 2022 18:03:06 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b52ebda398ed2c4602ea06056f78d45a59474ee4e2a020967251ba082424e7e2`  
		Last Modified: Wed, 21 Dec 2022 01:25:17 GMT  
		Size: 27.1 MB (27140331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd809e7e6338e9ff619aa861a2c83ea5794e2e9f1e27208941b0cb0830d586`  
		Last Modified: Wed, 21 Dec 2022 12:09:24 GMT  
		Size: 213.2 MB (213188652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7447a10d2ac09f77c91f4405dd22b28022ae50b65e4a89bd2b93bc773c1a76f`  
		Last Modified: Wed, 21 Dec 2022 12:09:01 GMT  
		Size: 13.5 MB (13515235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2a982470c9023112777135e16db2722d58d0e80637be6f6512ed77e73a0e45`  
		Last Modified: Wed, 21 Dec 2022 12:08:58 GMT  
		Size: 457.1 KB (457118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65cdb588c681f94113f521c0f28431c5de472bc7ff6784c9335567da66d3f7`  
		Last Modified: Tue, 27 Dec 2022 18:05:29 GMT  
		Size: 277.1 MB (277137254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461a77cb6390c035984eed1a65b7e3da3e5a03f4302fed0095fabd83bb5d7953`  
		Last Modified: Tue, 27 Dec 2022 18:04:56 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f884bab9414953aa12f5133c82dfca14f7e59e2344ad5f37cf102fe1ecb1a115`  
		Last Modified: Tue, 27 Dec 2022 18:04:56 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6658d04cd4fbd2a673381901cf7f14fa3621a5ebf4241703805cb02342cb711`  
		Last Modified: Tue, 27 Dec 2022 18:04:56 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25933233c7917cc3b2fc9e8e050bc8fe6af9ef31d1a2850605d27c5824040318`  
		Last Modified: Tue, 27 Dec 2022 18:04:56 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:0a4ebb233d878d20e682a7cc9b1bcdbde9d2f4cd30063623c796eed4103726b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:5b34d4c6cc56318eabdb9ad1725f251faecbdae27e255a060ca45b91b38d592c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **559.5 MB (559545277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e20f24a0e06c486a28fe2989be4051bdab89b97cc932d77a70c5f1ddec46258`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:59:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 21 Dec 2022 11:59:17 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 21 Dec 2022 11:59:17 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:00:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 21 Dec 2022 12:00:38 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:00:39 GMT
RUN npm install -g rtlcss
# Wed, 21 Dec 2022 12:02:25 GMT
ENV ODOO_VERSION=15.0
# Tue, 27 Dec 2022 17:59:57 GMT
ARG ODOO_RELEASE=20221226
# Tue, 27 Dec 2022 17:59:58 GMT
ARG ODOO_SHA=37216e653c8db933790cc994b7cbad526a285e2b
# Tue, 27 Dec 2022 18:01:13 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=37216e653c8db933790cc994b7cbad526a285e2b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Dec 2022 18:01:18 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 27 Dec 2022 18:01:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Dec 2022 18:01:18 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=37216e653c8db933790cc994b7cbad526a285e2b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Dec 2022 18:01:19 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Dec 2022 18:01:19 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Dec 2022 18:01:19 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Dec 2022 18:01:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Dec 2022 18:01:19 GMT
USER odoo
# Tue, 27 Dec 2022 18:01:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Dec 2022 18:01:19 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b33e635a777ad2593a9a160436a438c4cf068b815a9d16dc6e4975f5df5b1c`  
		Last Modified: Wed, 21 Dec 2022 12:07:50 GMT  
		Size: 220.3 MB (220298472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c52fa0ca226e1b60d6963a358d003976668bd83f0ec398305fc945994bf0de`  
		Last Modified: Wed, 21 Dec 2022 12:07:24 GMT  
		Size: 2.6 MB (2573903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb896edd9e6352eb0d87d3b7f13ed806d0cef48cb80e239f4867f41c8a2b79dc`  
		Last Modified: Wed, 21 Dec 2022 12:07:23 GMT  
		Size: 452.6 KB (452551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba187ee52a9f13c66b88ace472af84df3512406f658bfbda7886b1d783a8c3e3`  
		Last Modified: Tue, 27 Dec 2022 18:04:47 GMT  
		Size: 304.8 MB (304820945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576e0dea1d730130dc894c3d66df314fda2a051e7348826b66efc57d5303e604`  
		Last Modified: Tue, 27 Dec 2022 18:04:11 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dab0d0f8d1c3f45526713a172f7c3eb62436bde1d9c4c77a470d30180b2908`  
		Last Modified: Tue, 27 Dec 2022 18:04:11 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d5d96f10b9da5f0aeb176df99603a58a96ebf76053ece966e0b22eb78ea97b`  
		Last Modified: Tue, 27 Dec 2022 18:04:11 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b3212d5f4102ba292bed02550fe568858894cfa2815fc96c71fbd3d2fd7937`  
		Last Modified: Tue, 27 Dec 2022 18:04:12 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:0a4ebb233d878d20e682a7cc9b1bcdbde9d2f4cd30063623c796eed4103726b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:5b34d4c6cc56318eabdb9ad1725f251faecbdae27e255a060ca45b91b38d592c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **559.5 MB (559545277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e20f24a0e06c486a28fe2989be4051bdab89b97cc932d77a70c5f1ddec46258`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:59:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 21 Dec 2022 11:59:17 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 21 Dec 2022 11:59:17 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:00:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 21 Dec 2022 12:00:38 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:00:39 GMT
RUN npm install -g rtlcss
# Wed, 21 Dec 2022 12:02:25 GMT
ENV ODOO_VERSION=15.0
# Tue, 27 Dec 2022 17:59:57 GMT
ARG ODOO_RELEASE=20221226
# Tue, 27 Dec 2022 17:59:58 GMT
ARG ODOO_SHA=37216e653c8db933790cc994b7cbad526a285e2b
# Tue, 27 Dec 2022 18:01:13 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=37216e653c8db933790cc994b7cbad526a285e2b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Dec 2022 18:01:18 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 27 Dec 2022 18:01:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Dec 2022 18:01:18 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=37216e653c8db933790cc994b7cbad526a285e2b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Dec 2022 18:01:19 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Dec 2022 18:01:19 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Dec 2022 18:01:19 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Dec 2022 18:01:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Dec 2022 18:01:19 GMT
USER odoo
# Tue, 27 Dec 2022 18:01:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Dec 2022 18:01:19 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b33e635a777ad2593a9a160436a438c4cf068b815a9d16dc6e4975f5df5b1c`  
		Last Modified: Wed, 21 Dec 2022 12:07:50 GMT  
		Size: 220.3 MB (220298472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c52fa0ca226e1b60d6963a358d003976668bd83f0ec398305fc945994bf0de`  
		Last Modified: Wed, 21 Dec 2022 12:07:24 GMT  
		Size: 2.6 MB (2573903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb896edd9e6352eb0d87d3b7f13ed806d0cef48cb80e239f4867f41c8a2b79dc`  
		Last Modified: Wed, 21 Dec 2022 12:07:23 GMT  
		Size: 452.6 KB (452551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba187ee52a9f13c66b88ace472af84df3512406f658bfbda7886b1d783a8c3e3`  
		Last Modified: Tue, 27 Dec 2022 18:04:47 GMT  
		Size: 304.8 MB (304820945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576e0dea1d730130dc894c3d66df314fda2a051e7348826b66efc57d5303e604`  
		Last Modified: Tue, 27 Dec 2022 18:04:11 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dab0d0f8d1c3f45526713a172f7c3eb62436bde1d9c4c77a470d30180b2908`  
		Last Modified: Tue, 27 Dec 2022 18:04:11 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d5d96f10b9da5f0aeb176df99603a58a96ebf76053ece966e0b22eb78ea97b`  
		Last Modified: Tue, 27 Dec 2022 18:04:11 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b3212d5f4102ba292bed02550fe568858894cfa2815fc96c71fbd3d2fd7937`  
		Last Modified: Tue, 27 Dec 2022 18:04:12 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:a854b63f28e7ad0e0aac7d6d0b81c56593379c3f0e91fef041a945806b032ac6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:3934899d8b1d4cc0ff058dca355eb6632e61f21d251e9bd325c67ec3dcd2ccb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **564.9 MB (564854271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ffec15148074cac6e5f41195c62a4ffb52d5c48d02407c3794053ce5d3581f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:59:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 21 Dec 2022 11:59:17 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 21 Dec 2022 11:59:17 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:00:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 21 Dec 2022 12:00:38 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:00:39 GMT
RUN npm install -g rtlcss
# Wed, 21 Dec 2022 12:00:39 GMT
ENV ODOO_VERSION=16.0
# Tue, 27 Dec 2022 17:58:04 GMT
ARG ODOO_RELEASE=20221226
# Tue, 27 Dec 2022 17:58:05 GMT
ARG ODOO_SHA=09e2bc4c27fc92a7f26928de61c122d18f550917
# Tue, 27 Dec 2022 17:59:38 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=09e2bc4c27fc92a7f26928de61c122d18f550917
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Dec 2022 17:59:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 27 Dec 2022 17:59:42 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Dec 2022 17:59:43 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=09e2bc4c27fc92a7f26928de61c122d18f550917
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Dec 2022 17:59:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Dec 2022 17:59:43 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Dec 2022 17:59:43 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Dec 2022 17:59:43 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Dec 2022 17:59:44 GMT
USER odoo
# Tue, 27 Dec 2022 17:59:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Dec 2022 17:59:44 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b33e635a777ad2593a9a160436a438c4cf068b815a9d16dc6e4975f5df5b1c`  
		Last Modified: Wed, 21 Dec 2022 12:07:50 GMT  
		Size: 220.3 MB (220298472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c52fa0ca226e1b60d6963a358d003976668bd83f0ec398305fc945994bf0de`  
		Last Modified: Wed, 21 Dec 2022 12:07:24 GMT  
		Size: 2.6 MB (2573903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb896edd9e6352eb0d87d3b7f13ed806d0cef48cb80e239f4867f41c8a2b79dc`  
		Last Modified: Wed, 21 Dec 2022 12:07:23 GMT  
		Size: 452.6 KB (452551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856cea1d7de940ac9e924a07b4aa2ceb0d9e5aab7571c1c614e3e5b9d00124d8`  
		Last Modified: Tue, 27 Dec 2022 18:04:00 GMT  
		Size: 310.1 MB (310129935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e748bfaf7d3f476cd7d422c55789f8086c7d7e70468d2b04a16f8b2a21635`  
		Last Modified: Tue, 27 Dec 2022 18:03:24 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61def8f4a313cdb79c5ff9e0ce42c05b0d35ab8a7ba338cb384d88cbad0aeada`  
		Last Modified: Tue, 27 Dec 2022 18:03:23 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831fae3e388aaf71b786b16636bc60c8aa00c5e56e043fd6e90be2266541913`  
		Last Modified: Tue, 27 Dec 2022 18:03:24 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec43443b79e4b6d6d5af62a039d0118c45e406647749dd077ea7e4f6aded9bab`  
		Last Modified: Tue, 27 Dec 2022 18:03:24 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:a854b63f28e7ad0e0aac7d6d0b81c56593379c3f0e91fef041a945806b032ac6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:3934899d8b1d4cc0ff058dca355eb6632e61f21d251e9bd325c67ec3dcd2ccb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **564.9 MB (564854271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ffec15148074cac6e5f41195c62a4ffb52d5c48d02407c3794053ce5d3581f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:59:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 21 Dec 2022 11:59:17 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 21 Dec 2022 11:59:17 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:00:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 21 Dec 2022 12:00:38 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:00:39 GMT
RUN npm install -g rtlcss
# Wed, 21 Dec 2022 12:00:39 GMT
ENV ODOO_VERSION=16.0
# Tue, 27 Dec 2022 17:58:04 GMT
ARG ODOO_RELEASE=20221226
# Tue, 27 Dec 2022 17:58:05 GMT
ARG ODOO_SHA=09e2bc4c27fc92a7f26928de61c122d18f550917
# Tue, 27 Dec 2022 17:59:38 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=09e2bc4c27fc92a7f26928de61c122d18f550917
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Dec 2022 17:59:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 27 Dec 2022 17:59:42 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Dec 2022 17:59:43 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=09e2bc4c27fc92a7f26928de61c122d18f550917
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Dec 2022 17:59:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Dec 2022 17:59:43 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Dec 2022 17:59:43 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Dec 2022 17:59:43 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Dec 2022 17:59:44 GMT
USER odoo
# Tue, 27 Dec 2022 17:59:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Dec 2022 17:59:44 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b33e635a777ad2593a9a160436a438c4cf068b815a9d16dc6e4975f5df5b1c`  
		Last Modified: Wed, 21 Dec 2022 12:07:50 GMT  
		Size: 220.3 MB (220298472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c52fa0ca226e1b60d6963a358d003976668bd83f0ec398305fc945994bf0de`  
		Last Modified: Wed, 21 Dec 2022 12:07:24 GMT  
		Size: 2.6 MB (2573903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb896edd9e6352eb0d87d3b7f13ed806d0cef48cb80e239f4867f41c8a2b79dc`  
		Last Modified: Wed, 21 Dec 2022 12:07:23 GMT  
		Size: 452.6 KB (452551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856cea1d7de940ac9e924a07b4aa2ceb0d9e5aab7571c1c614e3e5b9d00124d8`  
		Last Modified: Tue, 27 Dec 2022 18:04:00 GMT  
		Size: 310.1 MB (310129935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e748bfaf7d3f476cd7d422c55789f8086c7d7e70468d2b04a16f8b2a21635`  
		Last Modified: Tue, 27 Dec 2022 18:03:24 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61def8f4a313cdb79c5ff9e0ce42c05b0d35ab8a7ba338cb384d88cbad0aeada`  
		Last Modified: Tue, 27 Dec 2022 18:03:23 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831fae3e388aaf71b786b16636bc60c8aa00c5e56e043fd6e90be2266541913`  
		Last Modified: Tue, 27 Dec 2022 18:03:24 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec43443b79e4b6d6d5af62a039d0118c45e406647749dd077ea7e4f6aded9bab`  
		Last Modified: Tue, 27 Dec 2022 18:03:24 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:a854b63f28e7ad0e0aac7d6d0b81c56593379c3f0e91fef041a945806b032ac6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:3934899d8b1d4cc0ff058dca355eb6632e61f21d251e9bd325c67ec3dcd2ccb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **564.9 MB (564854271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ffec15148074cac6e5f41195c62a4ffb52d5c48d02407c3794053ce5d3581f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:59:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 21 Dec 2022 11:59:17 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 21 Dec 2022 11:59:17 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:00:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 21 Dec 2022 12:00:38 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:00:39 GMT
RUN npm install -g rtlcss
# Wed, 21 Dec 2022 12:00:39 GMT
ENV ODOO_VERSION=16.0
# Tue, 27 Dec 2022 17:58:04 GMT
ARG ODOO_RELEASE=20221226
# Tue, 27 Dec 2022 17:58:05 GMT
ARG ODOO_SHA=09e2bc4c27fc92a7f26928de61c122d18f550917
# Tue, 27 Dec 2022 17:59:38 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=09e2bc4c27fc92a7f26928de61c122d18f550917
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Dec 2022 17:59:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 27 Dec 2022 17:59:42 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Dec 2022 17:59:43 GMT
# ARGS: ODOO_RELEASE=20221226 ODOO_SHA=09e2bc4c27fc92a7f26928de61c122d18f550917
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Dec 2022 17:59:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Dec 2022 17:59:43 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Dec 2022 17:59:43 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Dec 2022 17:59:43 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Dec 2022 17:59:44 GMT
USER odoo
# Tue, 27 Dec 2022 17:59:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Dec 2022 17:59:44 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b33e635a777ad2593a9a160436a438c4cf068b815a9d16dc6e4975f5df5b1c`  
		Last Modified: Wed, 21 Dec 2022 12:07:50 GMT  
		Size: 220.3 MB (220298472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c52fa0ca226e1b60d6963a358d003976668bd83f0ec398305fc945994bf0de`  
		Last Modified: Wed, 21 Dec 2022 12:07:24 GMT  
		Size: 2.6 MB (2573903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb896edd9e6352eb0d87d3b7f13ed806d0cef48cb80e239f4867f41c8a2b79dc`  
		Last Modified: Wed, 21 Dec 2022 12:07:23 GMT  
		Size: 452.6 KB (452551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856cea1d7de940ac9e924a07b4aa2ceb0d9e5aab7571c1c614e3e5b9d00124d8`  
		Last Modified: Tue, 27 Dec 2022 18:04:00 GMT  
		Size: 310.1 MB (310129935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e748bfaf7d3f476cd7d422c55789f8086c7d7e70468d2b04a16f8b2a21635`  
		Last Modified: Tue, 27 Dec 2022 18:03:24 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61def8f4a313cdb79c5ff9e0ce42c05b0d35ab8a7ba338cb384d88cbad0aeada`  
		Last Modified: Tue, 27 Dec 2022 18:03:23 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831fae3e388aaf71b786b16636bc60c8aa00c5e56e043fd6e90be2266541913`  
		Last Modified: Tue, 27 Dec 2022 18:03:24 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec43443b79e4b6d6d5af62a039d0118c45e406647749dd077ea7e4f6aded9bab`  
		Last Modified: Tue, 27 Dec 2022 18:03:24 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
