<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `odoo`

-	[`odoo:11`](#odoo11)
-	[`odoo:11.0`](#odoo110)
-	[`odoo:12`](#odoo12)
-	[`odoo:12.0`](#odoo120)
-	[`odoo:13`](#odoo13)
-	[`odoo:13.0`](#odoo130)
-	[`odoo:latest`](#odoolatest)

## `odoo:11`

```console
$ docker pull odoo@sha256:de57d9b543e92d291b57b51da97f229549d774251452109a292bdb3c7ffb665e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:11` - linux; amd64

```console
$ docker pull odoo@sha256:6540f7c577a3e3161bde3b7374b7a35a380804078a0799b4eb1bc9cf8dfcecd4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386119192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8566644ac9aa45f9ff7c59752ca79776b2dd31e4ceafd12aa566ca7b973b5b94`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 13 May 2020 21:23:54 GMT
ADD file:3e0b81347262efc5a7401a531be7ab45cb8ab05ddab528fbb849bea0053865a0 in / 
# Wed, 13 May 2020 21:23:54 GMT
CMD ["bash"]
# Thu, 14 May 2020 03:30:20 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 14 May 2020 03:30:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 14 May 2020 03:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 03:30:22 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Thu, 14 May 2020 03:32:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 14 May 2020 03:34:08 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 03:35:26 GMT
ENV ODOO_VERSION=11.0
# Thu, 14 May 2020 03:35:26 GMT
ARG ODOO_RELEASE=20200417
# Thu, 14 May 2020 03:35:26 GMT
ARG ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
# Thu, 14 May 2020 03:36:48 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb        && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 14 May 2020 03:36:50 GMT
COPY file:cdc612ad49467417b0321c166f94e4f99b071755cb6ade071774e83d3b6ee4cb in / 
# Thu, 14 May 2020 03:36:51 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 14 May 2020 03:36:52 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 14 May 2020 03:36:52 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 14 May 2020 03:36:53 GMT
EXPOSE 8069 8071 8072
# Thu, 14 May 2020 03:36:53 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 14 May 2020 03:36:53 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 14 May 2020 03:36:54 GMT
USER odoo
# Thu, 14 May 2020 03:36:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 03:36:55 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e4f2068f62324fe92e80c472afb3742bf506f2a52712bf36ec0456de94c5b14e`  
		Last Modified: Wed, 13 May 2020 21:30:12 GMT  
		Size: 22.5 MB (22513438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69706862e6023254330524f1fca1701e62faff84f32128cd2c278f3e97422bb3`  
		Last Modified: Thu, 14 May 2020 03:38:14 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1947c088fc14f7107dd124b253fa766a8cb5ccd46dcfb8f5d337c83115bbd`  
		Last Modified: Thu, 14 May 2020 03:38:54 GMT  
		Size: 219.7 MB (219651509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217e74fcb404ae29df200cb68fe054466043e2c64606686ec1297d7c90993911`  
		Last Modified: Thu, 14 May 2020 03:38:14 GMT  
		Size: 2.3 MB (2334752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810f19f693c3931a7dff46698b75f131fd13700a942028b507a4cca46df120d`  
		Last Modified: Thu, 14 May 2020 03:39:37 GMT  
		Size: 141.6 MB (141616856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67411c8bad3c84877b04ff6e96513c802e28d1f399a2cc41a148f9b7b697ee83`  
		Last Modified: Thu, 14 May 2020 03:38:59 GMT  
		Size: 673.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75cbc704c3c0ce763d63f4e20b56c388847b9cbac38ad2b7d1241ed02f0b7ae`  
		Last Modified: Thu, 14 May 2020 03:38:59 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf57c05519ff078789b4dd971dd6bcb951648b915297de0b8592e952ce53a57e`  
		Last Modified: Thu, 14 May 2020 03:39:00 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a1d33a7b1dadc13b5c40d3cb968164b72455da40990063599c9cb18428a896`  
		Last Modified: Thu, 14 May 2020 03:38:59 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:11.0`

```console
$ docker pull odoo@sha256:de57d9b543e92d291b57b51da97f229549d774251452109a292bdb3c7ffb665e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:11.0` - linux; amd64

```console
$ docker pull odoo@sha256:6540f7c577a3e3161bde3b7374b7a35a380804078a0799b4eb1bc9cf8dfcecd4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386119192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8566644ac9aa45f9ff7c59752ca79776b2dd31e4ceafd12aa566ca7b973b5b94`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 13 May 2020 21:23:54 GMT
ADD file:3e0b81347262efc5a7401a531be7ab45cb8ab05ddab528fbb849bea0053865a0 in / 
# Wed, 13 May 2020 21:23:54 GMT
CMD ["bash"]
# Thu, 14 May 2020 03:30:20 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 14 May 2020 03:30:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 14 May 2020 03:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 03:30:22 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Thu, 14 May 2020 03:32:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 14 May 2020 03:34:08 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 03:35:26 GMT
ENV ODOO_VERSION=11.0
# Thu, 14 May 2020 03:35:26 GMT
ARG ODOO_RELEASE=20200417
# Thu, 14 May 2020 03:35:26 GMT
ARG ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
# Thu, 14 May 2020 03:36:48 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb        && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 14 May 2020 03:36:50 GMT
COPY file:cdc612ad49467417b0321c166f94e4f99b071755cb6ade071774e83d3b6ee4cb in / 
# Thu, 14 May 2020 03:36:51 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 14 May 2020 03:36:52 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 14 May 2020 03:36:52 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 14 May 2020 03:36:53 GMT
EXPOSE 8069 8071 8072
# Thu, 14 May 2020 03:36:53 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 14 May 2020 03:36:53 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 14 May 2020 03:36:54 GMT
USER odoo
# Thu, 14 May 2020 03:36:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 03:36:55 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e4f2068f62324fe92e80c472afb3742bf506f2a52712bf36ec0456de94c5b14e`  
		Last Modified: Wed, 13 May 2020 21:30:12 GMT  
		Size: 22.5 MB (22513438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69706862e6023254330524f1fca1701e62faff84f32128cd2c278f3e97422bb3`  
		Last Modified: Thu, 14 May 2020 03:38:14 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1947c088fc14f7107dd124b253fa766a8cb5ccd46dcfb8f5d337c83115bbd`  
		Last Modified: Thu, 14 May 2020 03:38:54 GMT  
		Size: 219.7 MB (219651509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217e74fcb404ae29df200cb68fe054466043e2c64606686ec1297d7c90993911`  
		Last Modified: Thu, 14 May 2020 03:38:14 GMT  
		Size: 2.3 MB (2334752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810f19f693c3931a7dff46698b75f131fd13700a942028b507a4cca46df120d`  
		Last Modified: Thu, 14 May 2020 03:39:37 GMT  
		Size: 141.6 MB (141616856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67411c8bad3c84877b04ff6e96513c802e28d1f399a2cc41a148f9b7b697ee83`  
		Last Modified: Thu, 14 May 2020 03:38:59 GMT  
		Size: 673.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75cbc704c3c0ce763d63f4e20b56c388847b9cbac38ad2b7d1241ed02f0b7ae`  
		Last Modified: Thu, 14 May 2020 03:38:59 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf57c05519ff078789b4dd971dd6bcb951648b915297de0b8592e952ce53a57e`  
		Last Modified: Thu, 14 May 2020 03:39:00 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a1d33a7b1dadc13b5c40d3cb968164b72455da40990063599c9cb18428a896`  
		Last Modified: Thu, 14 May 2020 03:38:59 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12`

```console
$ docker pull odoo@sha256:6fa8e62ffaf408ea5e57228412bb072ea9fcb7ed52da74130fe06038e28a27d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:7506615be42157dea02bd9fe27b009a0ec593659e3eb22af623722c44aab5674
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.8 MB (395843555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10bef1facda91f3b3f93cea93836324c8494b5ee8ff82192fc6a068acb382b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 13 May 2020 21:23:54 GMT
ADD file:3e0b81347262efc5a7401a531be7ab45cb8ab05ddab528fbb849bea0053865a0 in / 
# Wed, 13 May 2020 21:23:54 GMT
CMD ["bash"]
# Thu, 14 May 2020 03:30:20 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 14 May 2020 03:30:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 14 May 2020 03:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 03:30:22 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Thu, 14 May 2020 03:32:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 14 May 2020 03:34:08 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 03:34:22 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 03:34:22 GMT
ENV ODOO_VERSION=12.0
# Thu, 14 May 2020 03:34:23 GMT
ARG ODOO_RELEASE=20200417
# Thu, 14 May 2020 03:34:23 GMT
ARG ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
# Thu, 14 May 2020 03:35:11 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 14 May 2020 03:35:12 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 14 May 2020 03:35:12 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 14 May 2020 03:35:13 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 14 May 2020 03:35:13 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 14 May 2020 03:35:13 GMT
EXPOSE 8069 8071 8072
# Thu, 14 May 2020 03:35:14 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 14 May 2020 03:35:14 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 14 May 2020 03:35:14 GMT
USER odoo
# Thu, 14 May 2020 03:35:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 03:35:14 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e4f2068f62324fe92e80c472afb3742bf506f2a52712bf36ec0456de94c5b14e`  
		Last Modified: Wed, 13 May 2020 21:30:12 GMT  
		Size: 22.5 MB (22513438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69706862e6023254330524f1fca1701e62faff84f32128cd2c278f3e97422bb3`  
		Last Modified: Thu, 14 May 2020 03:38:14 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1947c088fc14f7107dd124b253fa766a8cb5ccd46dcfb8f5d337c83115bbd`  
		Last Modified: Thu, 14 May 2020 03:38:54 GMT  
		Size: 219.7 MB (219651509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217e74fcb404ae29df200cb68fe054466043e2c64606686ec1297d7c90993911`  
		Last Modified: Thu, 14 May 2020 03:38:14 GMT  
		Size: 2.3 MB (2334752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6cd7e79bb8774fe6fe3d334ac5330373c01c6a724cb68c2ed546c6f88dfa68`  
		Last Modified: Thu, 14 May 2020 03:38:22 GMT  
		Size: 22.2 MB (22231932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6131f5bfd68245934bbde33583186bf533670eb95b1544a765ecc31021649dc2`  
		Last Modified: Thu, 14 May 2020 03:38:54 GMT  
		Size: 129.1 MB (129109289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e06408fd0546dfc093d262303b90a414cde2ffaece8874b1671db130ccc3dd9`  
		Last Modified: Thu, 14 May 2020 03:38:12 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa5e51289fb972fb7920c24059a53d20043a5f62bcae6b52973cfaddb677d1b`  
		Last Modified: Thu, 14 May 2020 03:38:12 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d615828bf5968dc084f7b5b460c65fc3b176e78dfe8cc87a52abe3994d1c31fc`  
		Last Modified: Thu, 14 May 2020 03:38:12 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed0ee72de06cb96a6573e480e33e5666cfbdc7dbe46d165f35a4df36833590d`  
		Last Modified: Thu, 14 May 2020 03:38:12 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:6fa8e62ffaf408ea5e57228412bb072ea9fcb7ed52da74130fe06038e28a27d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:7506615be42157dea02bd9fe27b009a0ec593659e3eb22af623722c44aab5674
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.8 MB (395843555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10bef1facda91f3b3f93cea93836324c8494b5ee8ff82192fc6a068acb382b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 13 May 2020 21:23:54 GMT
ADD file:3e0b81347262efc5a7401a531be7ab45cb8ab05ddab528fbb849bea0053865a0 in / 
# Wed, 13 May 2020 21:23:54 GMT
CMD ["bash"]
# Thu, 14 May 2020 03:30:20 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 14 May 2020 03:30:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 14 May 2020 03:30:21 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 03:30:22 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Thu, 14 May 2020 03:32:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 14 May 2020 03:34:08 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 03:34:22 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 03:34:22 GMT
ENV ODOO_VERSION=12.0
# Thu, 14 May 2020 03:34:23 GMT
ARG ODOO_RELEASE=20200417
# Thu, 14 May 2020 03:34:23 GMT
ARG ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
# Thu, 14 May 2020 03:35:11 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 14 May 2020 03:35:12 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 14 May 2020 03:35:12 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 14 May 2020 03:35:13 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 14 May 2020 03:35:13 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 14 May 2020 03:35:13 GMT
EXPOSE 8069 8071 8072
# Thu, 14 May 2020 03:35:14 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 14 May 2020 03:35:14 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 14 May 2020 03:35:14 GMT
USER odoo
# Thu, 14 May 2020 03:35:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 03:35:14 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e4f2068f62324fe92e80c472afb3742bf506f2a52712bf36ec0456de94c5b14e`  
		Last Modified: Wed, 13 May 2020 21:30:12 GMT  
		Size: 22.5 MB (22513438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69706862e6023254330524f1fca1701e62faff84f32128cd2c278f3e97422bb3`  
		Last Modified: Thu, 14 May 2020 03:38:14 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1947c088fc14f7107dd124b253fa766a8cb5ccd46dcfb8f5d337c83115bbd`  
		Last Modified: Thu, 14 May 2020 03:38:54 GMT  
		Size: 219.7 MB (219651509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217e74fcb404ae29df200cb68fe054466043e2c64606686ec1297d7c90993911`  
		Last Modified: Thu, 14 May 2020 03:38:14 GMT  
		Size: 2.3 MB (2334752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6cd7e79bb8774fe6fe3d334ac5330373c01c6a724cb68c2ed546c6f88dfa68`  
		Last Modified: Thu, 14 May 2020 03:38:22 GMT  
		Size: 22.2 MB (22231932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6131f5bfd68245934bbde33583186bf533670eb95b1544a765ecc31021649dc2`  
		Last Modified: Thu, 14 May 2020 03:38:54 GMT  
		Size: 129.1 MB (129109289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e06408fd0546dfc093d262303b90a414cde2ffaece8874b1671db130ccc3dd9`  
		Last Modified: Thu, 14 May 2020 03:38:12 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa5e51289fb972fb7920c24059a53d20043a5f62bcae6b52973cfaddb677d1b`  
		Last Modified: Thu, 14 May 2020 03:38:12 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d615828bf5968dc084f7b5b460c65fc3b176e78dfe8cc87a52abe3994d1c31fc`  
		Last Modified: Thu, 14 May 2020 03:38:12 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed0ee72de06cb96a6573e480e33e5666cfbdc7dbe46d165f35a4df36833590d`  
		Last Modified: Thu, 14 May 2020 03:38:12 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:57588e114333f6c841b8ddbdc4b1a4b43b89b2f2a8a12ba3dfefa5d1c0b3291b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:18de2d309e97833241d8ced9581eaba57a8945732bae737597571d0e5b47f2db
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.2 MB (378189168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867b6972498e9580f75e48112484f0224b02fcdc0143ff5ecc9d40614cf34089`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 13 May 2020 21:20:38 GMT
ADD file:ca8f84daab6688a5d8efa1fc57c754c162584fc99cd98a8ea357065661d6a48b in / 
# Wed, 13 May 2020 21:20:38 GMT
CMD ["bash"]
# Thu, 14 May 2020 03:26:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 14 May 2020 03:26:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 14 May 2020 03:26:33 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 03:28:01 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 14 May 2020 03:28:41 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 03:28:45 GMT
RUN npm install -g rtlcss
# Thu, 14 May 2020 03:28:46 GMT
ENV ODOO_VERSION=13.0
# Thu, 14 May 2020 03:28:46 GMT
ARG ODOO_RELEASE=20200417
# Thu, 14 May 2020 03:28:46 GMT
ARG ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
# Thu, 14 May 2020 03:30:01 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 14 May 2020 03:30:03 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 14 May 2020 03:30:03 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 14 May 2020 03:30:05 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 14 May 2020 03:30:05 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 14 May 2020 03:30:06 GMT
EXPOSE 8069 8071 8072
# Thu, 14 May 2020 03:30:06 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 14 May 2020 03:30:06 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 14 May 2020 03:30:07 GMT
USER odoo
# Thu, 14 May 2020 03:30:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 03:30:07 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:5b54d594fba7f30e90c967a80607905ba8d90ca8be45d5a4d30e69d75e65430b`  
		Last Modified: Wed, 13 May 2020 21:26:23 GMT  
		Size: 27.1 MB (27091990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4a5838eb0b52a43682a97551c8da20c7a5d02369556ea9fea830cdded0ba65`  
		Last Modified: Thu, 14 May 2020 03:38:04 GMT  
		Size: 204.1 MB (204071133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8efcae7f421df25e53aae03c98acf4eabf34dd6585b958f5328f1640466082`  
		Last Modified: Thu, 14 May 2020 03:37:19 GMT  
		Size: 2.3 MB (2333721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a995bb2082d35f3e74ed426089e00d4274c0f27edb3e0b2fde27cd3fee5f2d`  
		Last Modified: Thu, 14 May 2020 03:37:17 GMT  
		Size: 1.1 MB (1094713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c89c824ff96dda2737e33ba1189125c9c49c77b94b43d02dffd647e0e77ce2`  
		Last Modified: Thu, 14 May 2020 03:38:07 GMT  
		Size: 143.6 MB (143595208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be03406a69f033c4a70da5070fe1bebb6291c56d8a5983ef9864081dd17b39bc`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09833da04009f48c570fe96f4b29f910928ef8f07bf1a6f9d9f6618b349576ea`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604cbf2c646040ddb0281ebb1816820a17b1c69197b1816d3d5d087180dcf7c6`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840040811a64b0370acb71c13302ff380d3b203ae59ae21aa6a045219c344687`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:57588e114333f6c841b8ddbdc4b1a4b43b89b2f2a8a12ba3dfefa5d1c0b3291b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:18de2d309e97833241d8ced9581eaba57a8945732bae737597571d0e5b47f2db
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.2 MB (378189168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867b6972498e9580f75e48112484f0224b02fcdc0143ff5ecc9d40614cf34089`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 13 May 2020 21:20:38 GMT
ADD file:ca8f84daab6688a5d8efa1fc57c754c162584fc99cd98a8ea357065661d6a48b in / 
# Wed, 13 May 2020 21:20:38 GMT
CMD ["bash"]
# Thu, 14 May 2020 03:26:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 14 May 2020 03:26:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 14 May 2020 03:26:33 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 03:28:01 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 14 May 2020 03:28:41 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 03:28:45 GMT
RUN npm install -g rtlcss
# Thu, 14 May 2020 03:28:46 GMT
ENV ODOO_VERSION=13.0
# Thu, 14 May 2020 03:28:46 GMT
ARG ODOO_RELEASE=20200417
# Thu, 14 May 2020 03:28:46 GMT
ARG ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
# Thu, 14 May 2020 03:30:01 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 14 May 2020 03:30:03 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 14 May 2020 03:30:03 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 14 May 2020 03:30:05 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 14 May 2020 03:30:05 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 14 May 2020 03:30:06 GMT
EXPOSE 8069 8071 8072
# Thu, 14 May 2020 03:30:06 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 14 May 2020 03:30:06 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 14 May 2020 03:30:07 GMT
USER odoo
# Thu, 14 May 2020 03:30:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 03:30:07 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:5b54d594fba7f30e90c967a80607905ba8d90ca8be45d5a4d30e69d75e65430b`  
		Last Modified: Wed, 13 May 2020 21:26:23 GMT  
		Size: 27.1 MB (27091990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4a5838eb0b52a43682a97551c8da20c7a5d02369556ea9fea830cdded0ba65`  
		Last Modified: Thu, 14 May 2020 03:38:04 GMT  
		Size: 204.1 MB (204071133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8efcae7f421df25e53aae03c98acf4eabf34dd6585b958f5328f1640466082`  
		Last Modified: Thu, 14 May 2020 03:37:19 GMT  
		Size: 2.3 MB (2333721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a995bb2082d35f3e74ed426089e00d4274c0f27edb3e0b2fde27cd3fee5f2d`  
		Last Modified: Thu, 14 May 2020 03:37:17 GMT  
		Size: 1.1 MB (1094713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c89c824ff96dda2737e33ba1189125c9c49c77b94b43d02dffd647e0e77ce2`  
		Last Modified: Thu, 14 May 2020 03:38:07 GMT  
		Size: 143.6 MB (143595208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be03406a69f033c4a70da5070fe1bebb6291c56d8a5983ef9864081dd17b39bc`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09833da04009f48c570fe96f4b29f910928ef8f07bf1a6f9d9f6618b349576ea`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604cbf2c646040ddb0281ebb1816820a17b1c69197b1816d3d5d087180dcf7c6`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840040811a64b0370acb71c13302ff380d3b203ae59ae21aa6a045219c344687`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:57588e114333f6c841b8ddbdc4b1a4b43b89b2f2a8a12ba3dfefa5d1c0b3291b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:18de2d309e97833241d8ced9581eaba57a8945732bae737597571d0e5b47f2db
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.2 MB (378189168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867b6972498e9580f75e48112484f0224b02fcdc0143ff5ecc9d40614cf34089`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 13 May 2020 21:20:38 GMT
ADD file:ca8f84daab6688a5d8efa1fc57c754c162584fc99cd98a8ea357065661d6a48b in / 
# Wed, 13 May 2020 21:20:38 GMT
CMD ["bash"]
# Thu, 14 May 2020 03:26:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 14 May 2020 03:26:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 14 May 2020 03:26:33 GMT
ENV LANG=C.UTF-8
# Thu, 14 May 2020 03:28:01 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 14 May 2020 03:28:41 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 03:28:45 GMT
RUN npm install -g rtlcss
# Thu, 14 May 2020 03:28:46 GMT
ENV ODOO_VERSION=13.0
# Thu, 14 May 2020 03:28:46 GMT
ARG ODOO_RELEASE=20200417
# Thu, 14 May 2020 03:28:46 GMT
ARG ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
# Thu, 14 May 2020 03:30:01 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 14 May 2020 03:30:03 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 14 May 2020 03:30:03 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 14 May 2020 03:30:05 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 14 May 2020 03:30:05 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 14 May 2020 03:30:06 GMT
EXPOSE 8069 8071 8072
# Thu, 14 May 2020 03:30:06 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 14 May 2020 03:30:06 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 14 May 2020 03:30:07 GMT
USER odoo
# Thu, 14 May 2020 03:30:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 03:30:07 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:5b54d594fba7f30e90c967a80607905ba8d90ca8be45d5a4d30e69d75e65430b`  
		Last Modified: Wed, 13 May 2020 21:26:23 GMT  
		Size: 27.1 MB (27091990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4a5838eb0b52a43682a97551c8da20c7a5d02369556ea9fea830cdded0ba65`  
		Last Modified: Thu, 14 May 2020 03:38:04 GMT  
		Size: 204.1 MB (204071133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8efcae7f421df25e53aae03c98acf4eabf34dd6585b958f5328f1640466082`  
		Last Modified: Thu, 14 May 2020 03:37:19 GMT  
		Size: 2.3 MB (2333721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a995bb2082d35f3e74ed426089e00d4274c0f27edb3e0b2fde27cd3fee5f2d`  
		Last Modified: Thu, 14 May 2020 03:37:17 GMT  
		Size: 1.1 MB (1094713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c89c824ff96dda2737e33ba1189125c9c49c77b94b43d02dffd647e0e77ce2`  
		Last Modified: Thu, 14 May 2020 03:38:07 GMT  
		Size: 143.6 MB (143595208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be03406a69f033c4a70da5070fe1bebb6291c56d8a5983ef9864081dd17b39bc`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09833da04009f48c570fe96f4b29f910928ef8f07bf1a6f9d9f6618b349576ea`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604cbf2c646040ddb0281ebb1816820a17b1c69197b1816d3d5d087180dcf7c6`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840040811a64b0370acb71c13302ff380d3b203ae59ae21aa6a045219c344687`  
		Last Modified: Thu, 14 May 2020 03:37:16 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
