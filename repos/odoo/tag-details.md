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
$ docker pull odoo@sha256:ace1a6a26713e74a94c165c03aea89341e3177d57f80828421917d33011fe7b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:412fa6ed0024a6a807cb3c06125f7ce0c543e1965e6ec266a977eff5174bb549
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.6 MB (542574453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5eed6979a0268e19bc283f21475832a55a18c4d1ad6481a4d23b37f91da1fb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:55 GMT
ADD file:65a51da79ba9e2993b794078e3e24554bff59ac80185f12845c1426c7173f06f in / 
# Tue, 30 Mar 2021 21:50:55 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:33:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 31 Mar 2021 05:33:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 31 Mar 2021 05:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 05:33:52 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 31 Mar 2021 05:35:18 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 31 Mar 2021 05:35:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:35:41 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:35:42 GMT
ENV ODOO_VERSION=12.0
# Wed, 31 Mar 2021 05:35:42 GMT
ARG ODOO_RELEASE=20210329
# Wed, 31 Mar 2021 05:35:42 GMT
ARG ODOO_SHA=cd334511a519ec8b8fd3f4555171d17f94107b77
# Wed, 31 Mar 2021 05:36:47 GMT
# ARGS: ODOO_RELEASE=20210329 ODOO_SHA=cd334511a519ec8b8fd3f4555171d17f94107b77
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 31 Mar 2021 05:36:50 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 31 Mar 2021 05:36:51 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 31 Mar 2021 05:36:52 GMT
# ARGS: ODOO_RELEASE=20210329 ODOO_SHA=cd334511a519ec8b8fd3f4555171d17f94107b77
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 31 Mar 2021 05:36:52 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 31 Mar 2021 05:36:52 GMT
EXPOSE 8069 8071 8072
# Wed, 31 Mar 2021 05:36:52 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 31 Mar 2021 05:36:52 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 31 Mar 2021 05:36:52 GMT
USER odoo
# Wed, 31 Mar 2021 05:36:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 05:36:53 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:23a3602cd30cf5ce6da03e18c28bbbfdc12ae98f182462de8c55785a8d982431`  
		Last Modified: Tue, 30 Mar 2021 21:57:04 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c6915795ca8c7c8930ee76dd81824579247a9450e0bde952170b65c189cc05`  
		Last Modified: Wed, 31 Mar 2021 05:39:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d59774897a449e82a96dccda7da3a9181e64482d2a6670e5d96c91e27e83c1f`  
		Last Modified: Wed, 31 Mar 2021 05:39:30 GMT  
		Size: 219.7 MB (219658871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3f4875f05a0954aceee9441611ab9124140ed09e5366fe97dfe54fe35f8184`  
		Last Modified: Wed, 31 Mar 2021 05:39:01 GMT  
		Size: 2.2 MB (2224092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb531369e15e75947e95abf307ff62714c1f93d4f67ed947cd593d3056264ce`  
		Last Modified: Wed, 31 Mar 2021 05:39:06 GMT  
		Size: 22.0 MB (22042955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00873d1a12c8f7c34d0522b94175b40cd769ed30655f755b237bfa540e0d7326`  
		Last Modified: Wed, 31 Mar 2021 05:39:35 GMT  
		Size: 276.1 MB (276117606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b82b7deb1ef1568f3e301e74724e6f2100b9dd95f84d07138aedff3ac4a374f`  
		Last Modified: Wed, 31 Mar 2021 05:38:59 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb677ea011b6e3f37c083cd4a0cb44dc95e6588738c2c9dc28a1b938d64e0138`  
		Last Modified: Wed, 31 Mar 2021 05:38:58 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd3d4c0600a9b16d3897fb7d406cb0c71b355fafe64821c76e297fcfd9340d3`  
		Last Modified: Wed, 31 Mar 2021 05:38:58 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa68d081a73ef2045ecb590084a22e447dc01087d31de3b7d455684f3067117b`  
		Last Modified: Wed, 31 Mar 2021 05:38:58 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:ace1a6a26713e74a94c165c03aea89341e3177d57f80828421917d33011fe7b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:412fa6ed0024a6a807cb3c06125f7ce0c543e1965e6ec266a977eff5174bb549
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.6 MB (542574453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5eed6979a0268e19bc283f21475832a55a18c4d1ad6481a4d23b37f91da1fb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:55 GMT
ADD file:65a51da79ba9e2993b794078e3e24554bff59ac80185f12845c1426c7173f06f in / 
# Tue, 30 Mar 2021 21:50:55 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:33:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 31 Mar 2021 05:33:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 31 Mar 2021 05:33:51 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 05:33:52 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 31 Mar 2021 05:35:18 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 31 Mar 2021 05:35:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:35:41 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:35:42 GMT
ENV ODOO_VERSION=12.0
# Wed, 31 Mar 2021 05:35:42 GMT
ARG ODOO_RELEASE=20210329
# Wed, 31 Mar 2021 05:35:42 GMT
ARG ODOO_SHA=cd334511a519ec8b8fd3f4555171d17f94107b77
# Wed, 31 Mar 2021 05:36:47 GMT
# ARGS: ODOO_RELEASE=20210329 ODOO_SHA=cd334511a519ec8b8fd3f4555171d17f94107b77
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 31 Mar 2021 05:36:50 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 31 Mar 2021 05:36:51 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 31 Mar 2021 05:36:52 GMT
# ARGS: ODOO_RELEASE=20210329 ODOO_SHA=cd334511a519ec8b8fd3f4555171d17f94107b77
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 31 Mar 2021 05:36:52 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 31 Mar 2021 05:36:52 GMT
EXPOSE 8069 8071 8072
# Wed, 31 Mar 2021 05:36:52 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 31 Mar 2021 05:36:52 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 31 Mar 2021 05:36:52 GMT
USER odoo
# Wed, 31 Mar 2021 05:36:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 05:36:53 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:23a3602cd30cf5ce6da03e18c28bbbfdc12ae98f182462de8c55785a8d982431`  
		Last Modified: Tue, 30 Mar 2021 21:57:04 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c6915795ca8c7c8930ee76dd81824579247a9450e0bde952170b65c189cc05`  
		Last Modified: Wed, 31 Mar 2021 05:39:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d59774897a449e82a96dccda7da3a9181e64482d2a6670e5d96c91e27e83c1f`  
		Last Modified: Wed, 31 Mar 2021 05:39:30 GMT  
		Size: 219.7 MB (219658871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3f4875f05a0954aceee9441611ab9124140ed09e5366fe97dfe54fe35f8184`  
		Last Modified: Wed, 31 Mar 2021 05:39:01 GMT  
		Size: 2.2 MB (2224092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb531369e15e75947e95abf307ff62714c1f93d4f67ed947cd593d3056264ce`  
		Last Modified: Wed, 31 Mar 2021 05:39:06 GMT  
		Size: 22.0 MB (22042955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00873d1a12c8f7c34d0522b94175b40cd769ed30655f755b237bfa540e0d7326`  
		Last Modified: Wed, 31 Mar 2021 05:39:35 GMT  
		Size: 276.1 MB (276117606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b82b7deb1ef1568f3e301e74724e6f2100b9dd95f84d07138aedff3ac4a374f`  
		Last Modified: Wed, 31 Mar 2021 05:38:59 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb677ea011b6e3f37c083cd4a0cb44dc95e6588738c2c9dc28a1b938d64e0138`  
		Last Modified: Wed, 31 Mar 2021 05:38:58 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd3d4c0600a9b16d3897fb7d406cb0c71b355fafe64821c76e297fcfd9340d3`  
		Last Modified: Wed, 31 Mar 2021 05:38:58 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa68d081a73ef2045ecb590084a22e447dc01087d31de3b7d455684f3067117b`  
		Last Modified: Wed, 31 Mar 2021 05:38:58 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:c467865ec115a07b0d8afaa83392f8d09994c13db57358592c6fd6e4e3d38e6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:7970a800bbb3c33ca2377346bc2cf576ec038e4d953445de1da13092d5578284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.3 MB (532269116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52fc06b1d8af54dd7a479db4da5ce51e2e4117dbc342231c13cf243e8ef1bb8f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:28:28 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 31 Mar 2021 05:28:28 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 31 Mar 2021 05:28:29 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 05:32:06 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 31 Mar 2021 05:32:14 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:32:17 GMT
RUN npm install -g rtlcss
# Wed, 31 Mar 2021 05:32:18 GMT
ENV ODOO_VERSION=13.0
# Wed, 31 Mar 2021 05:32:18 GMT
ARG ODOO_RELEASE=20210330
# Wed, 31 Mar 2021 05:32:18 GMT
ARG ODOO_SHA=0e7a35f95285b360d01f6da0e64282519d025f31
# Wed, 31 Mar 2021 05:33:29 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0e7a35f95285b360d01f6da0e64282519d025f31
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 31 Mar 2021 05:33:32 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 31 Mar 2021 05:33:33 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 31 Mar 2021 05:33:34 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0e7a35f95285b360d01f6da0e64282519d025f31
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 31 Mar 2021 05:33:34 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 31 Mar 2021 05:33:34 GMT
EXPOSE 8069 8071 8072
# Wed, 31 Mar 2021 05:33:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 31 Mar 2021 05:33:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 31 Mar 2021 05:33:35 GMT
USER odoo
# Wed, 31 Mar 2021 05:33:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 05:33:35 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de28911af5f8767fc6fe7abf921e6faf5736251f49ad228e8cea796a6ff5981d`  
		Last Modified: Wed, 31 Mar 2021 05:38:39 GMT  
		Size: 207.1 MB (207123802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8b6f4271c30f6e5b71d1885f6089af04ebaa2754576ad658a29f17f6098a13`  
		Last Modified: Wed, 31 Mar 2021 05:38:10 GMT  
		Size: 2.3 MB (2345373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e216845aa303c372f43ecd3c7255099d37f5acb661344b8b0a764dca4dc5eb67`  
		Last Modified: Wed, 31 Mar 2021 05:38:09 GMT  
		Size: 894.0 KB (894002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43468d092c9f39982d1a37ffe680c4ddb16af65708f07747274f82e9af68ac`  
		Last Modified: Wed, 31 Mar 2021 05:38:46 GMT  
		Size: 294.8 MB (294764222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30974c81086c7d4ccaa51e1561ed5b22974c0b486cc02849ac6e9806f6c63c2`  
		Last Modified: Wed, 31 Mar 2021 05:38:06 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ae4d5cf1c21a50712a3c22d5eb69ec24d05660d9ac543d25efebf21a4b57c1`  
		Last Modified: Wed, 31 Mar 2021 05:38:06 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54428449f67ca124684846e2f2c0f9cc78b169001f1acfc88b0a815bed90242`  
		Last Modified: Wed, 31 Mar 2021 05:38:06 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd3141b0d11512b70b019b73bbec0cca8a8fe4c034da251d8aaf72fa53cb7c8`  
		Last Modified: Wed, 31 Mar 2021 05:38:06 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:c467865ec115a07b0d8afaa83392f8d09994c13db57358592c6fd6e4e3d38e6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:7970a800bbb3c33ca2377346bc2cf576ec038e4d953445de1da13092d5578284
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.3 MB (532269116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52fc06b1d8af54dd7a479db4da5ce51e2e4117dbc342231c13cf243e8ef1bb8f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:28:28 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 31 Mar 2021 05:28:28 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 31 Mar 2021 05:28:29 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 05:32:06 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 31 Mar 2021 05:32:14 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:32:17 GMT
RUN npm install -g rtlcss
# Wed, 31 Mar 2021 05:32:18 GMT
ENV ODOO_VERSION=13.0
# Wed, 31 Mar 2021 05:32:18 GMT
ARG ODOO_RELEASE=20210330
# Wed, 31 Mar 2021 05:32:18 GMT
ARG ODOO_SHA=0e7a35f95285b360d01f6da0e64282519d025f31
# Wed, 31 Mar 2021 05:33:29 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0e7a35f95285b360d01f6da0e64282519d025f31
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 31 Mar 2021 05:33:32 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 31 Mar 2021 05:33:33 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 31 Mar 2021 05:33:34 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0e7a35f95285b360d01f6da0e64282519d025f31
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 31 Mar 2021 05:33:34 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 31 Mar 2021 05:33:34 GMT
EXPOSE 8069 8071 8072
# Wed, 31 Mar 2021 05:33:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 31 Mar 2021 05:33:34 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 31 Mar 2021 05:33:35 GMT
USER odoo
# Wed, 31 Mar 2021 05:33:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 05:33:35 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de28911af5f8767fc6fe7abf921e6faf5736251f49ad228e8cea796a6ff5981d`  
		Last Modified: Wed, 31 Mar 2021 05:38:39 GMT  
		Size: 207.1 MB (207123802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8b6f4271c30f6e5b71d1885f6089af04ebaa2754576ad658a29f17f6098a13`  
		Last Modified: Wed, 31 Mar 2021 05:38:10 GMT  
		Size: 2.3 MB (2345373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e216845aa303c372f43ecd3c7255099d37f5acb661344b8b0a764dca4dc5eb67`  
		Last Modified: Wed, 31 Mar 2021 05:38:09 GMT  
		Size: 894.0 KB (894002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af43468d092c9f39982d1a37ffe680c4ddb16af65708f07747274f82e9af68ac`  
		Last Modified: Wed, 31 Mar 2021 05:38:46 GMT  
		Size: 294.8 MB (294764222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30974c81086c7d4ccaa51e1561ed5b22974c0b486cc02849ac6e9806f6c63c2`  
		Last Modified: Wed, 31 Mar 2021 05:38:06 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ae4d5cf1c21a50712a3c22d5eb69ec24d05660d9ac543d25efebf21a4b57c1`  
		Last Modified: Wed, 31 Mar 2021 05:38:06 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54428449f67ca124684846e2f2c0f9cc78b169001f1acfc88b0a815bed90242`  
		Last Modified: Wed, 31 Mar 2021 05:38:06 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd3141b0d11512b70b019b73bbec0cca8a8fe4c034da251d8aaf72fa53cb7c8`  
		Last Modified: Wed, 31 Mar 2021 05:38:06 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:2ecb515f376e3d4e70fe6553825d1a2e7103751b0711f6969ac04361a2cfddc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:597518465b4b472c487bd444d7fb22766f282840dcba49d99ec38d8a089e7be7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515795602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ba433d24bc66371eb98f141ebd811166f5c08994ad18bf44a04dba978e4e22`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:28:28 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 31 Mar 2021 05:28:28 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 31 Mar 2021 05:28:29 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 05:29:34 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 31 Mar 2021 05:29:44 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:29:47 GMT
RUN npm install -g rtlcss
# Wed, 31 Mar 2021 05:29:48 GMT
ENV ODOO_VERSION=14.0
# Wed, 31 Mar 2021 05:29:48 GMT
ARG ODOO_RELEASE=20210330
# Wed, 31 Mar 2021 05:29:48 GMT
ARG ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
# Wed, 31 Mar 2021 05:30:59 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 31 Mar 2021 05:31:01 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 31 Mar 2021 05:31:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 31 Mar 2021 05:31:02 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 31 Mar 2021 05:31:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 31 Mar 2021 05:31:02 GMT
EXPOSE 8069 8071 8072
# Wed, 31 Mar 2021 05:31:03 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 31 Mar 2021 05:31:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 31 Mar 2021 05:31:03 GMT
USER odoo
# Wed, 31 Mar 2021 05:31:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 05:31:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891b8c13a6557e87341fe3dae2cacc445b84d3061c83b252ca743c338d64cc83`  
		Last Modified: Wed, 31 Mar 2021 05:37:46 GMT  
		Size: 213.2 MB (213169537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acf2c1161bac7f6d917df1dab741f4f98b3d7d9bb4994d7fd1913385578875e`  
		Last Modified: Wed, 31 Mar 2021 05:37:18 GMT  
		Size: 2.3 MB (2348508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16b52e489bcfae111683bd0dc94749af43d9ea55931a3c2a703c8c3ff3dfb6e`  
		Last Modified: Wed, 31 Mar 2021 05:37:16 GMT  
		Size: 894.0 KB (894018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c12fc10a65fc5cc749140f39858c24345a40cd3a5c65cb1bd16564562f5863`  
		Last Modified: Wed, 31 Mar 2021 05:37:52 GMT  
		Size: 272.2 MB (272241819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99f91ee63f5d119d59cfb65a6bffadf64bde3db9e62735ca33afbf4059f9300`  
		Last Modified: Wed, 31 Mar 2021 05:37:13 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71b71de0f7f0c0868631d2ab856a984a6096b6eeae599564aa6a8ad7d4e440b`  
		Last Modified: Wed, 31 Mar 2021 05:37:13 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a363c38a84e7a64fe52ba04fa47a29eda88f5c223718f31032b258fcc191ea4`  
		Last Modified: Wed, 31 Mar 2021 05:37:14 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee9192eeed425ce8c67b4d2d92154b2082eb4838c326615ef35167d38cefbfd`  
		Last Modified: Wed, 31 Mar 2021 05:37:14 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:2ecb515f376e3d4e70fe6553825d1a2e7103751b0711f6969ac04361a2cfddc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:597518465b4b472c487bd444d7fb22766f282840dcba49d99ec38d8a089e7be7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515795602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ba433d24bc66371eb98f141ebd811166f5c08994ad18bf44a04dba978e4e22`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:28:28 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 31 Mar 2021 05:28:28 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 31 Mar 2021 05:28:29 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 05:29:34 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 31 Mar 2021 05:29:44 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:29:47 GMT
RUN npm install -g rtlcss
# Wed, 31 Mar 2021 05:29:48 GMT
ENV ODOO_VERSION=14.0
# Wed, 31 Mar 2021 05:29:48 GMT
ARG ODOO_RELEASE=20210330
# Wed, 31 Mar 2021 05:29:48 GMT
ARG ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
# Wed, 31 Mar 2021 05:30:59 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 31 Mar 2021 05:31:01 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 31 Mar 2021 05:31:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 31 Mar 2021 05:31:02 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 31 Mar 2021 05:31:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 31 Mar 2021 05:31:02 GMT
EXPOSE 8069 8071 8072
# Wed, 31 Mar 2021 05:31:03 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 31 Mar 2021 05:31:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 31 Mar 2021 05:31:03 GMT
USER odoo
# Wed, 31 Mar 2021 05:31:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 05:31:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891b8c13a6557e87341fe3dae2cacc445b84d3061c83b252ca743c338d64cc83`  
		Last Modified: Wed, 31 Mar 2021 05:37:46 GMT  
		Size: 213.2 MB (213169537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acf2c1161bac7f6d917df1dab741f4f98b3d7d9bb4994d7fd1913385578875e`  
		Last Modified: Wed, 31 Mar 2021 05:37:18 GMT  
		Size: 2.3 MB (2348508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16b52e489bcfae111683bd0dc94749af43d9ea55931a3c2a703c8c3ff3dfb6e`  
		Last Modified: Wed, 31 Mar 2021 05:37:16 GMT  
		Size: 894.0 KB (894018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c12fc10a65fc5cc749140f39858c24345a40cd3a5c65cb1bd16564562f5863`  
		Last Modified: Wed, 31 Mar 2021 05:37:52 GMT  
		Size: 272.2 MB (272241819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99f91ee63f5d119d59cfb65a6bffadf64bde3db9e62735ca33afbf4059f9300`  
		Last Modified: Wed, 31 Mar 2021 05:37:13 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71b71de0f7f0c0868631d2ab856a984a6096b6eeae599564aa6a8ad7d4e440b`  
		Last Modified: Wed, 31 Mar 2021 05:37:13 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a363c38a84e7a64fe52ba04fa47a29eda88f5c223718f31032b258fcc191ea4`  
		Last Modified: Wed, 31 Mar 2021 05:37:14 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee9192eeed425ce8c67b4d2d92154b2082eb4838c326615ef35167d38cefbfd`  
		Last Modified: Wed, 31 Mar 2021 05:37:14 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:2ecb515f376e3d4e70fe6553825d1a2e7103751b0711f6969ac04361a2cfddc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:597518465b4b472c487bd444d7fb22766f282840dcba49d99ec38d8a089e7be7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515795602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ba433d24bc66371eb98f141ebd811166f5c08994ad18bf44a04dba978e4e22`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:28:28 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 31 Mar 2021 05:28:28 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 31 Mar 2021 05:28:29 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 05:29:34 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 31 Mar 2021 05:29:44 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:29:47 GMT
RUN npm install -g rtlcss
# Wed, 31 Mar 2021 05:29:48 GMT
ENV ODOO_VERSION=14.0
# Wed, 31 Mar 2021 05:29:48 GMT
ARG ODOO_RELEASE=20210330
# Wed, 31 Mar 2021 05:29:48 GMT
ARG ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
# Wed, 31 Mar 2021 05:30:59 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 31 Mar 2021 05:31:01 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 31 Mar 2021 05:31:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 31 Mar 2021 05:31:02 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 31 Mar 2021 05:31:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 31 Mar 2021 05:31:02 GMT
EXPOSE 8069 8071 8072
# Wed, 31 Mar 2021 05:31:03 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 31 Mar 2021 05:31:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 31 Mar 2021 05:31:03 GMT
USER odoo
# Wed, 31 Mar 2021 05:31:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 05:31:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891b8c13a6557e87341fe3dae2cacc445b84d3061c83b252ca743c338d64cc83`  
		Last Modified: Wed, 31 Mar 2021 05:37:46 GMT  
		Size: 213.2 MB (213169537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acf2c1161bac7f6d917df1dab741f4f98b3d7d9bb4994d7fd1913385578875e`  
		Last Modified: Wed, 31 Mar 2021 05:37:18 GMT  
		Size: 2.3 MB (2348508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16b52e489bcfae111683bd0dc94749af43d9ea55931a3c2a703c8c3ff3dfb6e`  
		Last Modified: Wed, 31 Mar 2021 05:37:16 GMT  
		Size: 894.0 KB (894018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c12fc10a65fc5cc749140f39858c24345a40cd3a5c65cb1bd16564562f5863`  
		Last Modified: Wed, 31 Mar 2021 05:37:52 GMT  
		Size: 272.2 MB (272241819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99f91ee63f5d119d59cfb65a6bffadf64bde3db9e62735ca33afbf4059f9300`  
		Last Modified: Wed, 31 Mar 2021 05:37:13 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71b71de0f7f0c0868631d2ab856a984a6096b6eeae599564aa6a8ad7d4e440b`  
		Last Modified: Wed, 31 Mar 2021 05:37:13 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a363c38a84e7a64fe52ba04fa47a29eda88f5c223718f31032b258fcc191ea4`  
		Last Modified: Wed, 31 Mar 2021 05:37:14 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee9192eeed425ce8c67b4d2d92154b2082eb4838c326615ef35167d38cefbfd`  
		Last Modified: Wed, 31 Mar 2021 05:37:14 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
