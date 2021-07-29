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
$ docker pull odoo@sha256:a519687ec84a17271812fadeca1ed02f3b668b1d190d6013ab303874a5c4af1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:ab13caf4b4d67835cb6154520c40af4352b6dd720e3f1b0d2a15ee67ad9adff2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538381351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d4c65f46541c767de1969ddb873bb44f008bd6b38ae1b23b9453a4637fabc11`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:17 GMT
ADD file:55a25b93e8f2940a796f3cbf1e78bddf5f49c46b1b89b63b9b5673cbed9483ca in / 
# Thu, 22 Jul 2021 00:47:17 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:18:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 22 Jul 2021 14:18:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 22 Jul 2021 14:18:32 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:18:33 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Thu, 22 Jul 2021 14:19:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 22 Jul 2021 14:20:12 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:20:32 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:20:32 GMT
ENV ODOO_VERSION=12.0
# Wed, 28 Jul 2021 23:31:20 GMT
ARG ODOO_RELEASE=20210728
# Wed, 28 Jul 2021 23:31:20 GMT
ARG ODOO_SHA=b104aa197c922c88dc6db068f7aa2bafe44521e5
# Wed, 28 Jul 2021 23:32:24 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=b104aa197c922c88dc6db068f7aa2bafe44521e5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 28 Jul 2021 23:32:28 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 28 Jul 2021 23:32:28 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 28 Jul 2021 23:32:29 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=b104aa197c922c88dc6db068f7aa2bafe44521e5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 28 Jul 2021 23:32:29 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 28 Jul 2021 23:32:29 GMT
EXPOSE 8069 8071 8072
# Wed, 28 Jul 2021 23:32:29 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 28 Jul 2021 23:32:29 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 28 Jul 2021 23:32:30 GMT
USER odoo
# Wed, 28 Jul 2021 23:32:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 28 Jul 2021 23:32:30 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:778066204fb734c2fb80cb8127cb35d67d742806a4eaf1aba0b5393c4ae6f2a4`  
		Last Modified: Thu, 22 Jul 2021 00:53:22 GMT  
		Size: 22.5 MB (22527428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b204c7c8cc64bad523e886289c004fd49d89dca323966ac1b4e5988913eb92d`  
		Last Modified: Thu, 22 Jul 2021 14:23:56 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a9d0cb1723e7198eb716a0778314c493ea467b36143cbbe4b40c67b5d24ef9`  
		Last Modified: Thu, 22 Jul 2021 14:24:37 GMT  
		Size: 219.7 MB (219659230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624c7e60f85c5692a09efe6c44024a23d733d0bd828c8dfeb35b2dfd358e8826`  
		Last Modified: Thu, 22 Jul 2021 14:23:56 GMT  
		Size: 2.2 MB (2224668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfabe6def0f67df43daa7647f45a0a3ebf687d388c5beff7b0027c3e45d3e87d`  
		Last Modified: Thu, 22 Jul 2021 14:24:04 GMT  
		Size: 22.0 MB (22027409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d77a06445de7943c5e7a14c249f0dd12455526d40b0ee77d46f69cd37f6f22`  
		Last Modified: Wed, 28 Jul 2021 23:34:56 GMT  
		Size: 271.9 MB (271939959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0175de1e3700f819602aa5862b67338e7cb7841d4979333b904ec4ece531c5b`  
		Last Modified: Wed, 28 Jul 2021 23:34:29 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064f587626c91717fc6c5c5d41f53a0bcc82d3033bb8d57e393f890e386525f3`  
		Last Modified: Wed, 28 Jul 2021 23:34:29 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f240c247f845feb5fd60fcbc405ab18c59f13f0ac93191ab33af0aeb5f4bd`  
		Last Modified: Wed, 28 Jul 2021 23:34:29 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000b0a9bcef8e4a846ff431f9b19c457a0309e8e54e3d86071a379aa8f5f4138`  
		Last Modified: Wed, 28 Jul 2021 23:34:29 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:a519687ec84a17271812fadeca1ed02f3b668b1d190d6013ab303874a5c4af1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:ab13caf4b4d67835cb6154520c40af4352b6dd720e3f1b0d2a15ee67ad9adff2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538381351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d4c65f46541c767de1969ddb873bb44f008bd6b38ae1b23b9453a4637fabc11`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:17 GMT
ADD file:55a25b93e8f2940a796f3cbf1e78bddf5f49c46b1b89b63b9b5673cbed9483ca in / 
# Thu, 22 Jul 2021 00:47:17 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:18:32 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 22 Jul 2021 14:18:32 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 22 Jul 2021 14:18:32 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:18:33 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Thu, 22 Jul 2021 14:19:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 22 Jul 2021 14:20:12 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:20:32 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:20:32 GMT
ENV ODOO_VERSION=12.0
# Wed, 28 Jul 2021 23:31:20 GMT
ARG ODOO_RELEASE=20210728
# Wed, 28 Jul 2021 23:31:20 GMT
ARG ODOO_SHA=b104aa197c922c88dc6db068f7aa2bafe44521e5
# Wed, 28 Jul 2021 23:32:24 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=b104aa197c922c88dc6db068f7aa2bafe44521e5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 28 Jul 2021 23:32:28 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 28 Jul 2021 23:32:28 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 28 Jul 2021 23:32:29 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=b104aa197c922c88dc6db068f7aa2bafe44521e5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 28 Jul 2021 23:32:29 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 28 Jul 2021 23:32:29 GMT
EXPOSE 8069 8071 8072
# Wed, 28 Jul 2021 23:32:29 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 28 Jul 2021 23:32:29 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 28 Jul 2021 23:32:30 GMT
USER odoo
# Wed, 28 Jul 2021 23:32:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 28 Jul 2021 23:32:30 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:778066204fb734c2fb80cb8127cb35d67d742806a4eaf1aba0b5393c4ae6f2a4`  
		Last Modified: Thu, 22 Jul 2021 00:53:22 GMT  
		Size: 22.5 MB (22527428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b204c7c8cc64bad523e886289c004fd49d89dca323966ac1b4e5988913eb92d`  
		Last Modified: Thu, 22 Jul 2021 14:23:56 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a9d0cb1723e7198eb716a0778314c493ea467b36143cbbe4b40c67b5d24ef9`  
		Last Modified: Thu, 22 Jul 2021 14:24:37 GMT  
		Size: 219.7 MB (219659230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624c7e60f85c5692a09efe6c44024a23d733d0bd828c8dfeb35b2dfd358e8826`  
		Last Modified: Thu, 22 Jul 2021 14:23:56 GMT  
		Size: 2.2 MB (2224668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfabe6def0f67df43daa7647f45a0a3ebf687d388c5beff7b0027c3e45d3e87d`  
		Last Modified: Thu, 22 Jul 2021 14:24:04 GMT  
		Size: 22.0 MB (22027409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d77a06445de7943c5e7a14c249f0dd12455526d40b0ee77d46f69cd37f6f22`  
		Last Modified: Wed, 28 Jul 2021 23:34:56 GMT  
		Size: 271.9 MB (271939959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0175de1e3700f819602aa5862b67338e7cb7841d4979333b904ec4ece531c5b`  
		Last Modified: Wed, 28 Jul 2021 23:34:29 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064f587626c91717fc6c5c5d41f53a0bcc82d3033bb8d57e393f890e386525f3`  
		Last Modified: Wed, 28 Jul 2021 23:34:29 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f240c247f845feb5fd60fcbc405ab18c59f13f0ac93191ab33af0aeb5f4bd`  
		Last Modified: Wed, 28 Jul 2021 23:34:29 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000b0a9bcef8e4a846ff431f9b19c457a0309e8e54e3d86071a379aa8f5f4138`  
		Last Modified: Wed, 28 Jul 2021 23:34:29 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:092638e9a0a58d699b61b2a7b080259b64d7585fb6f04809073c35ef20ebb875
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:b51be7a7b1e5389c6f94f02ec40fc6e032a36c14db8061ec5e585db347cdfb77
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.3 MB (528320627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d84c890d7047a583143bd1c5161ff2b9a56be8d6b2f794dad6ee9432b3bc1c32`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:12:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 22 Jul 2021 14:12:41 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 22 Jul 2021 14:12:41 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:16:50 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 22 Jul 2021 14:16:57 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:17:00 GMT
RUN npm install -g rtlcss
# Thu, 22 Jul 2021 14:17:00 GMT
ENV ODOO_VERSION=13.0
# Wed, 28 Jul 2021 23:29:55 GMT
ARG ODOO_RELEASE=20210728
# Wed, 28 Jul 2021 23:29:55 GMT
ARG ODOO_SHA=3f1be7d8a149a898dcf1a958d49614c5fcf30e0e
# Wed, 28 Jul 2021 23:31:04 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=3f1be7d8a149a898dcf1a958d49614c5fcf30e0e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 28 Jul 2021 23:31:08 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 28 Jul 2021 23:31:08 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 28 Jul 2021 23:31:09 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=3f1be7d8a149a898dcf1a958d49614c5fcf30e0e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 28 Jul 2021 23:31:09 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 28 Jul 2021 23:31:10 GMT
EXPOSE 8069 8071 8072
# Wed, 28 Jul 2021 23:31:10 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 28 Jul 2021 23:31:10 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 28 Jul 2021 23:31:10 GMT
USER odoo
# Wed, 28 Jul 2021 23:31:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 28 Jul 2021 23:31:11 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8f3448dc635b32fd797faa7bd97abefb346d7a902095935c8e04f0f812bc8f`  
		Last Modified: Thu, 22 Jul 2021 14:23:34 GMT  
		Size: 207.1 MB (207125538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0bd24a54815ae14a888a2249982adc5e9d299f05ed362a896126ee25260548`  
		Last Modified: Thu, 22 Jul 2021 14:23:04 GMT  
		Size: 2.3 MB (2346808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a989fd222f0a84e1300dabf83f0d7f45734b16639a552c9d6849bcb0a84dd8c5`  
		Last Modified: Thu, 22 Jul 2021 14:23:04 GMT  
		Size: 889.1 KB (889054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711118774a7be4404a292c7d5ff572f97698112e0e7a01a91603fc75179d94b1`  
		Last Modified: Wed, 28 Jul 2021 23:34:14 GMT  
		Size: 290.8 MB (290811001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd81b87ec6824ada08f147d051f5dc6b1f1519e70517f02129be9a0f96aab20a`  
		Last Modified: Wed, 28 Jul 2021 23:33:45 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d07bbb90187fb5b60f6e94eb6b5f3a56a09ddff19e0a2f78c227ed58e0b114c`  
		Last Modified: Wed, 28 Jul 2021 23:33:45 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4942f795f49f8916379499db0bed48661294eac2dacad6b4da6fcb0a08b2cc49`  
		Last Modified: Wed, 28 Jul 2021 23:33:44 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce2cc0203d32695b6eddab2a625e1657240c58313d3b64d2e36712d5e5b8d9b`  
		Last Modified: Wed, 28 Jul 2021 23:33:45 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:092638e9a0a58d699b61b2a7b080259b64d7585fb6f04809073c35ef20ebb875
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:b51be7a7b1e5389c6f94f02ec40fc6e032a36c14db8061ec5e585db347cdfb77
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.3 MB (528320627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d84c890d7047a583143bd1c5161ff2b9a56be8d6b2f794dad6ee9432b3bc1c32`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:12:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 22 Jul 2021 14:12:41 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 22 Jul 2021 14:12:41 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:16:50 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 22 Jul 2021 14:16:57 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:17:00 GMT
RUN npm install -g rtlcss
# Thu, 22 Jul 2021 14:17:00 GMT
ENV ODOO_VERSION=13.0
# Wed, 28 Jul 2021 23:29:55 GMT
ARG ODOO_RELEASE=20210728
# Wed, 28 Jul 2021 23:29:55 GMT
ARG ODOO_SHA=3f1be7d8a149a898dcf1a958d49614c5fcf30e0e
# Wed, 28 Jul 2021 23:31:04 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=3f1be7d8a149a898dcf1a958d49614c5fcf30e0e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 28 Jul 2021 23:31:08 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 28 Jul 2021 23:31:08 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 28 Jul 2021 23:31:09 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=3f1be7d8a149a898dcf1a958d49614c5fcf30e0e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 28 Jul 2021 23:31:09 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 28 Jul 2021 23:31:10 GMT
EXPOSE 8069 8071 8072
# Wed, 28 Jul 2021 23:31:10 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 28 Jul 2021 23:31:10 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 28 Jul 2021 23:31:10 GMT
USER odoo
# Wed, 28 Jul 2021 23:31:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 28 Jul 2021 23:31:11 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8f3448dc635b32fd797faa7bd97abefb346d7a902095935c8e04f0f812bc8f`  
		Last Modified: Thu, 22 Jul 2021 14:23:34 GMT  
		Size: 207.1 MB (207125538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0bd24a54815ae14a888a2249982adc5e9d299f05ed362a896126ee25260548`  
		Last Modified: Thu, 22 Jul 2021 14:23:04 GMT  
		Size: 2.3 MB (2346808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a989fd222f0a84e1300dabf83f0d7f45734b16639a552c9d6849bcb0a84dd8c5`  
		Last Modified: Thu, 22 Jul 2021 14:23:04 GMT  
		Size: 889.1 KB (889054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711118774a7be4404a292c7d5ff572f97698112e0e7a01a91603fc75179d94b1`  
		Last Modified: Wed, 28 Jul 2021 23:34:14 GMT  
		Size: 290.8 MB (290811001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd81b87ec6824ada08f147d051f5dc6b1f1519e70517f02129be9a0f96aab20a`  
		Last Modified: Wed, 28 Jul 2021 23:33:45 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d07bbb90187fb5b60f6e94eb6b5f3a56a09ddff19e0a2f78c227ed58e0b114c`  
		Last Modified: Wed, 28 Jul 2021 23:33:45 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4942f795f49f8916379499db0bed48661294eac2dacad6b4da6fcb0a08b2cc49`  
		Last Modified: Wed, 28 Jul 2021 23:33:44 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce2cc0203d32695b6eddab2a625e1657240c58313d3b64d2e36712d5e5b8d9b`  
		Last Modified: Wed, 28 Jul 2021 23:33:45 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:37d39abe2912d79732fea45bcd3659d2099b1f9aec2578c964fb1a685a6ce05c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:103f240be57a7c109f4e6fcf91110e4a805dbd5ab7491a80e4b5e1c8198ab295
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.6 MB (516617058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79faaa8061a2a65d637d183f68f2d9493ca798efbb5f381d082eab8878205603`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:12:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 22 Jul 2021 14:12:41 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 22 Jul 2021 14:12:41 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:14:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 22 Jul 2021 14:14:14 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:14:17 GMT
RUN npm install -g rtlcss
# Thu, 22 Jul 2021 14:14:18 GMT
ENV ODOO_VERSION=14.0
# Wed, 28 Jul 2021 23:28:29 GMT
ARG ODOO_RELEASE=20210728
# Wed, 28 Jul 2021 23:28:29 GMT
ARG ODOO_SHA=9e4ba128935f9fdaca61965472248fedbebf62d3
# Wed, 28 Jul 2021 23:29:40 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=9e4ba128935f9fdaca61965472248fedbebf62d3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 28 Jul 2021 23:29:44 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 28 Jul 2021 23:29:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 28 Jul 2021 23:29:44 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=9e4ba128935f9fdaca61965472248fedbebf62d3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 28 Jul 2021 23:29:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 28 Jul 2021 23:29:45 GMT
EXPOSE 8069 8071 8072
# Wed, 28 Jul 2021 23:29:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 28 Jul 2021 23:29:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 28 Jul 2021 23:29:45 GMT
USER odoo
# Wed, 28 Jul 2021 23:29:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 28 Jul 2021 23:29:46 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5502f02c83eb9a5d2610c8d0caea8b6d8645db289895c5071886b9231f40ac51`  
		Last Modified: Thu, 22 Jul 2021 14:22:40 GMT  
		Size: 213.2 MB (213172386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a9b423102589afe08dee7c8ee26abe30dce0b452950ca9eb03c425cf098c16`  
		Last Modified: Thu, 22 Jul 2021 14:22:17 GMT  
		Size: 2.3 MB (2349817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62bb0f68ae1402800683d9694dc8f338be4ac729f14a2e24d738f4aa12ea7e6`  
		Last Modified: Thu, 22 Jul 2021 14:22:14 GMT  
		Size: 889.3 KB (889257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3289b5ff062f07b61928e2e2e2c54bdb88f8f80362284ab367a27157ddf55e7c`  
		Last Modified: Wed, 28 Jul 2021 23:33:28 GMT  
		Size: 273.1 MB (273057378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebcd71baa376b6f698dde328108bae5d9bbfc43d06bda7e36434e1fad73a956`  
		Last Modified: Wed, 28 Jul 2021 23:32:58 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb39fd5799c36b4ac550bfaced911a0c293f54f425a06d6b6abbb8305f3e1fb`  
		Last Modified: Wed, 28 Jul 2021 23:32:58 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da0e44fe94b75d280559b5a1f7811dd5a0c2b6b18236b9eb7a295b03dee6ca`  
		Last Modified: Wed, 28 Jul 2021 23:32:58 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f37587c20b715980546fe1857c21c4039d2ab9f676fe9e96dd188ab43a8172`  
		Last Modified: Wed, 28 Jul 2021 23:32:57 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:37d39abe2912d79732fea45bcd3659d2099b1f9aec2578c964fb1a685a6ce05c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:103f240be57a7c109f4e6fcf91110e4a805dbd5ab7491a80e4b5e1c8198ab295
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.6 MB (516617058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79faaa8061a2a65d637d183f68f2d9493ca798efbb5f381d082eab8878205603`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:12:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 22 Jul 2021 14:12:41 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 22 Jul 2021 14:12:41 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:14:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 22 Jul 2021 14:14:14 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:14:17 GMT
RUN npm install -g rtlcss
# Thu, 22 Jul 2021 14:14:18 GMT
ENV ODOO_VERSION=14.0
# Wed, 28 Jul 2021 23:28:29 GMT
ARG ODOO_RELEASE=20210728
# Wed, 28 Jul 2021 23:28:29 GMT
ARG ODOO_SHA=9e4ba128935f9fdaca61965472248fedbebf62d3
# Wed, 28 Jul 2021 23:29:40 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=9e4ba128935f9fdaca61965472248fedbebf62d3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 28 Jul 2021 23:29:44 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 28 Jul 2021 23:29:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 28 Jul 2021 23:29:44 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=9e4ba128935f9fdaca61965472248fedbebf62d3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 28 Jul 2021 23:29:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 28 Jul 2021 23:29:45 GMT
EXPOSE 8069 8071 8072
# Wed, 28 Jul 2021 23:29:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 28 Jul 2021 23:29:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 28 Jul 2021 23:29:45 GMT
USER odoo
# Wed, 28 Jul 2021 23:29:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 28 Jul 2021 23:29:46 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5502f02c83eb9a5d2610c8d0caea8b6d8645db289895c5071886b9231f40ac51`  
		Last Modified: Thu, 22 Jul 2021 14:22:40 GMT  
		Size: 213.2 MB (213172386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a9b423102589afe08dee7c8ee26abe30dce0b452950ca9eb03c425cf098c16`  
		Last Modified: Thu, 22 Jul 2021 14:22:17 GMT  
		Size: 2.3 MB (2349817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62bb0f68ae1402800683d9694dc8f338be4ac729f14a2e24d738f4aa12ea7e6`  
		Last Modified: Thu, 22 Jul 2021 14:22:14 GMT  
		Size: 889.3 KB (889257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3289b5ff062f07b61928e2e2e2c54bdb88f8f80362284ab367a27157ddf55e7c`  
		Last Modified: Wed, 28 Jul 2021 23:33:28 GMT  
		Size: 273.1 MB (273057378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebcd71baa376b6f698dde328108bae5d9bbfc43d06bda7e36434e1fad73a956`  
		Last Modified: Wed, 28 Jul 2021 23:32:58 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb39fd5799c36b4ac550bfaced911a0c293f54f425a06d6b6abbb8305f3e1fb`  
		Last Modified: Wed, 28 Jul 2021 23:32:58 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da0e44fe94b75d280559b5a1f7811dd5a0c2b6b18236b9eb7a295b03dee6ca`  
		Last Modified: Wed, 28 Jul 2021 23:32:58 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f37587c20b715980546fe1857c21c4039d2ab9f676fe9e96dd188ab43a8172`  
		Last Modified: Wed, 28 Jul 2021 23:32:57 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:37d39abe2912d79732fea45bcd3659d2099b1f9aec2578c964fb1a685a6ce05c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:103f240be57a7c109f4e6fcf91110e4a805dbd5ab7491a80e4b5e1c8198ab295
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.6 MB (516617058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79faaa8061a2a65d637d183f68f2d9493ca798efbb5f381d082eab8878205603`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:12:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 22 Jul 2021 14:12:41 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 22 Jul 2021 14:12:41 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:14:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 22 Jul 2021 14:14:14 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:14:17 GMT
RUN npm install -g rtlcss
# Thu, 22 Jul 2021 14:14:18 GMT
ENV ODOO_VERSION=14.0
# Wed, 28 Jul 2021 23:28:29 GMT
ARG ODOO_RELEASE=20210728
# Wed, 28 Jul 2021 23:28:29 GMT
ARG ODOO_SHA=9e4ba128935f9fdaca61965472248fedbebf62d3
# Wed, 28 Jul 2021 23:29:40 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=9e4ba128935f9fdaca61965472248fedbebf62d3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 28 Jul 2021 23:29:44 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 28 Jul 2021 23:29:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 28 Jul 2021 23:29:44 GMT
# ARGS: ODOO_RELEASE=20210728 ODOO_SHA=9e4ba128935f9fdaca61965472248fedbebf62d3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 28 Jul 2021 23:29:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 28 Jul 2021 23:29:45 GMT
EXPOSE 8069 8071 8072
# Wed, 28 Jul 2021 23:29:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 28 Jul 2021 23:29:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 28 Jul 2021 23:29:45 GMT
USER odoo
# Wed, 28 Jul 2021 23:29:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 28 Jul 2021 23:29:46 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5502f02c83eb9a5d2610c8d0caea8b6d8645db289895c5071886b9231f40ac51`  
		Last Modified: Thu, 22 Jul 2021 14:22:40 GMT  
		Size: 213.2 MB (213172386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a9b423102589afe08dee7c8ee26abe30dce0b452950ca9eb03c425cf098c16`  
		Last Modified: Thu, 22 Jul 2021 14:22:17 GMT  
		Size: 2.3 MB (2349817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62bb0f68ae1402800683d9694dc8f338be4ac729f14a2e24d738f4aa12ea7e6`  
		Last Modified: Thu, 22 Jul 2021 14:22:14 GMT  
		Size: 889.3 KB (889257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3289b5ff062f07b61928e2e2e2c54bdb88f8f80362284ab367a27157ddf55e7c`  
		Last Modified: Wed, 28 Jul 2021 23:33:28 GMT  
		Size: 273.1 MB (273057378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebcd71baa376b6f698dde328108bae5d9bbfc43d06bda7e36434e1fad73a956`  
		Last Modified: Wed, 28 Jul 2021 23:32:58 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb39fd5799c36b4ac550bfaced911a0c293f54f425a06d6b6abbb8305f3e1fb`  
		Last Modified: Wed, 28 Jul 2021 23:32:58 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da0e44fe94b75d280559b5a1f7811dd5a0c2b6b18236b9eb7a295b03dee6ca`  
		Last Modified: Wed, 28 Jul 2021 23:32:58 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f37587c20b715980546fe1857c21c4039d2ab9f676fe9e96dd188ab43a8172`  
		Last Modified: Wed, 28 Jul 2021 23:32:57 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
