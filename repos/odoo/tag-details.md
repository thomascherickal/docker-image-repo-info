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
$ docker pull odoo@sha256:a77cde81cdfa185f9d76c4f22c11a24e288ff13d19848802f05207cbd10c3c06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:536d914fb9b22195f6d2479dfa02e4c094e5b42df71b9aa0566f2d7eb2d12859
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538351097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d8ed9a0a71fc546c6ce35ebce1727e253e3bd07d2fe2f146e27b0e9f603220c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 08:50:47 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 May 2021 08:50:47 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 May 2021 08:50:47 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 08:50:48 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 12 May 2021 08:52:09 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 May 2021 08:52:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 08:52:45 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 08:52:46 GMT
ENV ODOO_VERSION=12.0
# Wed, 09 Jun 2021 18:08:11 GMT
ARG ODOO_RELEASE=20210609
# Wed, 09 Jun 2021 18:08:11 GMT
ARG ODOO_SHA=877cad69b0c39439523f23f53993a3e49447a814
# Wed, 09 Jun 2021 18:09:25 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=877cad69b0c39439523f23f53993a3e49447a814
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Jun 2021 18:09:28 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Jun 2021 18:09:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Jun 2021 18:09:30 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=877cad69b0c39439523f23f53993a3e49447a814
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Jun 2021 18:09:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Jun 2021 18:09:31 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Jun 2021 18:09:31 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Jun 2021 18:09:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Jun 2021 18:09:32 GMT
USER odoo
# Wed, 09 Jun 2021 18:09:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Jun 2021 18:09:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af54249d19fe626a77f15839d273f8d043ce913784302e4e5ee6a810b158f43`  
		Last Modified: Wed, 12 May 2021 08:56:45 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019e7996c57952fa770bb898324d340b77024067ab213469f9fefe533da19ea4`  
		Last Modified: Wed, 12 May 2021 08:57:13 GMT  
		Size: 219.6 MB (219644042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a2f907c0eef99db7b697ab129fdefdf63e755e22e9fee296c13a5179009c44`  
		Last Modified: Wed, 12 May 2021 08:56:45 GMT  
		Size: 2.2 MB (2224133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764a9260e7d9a4e20c20fb21502f10d7ff5406fe00b088e79e0a80a0c421d5f5`  
		Last Modified: Wed, 12 May 2021 08:56:50 GMT  
		Size: 22.0 MB (22043646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61f11f1d32a6673aaab200194d63e821c32fd23717750b7cfce532562634653`  
		Last Modified: Wed, 09 Jun 2021 18:12:23 GMT  
		Size: 271.9 MB (271908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9cb1aadcf8a65ff1fee396fa6bbc158d98982f7e3c974acda9019f4001d17c`  
		Last Modified: Wed, 09 Jun 2021 18:11:41 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8270ec8954dcc2614caac84f6eca0a819d54f50665aedafa74205b2d4d4f70eb`  
		Last Modified: Wed, 09 Jun 2021 18:11:41 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff7d18642cc886232d20c05d94689a6c57d96ea91067046bf1950b2882f06ac`  
		Last Modified: Wed, 09 Jun 2021 18:11:41 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e6b3634728183038b4aeff758c4b015c182042dcbe5fc0974c6a57af3b13c7`  
		Last Modified: Wed, 09 Jun 2021 18:11:41 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:a77cde81cdfa185f9d76c4f22c11a24e288ff13d19848802f05207cbd10c3c06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:536d914fb9b22195f6d2479dfa02e4c094e5b42df71b9aa0566f2d7eb2d12859
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538351097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d8ed9a0a71fc546c6ce35ebce1727e253e3bd07d2fe2f146e27b0e9f603220c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 08:50:47 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 May 2021 08:50:47 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 May 2021 08:50:47 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 08:50:48 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 12 May 2021 08:52:09 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 May 2021 08:52:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 08:52:45 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 08:52:46 GMT
ENV ODOO_VERSION=12.0
# Wed, 09 Jun 2021 18:08:11 GMT
ARG ODOO_RELEASE=20210609
# Wed, 09 Jun 2021 18:08:11 GMT
ARG ODOO_SHA=877cad69b0c39439523f23f53993a3e49447a814
# Wed, 09 Jun 2021 18:09:25 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=877cad69b0c39439523f23f53993a3e49447a814
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Jun 2021 18:09:28 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Jun 2021 18:09:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Jun 2021 18:09:30 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=877cad69b0c39439523f23f53993a3e49447a814
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Jun 2021 18:09:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Jun 2021 18:09:31 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Jun 2021 18:09:31 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Jun 2021 18:09:31 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Jun 2021 18:09:32 GMT
USER odoo
# Wed, 09 Jun 2021 18:09:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Jun 2021 18:09:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af54249d19fe626a77f15839d273f8d043ce913784302e4e5ee6a810b158f43`  
		Last Modified: Wed, 12 May 2021 08:56:45 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019e7996c57952fa770bb898324d340b77024067ab213469f9fefe533da19ea4`  
		Last Modified: Wed, 12 May 2021 08:57:13 GMT  
		Size: 219.6 MB (219644042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a2f907c0eef99db7b697ab129fdefdf63e755e22e9fee296c13a5179009c44`  
		Last Modified: Wed, 12 May 2021 08:56:45 GMT  
		Size: 2.2 MB (2224133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764a9260e7d9a4e20c20fb21502f10d7ff5406fe00b088e79e0a80a0c421d5f5`  
		Last Modified: Wed, 12 May 2021 08:56:50 GMT  
		Size: 22.0 MB (22043646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61f11f1d32a6673aaab200194d63e821c32fd23717750b7cfce532562634653`  
		Last Modified: Wed, 09 Jun 2021 18:12:23 GMT  
		Size: 271.9 MB (271908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9cb1aadcf8a65ff1fee396fa6bbc158d98982f7e3c974acda9019f4001d17c`  
		Last Modified: Wed, 09 Jun 2021 18:11:41 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8270ec8954dcc2614caac84f6eca0a819d54f50665aedafa74205b2d4d4f70eb`  
		Last Modified: Wed, 09 Jun 2021 18:11:41 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff7d18642cc886232d20c05d94689a6c57d96ea91067046bf1950b2882f06ac`  
		Last Modified: Wed, 09 Jun 2021 18:11:41 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e6b3634728183038b4aeff758c4b015c182042dcbe5fc0974c6a57af3b13c7`  
		Last Modified: Wed, 09 Jun 2021 18:11:41 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:e75bd2fe02a773e36b33743ac903e249c4ef979f89b33eb6614f6ef158252008
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:bae513d7d3d764c1980b80c8bfbfd357aa8049dca2fc1969ce57fa8d6a04e945
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.2 MB (528179513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b918c0e094af8e760d2b0bdb9d11f7ac52bdd3975121b91aa2ff280b788cb02f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 08:44:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 May 2021 08:44:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 May 2021 08:44:56 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 08:49:03 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 May 2021 08:49:10 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 08:49:14 GMT
RUN npm install -g rtlcss
# Wed, 12 May 2021 08:49:14 GMT
ENV ODOO_VERSION=13.0
# Wed, 09 Jun 2021 18:06:15 GMT
ARG ODOO_RELEASE=20210609
# Wed, 09 Jun 2021 18:06:15 GMT
ARG ODOO_SHA=6a697041b52a8330fdab225d2e49c97296224cd8
# Wed, 09 Jun 2021 18:07:46 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=6a697041b52a8330fdab225d2e49c97296224cd8
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Jun 2021 18:07:50 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Jun 2021 18:07:50 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Jun 2021 18:07:51 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=6a697041b52a8330fdab225d2e49c97296224cd8
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Jun 2021 18:07:52 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Jun 2021 18:07:52 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Jun 2021 18:07:52 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Jun 2021 18:07:53 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Jun 2021 18:07:53 GMT
USER odoo
# Wed, 09 Jun 2021 18:07:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Jun 2021 18:07:53 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd2340d2eb35cffa9ca9e4bde49346d44e9b5256f115d1d5ef505381aa063b2`  
		Last Modified: Wed, 12 May 2021 08:56:16 GMT  
		Size: 207.1 MB (207123504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2bf3253f515783426050c6c8a278f5d8a9d574287fae7bc3630e3586a0dc7`  
		Last Modified: Wed, 12 May 2021 08:55:20 GMT  
		Size: 2.3 MB (2345380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37981d08650c3b2e5a5e757ba40494eb86a34a4162414076c592efa41f10e3ea`  
		Last Modified: Wed, 12 May 2021 08:55:20 GMT  
		Size: 906.3 KB (906348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c59eab68ab6e5aede692d3c8b52acf01e29d9d083adc5bd0ac52c327332cc5e`  
		Last Modified: Wed, 09 Jun 2021 18:11:28 GMT  
		Size: 290.7 MB (290655941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cba5478a6091401b13a47891d1b37ef23dc76afcca1cd95fcd21c82475cd8da`  
		Last Modified: Wed, 09 Jun 2021 18:10:42 GMT  
		Size: 669.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61b8e429cd9bc685cfbcf642f0ca7b60940a48c12752b5fdbded968dce483ef`  
		Last Modified: Wed, 09 Jun 2021 18:10:42 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5a09f33b43e73226f348c1b792647178a7671d7985a737eca1f55f73c5f0fc`  
		Last Modified: Wed, 09 Jun 2021 18:10:42 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a3c2911a67b97be48aad44f9215a0b821776e9a33f304065fb1fa38df274f`  
		Last Modified: Wed, 09 Jun 2021 18:10:42 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:e75bd2fe02a773e36b33743ac903e249c4ef979f89b33eb6614f6ef158252008
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:bae513d7d3d764c1980b80c8bfbfd357aa8049dca2fc1969ce57fa8d6a04e945
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.2 MB (528179513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b918c0e094af8e760d2b0bdb9d11f7ac52bdd3975121b91aa2ff280b788cb02f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 08:44:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 May 2021 08:44:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 May 2021 08:44:56 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 08:49:03 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 May 2021 08:49:10 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 08:49:14 GMT
RUN npm install -g rtlcss
# Wed, 12 May 2021 08:49:14 GMT
ENV ODOO_VERSION=13.0
# Wed, 09 Jun 2021 18:06:15 GMT
ARG ODOO_RELEASE=20210609
# Wed, 09 Jun 2021 18:06:15 GMT
ARG ODOO_SHA=6a697041b52a8330fdab225d2e49c97296224cd8
# Wed, 09 Jun 2021 18:07:46 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=6a697041b52a8330fdab225d2e49c97296224cd8
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Jun 2021 18:07:50 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Jun 2021 18:07:50 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Jun 2021 18:07:51 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=6a697041b52a8330fdab225d2e49c97296224cd8
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Jun 2021 18:07:52 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Jun 2021 18:07:52 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Jun 2021 18:07:52 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Jun 2021 18:07:53 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Jun 2021 18:07:53 GMT
USER odoo
# Wed, 09 Jun 2021 18:07:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Jun 2021 18:07:53 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd2340d2eb35cffa9ca9e4bde49346d44e9b5256f115d1d5ef505381aa063b2`  
		Last Modified: Wed, 12 May 2021 08:56:16 GMT  
		Size: 207.1 MB (207123504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2bf3253f515783426050c6c8a278f5d8a9d574287fae7bc3630e3586a0dc7`  
		Last Modified: Wed, 12 May 2021 08:55:20 GMT  
		Size: 2.3 MB (2345380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37981d08650c3b2e5a5e757ba40494eb86a34a4162414076c592efa41f10e3ea`  
		Last Modified: Wed, 12 May 2021 08:55:20 GMT  
		Size: 906.3 KB (906348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c59eab68ab6e5aede692d3c8b52acf01e29d9d083adc5bd0ac52c327332cc5e`  
		Last Modified: Wed, 09 Jun 2021 18:11:28 GMT  
		Size: 290.7 MB (290655941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cba5478a6091401b13a47891d1b37ef23dc76afcca1cd95fcd21c82475cd8da`  
		Last Modified: Wed, 09 Jun 2021 18:10:42 GMT  
		Size: 669.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61b8e429cd9bc685cfbcf642f0ca7b60940a48c12752b5fdbded968dce483ef`  
		Last Modified: Wed, 09 Jun 2021 18:10:42 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5a09f33b43e73226f348c1b792647178a7671d7985a737eca1f55f73c5f0fc`  
		Last Modified: Wed, 09 Jun 2021 18:10:42 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4a3c2911a67b97be48aad44f9215a0b821776e9a33f304065fb1fa38df274f`  
		Last Modified: Wed, 09 Jun 2021 18:10:42 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:f1e43de632ebfbddbaac6312572cddeb2109f406295aa97e8e4b51a760e3e5ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:e0ccc064ce3b83199a4c3b056ca54f021e6fb49a9bc5990d3a3a6b07777b5864
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **514.2 MB (514195630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abad5085a097c1e5861a495ae32cc977e1083e792b13e31825a6c00250a97d57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 08:44:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 May 2021 08:44:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 May 2021 08:44:56 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 08:46:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 May 2021 08:46:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 08:46:32 GMT
RUN npm install -g rtlcss
# Wed, 12 May 2021 08:46:32 GMT
ENV ODOO_VERSION=14.0
# Wed, 09 Jun 2021 18:04:19 GMT
ARG ODOO_RELEASE=20210609
# Wed, 09 Jun 2021 18:04:19 GMT
ARG ODOO_SHA=5d0f9f7f49e60e74ec5505a05cfb61f3fb73761c
# Wed, 09 Jun 2021 18:05:54 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=5d0f9f7f49e60e74ec5505a05cfb61f3fb73761c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Jun 2021 18:05:58 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Jun 2021 18:05:59 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Jun 2021 18:06:00 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=5d0f9f7f49e60e74ec5505a05cfb61f3fb73761c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Jun 2021 18:06:00 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Jun 2021 18:06:00 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Jun 2021 18:06:01 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Jun 2021 18:06:01 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Jun 2021 18:06:01 GMT
USER odoo
# Wed, 09 Jun 2021 18:06:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Jun 2021 18:06:02 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4b0e38652c25af879825f24dbea2383353d341f344d6380e333c3acfe1fdaa`  
		Last Modified: Wed, 12 May 2021 08:54:57 GMT  
		Size: 213.2 MB (213170176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9893a9d4028d8617a36b2cec12ad0bd2f635a565ad68099c04d5e7f25aebe81`  
		Last Modified: Wed, 12 May 2021 08:54:27 GMT  
		Size: 2.3 MB (2348569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2646c61bff1d0763d58e8409ab91365ab8469566e7f5cf9a1f9be81b21d4eeeb`  
		Last Modified: Wed, 12 May 2021 08:54:27 GMT  
		Size: 906.3 KB (906251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2457b16d6c6caf48b6e02203d257cc90c057776bf9716b239c3e56e2da2e7e`  
		Last Modified: Wed, 09 Jun 2021 18:10:26 GMT  
		Size: 270.6 MB (270622289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e576726996bedd3f7b8d2b48fd99851147c46d7b1f96f38307914867e48dde68`  
		Last Modified: Wed, 09 Jun 2021 18:09:49 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf874dc23ac1e3a1e1e06363381c8a2c439b2990580fcdf732db9c53de58c70`  
		Last Modified: Wed, 09 Jun 2021 18:09:49 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c885579af43d7a575982edc124a5e6fe1b276e63ea49f4a8ebf3a70fe077d2b`  
		Last Modified: Wed, 09 Jun 2021 18:09:50 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73d778d8dfd0b20025c681a7c58b814b2668c891eaf87b65ae3242abc20d3ed`  
		Last Modified: Wed, 09 Jun 2021 18:09:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:f1e43de632ebfbddbaac6312572cddeb2109f406295aa97e8e4b51a760e3e5ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:e0ccc064ce3b83199a4c3b056ca54f021e6fb49a9bc5990d3a3a6b07777b5864
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **514.2 MB (514195630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abad5085a097c1e5861a495ae32cc977e1083e792b13e31825a6c00250a97d57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 08:44:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 May 2021 08:44:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 May 2021 08:44:56 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 08:46:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 May 2021 08:46:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 08:46:32 GMT
RUN npm install -g rtlcss
# Wed, 12 May 2021 08:46:32 GMT
ENV ODOO_VERSION=14.0
# Wed, 09 Jun 2021 18:04:19 GMT
ARG ODOO_RELEASE=20210609
# Wed, 09 Jun 2021 18:04:19 GMT
ARG ODOO_SHA=5d0f9f7f49e60e74ec5505a05cfb61f3fb73761c
# Wed, 09 Jun 2021 18:05:54 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=5d0f9f7f49e60e74ec5505a05cfb61f3fb73761c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Jun 2021 18:05:58 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Jun 2021 18:05:59 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Jun 2021 18:06:00 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=5d0f9f7f49e60e74ec5505a05cfb61f3fb73761c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Jun 2021 18:06:00 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Jun 2021 18:06:00 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Jun 2021 18:06:01 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Jun 2021 18:06:01 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Jun 2021 18:06:01 GMT
USER odoo
# Wed, 09 Jun 2021 18:06:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Jun 2021 18:06:02 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4b0e38652c25af879825f24dbea2383353d341f344d6380e333c3acfe1fdaa`  
		Last Modified: Wed, 12 May 2021 08:54:57 GMT  
		Size: 213.2 MB (213170176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9893a9d4028d8617a36b2cec12ad0bd2f635a565ad68099c04d5e7f25aebe81`  
		Last Modified: Wed, 12 May 2021 08:54:27 GMT  
		Size: 2.3 MB (2348569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2646c61bff1d0763d58e8409ab91365ab8469566e7f5cf9a1f9be81b21d4eeeb`  
		Last Modified: Wed, 12 May 2021 08:54:27 GMT  
		Size: 906.3 KB (906251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2457b16d6c6caf48b6e02203d257cc90c057776bf9716b239c3e56e2da2e7e`  
		Last Modified: Wed, 09 Jun 2021 18:10:26 GMT  
		Size: 270.6 MB (270622289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e576726996bedd3f7b8d2b48fd99851147c46d7b1f96f38307914867e48dde68`  
		Last Modified: Wed, 09 Jun 2021 18:09:49 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf874dc23ac1e3a1e1e06363381c8a2c439b2990580fcdf732db9c53de58c70`  
		Last Modified: Wed, 09 Jun 2021 18:09:49 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c885579af43d7a575982edc124a5e6fe1b276e63ea49f4a8ebf3a70fe077d2b`  
		Last Modified: Wed, 09 Jun 2021 18:09:50 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73d778d8dfd0b20025c681a7c58b814b2668c891eaf87b65ae3242abc20d3ed`  
		Last Modified: Wed, 09 Jun 2021 18:09:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:f1e43de632ebfbddbaac6312572cddeb2109f406295aa97e8e4b51a760e3e5ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:e0ccc064ce3b83199a4c3b056ca54f021e6fb49a9bc5990d3a3a6b07777b5864
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **514.2 MB (514195630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abad5085a097c1e5861a495ae32cc977e1083e792b13e31825a6c00250a97d57`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 08:44:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 May 2021 08:44:56 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 May 2021 08:44:56 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 08:46:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 May 2021 08:46:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 08:46:32 GMT
RUN npm install -g rtlcss
# Wed, 12 May 2021 08:46:32 GMT
ENV ODOO_VERSION=14.0
# Wed, 09 Jun 2021 18:04:19 GMT
ARG ODOO_RELEASE=20210609
# Wed, 09 Jun 2021 18:04:19 GMT
ARG ODOO_SHA=5d0f9f7f49e60e74ec5505a05cfb61f3fb73761c
# Wed, 09 Jun 2021 18:05:54 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=5d0f9f7f49e60e74ec5505a05cfb61f3fb73761c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 09 Jun 2021 18:05:58 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 09 Jun 2021 18:05:59 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 09 Jun 2021 18:06:00 GMT
# ARGS: ODOO_RELEASE=20210609 ODOO_SHA=5d0f9f7f49e60e74ec5505a05cfb61f3fb73761c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 09 Jun 2021 18:06:00 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 09 Jun 2021 18:06:00 GMT
EXPOSE 8069 8071 8072
# Wed, 09 Jun 2021 18:06:01 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 09 Jun 2021 18:06:01 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 09 Jun 2021 18:06:01 GMT
USER odoo
# Wed, 09 Jun 2021 18:06:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Jun 2021 18:06:02 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4b0e38652c25af879825f24dbea2383353d341f344d6380e333c3acfe1fdaa`  
		Last Modified: Wed, 12 May 2021 08:54:57 GMT  
		Size: 213.2 MB (213170176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9893a9d4028d8617a36b2cec12ad0bd2f635a565ad68099c04d5e7f25aebe81`  
		Last Modified: Wed, 12 May 2021 08:54:27 GMT  
		Size: 2.3 MB (2348569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2646c61bff1d0763d58e8409ab91365ab8469566e7f5cf9a1f9be81b21d4eeeb`  
		Last Modified: Wed, 12 May 2021 08:54:27 GMT  
		Size: 906.3 KB (906251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2457b16d6c6caf48b6e02203d257cc90c057776bf9716b239c3e56e2da2e7e`  
		Last Modified: Wed, 09 Jun 2021 18:10:26 GMT  
		Size: 270.6 MB (270622289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e576726996bedd3f7b8d2b48fd99851147c46d7b1f96f38307914867e48dde68`  
		Last Modified: Wed, 09 Jun 2021 18:09:49 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf874dc23ac1e3a1e1e06363381c8a2c439b2990580fcdf732db9c53de58c70`  
		Last Modified: Wed, 09 Jun 2021 18:09:49 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c885579af43d7a575982edc124a5e6fe1b276e63ea49f4a8ebf3a70fe077d2b`  
		Last Modified: Wed, 09 Jun 2021 18:09:50 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73d778d8dfd0b20025c681a7c58b814b2668c891eaf87b65ae3242abc20d3ed`  
		Last Modified: Wed, 09 Jun 2021 18:09:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
