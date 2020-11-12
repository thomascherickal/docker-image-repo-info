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
$ docker pull odoo@sha256:3b38b8a7f712e4bbc7344de93abb7a60c688f09eafafd8a4b02c6f8321898dbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:c9bf309937f0d2fb0e60288a566c6cf1deb3db960332a64115b7c18fa506a954
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.9 MB (396857727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d0953919b1c73a9b3dfd5ebb6f79dd193527d8b0435bc6359269b7f8cd986d6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 17:55:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Oct 2020 17:55:34 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Oct 2020 17:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 17:55:36 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 13 Oct 2020 17:57:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 13 Oct 2020 17:58:05 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 17:58:19 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 17:58:19 GMT
ENV ODOO_VERSION=12.0
# Thu, 12 Nov 2020 19:24:20 GMT
ARG ODOO_RELEASE=20201112
# Thu, 12 Nov 2020 19:24:20 GMT
ARG ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
# Thu, 12 Nov 2020 19:25:08 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Nov 2020 19:25:09 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 12 Nov 2020 19:25:09 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Nov 2020 19:25:10 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Nov 2020 19:25:10 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Nov 2020 19:25:11 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Nov 2020 19:25:11 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Nov 2020 19:25:11 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Nov 2020 19:25:11 GMT
USER odoo
# Thu, 12 Nov 2020 19:25:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Nov 2020 19:25:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7e899471950fb23135e6e3ba4bf5e7d333956a9c8fefef201edb318f76ce8a`  
		Last Modified: Tue, 13 Oct 2020 18:03:25 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469473cc24d8d8f285e28db154936eb275da7e3a962ebb2fb2f6008212d92a36`  
		Last Modified: Tue, 13 Oct 2020 18:04:13 GMT  
		Size: 219.6 MB (219609741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c32bdce53191bc591f6a2ef86c27ad27c001afe93d12b1b168c7a49d0c8cf79`  
		Last Modified: Tue, 13 Oct 2020 18:03:26 GMT  
		Size: 2.4 MB (2430770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd870da114a745cbea66677bec90b500570bdfbd3c22ad988b098c8fb150963f`  
		Last Modified: Tue, 13 Oct 2020 18:03:31 GMT  
		Size: 22.3 MB (22262444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b173f4dbb219d5a4978aec0657b9d4ef380e4309d34c9df347ee6c3b6558bbe`  
		Last Modified: Thu, 12 Nov 2020 19:27:11 GMT  
		Size: 130.0 MB (130030041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731f7d6eff2bba16fa0b61b4d2de54e3e3de8475d9999f76d3f688ce37afdf27`  
		Last Modified: Thu, 12 Nov 2020 19:26:44 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b026c7ef0bdd45d9d7597fc4d718414b60b00826c9b0719c65408cc97e948e54`  
		Last Modified: Thu, 12 Nov 2020 19:26:45 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba281356d890b43a295f2a2cb103a6debb39577dbe973a5e40aca50c280224ed`  
		Last Modified: Thu, 12 Nov 2020 19:26:44 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd511ddf87b16c9c490fdd70a8f1854c35c420c50f4e58ca67977ec2ffb87cb`  
		Last Modified: Thu, 12 Nov 2020 19:26:44 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:3b38b8a7f712e4bbc7344de93abb7a60c688f09eafafd8a4b02c6f8321898dbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:c9bf309937f0d2fb0e60288a566c6cf1deb3db960332a64115b7c18fa506a954
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.9 MB (396857727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d0953919b1c73a9b3dfd5ebb6f79dd193527d8b0435bc6359269b7f8cd986d6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 17:55:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Oct 2020 17:55:34 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Oct 2020 17:55:34 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 17:55:36 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 13 Oct 2020 17:57:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 13 Oct 2020 17:58:05 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 17:58:19 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 17:58:19 GMT
ENV ODOO_VERSION=12.0
# Thu, 12 Nov 2020 19:24:20 GMT
ARG ODOO_RELEASE=20201112
# Thu, 12 Nov 2020 19:24:20 GMT
ARG ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
# Thu, 12 Nov 2020 19:25:08 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Nov 2020 19:25:09 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 12 Nov 2020 19:25:09 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Nov 2020 19:25:10 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Nov 2020 19:25:10 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Nov 2020 19:25:11 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Nov 2020 19:25:11 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Nov 2020 19:25:11 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Nov 2020 19:25:11 GMT
USER odoo
# Thu, 12 Nov 2020 19:25:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Nov 2020 19:25:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7e899471950fb23135e6e3ba4bf5e7d333956a9c8fefef201edb318f76ce8a`  
		Last Modified: Tue, 13 Oct 2020 18:03:25 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469473cc24d8d8f285e28db154936eb275da7e3a962ebb2fb2f6008212d92a36`  
		Last Modified: Tue, 13 Oct 2020 18:04:13 GMT  
		Size: 219.6 MB (219609741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c32bdce53191bc591f6a2ef86c27ad27c001afe93d12b1b168c7a49d0c8cf79`  
		Last Modified: Tue, 13 Oct 2020 18:03:26 GMT  
		Size: 2.4 MB (2430770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd870da114a745cbea66677bec90b500570bdfbd3c22ad988b098c8fb150963f`  
		Last Modified: Tue, 13 Oct 2020 18:03:31 GMT  
		Size: 22.3 MB (22262444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b173f4dbb219d5a4978aec0657b9d4ef380e4309d34c9df347ee6c3b6558bbe`  
		Last Modified: Thu, 12 Nov 2020 19:27:11 GMT  
		Size: 130.0 MB (130030041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731f7d6eff2bba16fa0b61b4d2de54e3e3de8475d9999f76d3f688ce37afdf27`  
		Last Modified: Thu, 12 Nov 2020 19:26:44 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b026c7ef0bdd45d9d7597fc4d718414b60b00826c9b0719c65408cc97e948e54`  
		Last Modified: Thu, 12 Nov 2020 19:26:45 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba281356d890b43a295f2a2cb103a6debb39577dbe973a5e40aca50c280224ed`  
		Last Modified: Thu, 12 Nov 2020 19:26:44 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd511ddf87b16c9c490fdd70a8f1854c35c420c50f4e58ca67977ec2ffb87cb`  
		Last Modified: Thu, 12 Nov 2020 19:26:44 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:633a65ff9ee0278d8927de36c9f2f299432d7e4938cee86f030e8ef89ba1828e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:65fc8fac1d97e7bc9dcf08d5181bc22bce699c5f5dd68c69e98c64180eb29ac4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7853ec6f5d1abd01f3289d096725f68a402351ae7d2ce24ff75c8618df555945`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 17:49:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Oct 2020 17:49:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Oct 2020 17:49:11 GMT
ENV LANG=C.UTF-8
# Mon, 26 Oct 2020 17:47:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 26 Oct 2020 17:48:07 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Mon, 26 Oct 2020 17:48:12 GMT
RUN npm install -g rtlcss
# Mon, 26 Oct 2020 17:48:12 GMT
ENV ODOO_VERSION=13.0
# Thu, 12 Nov 2020 19:23:15 GMT
ARG ODOO_RELEASE=20201112
# Thu, 12 Nov 2020 19:23:15 GMT
ARG ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
# Thu, 12 Nov 2020 19:24:08 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Nov 2020 19:24:09 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 12 Nov 2020 19:24:10 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Nov 2020 19:24:11 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Nov 2020 19:24:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Nov 2020 19:24:11 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Nov 2020 19:24:11 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Nov 2020 19:24:11 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Nov 2020 19:24:11 GMT
USER odoo
# Thu, 12 Nov 2020 19:24:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Nov 2020 19:24:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086dfd04ee4f09e3759168af225fb6366b6e33e604235abf1da4e3aea207c9d8`  
		Last Modified: Mon, 26 Oct 2020 17:52:13 GMT  
		Size: 207.1 MB (207077082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab0ca83605acca7d829847eac227f94f377dab01aae73e84e2a3496b2ea03f9`  
		Last Modified: Mon, 26 Oct 2020 17:51:36 GMT  
		Size: 2.4 MB (2432974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4997f88b88be6c179a0d473e2f0e9d90ee165e3a84cc19f956c383f31eb8e7b9`  
		Last Modified: Mon, 26 Oct 2020 17:51:35 GMT  
		Size: 1.1 MB (1118722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a111ce48f1cb58f0a1bbaebb4b706db28db58102f1483b3d92d7e6b49c4e4e90`  
		Last Modified: Thu, 12 Nov 2020 19:26:37 GMT  
		Size: 148.4 MB (148420263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d0a1305fc45ae54b7800653dd3466e963866c120fa69ae7c9eb4fcc0d6e1c5`  
		Last Modified: Thu, 12 Nov 2020 19:26:09 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d982db4106225d554c67cdd60a8c137ca485aa23ca27eab2248b059f39d22090`  
		Last Modified: Thu, 12 Nov 2020 19:26:08 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecdc4d63e012da4969c0ef37399c47c5d22160305f717aa7dc7040e7a1ad411`  
		Last Modified: Thu, 12 Nov 2020 19:26:09 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1027ff163e68b597192399ff5346f33b7df1c093cfb61e0472b8c4c8689ee`  
		Last Modified: Thu, 12 Nov 2020 19:26:08 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:633a65ff9ee0278d8927de36c9f2f299432d7e4938cee86f030e8ef89ba1828e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:65fc8fac1d97e7bc9dcf08d5181bc22bce699c5f5dd68c69e98c64180eb29ac4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386143673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7853ec6f5d1abd01f3289d096725f68a402351ae7d2ce24ff75c8618df555945`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 17:49:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Oct 2020 17:49:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Oct 2020 17:49:11 GMT
ENV LANG=C.UTF-8
# Mon, 26 Oct 2020 17:47:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 26 Oct 2020 17:48:07 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Mon, 26 Oct 2020 17:48:12 GMT
RUN npm install -g rtlcss
# Mon, 26 Oct 2020 17:48:12 GMT
ENV ODOO_VERSION=13.0
# Thu, 12 Nov 2020 19:23:15 GMT
ARG ODOO_RELEASE=20201112
# Thu, 12 Nov 2020 19:23:15 GMT
ARG ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
# Thu, 12 Nov 2020 19:24:08 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Nov 2020 19:24:09 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 12 Nov 2020 19:24:10 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Nov 2020 19:24:11 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Nov 2020 19:24:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Nov 2020 19:24:11 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Nov 2020 19:24:11 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Nov 2020 19:24:11 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Nov 2020 19:24:11 GMT
USER odoo
# Thu, 12 Nov 2020 19:24:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Nov 2020 19:24:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086dfd04ee4f09e3759168af225fb6366b6e33e604235abf1da4e3aea207c9d8`  
		Last Modified: Mon, 26 Oct 2020 17:52:13 GMT  
		Size: 207.1 MB (207077082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab0ca83605acca7d829847eac227f94f377dab01aae73e84e2a3496b2ea03f9`  
		Last Modified: Mon, 26 Oct 2020 17:51:36 GMT  
		Size: 2.4 MB (2432974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4997f88b88be6c179a0d473e2f0e9d90ee165e3a84cc19f956c383f31eb8e7b9`  
		Last Modified: Mon, 26 Oct 2020 17:51:35 GMT  
		Size: 1.1 MB (1118722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a111ce48f1cb58f0a1bbaebb4b706db28db58102f1483b3d92d7e6b49c4e4e90`  
		Last Modified: Thu, 12 Nov 2020 19:26:37 GMT  
		Size: 148.4 MB (148420263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d0a1305fc45ae54b7800653dd3466e963866c120fa69ae7c9eb4fcc0d6e1c5`  
		Last Modified: Thu, 12 Nov 2020 19:26:09 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d982db4106225d554c67cdd60a8c137ca485aa23ca27eab2248b059f39d22090`  
		Last Modified: Thu, 12 Nov 2020 19:26:08 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecdc4d63e012da4969c0ef37399c47c5d22160305f717aa7dc7040e7a1ad411`  
		Last Modified: Thu, 12 Nov 2020 19:26:09 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1027ff163e68b597192399ff5346f33b7df1c093cfb61e0472b8c4c8689ee`  
		Last Modified: Thu, 12 Nov 2020 19:26:08 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:a34cf6b6fb0f96039d9c1aaadf0d3840b01700a8fba427b779b3ed36290b0849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:74b2fd8ed7e4ba6ba815a25aa08074cea518bed95d7ddf9cdb2c252951c56424
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.1 MB (402071237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa9ee392a4951c09b82024803109dd6ed8c5ff3a7754f8667da81fc76b042b68`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 17:49:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Oct 2020 17:49:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Oct 2020 17:49:11 GMT
ENV LANG=C.UTF-8
# Mon, 26 Oct 2020 17:45:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 26 Oct 2020 17:45:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Oct 2020 17:45:21 GMT
RUN npm install -g rtlcss
# Mon, 26 Oct 2020 17:45:21 GMT
ENV ODOO_VERSION=14.0
# Thu, 12 Nov 2020 19:22:09 GMT
ARG ODOO_RELEASE=20201112
# Thu, 12 Nov 2020 19:22:10 GMT
ARG ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
# Thu, 12 Nov 2020 19:22:59 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Nov 2020 19:23:00 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 12 Nov 2020 19:23:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Nov 2020 19:23:02 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Nov 2020 19:23:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Nov 2020 19:23:02 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Nov 2020 19:23:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Nov 2020 19:23:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Nov 2020 19:23:03 GMT
USER odoo
# Thu, 12 Nov 2020 19:23:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Nov 2020 19:23:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c69f32ce0e0b8c40da731c837dc4af71c91d64af3a383306b1998b87065248f`  
		Last Modified: Mon, 26 Oct 2020 17:51:27 GMT  
		Size: 213.1 MB (213119031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79914c2df80be97bf35af10e222d03a9673bdb70868542859f4ca306713ea83f`  
		Last Modified: Mon, 26 Oct 2020 17:50:46 GMT  
		Size: 2.4 MB (2435820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64083ae2108cec48181a94003bae0b8399a4a7b6471f1e2d1be462f3b80856bf`  
		Last Modified: Mon, 26 Oct 2020 17:50:45 GMT  
		Size: 1.1 MB (1118509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01edfe5d1f72ce612c1c5cc8c8fd1c632d466f9ae9a7c2b687f7dfe1a9db52bf`  
		Last Modified: Thu, 12 Nov 2020 19:26:01 GMT  
		Size: 158.3 MB (158303244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1469ce57930f123780015a29d2181ecca47034ed282d389c1c16a9b48f2a`  
		Last Modified: Thu, 12 Nov 2020 19:25:30 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c91fa07954c1f88edd13bc7da55c82ad466f6a17046cbed153cdd1193545ea9`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13f72919012cc465c0c6fbdf95426594bfe9f624ecea38f6006f33ee6b7e416`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25543eac24aeaf3949be246262ab118f76d0eb6e61fde74ab56951d58fe7383d`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:a34cf6b6fb0f96039d9c1aaadf0d3840b01700a8fba427b779b3ed36290b0849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:74b2fd8ed7e4ba6ba815a25aa08074cea518bed95d7ddf9cdb2c252951c56424
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.1 MB (402071237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa9ee392a4951c09b82024803109dd6ed8c5ff3a7754f8667da81fc76b042b68`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 17:49:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Oct 2020 17:49:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Oct 2020 17:49:11 GMT
ENV LANG=C.UTF-8
# Mon, 26 Oct 2020 17:45:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 26 Oct 2020 17:45:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Oct 2020 17:45:21 GMT
RUN npm install -g rtlcss
# Mon, 26 Oct 2020 17:45:21 GMT
ENV ODOO_VERSION=14.0
# Thu, 12 Nov 2020 19:22:09 GMT
ARG ODOO_RELEASE=20201112
# Thu, 12 Nov 2020 19:22:10 GMT
ARG ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
# Thu, 12 Nov 2020 19:22:59 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Nov 2020 19:23:00 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 12 Nov 2020 19:23:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Nov 2020 19:23:02 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Nov 2020 19:23:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Nov 2020 19:23:02 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Nov 2020 19:23:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Nov 2020 19:23:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Nov 2020 19:23:03 GMT
USER odoo
# Thu, 12 Nov 2020 19:23:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Nov 2020 19:23:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c69f32ce0e0b8c40da731c837dc4af71c91d64af3a383306b1998b87065248f`  
		Last Modified: Mon, 26 Oct 2020 17:51:27 GMT  
		Size: 213.1 MB (213119031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79914c2df80be97bf35af10e222d03a9673bdb70868542859f4ca306713ea83f`  
		Last Modified: Mon, 26 Oct 2020 17:50:46 GMT  
		Size: 2.4 MB (2435820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64083ae2108cec48181a94003bae0b8399a4a7b6471f1e2d1be462f3b80856bf`  
		Last Modified: Mon, 26 Oct 2020 17:50:45 GMT  
		Size: 1.1 MB (1118509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01edfe5d1f72ce612c1c5cc8c8fd1c632d466f9ae9a7c2b687f7dfe1a9db52bf`  
		Last Modified: Thu, 12 Nov 2020 19:26:01 GMT  
		Size: 158.3 MB (158303244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1469ce57930f123780015a29d2181ecca47034ed282d389c1c16a9b48f2a`  
		Last Modified: Thu, 12 Nov 2020 19:25:30 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c91fa07954c1f88edd13bc7da55c82ad466f6a17046cbed153cdd1193545ea9`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13f72919012cc465c0c6fbdf95426594bfe9f624ecea38f6006f33ee6b7e416`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25543eac24aeaf3949be246262ab118f76d0eb6e61fde74ab56951d58fe7383d`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:a34cf6b6fb0f96039d9c1aaadf0d3840b01700a8fba427b779b3ed36290b0849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:74b2fd8ed7e4ba6ba815a25aa08074cea518bed95d7ddf9cdb2c252951c56424
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.1 MB (402071237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa9ee392a4951c09b82024803109dd6ed8c5ff3a7754f8667da81fc76b042b68`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 17:49:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Oct 2020 17:49:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Oct 2020 17:49:11 GMT
ENV LANG=C.UTF-8
# Mon, 26 Oct 2020 17:45:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 26 Oct 2020 17:45:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Oct 2020 17:45:21 GMT
RUN npm install -g rtlcss
# Mon, 26 Oct 2020 17:45:21 GMT
ENV ODOO_VERSION=14.0
# Thu, 12 Nov 2020 19:22:09 GMT
ARG ODOO_RELEASE=20201112
# Thu, 12 Nov 2020 19:22:10 GMT
ARG ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
# Thu, 12 Nov 2020 19:22:59 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Nov 2020 19:23:00 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 12 Nov 2020 19:23:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Nov 2020 19:23:02 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Nov 2020 19:23:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Nov 2020 19:23:02 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Nov 2020 19:23:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Nov 2020 19:23:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Nov 2020 19:23:03 GMT
USER odoo
# Thu, 12 Nov 2020 19:23:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Nov 2020 19:23:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c69f32ce0e0b8c40da731c837dc4af71c91d64af3a383306b1998b87065248f`  
		Last Modified: Mon, 26 Oct 2020 17:51:27 GMT  
		Size: 213.1 MB (213119031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79914c2df80be97bf35af10e222d03a9673bdb70868542859f4ca306713ea83f`  
		Last Modified: Mon, 26 Oct 2020 17:50:46 GMT  
		Size: 2.4 MB (2435820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64083ae2108cec48181a94003bae0b8399a4a7b6471f1e2d1be462f3b80856bf`  
		Last Modified: Mon, 26 Oct 2020 17:50:45 GMT  
		Size: 1.1 MB (1118509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01edfe5d1f72ce612c1c5cc8c8fd1c632d466f9ae9a7c2b687f7dfe1a9db52bf`  
		Last Modified: Thu, 12 Nov 2020 19:26:01 GMT  
		Size: 158.3 MB (158303244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1469ce57930f123780015a29d2181ecca47034ed282d389c1c16a9b48f2a`  
		Last Modified: Thu, 12 Nov 2020 19:25:30 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c91fa07954c1f88edd13bc7da55c82ad466f6a17046cbed153cdd1193545ea9`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13f72919012cc465c0c6fbdf95426594bfe9f624ecea38f6006f33ee6b7e416`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25543eac24aeaf3949be246262ab118f76d0eb6e61fde74ab56951d58fe7383d`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
