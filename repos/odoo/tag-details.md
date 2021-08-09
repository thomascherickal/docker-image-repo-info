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
$ docker pull odoo@sha256:4b1b72c86c37ed95a1d801f37d1ddab00a1a29f3c90b34db464bef82e8793b10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:62edade3da33c32b8d7748bd4049863e6ecd548d4f6a50fbd9058d9d2381f44c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538408091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e38034fe266b452e484aa5a3b71905b54707a1028b4c772d6b5142472ec758bf`
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
# Mon, 09 Aug 2021 19:33:35 GMT
ARG ODOO_RELEASE=20210809
# Mon, 09 Aug 2021 19:33:35 GMT
ARG ODOO_SHA=7834befe1d22ae1c30bce23e1c10ab83a2963d26
# Mon, 09 Aug 2021 19:34:41 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=7834befe1d22ae1c30bce23e1c10ab83a2963d26
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 09 Aug 2021 19:34:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 09 Aug 2021 19:34:42 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 09 Aug 2021 19:34:43 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=7834befe1d22ae1c30bce23e1c10ab83a2963d26
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 09 Aug 2021 19:34:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 09 Aug 2021 19:34:43 GMT
EXPOSE 8069 8071 8072
# Mon, 09 Aug 2021 19:34:44 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 09 Aug 2021 19:34:44 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 09 Aug 2021 19:34:44 GMT
USER odoo
# Mon, 09 Aug 2021 19:34:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 09 Aug 2021 19:34:44 GMT
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
	-	`sha256:fcf106555a28162a7a40505496359280758eb1f49fe255ab47d2697f5039a138`  
		Last Modified: Mon, 09 Aug 2021 19:36:50 GMT  
		Size: 272.0 MB (271966662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332fbf9978340c62c288ea67236a3cb888bb825d664922ebf3bbc9d4cb4f19df`  
		Last Modified: Mon, 09 Aug 2021 19:36:23 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be71fc1bd1ca9ff3577a38cab05ce20271d6f7f58be67f50f1cce28274cd436e`  
		Last Modified: Mon, 09 Aug 2021 19:36:23 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8235713cf2ea55f9a605446a5fc4cd9d31e4af91c402de5a946969267c1e3b8`  
		Last Modified: Mon, 09 Aug 2021 19:36:24 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0506193856c038a7179d4fe59e4f247ce88e4d0d64250fdafbe78aaed0812f9d`  
		Last Modified: Mon, 09 Aug 2021 19:36:23 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:4b1b72c86c37ed95a1d801f37d1ddab00a1a29f3c90b34db464bef82e8793b10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:62edade3da33c32b8d7748bd4049863e6ecd548d4f6a50fbd9058d9d2381f44c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538408091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e38034fe266b452e484aa5a3b71905b54707a1028b4c772d6b5142472ec758bf`
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
# Mon, 09 Aug 2021 19:33:35 GMT
ARG ODOO_RELEASE=20210809
# Mon, 09 Aug 2021 19:33:35 GMT
ARG ODOO_SHA=7834befe1d22ae1c30bce23e1c10ab83a2963d26
# Mon, 09 Aug 2021 19:34:41 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=7834befe1d22ae1c30bce23e1c10ab83a2963d26
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 09 Aug 2021 19:34:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 09 Aug 2021 19:34:42 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 09 Aug 2021 19:34:43 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=7834befe1d22ae1c30bce23e1c10ab83a2963d26
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 09 Aug 2021 19:34:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 09 Aug 2021 19:34:43 GMT
EXPOSE 8069 8071 8072
# Mon, 09 Aug 2021 19:34:44 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 09 Aug 2021 19:34:44 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 09 Aug 2021 19:34:44 GMT
USER odoo
# Mon, 09 Aug 2021 19:34:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 09 Aug 2021 19:34:44 GMT
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
	-	`sha256:fcf106555a28162a7a40505496359280758eb1f49fe255ab47d2697f5039a138`  
		Last Modified: Mon, 09 Aug 2021 19:36:50 GMT  
		Size: 272.0 MB (271966662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332fbf9978340c62c288ea67236a3cb888bb825d664922ebf3bbc9d4cb4f19df`  
		Last Modified: Mon, 09 Aug 2021 19:36:23 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be71fc1bd1ca9ff3577a38cab05ce20271d6f7f58be67f50f1cce28274cd436e`  
		Last Modified: Mon, 09 Aug 2021 19:36:23 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8235713cf2ea55f9a605446a5fc4cd9d31e4af91c402de5a946969267c1e3b8`  
		Last Modified: Mon, 09 Aug 2021 19:36:24 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0506193856c038a7179d4fe59e4f247ce88e4d0d64250fdafbe78aaed0812f9d`  
		Last Modified: Mon, 09 Aug 2021 19:36:23 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:eaaa3f767ea8c12df5a51297491846e23d64d0b0d79c9e3c61cbda60ae0d46d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:ca9173a12638ed059e4214959e2db5f215f654554ea5ddd3575170ecd3d25b76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.4 MB (528400194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9db3bb4ad5158b9d34e5093237e6ed5f2c69ea4da00927fb9fc3da1212d7ada0`
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
# Mon, 09 Aug 2021 19:32:09 GMT
ARG ODOO_RELEASE=20210809
# Mon, 09 Aug 2021 19:32:09 GMT
ARG ODOO_SHA=dd7613080ed2b919e6d0b0d819b271400f29a9f9
# Mon, 09 Aug 2021 19:33:20 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=dd7613080ed2b919e6d0b0d819b271400f29a9f9
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 09 Aug 2021 19:33:24 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 09 Aug 2021 19:33:24 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 09 Aug 2021 19:33:25 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=dd7613080ed2b919e6d0b0d819b271400f29a9f9
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 09 Aug 2021 19:33:25 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 09 Aug 2021 19:33:25 GMT
EXPOSE 8069 8071 8072
# Mon, 09 Aug 2021 19:33:25 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 09 Aug 2021 19:33:25 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 09 Aug 2021 19:33:26 GMT
USER odoo
# Mon, 09 Aug 2021 19:33:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 09 Aug 2021 19:33:26 GMT
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
	-	`sha256:af483cd59a0df06553fb3ce18995cd3f32f974dab13d21b0e3d467aa0f849479`  
		Last Modified: Mon, 09 Aug 2021 19:36:13 GMT  
		Size: 290.9 MB (290890539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b9402c9270b4f31d06cc07ab27b8b713382d4626e1ca89a3fe71be36fa1b47`  
		Last Modified: Mon, 09 Aug 2021 19:35:43 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0d972d41a2702a30d4a47260ac163f4aae8563f42d8d796e933af213c1017f`  
		Last Modified: Mon, 09 Aug 2021 19:35:43 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10c1db59febe2018b1991fd84c2f36382ef5777c62657ce8f6987c45bc66c87`  
		Last Modified: Mon, 09 Aug 2021 19:35:43 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa06360bea9e61476462ab0488aed1505b6743284079939f405fca5eb79921`  
		Last Modified: Mon, 09 Aug 2021 19:35:43 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:eaaa3f767ea8c12df5a51297491846e23d64d0b0d79c9e3c61cbda60ae0d46d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:ca9173a12638ed059e4214959e2db5f215f654554ea5ddd3575170ecd3d25b76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.4 MB (528400194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9db3bb4ad5158b9d34e5093237e6ed5f2c69ea4da00927fb9fc3da1212d7ada0`
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
# Mon, 09 Aug 2021 19:32:09 GMT
ARG ODOO_RELEASE=20210809
# Mon, 09 Aug 2021 19:32:09 GMT
ARG ODOO_SHA=dd7613080ed2b919e6d0b0d819b271400f29a9f9
# Mon, 09 Aug 2021 19:33:20 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=dd7613080ed2b919e6d0b0d819b271400f29a9f9
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 09 Aug 2021 19:33:24 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 09 Aug 2021 19:33:24 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 09 Aug 2021 19:33:25 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=dd7613080ed2b919e6d0b0d819b271400f29a9f9
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 09 Aug 2021 19:33:25 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 09 Aug 2021 19:33:25 GMT
EXPOSE 8069 8071 8072
# Mon, 09 Aug 2021 19:33:25 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 09 Aug 2021 19:33:25 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 09 Aug 2021 19:33:26 GMT
USER odoo
# Mon, 09 Aug 2021 19:33:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 09 Aug 2021 19:33:26 GMT
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
	-	`sha256:af483cd59a0df06553fb3ce18995cd3f32f974dab13d21b0e3d467aa0f849479`  
		Last Modified: Mon, 09 Aug 2021 19:36:13 GMT  
		Size: 290.9 MB (290890539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b9402c9270b4f31d06cc07ab27b8b713382d4626e1ca89a3fe71be36fa1b47`  
		Last Modified: Mon, 09 Aug 2021 19:35:43 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0d972d41a2702a30d4a47260ac163f4aae8563f42d8d796e933af213c1017f`  
		Last Modified: Mon, 09 Aug 2021 19:35:43 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10c1db59febe2018b1991fd84c2f36382ef5777c62657ce8f6987c45bc66c87`  
		Last Modified: Mon, 09 Aug 2021 19:35:43 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa06360bea9e61476462ab0488aed1505b6743284079939f405fca5eb79921`  
		Last Modified: Mon, 09 Aug 2021 19:35:43 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:c2caf23c2b940064f30bae94abd1028413e315b0ca533785365437175cf48d41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:2925b6645adcab494057f6bf958c6acab490d5f3072ab79b1158973890f2a8eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.8 MB (516759147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84ff60d660b8290bbf969258d88757cd669afb1640bbdccd0f143a4e03895a33`
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
# Mon, 09 Aug 2021 19:30:44 GMT
ARG ODOO_RELEASE=20210809
# Mon, 09 Aug 2021 19:30:44 GMT
ARG ODOO_SHA=d9d18498eab946032cacd23d9e8ae69bfbce046b
# Mon, 09 Aug 2021 19:31:52 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=d9d18498eab946032cacd23d9e8ae69bfbce046b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 09 Aug 2021 19:31:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 09 Aug 2021 19:31:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 09 Aug 2021 19:31:57 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=d9d18498eab946032cacd23d9e8ae69bfbce046b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 09 Aug 2021 19:31:57 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 09 Aug 2021 19:31:57 GMT
EXPOSE 8069 8071 8072
# Mon, 09 Aug 2021 19:31:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 09 Aug 2021 19:31:58 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 09 Aug 2021 19:31:58 GMT
USER odoo
# Mon, 09 Aug 2021 19:31:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 09 Aug 2021 19:31:58 GMT
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
	-	`sha256:43f5830b2f5008db3427bb95771a3e67da5e99086b76d4368b4d9fde100c0011`  
		Last Modified: Mon, 09 Aug 2021 19:35:30 GMT  
		Size: 273.2 MB (273199433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99e1f6d93cb84b5831f1e2c9fdb1ee3efc3ab70c20a6b3fac28e2186a84c2d3`  
		Last Modified: Mon, 09 Aug 2021 19:34:59 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36984368930c07b19f314963636d5255a2b352b16e384ee8d1a19585e12426d6`  
		Last Modified: Mon, 09 Aug 2021 19:34:58 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b63972506ef96de83e913b22631af6483c5820df3ce7f2231f299109640d8e`  
		Last Modified: Mon, 09 Aug 2021 19:34:58 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b40fbbb503d8561bb8cca5e7445e6d75547f9597a7208a16d45284ec440d96d`  
		Last Modified: Mon, 09 Aug 2021 19:34:58 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:c2caf23c2b940064f30bae94abd1028413e315b0ca533785365437175cf48d41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:2925b6645adcab494057f6bf958c6acab490d5f3072ab79b1158973890f2a8eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.8 MB (516759147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84ff60d660b8290bbf969258d88757cd669afb1640bbdccd0f143a4e03895a33`
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
# Mon, 09 Aug 2021 19:30:44 GMT
ARG ODOO_RELEASE=20210809
# Mon, 09 Aug 2021 19:30:44 GMT
ARG ODOO_SHA=d9d18498eab946032cacd23d9e8ae69bfbce046b
# Mon, 09 Aug 2021 19:31:52 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=d9d18498eab946032cacd23d9e8ae69bfbce046b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 09 Aug 2021 19:31:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 09 Aug 2021 19:31:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 09 Aug 2021 19:31:57 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=d9d18498eab946032cacd23d9e8ae69bfbce046b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 09 Aug 2021 19:31:57 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 09 Aug 2021 19:31:57 GMT
EXPOSE 8069 8071 8072
# Mon, 09 Aug 2021 19:31:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 09 Aug 2021 19:31:58 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 09 Aug 2021 19:31:58 GMT
USER odoo
# Mon, 09 Aug 2021 19:31:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 09 Aug 2021 19:31:58 GMT
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
	-	`sha256:43f5830b2f5008db3427bb95771a3e67da5e99086b76d4368b4d9fde100c0011`  
		Last Modified: Mon, 09 Aug 2021 19:35:30 GMT  
		Size: 273.2 MB (273199433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99e1f6d93cb84b5831f1e2c9fdb1ee3efc3ab70c20a6b3fac28e2186a84c2d3`  
		Last Modified: Mon, 09 Aug 2021 19:34:59 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36984368930c07b19f314963636d5255a2b352b16e384ee8d1a19585e12426d6`  
		Last Modified: Mon, 09 Aug 2021 19:34:58 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b63972506ef96de83e913b22631af6483c5820df3ce7f2231f299109640d8e`  
		Last Modified: Mon, 09 Aug 2021 19:34:58 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b40fbbb503d8561bb8cca5e7445e6d75547f9597a7208a16d45284ec440d96d`  
		Last Modified: Mon, 09 Aug 2021 19:34:58 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:c2caf23c2b940064f30bae94abd1028413e315b0ca533785365437175cf48d41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:2925b6645adcab494057f6bf958c6acab490d5f3072ab79b1158973890f2a8eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.8 MB (516759147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84ff60d660b8290bbf969258d88757cd669afb1640bbdccd0f143a4e03895a33`
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
# Mon, 09 Aug 2021 19:30:44 GMT
ARG ODOO_RELEASE=20210809
# Mon, 09 Aug 2021 19:30:44 GMT
ARG ODOO_SHA=d9d18498eab946032cacd23d9e8ae69bfbce046b
# Mon, 09 Aug 2021 19:31:52 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=d9d18498eab946032cacd23d9e8ae69bfbce046b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 09 Aug 2021 19:31:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 09 Aug 2021 19:31:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 09 Aug 2021 19:31:57 GMT
# ARGS: ODOO_RELEASE=20210809 ODOO_SHA=d9d18498eab946032cacd23d9e8ae69bfbce046b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 09 Aug 2021 19:31:57 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 09 Aug 2021 19:31:57 GMT
EXPOSE 8069 8071 8072
# Mon, 09 Aug 2021 19:31:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 09 Aug 2021 19:31:58 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 09 Aug 2021 19:31:58 GMT
USER odoo
# Mon, 09 Aug 2021 19:31:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 09 Aug 2021 19:31:58 GMT
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
	-	`sha256:43f5830b2f5008db3427bb95771a3e67da5e99086b76d4368b4d9fde100c0011`  
		Last Modified: Mon, 09 Aug 2021 19:35:30 GMT  
		Size: 273.2 MB (273199433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99e1f6d93cb84b5831f1e2c9fdb1ee3efc3ab70c20a6b3fac28e2186a84c2d3`  
		Last Modified: Mon, 09 Aug 2021 19:34:59 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36984368930c07b19f314963636d5255a2b352b16e384ee8d1a19585e12426d6`  
		Last Modified: Mon, 09 Aug 2021 19:34:58 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b63972506ef96de83e913b22631af6483c5820df3ce7f2231f299109640d8e`  
		Last Modified: Mon, 09 Aug 2021 19:34:58 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b40fbbb503d8561bb8cca5e7445e6d75547f9597a7208a16d45284ec440d96d`  
		Last Modified: Mon, 09 Aug 2021 19:34:58 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
