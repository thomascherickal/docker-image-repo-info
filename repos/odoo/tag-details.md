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
$ docker pull odoo@sha256:f11952eeefab3a76509b325911bc586b27722cdef2efa4ba9aa39d0b2d287231
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:362db7c43c2b93e52837b481add214b8359c114f9d9b08e7d940744b9f17e085
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.7 MB (396737523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4da605d28b629d81a0d7b906ab343b2898ff291077f769952f2800eccb857d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:33:15 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 18 Nov 2020 06:33:15 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 18 Nov 2020 06:33:15 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 06:33:18 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 18 Nov 2020 06:35:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 18 Nov 2020 06:36:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:36:34 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:36:34 GMT
ENV ODOO_VERSION=12.0
# Tue, 24 Nov 2020 00:52:49 GMT
ARG ODOO_RELEASE=20201123
# Tue, 24 Nov 2020 00:52:49 GMT
ARG ODOO_SHA=ee05f5fb87fd762219a882eecc95c80569c7f3da
# Tue, 24 Nov 2020 00:53:37 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=ee05f5fb87fd762219a882eecc95c80569c7f3da
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 24 Nov 2020 00:53:38 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 24 Nov 2020 00:53:38 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 24 Nov 2020 00:53:39 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=ee05f5fb87fd762219a882eecc95c80569c7f3da
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 24 Nov 2020 00:53:40 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 24 Nov 2020 00:53:40 GMT
EXPOSE 8069 8071 8072
# Tue, 24 Nov 2020 00:53:40 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 24 Nov 2020 00:53:40 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 24 Nov 2020 00:53:40 GMT
USER odoo
# Tue, 24 Nov 2020 00:53:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 24 Nov 2020 00:53:41 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d40e2b4e18951bd08dba5a82a5c328bfd4f61527e674f2a27b592f59d48bf6`  
		Last Modified: Wed, 18 Nov 2020 06:39:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c87e7f63cf9421776bf4d5a4877ea56fd8421a04064560e873b269b75114128`  
		Last Modified: Wed, 18 Nov 2020 06:39:54 GMT  
		Size: 219.6 MB (219609554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69408741c653b462cb1135d9da405c149199db6026a991cdfdeb003fea56bbbf`  
		Last Modified: Wed, 18 Nov 2020 06:39:23 GMT  
		Size: 2.2 MB (2222431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588c13b5e1b3821514e94ca7f96ce88324f5c429f3c16c74edf0548b29a1920e`  
		Last Modified: Wed, 18 Nov 2020 06:39:28 GMT  
		Size: 22.3 MB (22274707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d823588c5a50118b403cff431bf343aed2350aa011fb5f857dae62a12f50d9`  
		Last Modified: Tue, 24 Nov 2020 00:55:49 GMT  
		Size: 130.1 MB (130100531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c21d7113d7728650862d587c9b51a75962f88e14243fc0291db25ceb52350cc`  
		Last Modified: Tue, 24 Nov 2020 00:55:20 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e8660cf5aa4a79fd89f1735e67a553761a22296a49346ae46e0827fa517fe3`  
		Last Modified: Tue, 24 Nov 2020 00:55:20 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671ac66bbd396ff946b5f672be2b8057c2884df03bae5dd703bf1ba43e387ef9`  
		Last Modified: Tue, 24 Nov 2020 00:55:20 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45440eef983789132e88816ce1c217832aa3858c3c4f4beda399f8a25699f949`  
		Last Modified: Tue, 24 Nov 2020 00:55:20 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:f11952eeefab3a76509b325911bc586b27722cdef2efa4ba9aa39d0b2d287231
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:362db7c43c2b93e52837b481add214b8359c114f9d9b08e7d940744b9f17e085
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.7 MB (396737523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4da605d28b629d81a0d7b906ab343b2898ff291077f769952f2800eccb857d8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:29 GMT
ADD file:02294bc9e72a3f3314955f0b5e0e728cd75321e88a1fae9bfbac77c76bfaf05d in / 
# Tue, 17 Nov 2020 20:24:29 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:33:15 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 18 Nov 2020 06:33:15 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 18 Nov 2020 06:33:15 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 06:33:18 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 18 Nov 2020 06:35:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 18 Nov 2020 06:36:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:36:34 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:36:34 GMT
ENV ODOO_VERSION=12.0
# Tue, 24 Nov 2020 00:52:49 GMT
ARG ODOO_RELEASE=20201123
# Tue, 24 Nov 2020 00:52:49 GMT
ARG ODOO_SHA=ee05f5fb87fd762219a882eecc95c80569c7f3da
# Tue, 24 Nov 2020 00:53:37 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=ee05f5fb87fd762219a882eecc95c80569c7f3da
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 24 Nov 2020 00:53:38 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 24 Nov 2020 00:53:38 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 24 Nov 2020 00:53:39 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=ee05f5fb87fd762219a882eecc95c80569c7f3da
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 24 Nov 2020 00:53:40 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 24 Nov 2020 00:53:40 GMT
EXPOSE 8069 8071 8072
# Tue, 24 Nov 2020 00:53:40 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 24 Nov 2020 00:53:40 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 24 Nov 2020 00:53:40 GMT
USER odoo
# Tue, 24 Nov 2020 00:53:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 24 Nov 2020 00:53:41 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:4297e02295585beb3f148a5740b644ce87e059455f8d98a5adb7bf95105e011c`  
		Last Modified: Tue, 17 Nov 2020 20:30:42 GMT  
		Size: 22.5 MB (22527663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d40e2b4e18951bd08dba5a82a5c328bfd4f61527e674f2a27b592f59d48bf6`  
		Last Modified: Wed, 18 Nov 2020 06:39:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c87e7f63cf9421776bf4d5a4877ea56fd8421a04064560e873b269b75114128`  
		Last Modified: Wed, 18 Nov 2020 06:39:54 GMT  
		Size: 219.6 MB (219609554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69408741c653b462cb1135d9da405c149199db6026a991cdfdeb003fea56bbbf`  
		Last Modified: Wed, 18 Nov 2020 06:39:23 GMT  
		Size: 2.2 MB (2222431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588c13b5e1b3821514e94ca7f96ce88324f5c429f3c16c74edf0548b29a1920e`  
		Last Modified: Wed, 18 Nov 2020 06:39:28 GMT  
		Size: 22.3 MB (22274707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d823588c5a50118b403cff431bf343aed2350aa011fb5f857dae62a12f50d9`  
		Last Modified: Tue, 24 Nov 2020 00:55:49 GMT  
		Size: 130.1 MB (130100531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c21d7113d7728650862d587c9b51a75962f88e14243fc0291db25ceb52350cc`  
		Last Modified: Tue, 24 Nov 2020 00:55:20 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e8660cf5aa4a79fd89f1735e67a553761a22296a49346ae46e0827fa517fe3`  
		Last Modified: Tue, 24 Nov 2020 00:55:20 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671ac66bbd396ff946b5f672be2b8057c2884df03bae5dd703bf1ba43e387ef9`  
		Last Modified: Tue, 24 Nov 2020 00:55:20 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45440eef983789132e88816ce1c217832aa3858c3c4f4beda399f8a25699f949`  
		Last Modified: Tue, 24 Nov 2020 00:55:20 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:88fe298a95bb93f455a3d4489aa1a8c7b264d106a00c199f6be75b8b332d6e93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:bfc01dbb6a49576ac88aca664bf59fe2afc0a1bba94743699c49a11acf0a4cd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.2 MB (386168233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20ab96138129f3a8c9f0bcabf32a0b12118fa168d6a46d915095e65a6d459b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:26:23 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 18 Nov 2020 06:26:24 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 18 Nov 2020 06:26:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 06:31:23 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 18 Nov 2020 06:31:29 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:31:34 GMT
RUN npm install -g rtlcss
# Wed, 18 Nov 2020 06:31:34 GMT
ENV ODOO_VERSION=13.0
# Tue, 24 Nov 2020 00:51:32 GMT
ARG ODOO_RELEASE=20201123
# Tue, 24 Nov 2020 00:51:33 GMT
ARG ODOO_SHA=1af64956f215ba0a2991ac6c86b98610c480c17b
# Tue, 24 Nov 2020 00:52:33 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=1af64956f215ba0a2991ac6c86b98610c480c17b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 24 Nov 2020 00:52:34 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 24 Nov 2020 00:52:34 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 24 Nov 2020 00:52:35 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=1af64956f215ba0a2991ac6c86b98610c480c17b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 24 Nov 2020 00:52:36 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 24 Nov 2020 00:52:36 GMT
EXPOSE 8069 8071 8072
# Tue, 24 Nov 2020 00:52:36 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 24 Nov 2020 00:52:36 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 24 Nov 2020 00:52:36 GMT
USER odoo
# Tue, 24 Nov 2020 00:52:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 24 Nov 2020 00:52:37 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c783d4a932f38653fa5103b08d8864e5e286a4d09e52582cca80c2a130b2df`  
		Last Modified: Wed, 18 Nov 2020 06:39:05 GMT  
		Size: 207.1 MB (207077490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1198c7d9e40b780e43f9dd77c39e0c2cb53b710d2706dd7708ebd459410972e9`  
		Last Modified: Wed, 18 Nov 2020 06:38:29 GMT  
		Size: 2.3 MB (2343744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46efa4ed6bcbf5bf3d31663a949f2737a3d614b5096ab406873383a7cef6c8a3`  
		Last Modified: Wed, 18 Nov 2020 06:38:28 GMT  
		Size: 1.1 MB (1123708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d179f1a7050b52b02a9d7bb384292ee10c93b3017e96fa476bed32e41c875e`  
		Last Modified: Tue, 24 Nov 2020 00:55:15 GMT  
		Size: 148.5 MB (148515408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820ceae080724c9a843ea752e54a4a92408fe3857e749b7f95a768454dbc394e`  
		Last Modified: Tue, 24 Nov 2020 00:54:39 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a1f6019a8f804c30926c45697d06bbba98ca87266a1d378ff01609fde81d6e`  
		Last Modified: Tue, 24 Nov 2020 00:54:39 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3384599ebc1ebaba6b586efdef2e3363b37659431d5754c3e566cbc32ab9bbe4`  
		Last Modified: Tue, 24 Nov 2020 00:54:39 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3acc520f2e865831068156e54cd167a36d0c6031995f600bbfabc3f6c817469`  
		Last Modified: Tue, 24 Nov 2020 00:54:39 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:88fe298a95bb93f455a3d4489aa1a8c7b264d106a00c199f6be75b8b332d6e93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:bfc01dbb6a49576ac88aca664bf59fe2afc0a1bba94743699c49a11acf0a4cd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.2 MB (386168233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20ab96138129f3a8c9f0bcabf32a0b12118fa168d6a46d915095e65a6d459b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:26:23 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 18 Nov 2020 06:26:24 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 18 Nov 2020 06:26:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 06:31:23 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 18 Nov 2020 06:31:29 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:31:34 GMT
RUN npm install -g rtlcss
# Wed, 18 Nov 2020 06:31:34 GMT
ENV ODOO_VERSION=13.0
# Tue, 24 Nov 2020 00:51:32 GMT
ARG ODOO_RELEASE=20201123
# Tue, 24 Nov 2020 00:51:33 GMT
ARG ODOO_SHA=1af64956f215ba0a2991ac6c86b98610c480c17b
# Tue, 24 Nov 2020 00:52:33 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=1af64956f215ba0a2991ac6c86b98610c480c17b
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 24 Nov 2020 00:52:34 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 24 Nov 2020 00:52:34 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 24 Nov 2020 00:52:35 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=1af64956f215ba0a2991ac6c86b98610c480c17b
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 24 Nov 2020 00:52:36 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 24 Nov 2020 00:52:36 GMT
EXPOSE 8069 8071 8072
# Tue, 24 Nov 2020 00:52:36 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 24 Nov 2020 00:52:36 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 24 Nov 2020 00:52:36 GMT
USER odoo
# Tue, 24 Nov 2020 00:52:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 24 Nov 2020 00:52:37 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c783d4a932f38653fa5103b08d8864e5e286a4d09e52582cca80c2a130b2df`  
		Last Modified: Wed, 18 Nov 2020 06:39:05 GMT  
		Size: 207.1 MB (207077490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1198c7d9e40b780e43f9dd77c39e0c2cb53b710d2706dd7708ebd459410972e9`  
		Last Modified: Wed, 18 Nov 2020 06:38:29 GMT  
		Size: 2.3 MB (2343744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46efa4ed6bcbf5bf3d31663a949f2737a3d614b5096ab406873383a7cef6c8a3`  
		Last Modified: Wed, 18 Nov 2020 06:38:28 GMT  
		Size: 1.1 MB (1123708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d179f1a7050b52b02a9d7bb384292ee10c93b3017e96fa476bed32e41c875e`  
		Last Modified: Tue, 24 Nov 2020 00:55:15 GMT  
		Size: 148.5 MB (148515408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820ceae080724c9a843ea752e54a4a92408fe3857e749b7f95a768454dbc394e`  
		Last Modified: Tue, 24 Nov 2020 00:54:39 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a1f6019a8f804c30926c45697d06bbba98ca87266a1d378ff01609fde81d6e`  
		Last Modified: Tue, 24 Nov 2020 00:54:39 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3384599ebc1ebaba6b586efdef2e3363b37659431d5754c3e566cbc32ab9bbe4`  
		Last Modified: Tue, 24 Nov 2020 00:54:39 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3acc520f2e865831068156e54cd167a36d0c6031995f600bbfabc3f6c817469`  
		Last Modified: Tue, 24 Nov 2020 00:54:39 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:7889037d626ee226e21b956474b9b0c04ab3aa7d9a01228fed08062ee58f45d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:ac884a5f7166600a3cecf7fd95aa6ffbacd989e98a0483ff59f0e542c6a84f76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403277844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8363e01420b14f57c3634d1998a67fd98e5fa7df68eb4c5d210f5b14772efbc1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:26:23 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 18 Nov 2020 06:26:24 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 18 Nov 2020 06:26:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 06:28:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 18 Nov 2020 06:28:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:28:24 GMT
RUN npm install -g rtlcss
# Wed, 18 Nov 2020 06:28:24 GMT
ENV ODOO_VERSION=14.0
# Tue, 24 Nov 2020 00:50:28 GMT
ARG ODOO_RELEASE=20201123
# Tue, 24 Nov 2020 00:50:28 GMT
ARG ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
# Tue, 24 Nov 2020 00:51:24 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 24 Nov 2020 00:51:25 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 24 Nov 2020 00:51:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 24 Nov 2020 00:51:26 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 24 Nov 2020 00:51:27 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 24 Nov 2020 00:51:27 GMT
EXPOSE 8069 8071 8072
# Tue, 24 Nov 2020 00:51:27 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 24 Nov 2020 00:51:27 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 24 Nov 2020 00:51:27 GMT
USER odoo
# Tue, 24 Nov 2020 00:51:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 24 Nov 2020 00:51:28 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9f15f1287f3c33a7386fc4db89367a1bf2b0176e5652a9f2528a8a0db43473`  
		Last Modified: Wed, 18 Nov 2020 06:38:20 GMT  
		Size: 213.1 MB (213118132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de1b21a1ad400a20f2ccf8539b0c965f9d2762f4de39c4646b95b631b52066d`  
		Last Modified: Wed, 18 Nov 2020 06:37:42 GMT  
		Size: 2.3 MB (2346385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe648d082dcfa3a00b257cade6256af02e9e4f2f070eb8fa3f124fd9d4de40`  
		Last Modified: Wed, 18 Nov 2020 06:37:41 GMT  
		Size: 1.1 MB (1123493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dda9173147ac3ce3f76bc56a583c24691348f936b9bfc96f55013f2339351d`  
		Last Modified: Tue, 24 Nov 2020 00:54:32 GMT  
		Size: 159.6 MB (159581948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020e9ea6a75b592d63282cf7b751fd15b99a0be5eec6b6e69dd0efd0e32f8324`  
		Last Modified: Tue, 24 Nov 2020 00:53:58 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a205c7662c9bedcb581b00da4ff7b25122c74ec41b5f9ed1f65c064bb73aadb9`  
		Last Modified: Tue, 24 Nov 2020 00:53:59 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b3e944bdd34743c74f801f9033426547493bdfb0e6d5e1f9afc34210a34d2b`  
		Last Modified: Tue, 24 Nov 2020 00:53:59 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bafa32d6e7a434c652194a541f4d3516409542bea9eb2b4db3a5168f839b70`  
		Last Modified: Tue, 24 Nov 2020 00:53:58 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:7889037d626ee226e21b956474b9b0c04ab3aa7d9a01228fed08062ee58f45d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:ac884a5f7166600a3cecf7fd95aa6ffbacd989e98a0483ff59f0e542c6a84f76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403277844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8363e01420b14f57c3634d1998a67fd98e5fa7df68eb4c5d210f5b14772efbc1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:26:23 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 18 Nov 2020 06:26:24 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 18 Nov 2020 06:26:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 06:28:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 18 Nov 2020 06:28:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:28:24 GMT
RUN npm install -g rtlcss
# Wed, 18 Nov 2020 06:28:24 GMT
ENV ODOO_VERSION=14.0
# Tue, 24 Nov 2020 00:50:28 GMT
ARG ODOO_RELEASE=20201123
# Tue, 24 Nov 2020 00:50:28 GMT
ARG ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
# Tue, 24 Nov 2020 00:51:24 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 24 Nov 2020 00:51:25 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 24 Nov 2020 00:51:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 24 Nov 2020 00:51:26 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 24 Nov 2020 00:51:27 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 24 Nov 2020 00:51:27 GMT
EXPOSE 8069 8071 8072
# Tue, 24 Nov 2020 00:51:27 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 24 Nov 2020 00:51:27 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 24 Nov 2020 00:51:27 GMT
USER odoo
# Tue, 24 Nov 2020 00:51:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 24 Nov 2020 00:51:28 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9f15f1287f3c33a7386fc4db89367a1bf2b0176e5652a9f2528a8a0db43473`  
		Last Modified: Wed, 18 Nov 2020 06:38:20 GMT  
		Size: 213.1 MB (213118132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de1b21a1ad400a20f2ccf8539b0c965f9d2762f4de39c4646b95b631b52066d`  
		Last Modified: Wed, 18 Nov 2020 06:37:42 GMT  
		Size: 2.3 MB (2346385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe648d082dcfa3a00b257cade6256af02e9e4f2f070eb8fa3f124fd9d4de40`  
		Last Modified: Wed, 18 Nov 2020 06:37:41 GMT  
		Size: 1.1 MB (1123493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dda9173147ac3ce3f76bc56a583c24691348f936b9bfc96f55013f2339351d`  
		Last Modified: Tue, 24 Nov 2020 00:54:32 GMT  
		Size: 159.6 MB (159581948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020e9ea6a75b592d63282cf7b751fd15b99a0be5eec6b6e69dd0efd0e32f8324`  
		Last Modified: Tue, 24 Nov 2020 00:53:58 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a205c7662c9bedcb581b00da4ff7b25122c74ec41b5f9ed1f65c064bb73aadb9`  
		Last Modified: Tue, 24 Nov 2020 00:53:59 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b3e944bdd34743c74f801f9033426547493bdfb0e6d5e1f9afc34210a34d2b`  
		Last Modified: Tue, 24 Nov 2020 00:53:59 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bafa32d6e7a434c652194a541f4d3516409542bea9eb2b4db3a5168f839b70`  
		Last Modified: Tue, 24 Nov 2020 00:53:58 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:7889037d626ee226e21b956474b9b0c04ab3aa7d9a01228fed08062ee58f45d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:ac884a5f7166600a3cecf7fd95aa6ffbacd989e98a0483ff59f0e542c6a84f76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403277844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8363e01420b14f57c3634d1998a67fd98e5fa7df68eb4c5d210f5b14772efbc1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:26:23 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 18 Nov 2020 06:26:24 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 18 Nov 2020 06:26:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 06:28:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 18 Nov 2020 06:28:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:28:24 GMT
RUN npm install -g rtlcss
# Wed, 18 Nov 2020 06:28:24 GMT
ENV ODOO_VERSION=14.0
# Tue, 24 Nov 2020 00:50:28 GMT
ARG ODOO_RELEASE=20201123
# Tue, 24 Nov 2020 00:50:28 GMT
ARG ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
# Tue, 24 Nov 2020 00:51:24 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 24 Nov 2020 00:51:25 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 24 Nov 2020 00:51:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 24 Nov 2020 00:51:26 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 24 Nov 2020 00:51:27 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 24 Nov 2020 00:51:27 GMT
EXPOSE 8069 8071 8072
# Tue, 24 Nov 2020 00:51:27 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 24 Nov 2020 00:51:27 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 24 Nov 2020 00:51:27 GMT
USER odoo
# Tue, 24 Nov 2020 00:51:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 24 Nov 2020 00:51:28 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9f15f1287f3c33a7386fc4db89367a1bf2b0176e5652a9f2528a8a0db43473`  
		Last Modified: Wed, 18 Nov 2020 06:38:20 GMT  
		Size: 213.1 MB (213118132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de1b21a1ad400a20f2ccf8539b0c965f9d2762f4de39c4646b95b631b52066d`  
		Last Modified: Wed, 18 Nov 2020 06:37:42 GMT  
		Size: 2.3 MB (2346385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe648d082dcfa3a00b257cade6256af02e9e4f2f070eb8fa3f124fd9d4de40`  
		Last Modified: Wed, 18 Nov 2020 06:37:41 GMT  
		Size: 1.1 MB (1123493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dda9173147ac3ce3f76bc56a583c24691348f936b9bfc96f55013f2339351d`  
		Last Modified: Tue, 24 Nov 2020 00:54:32 GMT  
		Size: 159.6 MB (159581948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020e9ea6a75b592d63282cf7b751fd15b99a0be5eec6b6e69dd0efd0e32f8324`  
		Last Modified: Tue, 24 Nov 2020 00:53:58 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a205c7662c9bedcb581b00da4ff7b25122c74ec41b5f9ed1f65c064bb73aadb9`  
		Last Modified: Tue, 24 Nov 2020 00:53:59 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b3e944bdd34743c74f801f9033426547493bdfb0e6d5e1f9afc34210a34d2b`  
		Last Modified: Tue, 24 Nov 2020 00:53:59 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bafa32d6e7a434c652194a541f4d3516409542bea9eb2b4db3a5168f839b70`  
		Last Modified: Tue, 24 Nov 2020 00:53:58 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
