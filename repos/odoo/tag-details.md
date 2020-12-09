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
$ docker pull odoo@sha256:fea533fce2028a3d82856fd6d6f0b19afa768fddc23f94b1c1411132dab42be7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:bd4551b1271847638697c929a6247c6211d5427cbc0d6068f6258645edcad290
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.9 MB (396898576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2649710975f366c1f9652404511899a7bae38abf45678519dff4420e70fa030b`
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
# Wed, 09 Dec 2020 04:30:41 GMT
ARG ODOO_RELEASE=20201208
# Wed, 09 Dec 2020 04:30:41 GMT
ARG ODOO_SHA=9b055f129756442f58fce0b3d819be4a0e61709e
# Wed, 09 Dec 2020 04:31:51 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=9b055f129756442f58fce0b3d819be4a0e61709e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Dec 2020 04:31:53 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Dec 2020 04:31:53 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Dec 2020 04:31:55 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=9b055f129756442f58fce0b3d819be4a0e61709e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Dec 2020 04:31:55 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Dec 2020 04:31:56 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Dec 2020 04:31:56 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Dec 2020 04:31:56 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Dec 2020 04:31:57 GMT
USER odoo
# Wed, 09 Dec 2020 04:31:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Dec 2020 04:31:57 GMT
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
	-	`sha256:b25f0d529e3f72d6b9ed3759c6d936ca54afce012cee67667ba00f1cab381b58`  
		Last Modified: Wed, 09 Dec 2020 04:34:51 GMT  
		Size: 130.3 MB (130261581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e708ec5b10c2f222f7c0cd35637dd58d2a1d8abb14822abd6066936eba8d34`  
		Last Modified: Wed, 09 Dec 2020 04:34:21 GMT  
		Size: 673.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47468ac3f917136ff65bc51084c565abb96ebb713b6353ab0f04a0603167aa9c`  
		Last Modified: Wed, 09 Dec 2020 04:34:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482c5f18de65e4f5df025d806353273bb4b03d3641c9e04ce429534771ffab57`  
		Last Modified: Wed, 09 Dec 2020 04:34:21 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8645bb3d942be3af62214fbd278da8a87a4ea5fb934650419c38db202e30cb72`  
		Last Modified: Wed, 09 Dec 2020 04:34:20 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:fea533fce2028a3d82856fd6d6f0b19afa768fddc23f94b1c1411132dab42be7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:bd4551b1271847638697c929a6247c6211d5427cbc0d6068f6258645edcad290
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.9 MB (396898576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2649710975f366c1f9652404511899a7bae38abf45678519dff4420e70fa030b`
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
# Wed, 09 Dec 2020 04:30:41 GMT
ARG ODOO_RELEASE=20201208
# Wed, 09 Dec 2020 04:30:41 GMT
ARG ODOO_SHA=9b055f129756442f58fce0b3d819be4a0e61709e
# Wed, 09 Dec 2020 04:31:51 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=9b055f129756442f58fce0b3d819be4a0e61709e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Dec 2020 04:31:53 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Dec 2020 04:31:53 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Dec 2020 04:31:55 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=9b055f129756442f58fce0b3d819be4a0e61709e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Dec 2020 04:31:55 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Dec 2020 04:31:56 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Dec 2020 04:31:56 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Dec 2020 04:31:56 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Dec 2020 04:31:57 GMT
USER odoo
# Wed, 09 Dec 2020 04:31:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Dec 2020 04:31:57 GMT
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
	-	`sha256:b25f0d529e3f72d6b9ed3759c6d936ca54afce012cee67667ba00f1cab381b58`  
		Last Modified: Wed, 09 Dec 2020 04:34:51 GMT  
		Size: 130.3 MB (130261581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e708ec5b10c2f222f7c0cd35637dd58d2a1d8abb14822abd6066936eba8d34`  
		Last Modified: Wed, 09 Dec 2020 04:34:21 GMT  
		Size: 673.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47468ac3f917136ff65bc51084c565abb96ebb713b6353ab0f04a0603167aa9c`  
		Last Modified: Wed, 09 Dec 2020 04:34:21 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482c5f18de65e4f5df025d806353273bb4b03d3641c9e04ce429534771ffab57`  
		Last Modified: Wed, 09 Dec 2020 04:34:21 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8645bb3d942be3af62214fbd278da8a87a4ea5fb934650419c38db202e30cb72`  
		Last Modified: Wed, 09 Dec 2020 04:34:20 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:7dd3a35ca65901daadf23cceaaccf2272eb5a6aedcffdd6829a1d452f49311c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:d6d4a7f387b0dfc61a91d05a17b4b3996b5f1e6ce386d3713a0419e3da740bee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.4 MB (386444490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca7856e6813aefa4b4b4fe956c409e58a099ae39b908f54dd38b6fb33cccdc2`
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
# Wed, 09 Dec 2020 04:28:53 GMT
ARG ODOO_RELEASE=20201208
# Wed, 09 Dec 2020 04:28:54 GMT
ARG ODOO_SHA=acb26cf02f554009ba99510acc5631d29616dd10
# Wed, 09 Dec 2020 04:30:16 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=acb26cf02f554009ba99510acc5631d29616dd10
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Dec 2020 04:30:18 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Dec 2020 04:30:19 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Dec 2020 04:30:21 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=acb26cf02f554009ba99510acc5631d29616dd10
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Dec 2020 04:30:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Dec 2020 04:30:21 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Dec 2020 04:30:22 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Dec 2020 04:30:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Dec 2020 04:30:22 GMT
USER odoo
# Wed, 09 Dec 2020 04:30:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Dec 2020 04:30:23 GMT
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
	-	`sha256:8c25e4a79956d2c668feedc7ee1c63df652cfe94217efe1ee57c45ca8801e192`  
		Last Modified: Wed, 09 Dec 2020 04:34:15 GMT  
		Size: 148.8 MB (148791661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d97fdd908d9fbd80924bcded775e24080656382a87eb32147518be9bda9a5`  
		Last Modified: Wed, 09 Dec 2020 04:33:30 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43baa92f88ab74712670cba8ca4cbb490d95db0cac8c1f1a3a29405a410080b`  
		Last Modified: Wed, 09 Dec 2020 04:33:30 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e3015ee4017880ae3ce71d33c71ccc259d694cef0e1224ec940eb9ffdda4bc`  
		Last Modified: Wed, 09 Dec 2020 04:33:30 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe26b417fab01f7f46783cbdc3fceb4c1ccd6f0cadde839403cb4314d19140a`  
		Last Modified: Wed, 09 Dec 2020 04:33:30 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:7dd3a35ca65901daadf23cceaaccf2272eb5a6aedcffdd6829a1d452f49311c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:d6d4a7f387b0dfc61a91d05a17b4b3996b5f1e6ce386d3713a0419e3da740bee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.4 MB (386444490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca7856e6813aefa4b4b4fe956c409e58a099ae39b908f54dd38b6fb33cccdc2`
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
# Wed, 09 Dec 2020 04:28:53 GMT
ARG ODOO_RELEASE=20201208
# Wed, 09 Dec 2020 04:28:54 GMT
ARG ODOO_SHA=acb26cf02f554009ba99510acc5631d29616dd10
# Wed, 09 Dec 2020 04:30:16 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=acb26cf02f554009ba99510acc5631d29616dd10
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Dec 2020 04:30:18 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Dec 2020 04:30:19 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Dec 2020 04:30:21 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=acb26cf02f554009ba99510acc5631d29616dd10
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Dec 2020 04:30:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Dec 2020 04:30:21 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Dec 2020 04:30:22 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Dec 2020 04:30:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Dec 2020 04:30:22 GMT
USER odoo
# Wed, 09 Dec 2020 04:30:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Dec 2020 04:30:23 GMT
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
	-	`sha256:8c25e4a79956d2c668feedc7ee1c63df652cfe94217efe1ee57c45ca8801e192`  
		Last Modified: Wed, 09 Dec 2020 04:34:15 GMT  
		Size: 148.8 MB (148791661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d97fdd908d9fbd80924bcded775e24080656382a87eb32147518be9bda9a5`  
		Last Modified: Wed, 09 Dec 2020 04:33:30 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43baa92f88ab74712670cba8ca4cbb490d95db0cac8c1f1a3a29405a410080b`  
		Last Modified: Wed, 09 Dec 2020 04:33:30 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e3015ee4017880ae3ce71d33c71ccc259d694cef0e1224ec940eb9ffdda4bc`  
		Last Modified: Wed, 09 Dec 2020 04:33:30 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe26b417fab01f7f46783cbdc3fceb4c1ccd6f0cadde839403cb4314d19140a`  
		Last Modified: Wed, 09 Dec 2020 04:33:30 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:1f54097985f4a85b4a86f7d121d26938ed663983cb563b9edbaea5ada7310e28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:e6ce38cbfe42d319c472e9cb191c7bda1d204a6f1e0c06a312d2affff273f9c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.4 MB (404417418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8336349dcd3487c36812156094b29fc04e9cadc66a0e2fe0b5acb23ddcac25ee`
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
# Wed, 09 Dec 2020 04:27:05 GMT
ARG ODOO_RELEASE=20201208
# Wed, 09 Dec 2020 04:27:05 GMT
ARG ODOO_SHA=37dd5d71d5b8439fddf88d7e161cc3502721c4b5
# Wed, 09 Dec 2020 04:28:28 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=37dd5d71d5b8439fddf88d7e161cc3502721c4b5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Dec 2020 04:28:30 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Dec 2020 04:28:30 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Dec 2020 04:28:32 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=37dd5d71d5b8439fddf88d7e161cc3502721c4b5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Dec 2020 04:28:32 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Dec 2020 04:28:33 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Dec 2020 04:28:33 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Dec 2020 04:28:33 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Dec 2020 04:28:34 GMT
USER odoo
# Wed, 09 Dec 2020 04:28:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Dec 2020 04:28:34 GMT
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
	-	`sha256:8757beca99a0b8de9fe8307d45f13857dacde43752d9f90ff8630ed5d9a9f1fc`  
		Last Modified: Wed, 09 Dec 2020 04:33:22 GMT  
		Size: 160.7 MB (160721521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27bcfc5dfd7c0a97e9ea752f840f87cb0253a90111e40d846d649aa270df623`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbf81abaaf2b969dd75fc8680704a9d4cfb7fa340dbb8e2b030d333b76ef981`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b81b945890cdb369b4c9bfb51e8313ce842424c683df6732fa003736e7eca3`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e119dd0d61159aeeb3a4907d4609a4ded06b23f7bc4c88bba69892d3b168bc`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:1f54097985f4a85b4a86f7d121d26938ed663983cb563b9edbaea5ada7310e28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:e6ce38cbfe42d319c472e9cb191c7bda1d204a6f1e0c06a312d2affff273f9c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.4 MB (404417418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8336349dcd3487c36812156094b29fc04e9cadc66a0e2fe0b5acb23ddcac25ee`
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
# Wed, 09 Dec 2020 04:27:05 GMT
ARG ODOO_RELEASE=20201208
# Wed, 09 Dec 2020 04:27:05 GMT
ARG ODOO_SHA=37dd5d71d5b8439fddf88d7e161cc3502721c4b5
# Wed, 09 Dec 2020 04:28:28 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=37dd5d71d5b8439fddf88d7e161cc3502721c4b5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Dec 2020 04:28:30 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Dec 2020 04:28:30 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Dec 2020 04:28:32 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=37dd5d71d5b8439fddf88d7e161cc3502721c4b5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Dec 2020 04:28:32 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Dec 2020 04:28:33 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Dec 2020 04:28:33 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Dec 2020 04:28:33 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Dec 2020 04:28:34 GMT
USER odoo
# Wed, 09 Dec 2020 04:28:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Dec 2020 04:28:34 GMT
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
	-	`sha256:8757beca99a0b8de9fe8307d45f13857dacde43752d9f90ff8630ed5d9a9f1fc`  
		Last Modified: Wed, 09 Dec 2020 04:33:22 GMT  
		Size: 160.7 MB (160721521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27bcfc5dfd7c0a97e9ea752f840f87cb0253a90111e40d846d649aa270df623`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbf81abaaf2b969dd75fc8680704a9d4cfb7fa340dbb8e2b030d333b76ef981`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b81b945890cdb369b4c9bfb51e8313ce842424c683df6732fa003736e7eca3`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e119dd0d61159aeeb3a4907d4609a4ded06b23f7bc4c88bba69892d3b168bc`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:1f54097985f4a85b4a86f7d121d26938ed663983cb563b9edbaea5ada7310e28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:e6ce38cbfe42d319c472e9cb191c7bda1d204a6f1e0c06a312d2affff273f9c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.4 MB (404417418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8336349dcd3487c36812156094b29fc04e9cadc66a0e2fe0b5acb23ddcac25ee`
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
# Wed, 09 Dec 2020 04:27:05 GMT
ARG ODOO_RELEASE=20201208
# Wed, 09 Dec 2020 04:27:05 GMT
ARG ODOO_SHA=37dd5d71d5b8439fddf88d7e161cc3502721c4b5
# Wed, 09 Dec 2020 04:28:28 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=37dd5d71d5b8439fddf88d7e161cc3502721c4b5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Dec 2020 04:28:30 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Dec 2020 04:28:30 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Dec 2020 04:28:32 GMT
# ARGS: ODOO_RELEASE=20201208 ODOO_SHA=37dd5d71d5b8439fddf88d7e161cc3502721c4b5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Dec 2020 04:28:32 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Dec 2020 04:28:33 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Dec 2020 04:28:33 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Dec 2020 04:28:33 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Dec 2020 04:28:34 GMT
USER odoo
# Wed, 09 Dec 2020 04:28:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Dec 2020 04:28:34 GMT
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
	-	`sha256:8757beca99a0b8de9fe8307d45f13857dacde43752d9f90ff8630ed5d9a9f1fc`  
		Last Modified: Wed, 09 Dec 2020 04:33:22 GMT  
		Size: 160.7 MB (160721521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27bcfc5dfd7c0a97e9ea752f840f87cb0253a90111e40d846d649aa270df623`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbf81abaaf2b969dd75fc8680704a9d4cfb7fa340dbb8e2b030d333b76ef981`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b81b945890cdb369b4c9bfb51e8313ce842424c683df6732fa003736e7eca3`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e119dd0d61159aeeb3a4907d4609a4ded06b23f7bc4c88bba69892d3b168bc`  
		Last Modified: Wed, 09 Dec 2020 04:32:23 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
