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
$ docker pull odoo@sha256:57017b926dcceefae8046ebaafe3d71dfbc10d84396a6c1cacde5b8ad24f8b19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:9e8418a3437e05fdc5a56310d8a150beb8be327100c123b59e498bf58a0d6585
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.7 MB (396666959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a437a1c91628965541485f68f06ebf9f0d47ba89573fae2335cf65e8eeb07e08`
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
# Wed, 18 Nov 2020 06:36:34 GMT
ARG ODOO_RELEASE=20201112
# Wed, 18 Nov 2020 06:36:35 GMT
ARG ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
# Wed, 18 Nov 2020 06:37:20 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 18 Nov 2020 06:37:21 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 18 Nov 2020 06:37:21 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 18 Nov 2020 06:37:22 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 18 Nov 2020 06:37:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 18 Nov 2020 06:37:23 GMT
EXPOSE 8069 8071 8072
# Wed, 18 Nov 2020 06:37:23 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 18 Nov 2020 06:37:23 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 18 Nov 2020 06:37:23 GMT
USER odoo
# Wed, 18 Nov 2020 06:37:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 06:37:24 GMT
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
	-	`sha256:0736efc84cbd24ec126b42fb40b44e9f0633ee62c7a73184eb4271ec0a788c91`  
		Last Modified: Wed, 18 Nov 2020 06:39:52 GMT  
		Size: 130.0 MB (130029967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b90d0c0301052f720910ce2b46184127dbfacc02f8d0eab39a2ae1f2f0f130b`  
		Last Modified: Wed, 18 Nov 2020 06:39:20 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a14a1726235cf122a6fafe0fcb53ca0b476c88949b670f60913533524bc56e`  
		Last Modified: Wed, 18 Nov 2020 06:39:20 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a71e54b9806c338f6fab8f3802c4ec4f95b43d65786a8e0e0f02613be0180d`  
		Last Modified: Wed, 18 Nov 2020 06:39:20 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223394d951eac2631cb985e5fb57e8f7264ebae2085c9af224a83daf151c2f4e`  
		Last Modified: Wed, 18 Nov 2020 06:39:20 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:57017b926dcceefae8046ebaafe3d71dfbc10d84396a6c1cacde5b8ad24f8b19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:9e8418a3437e05fdc5a56310d8a150beb8be327100c123b59e498bf58a0d6585
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.7 MB (396666959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a437a1c91628965541485f68f06ebf9f0d47ba89573fae2335cf65e8eeb07e08`
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
# Wed, 18 Nov 2020 06:36:34 GMT
ARG ODOO_RELEASE=20201112
# Wed, 18 Nov 2020 06:36:35 GMT
ARG ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
# Wed, 18 Nov 2020 06:37:20 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 18 Nov 2020 06:37:21 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 18 Nov 2020 06:37:21 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 18 Nov 2020 06:37:22 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=9f0b063fa41a15410fec4afcc513a1e27c1150fa
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 18 Nov 2020 06:37:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 18 Nov 2020 06:37:23 GMT
EXPOSE 8069 8071 8072
# Wed, 18 Nov 2020 06:37:23 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 18 Nov 2020 06:37:23 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 18 Nov 2020 06:37:23 GMT
USER odoo
# Wed, 18 Nov 2020 06:37:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 06:37:24 GMT
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
	-	`sha256:0736efc84cbd24ec126b42fb40b44e9f0633ee62c7a73184eb4271ec0a788c91`  
		Last Modified: Wed, 18 Nov 2020 06:39:52 GMT  
		Size: 130.0 MB (130029967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b90d0c0301052f720910ce2b46184127dbfacc02f8d0eab39a2ae1f2f0f130b`  
		Last Modified: Wed, 18 Nov 2020 06:39:20 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a14a1726235cf122a6fafe0fcb53ca0b476c88949b670f60913533524bc56e`  
		Last Modified: Wed, 18 Nov 2020 06:39:20 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a71e54b9806c338f6fab8f3802c4ec4f95b43d65786a8e0e0f02613be0180d`  
		Last Modified: Wed, 18 Nov 2020 06:39:20 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223394d951eac2631cb985e5fb57e8f7264ebae2085c9af224a83daf151c2f4e`  
		Last Modified: Wed, 18 Nov 2020 06:39:20 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:97d2059d36e8d05380521cfe1a297ebbcd8b8fe3d2a6210ff7e9753a8719c592
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:2cd2b4c32d82ace42211e65a43c4853bc44f17a52269d96d2088483e392ca2d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386077149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1eed4f7ba9183f076ef82fa8fbbe0222cf19dcc0dbb3471c6dfa3226f25bb87`
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
# Wed, 18 Nov 2020 06:31:34 GMT
ARG ODOO_RELEASE=20201112
# Wed, 18 Nov 2020 06:31:34 GMT
ARG ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
# Wed, 18 Nov 2020 06:33:01 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 18 Nov 2020 06:33:03 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 18 Nov 2020 06:33:03 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 18 Nov 2020 06:33:05 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 18 Nov 2020 06:33:06 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 18 Nov 2020 06:33:06 GMT
EXPOSE 8069 8071 8072
# Wed, 18 Nov 2020 06:33:06 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 18 Nov 2020 06:33:07 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 18 Nov 2020 06:33:07 GMT
USER odoo
# Wed, 18 Nov 2020 06:33:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 06:33:08 GMT
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
	-	`sha256:73f993f10c50051da6707bd15526bdc3eeaf9fd22c138a81fe82872c5f4de5a3`  
		Last Modified: Wed, 18 Nov 2020 06:39:09 GMT  
		Size: 148.4 MB (148424316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f3b90669cd082ca8359255e98e4253e8da4e61ca6efd55f3e7239c8ee2e1c3`  
		Last Modified: Wed, 18 Nov 2020 06:38:27 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f746c059df0fd954c6335f7f9426cbc29eb9a05545d8fbc57c74ba6d829b1f31`  
		Last Modified: Wed, 18 Nov 2020 06:38:27 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ade187efae51ac7fd3aaa46465630379c1ab8ba97469fa8bc3070af0ffb4bf8`  
		Last Modified: Wed, 18 Nov 2020 06:38:26 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c03262a4548ca4ae7d6dec931f9243597d6001b207e81d8c033bb70f307bb`  
		Last Modified: Wed, 18 Nov 2020 06:38:27 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:97d2059d36e8d05380521cfe1a297ebbcd8b8fe3d2a6210ff7e9753a8719c592
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:2cd2b4c32d82ace42211e65a43c4853bc44f17a52269d96d2088483e392ca2d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386077149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1eed4f7ba9183f076ef82fa8fbbe0222cf19dcc0dbb3471c6dfa3226f25bb87`
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
# Wed, 18 Nov 2020 06:31:34 GMT
ARG ODOO_RELEASE=20201112
# Wed, 18 Nov 2020 06:31:34 GMT
ARG ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
# Wed, 18 Nov 2020 06:33:01 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 18 Nov 2020 06:33:03 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 18 Nov 2020 06:33:03 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 18 Nov 2020 06:33:05 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=5658d799122aac82ab07dc55e6af28a35adda3ea
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 18 Nov 2020 06:33:06 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 18 Nov 2020 06:33:06 GMT
EXPOSE 8069 8071 8072
# Wed, 18 Nov 2020 06:33:06 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 18 Nov 2020 06:33:07 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 18 Nov 2020 06:33:07 GMT
USER odoo
# Wed, 18 Nov 2020 06:33:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 06:33:08 GMT
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
	-	`sha256:73f993f10c50051da6707bd15526bdc3eeaf9fd22c138a81fe82872c5f4de5a3`  
		Last Modified: Wed, 18 Nov 2020 06:39:09 GMT  
		Size: 148.4 MB (148424316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f3b90669cd082ca8359255e98e4253e8da4e61ca6efd55f3e7239c8ee2e1c3`  
		Last Modified: Wed, 18 Nov 2020 06:38:27 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f746c059df0fd954c6335f7f9426cbc29eb9a05545d8fbc57c74ba6d829b1f31`  
		Last Modified: Wed, 18 Nov 2020 06:38:27 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ade187efae51ac7fd3aaa46465630379c1ab8ba97469fa8bc3070af0ffb4bf8`  
		Last Modified: Wed, 18 Nov 2020 06:38:26 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217c03262a4548ca4ae7d6dec931f9243597d6001b207e81d8c033bb70f307bb`  
		Last Modified: Wed, 18 Nov 2020 06:38:27 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:585c91e81923e5dc9ac613df12a9e7f50447a9e483c1296b6be7a96dcaa951e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:59ad672d555085eee5b505a55893ef5936b4f1e9033e448c1c31ec9280e8549f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.0 MB (401991478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c21f4d0287ede36cdb23b4027b60035bf8008fa5fe36d71e63e8822c5b6074`
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
# Wed, 18 Nov 2020 06:28:25 GMT
ARG ODOO_RELEASE=20201112
# Wed, 18 Nov 2020 06:28:25 GMT
ARG ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
# Wed, 18 Nov 2020 06:29:53 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 18 Nov 2020 06:29:54 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 18 Nov 2020 06:29:54 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 18 Nov 2020 06:29:55 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 18 Nov 2020 06:29:55 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 18 Nov 2020 06:29:55 GMT
EXPOSE 8069 8071 8072
# Wed, 18 Nov 2020 06:29:56 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 18 Nov 2020 06:29:56 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 18 Nov 2020 06:29:56 GMT
USER odoo
# Wed, 18 Nov 2020 06:29:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 06:29:57 GMT
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
	-	`sha256:69b6302a229e9772d714114c0fa9ad72852c4753dfa0e2df81a4109f3df2a6e0`  
		Last Modified: Wed, 18 Nov 2020 06:38:16 GMT  
		Size: 158.3 MB (158295585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b61732438e157d757b4813cc6db99dbab2eb72c26692a88741c248e907397b4`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea74207933b3857f9426a552f7e679ea661d6357969e642eb5162276b7ccbd22`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7a7aba287024d649a29d3d71b9730602ba4b46f47f5e377e5a8c4447d81f4f`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a369b10b957ee42a6b56c2460dda0e3a9d4822f82305473830e44f6ae8cbcdc`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:585c91e81923e5dc9ac613df12a9e7f50447a9e483c1296b6be7a96dcaa951e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:59ad672d555085eee5b505a55893ef5936b4f1e9033e448c1c31ec9280e8549f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.0 MB (401991478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c21f4d0287ede36cdb23b4027b60035bf8008fa5fe36d71e63e8822c5b6074`
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
# Wed, 18 Nov 2020 06:28:25 GMT
ARG ODOO_RELEASE=20201112
# Wed, 18 Nov 2020 06:28:25 GMT
ARG ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
# Wed, 18 Nov 2020 06:29:53 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 18 Nov 2020 06:29:54 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 18 Nov 2020 06:29:54 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 18 Nov 2020 06:29:55 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 18 Nov 2020 06:29:55 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 18 Nov 2020 06:29:55 GMT
EXPOSE 8069 8071 8072
# Wed, 18 Nov 2020 06:29:56 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 18 Nov 2020 06:29:56 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 18 Nov 2020 06:29:56 GMT
USER odoo
# Wed, 18 Nov 2020 06:29:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 06:29:57 GMT
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
	-	`sha256:69b6302a229e9772d714114c0fa9ad72852c4753dfa0e2df81a4109f3df2a6e0`  
		Last Modified: Wed, 18 Nov 2020 06:38:16 GMT  
		Size: 158.3 MB (158295585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b61732438e157d757b4813cc6db99dbab2eb72c26692a88741c248e907397b4`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea74207933b3857f9426a552f7e679ea661d6357969e642eb5162276b7ccbd22`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7a7aba287024d649a29d3d71b9730602ba4b46f47f5e377e5a8c4447d81f4f`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a369b10b957ee42a6b56c2460dda0e3a9d4822f82305473830e44f6ae8cbcdc`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:585c91e81923e5dc9ac613df12a9e7f50447a9e483c1296b6be7a96dcaa951e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:59ad672d555085eee5b505a55893ef5936b4f1e9033e448c1c31ec9280e8549f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.0 MB (401991478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c21f4d0287ede36cdb23b4027b60035bf8008fa5fe36d71e63e8822c5b6074`
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
# Wed, 18 Nov 2020 06:28:25 GMT
ARG ODOO_RELEASE=20201112
# Wed, 18 Nov 2020 06:28:25 GMT
ARG ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
# Wed, 18 Nov 2020 06:29:53 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 18 Nov 2020 06:29:54 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 18 Nov 2020 06:29:54 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 18 Nov 2020 06:29:55 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 18 Nov 2020 06:29:55 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 18 Nov 2020 06:29:55 GMT
EXPOSE 8069 8071 8072
# Wed, 18 Nov 2020 06:29:56 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 18 Nov 2020 06:29:56 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 18 Nov 2020 06:29:56 GMT
USER odoo
# Wed, 18 Nov 2020 06:29:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 06:29:57 GMT
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
	-	`sha256:69b6302a229e9772d714114c0fa9ad72852c4753dfa0e2df81a4109f3df2a6e0`  
		Last Modified: Wed, 18 Nov 2020 06:38:16 GMT  
		Size: 158.3 MB (158295585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b61732438e157d757b4813cc6db99dbab2eb72c26692a88741c248e907397b4`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea74207933b3857f9426a552f7e679ea661d6357969e642eb5162276b7ccbd22`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7a7aba287024d649a29d3d71b9730602ba4b46f47f5e377e5a8c4447d81f4f`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a369b10b957ee42a6b56c2460dda0e3a9d4822f82305473830e44f6ae8cbcdc`  
		Last Modified: Wed, 18 Nov 2020 06:37:39 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
