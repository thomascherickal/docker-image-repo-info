<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `odoo`

-	[`odoo:12`](#odoo12)
-	[`odoo:12.0`](#odoo120)
-	[`odoo:13`](#odoo13)
-	[`odoo:13.0`](#odoo130)
-	[`odoo:14`](#odoo14)
-	[`odoo:14.0`](#odoo140)
-	[`odoo:latest`](#odoolatest)

## `odoo:12`

```console
$ docker pull odoo@sha256:4ca06347b60c7bac47107050978a878ce398985c71a86f8e6a6ea058dac7c6b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:5c33da740c26838e4bda72b44f093cc96418b903a0299587e3e7768b44a74229
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538428471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53147c285847ac81a240f7ed49965ac14d0ca93d833a21891beeea78f72b9c3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:46 GMT
ADD file:b8ae56829d548d5bff373622e23d0352bb9d313f09d8fea76dc1892b16c768c8 in / 
# Fri, 03 Sep 2021 01:23:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:21:41 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 03 Sep 2021 08:21:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 03 Sep 2021 08:21:42 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:21:43 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Fri, 03 Sep 2021 08:23:12 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 03 Sep 2021 08:24:43 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:25:00 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:25:01 GMT
ENV ODOO_VERSION=12.0
# Mon, 13 Sep 2021 18:29:04 GMT
ARG ODOO_RELEASE=20210913
# Mon, 13 Sep 2021 18:29:04 GMT
ARG ODOO_SHA=04d2f6d6ebc176cadd51873518966d2781c340b6
# Mon, 13 Sep 2021 18:30:07 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=04d2f6d6ebc176cadd51873518966d2781c340b6
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Sep 2021 18:30:10 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Sep 2021 18:30:10 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Sep 2021 18:30:11 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=04d2f6d6ebc176cadd51873518966d2781c340b6
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Sep 2021 18:30:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Sep 2021 18:30:11 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Sep 2021 18:30:11 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Sep 2021 18:30:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Sep 2021 18:30:12 GMT
USER odoo
# Mon, 13 Sep 2021 18:30:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Sep 2021 18:30:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:442547fc262c2ebd1e2d44ea04cb011b78ec62cc2314c8c71c68ba31ae002cdb`  
		Last Modified: Fri, 03 Sep 2021 01:32:07 GMT  
		Size: 22.5 MB (22527429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ef1fc36ce9f3859bf889c86d8cd74979ed71ae7106adb1aad7d64adb740273`  
		Last Modified: Fri, 03 Sep 2021 08:29:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff2c6c124745ce3574461d76e169045d3084e09b9c4f9a596b17659b03b4dd2`  
		Last Modified: Fri, 03 Sep 2021 08:29:29 GMT  
		Size: 219.7 MB (219657617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dde6f436aefae775b74932ee4deb96d884f715e70db318fa94b046d3080086`  
		Last Modified: Fri, 03 Sep 2021 08:29:02 GMT  
		Size: 2.2 MB (2227388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6736d7cb64ee6e1a364dcddaedf7d1e246cbf2e7cd24b3fa9c63f244fbc1b5`  
		Last Modified: Fri, 03 Sep 2021 08:29:07 GMT  
		Size: 22.0 MB (22030059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3446258906f9d0c23a595dbf3d0b307394f59944540c80ca452977e3c2124d6`  
		Last Modified: Mon, 13 Sep 2021 18:32:21 GMT  
		Size: 272.0 MB (271983286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2f51fd046ed89bc29504a79107d8976421b793e22babedb0fec1987d17d1fe`  
		Last Modified: Mon, 13 Sep 2021 18:31:56 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b0a6b17979c9e32af1c6165d2b9025911b616dab43277e2a005d46a91ce6c0`  
		Last Modified: Mon, 13 Sep 2021 18:31:55 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa349068560663eed6ae22759d95aa55a2133b138f720f6d68e4d560898ef725`  
		Last Modified: Mon, 13 Sep 2021 18:31:55 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0c17fe3eb00b762fc2e8394c1ce0f3b6efe00b49a142c6766b28c0e4121397`  
		Last Modified: Mon, 13 Sep 2021 18:31:55 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:4ca06347b60c7bac47107050978a878ce398985c71a86f8e6a6ea058dac7c6b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:5c33da740c26838e4bda72b44f093cc96418b903a0299587e3e7768b44a74229
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538428471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53147c285847ac81a240f7ed49965ac14d0ca93d833a21891beeea78f72b9c3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:46 GMT
ADD file:b8ae56829d548d5bff373622e23d0352bb9d313f09d8fea76dc1892b16c768c8 in / 
# Fri, 03 Sep 2021 01:23:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:21:41 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 03 Sep 2021 08:21:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 03 Sep 2021 08:21:42 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:21:43 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Fri, 03 Sep 2021 08:23:12 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 03 Sep 2021 08:24:43 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:25:00 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:25:01 GMT
ENV ODOO_VERSION=12.0
# Mon, 13 Sep 2021 18:29:04 GMT
ARG ODOO_RELEASE=20210913
# Mon, 13 Sep 2021 18:29:04 GMT
ARG ODOO_SHA=04d2f6d6ebc176cadd51873518966d2781c340b6
# Mon, 13 Sep 2021 18:30:07 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=04d2f6d6ebc176cadd51873518966d2781c340b6
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Sep 2021 18:30:10 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Sep 2021 18:30:10 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Sep 2021 18:30:11 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=04d2f6d6ebc176cadd51873518966d2781c340b6
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Sep 2021 18:30:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Sep 2021 18:30:11 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Sep 2021 18:30:11 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Sep 2021 18:30:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Sep 2021 18:30:12 GMT
USER odoo
# Mon, 13 Sep 2021 18:30:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Sep 2021 18:30:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:442547fc262c2ebd1e2d44ea04cb011b78ec62cc2314c8c71c68ba31ae002cdb`  
		Last Modified: Fri, 03 Sep 2021 01:32:07 GMT  
		Size: 22.5 MB (22527429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ef1fc36ce9f3859bf889c86d8cd74979ed71ae7106adb1aad7d64adb740273`  
		Last Modified: Fri, 03 Sep 2021 08:29:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff2c6c124745ce3574461d76e169045d3084e09b9c4f9a596b17659b03b4dd2`  
		Last Modified: Fri, 03 Sep 2021 08:29:29 GMT  
		Size: 219.7 MB (219657617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4dde6f436aefae775b74932ee4deb96d884f715e70db318fa94b046d3080086`  
		Last Modified: Fri, 03 Sep 2021 08:29:02 GMT  
		Size: 2.2 MB (2227388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6736d7cb64ee6e1a364dcddaedf7d1e246cbf2e7cd24b3fa9c63f244fbc1b5`  
		Last Modified: Fri, 03 Sep 2021 08:29:07 GMT  
		Size: 22.0 MB (22030059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3446258906f9d0c23a595dbf3d0b307394f59944540c80ca452977e3c2124d6`  
		Last Modified: Mon, 13 Sep 2021 18:32:21 GMT  
		Size: 272.0 MB (271983286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2f51fd046ed89bc29504a79107d8976421b793e22babedb0fec1987d17d1fe`  
		Last Modified: Mon, 13 Sep 2021 18:31:56 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b0a6b17979c9e32af1c6165d2b9025911b616dab43277e2a005d46a91ce6c0`  
		Last Modified: Mon, 13 Sep 2021 18:31:55 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa349068560663eed6ae22759d95aa55a2133b138f720f6d68e4d560898ef725`  
		Last Modified: Mon, 13 Sep 2021 18:31:55 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0c17fe3eb00b762fc2e8394c1ce0f3b6efe00b49a142c6766b28c0e4121397`  
		Last Modified: Mon, 13 Sep 2021 18:31:55 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:415a6f13562289e9c9012a31b535820f548bf9860a511cde04e8706db7cb08d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:ae077bf1d63c5d7a992b8f40282886a2da3342a2e27bce70aab04dbf422de70c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.4 MB (528405919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb2710a3749f53a556b5768854ea877d37eacc993692279ff0af22d1e23cc126`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:14:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 03 Sep 2021 08:14:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 03 Sep 2021 08:14:49 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:19:29 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 03 Sep 2021 08:19:42 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:19:47 GMT
RUN npm install -g rtlcss
# Fri, 03 Sep 2021 08:19:48 GMT
ENV ODOO_VERSION=13.0
# Mon, 13 Sep 2021 18:27:38 GMT
ARG ODOO_RELEASE=20210913
# Mon, 13 Sep 2021 18:27:38 GMT
ARG ODOO_SHA=2d7fd9bfe044fd7513d82a8ce5c1ee6b08498468
# Mon, 13 Sep 2021 18:28:45 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=2d7fd9bfe044fd7513d82a8ce5c1ee6b08498468
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Sep 2021 18:28:49 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Sep 2021 18:28:49 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Sep 2021 18:28:50 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=2d7fd9bfe044fd7513d82a8ce5c1ee6b08498468
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Sep 2021 18:28:50 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Sep 2021 18:28:50 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Sep 2021 18:28:50 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Sep 2021 18:28:51 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Sep 2021 18:28:51 GMT
USER odoo
# Mon, 13 Sep 2021 18:28:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Sep 2021 18:28:51 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f62eaaa3a419466e2cd8478b7344c1acd06a6095fb959f5981431356166c72`  
		Last Modified: Fri, 03 Sep 2021 08:28:43 GMT  
		Size: 207.1 MB (207129591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564b1b987da5a51f9753c4e9903495b0b9cb9d58f79cf0e7ff747938a4237a5`  
		Last Modified: Fri, 03 Sep 2021 08:28:15 GMT  
		Size: 2.3 MB (2347919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f6c8a96ec08781ed03569e5dc126ee49838d7d7891d7606e9aa97091348ad6`  
		Last Modified: Fri, 03 Sep 2021 08:28:14 GMT  
		Size: 893.4 KB (893373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e0169b70e4414bca2518044862a9d8406d3132f475ef5ecc9848f23db3efa6`  
		Last Modified: Mon, 13 Sep 2021 18:31:44 GMT  
		Size: 290.9 MB (290886732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bc5bf176a644018ae521c70fa329e0b5b0a35510f69e6c75a895a96c0f9643`  
		Last Modified: Mon, 13 Sep 2021 18:31:14 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb369e8a2e03da181b7f5e59cbb41b47b3acc0a892c3d84079abffa5b2e825de`  
		Last Modified: Mon, 13 Sep 2021 18:31:14 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4240148eb0031a1c7c7ae6e8111e31cfbbec480b9a59445c3dfd7bda4e2a85bf`  
		Last Modified: Mon, 13 Sep 2021 18:31:14 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90dd9e98125639b9635e8863ca738ea16a99757bc5e10e240332b49b95f4fe0c`  
		Last Modified: Mon, 13 Sep 2021 18:31:15 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:415a6f13562289e9c9012a31b535820f548bf9860a511cde04e8706db7cb08d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:ae077bf1d63c5d7a992b8f40282886a2da3342a2e27bce70aab04dbf422de70c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.4 MB (528405919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb2710a3749f53a556b5768854ea877d37eacc993692279ff0af22d1e23cc126`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:14:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 03 Sep 2021 08:14:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 03 Sep 2021 08:14:49 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:19:29 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 03 Sep 2021 08:19:42 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:19:47 GMT
RUN npm install -g rtlcss
# Fri, 03 Sep 2021 08:19:48 GMT
ENV ODOO_VERSION=13.0
# Mon, 13 Sep 2021 18:27:38 GMT
ARG ODOO_RELEASE=20210913
# Mon, 13 Sep 2021 18:27:38 GMT
ARG ODOO_SHA=2d7fd9bfe044fd7513d82a8ce5c1ee6b08498468
# Mon, 13 Sep 2021 18:28:45 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=2d7fd9bfe044fd7513d82a8ce5c1ee6b08498468
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Sep 2021 18:28:49 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Sep 2021 18:28:49 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Sep 2021 18:28:50 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=2d7fd9bfe044fd7513d82a8ce5c1ee6b08498468
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Sep 2021 18:28:50 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Sep 2021 18:28:50 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Sep 2021 18:28:50 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Sep 2021 18:28:51 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Sep 2021 18:28:51 GMT
USER odoo
# Mon, 13 Sep 2021 18:28:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Sep 2021 18:28:51 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f62eaaa3a419466e2cd8478b7344c1acd06a6095fb959f5981431356166c72`  
		Last Modified: Fri, 03 Sep 2021 08:28:43 GMT  
		Size: 207.1 MB (207129591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564b1b987da5a51f9753c4e9903495b0b9cb9d58f79cf0e7ff747938a4237a5`  
		Last Modified: Fri, 03 Sep 2021 08:28:15 GMT  
		Size: 2.3 MB (2347919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f6c8a96ec08781ed03569e5dc126ee49838d7d7891d7606e9aa97091348ad6`  
		Last Modified: Fri, 03 Sep 2021 08:28:14 GMT  
		Size: 893.4 KB (893373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e0169b70e4414bca2518044862a9d8406d3132f475ef5ecc9848f23db3efa6`  
		Last Modified: Mon, 13 Sep 2021 18:31:44 GMT  
		Size: 290.9 MB (290886732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bc5bf176a644018ae521c70fa329e0b5b0a35510f69e6c75a895a96c0f9643`  
		Last Modified: Mon, 13 Sep 2021 18:31:14 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb369e8a2e03da181b7f5e59cbb41b47b3acc0a892c3d84079abffa5b2e825de`  
		Last Modified: Mon, 13 Sep 2021 18:31:14 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4240148eb0031a1c7c7ae6e8111e31cfbbec480b9a59445c3dfd7bda4e2a85bf`  
		Last Modified: Mon, 13 Sep 2021 18:31:14 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90dd9e98125639b9635e8863ca738ea16a99757bc5e10e240332b49b95f4fe0c`  
		Last Modified: Mon, 13 Sep 2021 18:31:15 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:b06f421aecb7cbcf1e6a60eb4c72a90c9cea7af25adc07b2fbee2a109b195939
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:fa14bbcd37e6a9b96715261d7e53c659f741adb8139bbed550b8e9a9b2ed054b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **517.1 MB (517075146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe9154a0461253d629e5797bc8d155c8b76a2617b8262bded7f0e2a880d431bf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:14:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 03 Sep 2021 08:14:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 03 Sep 2021 08:14:49 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:15:56 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 03 Sep 2021 08:16:09 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:16:12 GMT
RUN npm install -g rtlcss
# Fri, 03 Sep 2021 08:16:13 GMT
ENV ODOO_VERSION=14.0
# Mon, 13 Sep 2021 18:26:13 GMT
ARG ODOO_RELEASE=20210913
# Mon, 13 Sep 2021 18:26:13 GMT
ARG ODOO_SHA=fcd89fb35456b365368d6400d33664d996e6be4c
# Mon, 13 Sep 2021 18:27:19 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=fcd89fb35456b365368d6400d33664d996e6be4c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Sep 2021 18:27:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Sep 2021 18:27:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Sep 2021 18:27:24 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=fcd89fb35456b365368d6400d33664d996e6be4c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Sep 2021 18:27:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Sep 2021 18:27:24 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Sep 2021 18:27:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Sep 2021 18:27:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Sep 2021 18:27:24 GMT
USER odoo
# Mon, 13 Sep 2021 18:27:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Sep 2021 18:27:25 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747cf09456121867c9a11a2b2e1b877b80dd32b1ffe451e88685f790bd2188f6`  
		Last Modified: Fri, 03 Sep 2021 08:27:50 GMT  
		Size: 213.2 MB (213172901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51c6b9c93241bd96d38967891f77680616b4df0ad6f2255bf7b4e375736d481`  
		Last Modified: Fri, 03 Sep 2021 08:27:14 GMT  
		Size: 2.4 MB (2350482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644c7d878f88578d6d5aa3edcc8f5f864b3568da52f0cbd89f566950d57bc9c8`  
		Last Modified: Fri, 03 Sep 2021 08:27:13 GMT  
		Size: 893.3 KB (893252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872f8ed1a2e2f8c4a7effa367ad251a380b9d79ca6d3246ae700ca0d2c7eec30`  
		Last Modified: Mon, 13 Sep 2021 18:30:56 GMT  
		Size: 273.5 MB (273510207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8ec17cc775dc69aa8d310942318aa0e6dbb3b611568c8286e543138d24229`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ed770a05c36a592806199c5619385b4b879549e18761f31eda0f048a629624`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9aefa3fa6b6bb4e758a44a991487ccfc7e4e53f58b8d67179d22728317c730e`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecec78a560284f3a35100b9d2727ab1420190b359058e30fe720f5be7e427fa8`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:b06f421aecb7cbcf1e6a60eb4c72a90c9cea7af25adc07b2fbee2a109b195939
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:fa14bbcd37e6a9b96715261d7e53c659f741adb8139bbed550b8e9a9b2ed054b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **517.1 MB (517075146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe9154a0461253d629e5797bc8d155c8b76a2617b8262bded7f0e2a880d431bf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:14:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 03 Sep 2021 08:14:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 03 Sep 2021 08:14:49 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:15:56 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 03 Sep 2021 08:16:09 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:16:12 GMT
RUN npm install -g rtlcss
# Fri, 03 Sep 2021 08:16:13 GMT
ENV ODOO_VERSION=14.0
# Mon, 13 Sep 2021 18:26:13 GMT
ARG ODOO_RELEASE=20210913
# Mon, 13 Sep 2021 18:26:13 GMT
ARG ODOO_SHA=fcd89fb35456b365368d6400d33664d996e6be4c
# Mon, 13 Sep 2021 18:27:19 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=fcd89fb35456b365368d6400d33664d996e6be4c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Sep 2021 18:27:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Sep 2021 18:27:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Sep 2021 18:27:24 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=fcd89fb35456b365368d6400d33664d996e6be4c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Sep 2021 18:27:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Sep 2021 18:27:24 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Sep 2021 18:27:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Sep 2021 18:27:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Sep 2021 18:27:24 GMT
USER odoo
# Mon, 13 Sep 2021 18:27:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Sep 2021 18:27:25 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747cf09456121867c9a11a2b2e1b877b80dd32b1ffe451e88685f790bd2188f6`  
		Last Modified: Fri, 03 Sep 2021 08:27:50 GMT  
		Size: 213.2 MB (213172901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51c6b9c93241bd96d38967891f77680616b4df0ad6f2255bf7b4e375736d481`  
		Last Modified: Fri, 03 Sep 2021 08:27:14 GMT  
		Size: 2.4 MB (2350482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644c7d878f88578d6d5aa3edcc8f5f864b3568da52f0cbd89f566950d57bc9c8`  
		Last Modified: Fri, 03 Sep 2021 08:27:13 GMT  
		Size: 893.3 KB (893252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872f8ed1a2e2f8c4a7effa367ad251a380b9d79ca6d3246ae700ca0d2c7eec30`  
		Last Modified: Mon, 13 Sep 2021 18:30:56 GMT  
		Size: 273.5 MB (273510207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8ec17cc775dc69aa8d310942318aa0e6dbb3b611568c8286e543138d24229`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ed770a05c36a592806199c5619385b4b879549e18761f31eda0f048a629624`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9aefa3fa6b6bb4e758a44a991487ccfc7e4e53f58b8d67179d22728317c730e`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecec78a560284f3a35100b9d2727ab1420190b359058e30fe720f5be7e427fa8`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:b06f421aecb7cbcf1e6a60eb4c72a90c9cea7af25adc07b2fbee2a109b195939
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:fa14bbcd37e6a9b96715261d7e53c659f741adb8139bbed550b8e9a9b2ed054b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **517.1 MB (517075146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe9154a0461253d629e5797bc8d155c8b76a2617b8262bded7f0e2a880d431bf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:14:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 03 Sep 2021 08:14:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 03 Sep 2021 08:14:49 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:15:56 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 03 Sep 2021 08:16:09 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:16:12 GMT
RUN npm install -g rtlcss
# Fri, 03 Sep 2021 08:16:13 GMT
ENV ODOO_VERSION=14.0
# Mon, 13 Sep 2021 18:26:13 GMT
ARG ODOO_RELEASE=20210913
# Mon, 13 Sep 2021 18:26:13 GMT
ARG ODOO_SHA=fcd89fb35456b365368d6400d33664d996e6be4c
# Mon, 13 Sep 2021 18:27:19 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=fcd89fb35456b365368d6400d33664d996e6be4c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 13 Sep 2021 18:27:22 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 13 Sep 2021 18:27:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 13 Sep 2021 18:27:24 GMT
# ARGS: ODOO_RELEASE=20210913 ODOO_SHA=fcd89fb35456b365368d6400d33664d996e6be4c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 13 Sep 2021 18:27:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 13 Sep 2021 18:27:24 GMT
EXPOSE 8069 8071 8072
# Mon, 13 Sep 2021 18:27:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 13 Sep 2021 18:27:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 13 Sep 2021 18:27:24 GMT
USER odoo
# Mon, 13 Sep 2021 18:27:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Sep 2021 18:27:25 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747cf09456121867c9a11a2b2e1b877b80dd32b1ffe451e88685f790bd2188f6`  
		Last Modified: Fri, 03 Sep 2021 08:27:50 GMT  
		Size: 213.2 MB (213172901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51c6b9c93241bd96d38967891f77680616b4df0ad6f2255bf7b4e375736d481`  
		Last Modified: Fri, 03 Sep 2021 08:27:14 GMT  
		Size: 2.4 MB (2350482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644c7d878f88578d6d5aa3edcc8f5f864b3568da52f0cbd89f566950d57bc9c8`  
		Last Modified: Fri, 03 Sep 2021 08:27:13 GMT  
		Size: 893.3 KB (893252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872f8ed1a2e2f8c4a7effa367ad251a380b9d79ca6d3246ae700ca0d2c7eec30`  
		Last Modified: Mon, 13 Sep 2021 18:30:56 GMT  
		Size: 273.5 MB (273510207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8ec17cc775dc69aa8d310942318aa0e6dbb3b611568c8286e543138d24229`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ed770a05c36a592806199c5619385b4b879549e18761f31eda0f048a629624`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9aefa3fa6b6bb4e758a44a991487ccfc7e4e53f58b8d67179d22728317c730e`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecec78a560284f3a35100b9d2727ab1420190b359058e30fe720f5be7e427fa8`  
		Last Modified: Mon, 13 Sep 2021 18:30:26 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
