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
$ docker pull odoo@sha256:8c0a94658711ba6778ac1942003b70c4d5a9c61b77e1b032420196098de08193
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:7b8ea1938bdc21561816a37227f454a96f45340edfb718571a4c0203cd8576f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.6 MB (542589540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c95932e9ddf5401af16b4b8bae1eb59eb3eb376dd73b51537c92da04f07b484`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 12:37:46 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 10 Apr 2021 12:37:46 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 10 Apr 2021 12:37:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 12:37:47 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Sat, 10 Apr 2021 12:39:11 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 10 Apr 2021 12:39:27 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:39:39 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:39:39 GMT
ENV ODOO_VERSION=12.0
# Tue, 27 Apr 2021 21:26:52 GMT
ARG ODOO_RELEASE=20210427
# Tue, 27 Apr 2021 21:26:52 GMT
ARG ODOO_SHA=9e00c380b73efce6b164c2a0d7127de65feed2e3
# Tue, 27 Apr 2021 21:27:57 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9e00c380b73efce6b164c2a0d7127de65feed2e3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Apr 2021 21:28:01 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 27 Apr 2021 21:28:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Apr 2021 21:28:02 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9e00c380b73efce6b164c2a0d7127de65feed2e3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Apr 2021 21:28:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Apr 2021 21:28:02 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Apr 2021 21:28:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Apr 2021 21:28:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Apr 2021 21:28:03 GMT
USER odoo
# Tue, 27 Apr 2021 21:28:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Apr 2021 21:28:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cf89834cbbd2b3cee3b8a944f6b45e4a1507584664ee0a1b02259590615d59`  
		Last Modified: Sat, 10 Apr 2021 12:42:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b11cee4db50450b66bc29b47f68b86380f02d6097f24e2b69a05dab9b82788`  
		Last Modified: Sat, 10 Apr 2021 12:43:18 GMT  
		Size: 219.6 MB (219645154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98555f4c9e696b99e0a4429cafe8848f74f7baa37c2265bd07bdc5d7ca50ece3`  
		Last Modified: Sat, 10 Apr 2021 12:42:52 GMT  
		Size: 2.2 MB (2224102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd66427a8f8ee5f5e15e695a9171413d51a17fd3fa05b78c6b7b8f7f2b8a259`  
		Last Modified: Sat, 10 Apr 2021 12:42:56 GMT  
		Size: 22.0 MB (22046831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8321ff954c4b2aba8c5626362d7ff51082e97e348c7ba2a8fdda0b102fefb94`  
		Last Modified: Tue, 27 Apr 2021 21:30:39 GMT  
		Size: 276.1 MB (276142526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565b026b882cad92844dfc1c4c5d0619d4d0fe95790eb902171c48202b3aae9a`  
		Last Modified: Tue, 27 Apr 2021 21:30:11 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f0de3e0d9c5c3715a2c8c808ad51b45af2b6141ae0a13ebd36e3e05ad7b16e`  
		Last Modified: Tue, 27 Apr 2021 21:30:10 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25251fc5f00fa4b60910029578b9d0dadd3fdc684c1be0e8042d01afc810610f`  
		Last Modified: Tue, 27 Apr 2021 21:30:10 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b5b04b5eb330c38aa6c0fd95d74220744ff5805bfad4b8176e20b200b4bedf`  
		Last Modified: Tue, 27 Apr 2021 21:30:10 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:8c0a94658711ba6778ac1942003b70c4d5a9c61b77e1b032420196098de08193
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:7b8ea1938bdc21561816a37227f454a96f45340edfb718571a4c0203cd8576f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.6 MB (542589540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c95932e9ddf5401af16b4b8bae1eb59eb3eb376dd73b51537c92da04f07b484`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 12:37:46 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 10 Apr 2021 12:37:46 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 10 Apr 2021 12:37:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 12:37:47 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Sat, 10 Apr 2021 12:39:11 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 10 Apr 2021 12:39:27 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:39:39 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:39:39 GMT
ENV ODOO_VERSION=12.0
# Tue, 27 Apr 2021 21:26:52 GMT
ARG ODOO_RELEASE=20210427
# Tue, 27 Apr 2021 21:26:52 GMT
ARG ODOO_SHA=9e00c380b73efce6b164c2a0d7127de65feed2e3
# Tue, 27 Apr 2021 21:27:57 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9e00c380b73efce6b164c2a0d7127de65feed2e3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Apr 2021 21:28:01 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 27 Apr 2021 21:28:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Apr 2021 21:28:02 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9e00c380b73efce6b164c2a0d7127de65feed2e3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Apr 2021 21:28:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Apr 2021 21:28:02 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Apr 2021 21:28:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Apr 2021 21:28:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Apr 2021 21:28:03 GMT
USER odoo
# Tue, 27 Apr 2021 21:28:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Apr 2021 21:28:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cf89834cbbd2b3cee3b8a944f6b45e4a1507584664ee0a1b02259590615d59`  
		Last Modified: Sat, 10 Apr 2021 12:42:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b11cee4db50450b66bc29b47f68b86380f02d6097f24e2b69a05dab9b82788`  
		Last Modified: Sat, 10 Apr 2021 12:43:18 GMT  
		Size: 219.6 MB (219645154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98555f4c9e696b99e0a4429cafe8848f74f7baa37c2265bd07bdc5d7ca50ece3`  
		Last Modified: Sat, 10 Apr 2021 12:42:52 GMT  
		Size: 2.2 MB (2224102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd66427a8f8ee5f5e15e695a9171413d51a17fd3fa05b78c6b7b8f7f2b8a259`  
		Last Modified: Sat, 10 Apr 2021 12:42:56 GMT  
		Size: 22.0 MB (22046831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8321ff954c4b2aba8c5626362d7ff51082e97e348c7ba2a8fdda0b102fefb94`  
		Last Modified: Tue, 27 Apr 2021 21:30:39 GMT  
		Size: 276.1 MB (276142526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565b026b882cad92844dfc1c4c5d0619d4d0fe95790eb902171c48202b3aae9a`  
		Last Modified: Tue, 27 Apr 2021 21:30:11 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f0de3e0d9c5c3715a2c8c808ad51b45af2b6141ae0a13ebd36e3e05ad7b16e`  
		Last Modified: Tue, 27 Apr 2021 21:30:10 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25251fc5f00fa4b60910029578b9d0dadd3fdc684c1be0e8042d01afc810610f`  
		Last Modified: Tue, 27 Apr 2021 21:30:10 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b5b04b5eb330c38aa6c0fd95d74220744ff5805bfad4b8176e20b200b4bedf`  
		Last Modified: Tue, 27 Apr 2021 21:30:10 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:248d53161381f188435217e10a626509bc9edce16a7288ff9f19bad4c6f9f6c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:ef35fb62a08eede1c92f082e6f208fb78c15ac99f9e8b768eeb26b70ea0a6688
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.3 MB (532339535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70b4a641acfbce02b087878e5edf12587b8977cd830a7d1fd5b4ba4800566c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 12:30:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 10 Apr 2021 12:30:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 10 Apr 2021 12:30:54 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 12:35:54 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 10 Apr 2021 12:36:08 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:36:13 GMT
RUN npm install -g rtlcss
# Sat, 10 Apr 2021 12:36:14 GMT
ENV ODOO_VERSION=13.0
# Tue, 27 Apr 2021 21:25:26 GMT
ARG ODOO_RELEASE=20210427
# Tue, 27 Apr 2021 21:25:27 GMT
ARG ODOO_SHA=57acf994bb3ed666494231138a7318cfa8d30bec
# Tue, 27 Apr 2021 21:26:38 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=57acf994bb3ed666494231138a7318cfa8d30bec
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Apr 2021 21:26:39 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 27 Apr 2021 21:26:39 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Apr 2021 21:26:40 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=57acf994bb3ed666494231138a7318cfa8d30bec
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Apr 2021 21:26:40 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Apr 2021 21:26:41 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Apr 2021 21:26:41 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Apr 2021 21:26:41 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Apr 2021 21:26:41 GMT
USER odoo
# Tue, 27 Apr 2021 21:26:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Apr 2021 21:26:41 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f81febf0e37dd17e29257f92caf652e1fead27661526fffe25491be70915d3`  
		Last Modified: Sat, 10 Apr 2021 12:42:31 GMT  
		Size: 207.1 MB (207124621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79303e39ab88305c57546603826b66e6eb084ae3937717320b18885c8f73fb60`  
		Last Modified: Sat, 10 Apr 2021 12:42:03 GMT  
		Size: 2.3 MB (2345472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185986373d8432024fd24e5a223928c83785fd54e9527e2380262b64e621206b`  
		Last Modified: Sat, 10 Apr 2021 12:42:06 GMT  
		Size: 896.8 KB (896834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9231325b603a112f3c41f92a85cb460e5b57e820ba3cc0ad1d02892c5237acb`  
		Last Modified: Tue, 27 Apr 2021 21:29:56 GMT  
		Size: 294.8 MB (294830804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7399ae52898c55bcb9b11c29f36dcb032ce4b151c85e86cbd167eafaa732dd28`  
		Last Modified: Tue, 27 Apr 2021 21:29:23 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170ae46f0bd75e5b6adae879b1dc4fbbebd3b0b53ac5d8d6be0d2de046aed10a`  
		Last Modified: Tue, 27 Apr 2021 21:29:23 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c954a43d58d1ba91f502b76030c99357869828c67c1fc70ee243901baee7af`  
		Last Modified: Tue, 27 Apr 2021 21:29:23 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eade6b558200861ba6240bbfc71f208d67053618ada527e845cce878fa631e4`  
		Last Modified: Tue, 27 Apr 2021 21:29:23 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:248d53161381f188435217e10a626509bc9edce16a7288ff9f19bad4c6f9f6c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:ef35fb62a08eede1c92f082e6f208fb78c15ac99f9e8b768eeb26b70ea0a6688
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.3 MB (532339535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70b4a641acfbce02b087878e5edf12587b8977cd830a7d1fd5b4ba4800566c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 12:30:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 10 Apr 2021 12:30:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 10 Apr 2021 12:30:54 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 12:35:54 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 10 Apr 2021 12:36:08 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:36:13 GMT
RUN npm install -g rtlcss
# Sat, 10 Apr 2021 12:36:14 GMT
ENV ODOO_VERSION=13.0
# Tue, 27 Apr 2021 21:25:26 GMT
ARG ODOO_RELEASE=20210427
# Tue, 27 Apr 2021 21:25:27 GMT
ARG ODOO_SHA=57acf994bb3ed666494231138a7318cfa8d30bec
# Tue, 27 Apr 2021 21:26:38 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=57acf994bb3ed666494231138a7318cfa8d30bec
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Apr 2021 21:26:39 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 27 Apr 2021 21:26:39 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Apr 2021 21:26:40 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=57acf994bb3ed666494231138a7318cfa8d30bec
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Apr 2021 21:26:40 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Apr 2021 21:26:41 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Apr 2021 21:26:41 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Apr 2021 21:26:41 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Apr 2021 21:26:41 GMT
USER odoo
# Tue, 27 Apr 2021 21:26:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Apr 2021 21:26:41 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f81febf0e37dd17e29257f92caf652e1fead27661526fffe25491be70915d3`  
		Last Modified: Sat, 10 Apr 2021 12:42:31 GMT  
		Size: 207.1 MB (207124621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79303e39ab88305c57546603826b66e6eb084ae3937717320b18885c8f73fb60`  
		Last Modified: Sat, 10 Apr 2021 12:42:03 GMT  
		Size: 2.3 MB (2345472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185986373d8432024fd24e5a223928c83785fd54e9527e2380262b64e621206b`  
		Last Modified: Sat, 10 Apr 2021 12:42:06 GMT  
		Size: 896.8 KB (896834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9231325b603a112f3c41f92a85cb460e5b57e820ba3cc0ad1d02892c5237acb`  
		Last Modified: Tue, 27 Apr 2021 21:29:56 GMT  
		Size: 294.8 MB (294830804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7399ae52898c55bcb9b11c29f36dcb032ce4b151c85e86cbd167eafaa732dd28`  
		Last Modified: Tue, 27 Apr 2021 21:29:23 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170ae46f0bd75e5b6adae879b1dc4fbbebd3b0b53ac5d8d6be0d2de046aed10a`  
		Last Modified: Tue, 27 Apr 2021 21:29:23 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c954a43d58d1ba91f502b76030c99357869828c67c1fc70ee243901baee7af`  
		Last Modified: Tue, 27 Apr 2021 21:29:23 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eade6b558200861ba6240bbfc71f208d67053618ada527e845cce878fa631e4`  
		Last Modified: Tue, 27 Apr 2021 21:29:23 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:cbf4d2c87bbce86a0cae5db2d8f08debb8072222fba043ceab755b7b6c8a0e41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:5c134193f01ac4b36ead740d2cb828865f83d2ef3833dd1c298379773937fcaa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.1 MB (516118672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f97cdf3e7abe1fa762f3699ad9e1884f9c5bc9c51659ec570660deb1a6f31d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 12:30:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 10 Apr 2021 12:30:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 10 Apr 2021 12:30:54 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 12:32:34 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 10 Apr 2021 12:32:46 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:32:51 GMT
RUN npm install -g rtlcss
# Sat, 10 Apr 2021 12:32:51 GMT
ENV ODOO_VERSION=14.0
# Tue, 27 Apr 2021 21:24:01 GMT
ARG ODOO_RELEASE=20210427
# Tue, 27 Apr 2021 21:24:01 GMT
ARG ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
# Tue, 27 Apr 2021 21:25:13 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Apr 2021 21:25:17 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 27 Apr 2021 21:25:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Apr 2021 21:25:19 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Apr 2021 21:25:19 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Apr 2021 21:25:19 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Apr 2021 21:25:19 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Apr 2021 21:25:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Apr 2021 21:25:20 GMT
USER odoo
# Tue, 27 Apr 2021 21:25:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Apr 2021 21:25:20 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df7a8fcf45065b035b83165d399d7900a139dc5e00d9e4d6ce8699785fb5343`  
		Last Modified: Sat, 10 Apr 2021 12:41:41 GMT  
		Size: 213.2 MB (213170428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6128de947157b937143a4ca96babae9ce2e9b71d01a4b53dc0a4e1301bdaa0d4`  
		Last Modified: Sat, 10 Apr 2021 12:41:12 GMT  
		Size: 2.3 MB (2348669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963607ad2a1b5492ef59daa14209ad6d7e164abe8c9f0636566235cff0d20ade`  
		Last Modified: Sat, 10 Apr 2021 12:41:11 GMT  
		Size: 896.6 KB (896573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca57d7a391cae7292e0bc1b366c0235632ce91ec42f6ddf11e87eed7a0f78ff`  
		Last Modified: Tue, 27 Apr 2021 21:29:03 GMT  
		Size: 272.6 MB (272561198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa28544e22fad79a6ff3318efd2f9637f3e7132129a3736e6260be436d937906`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58612f6171ea665c9f2a89e0c8289ec06b8e4ba6e415be926a196da48b1f1e1`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9578101cbabb3a13af26665ba25b59d7a6db44e1215db0bdb8cb3c2e17a019ba`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc314e016235206bc8b95f020e07554a3ffa4eb36ff256201d40228290b94f47`  
		Last Modified: Tue, 27 Apr 2021 21:28:32 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:cbf4d2c87bbce86a0cae5db2d8f08debb8072222fba043ceab755b7b6c8a0e41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:5c134193f01ac4b36ead740d2cb828865f83d2ef3833dd1c298379773937fcaa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.1 MB (516118672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f97cdf3e7abe1fa762f3699ad9e1884f9c5bc9c51659ec570660deb1a6f31d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 12:30:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 10 Apr 2021 12:30:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 10 Apr 2021 12:30:54 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 12:32:34 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 10 Apr 2021 12:32:46 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:32:51 GMT
RUN npm install -g rtlcss
# Sat, 10 Apr 2021 12:32:51 GMT
ENV ODOO_VERSION=14.0
# Tue, 27 Apr 2021 21:24:01 GMT
ARG ODOO_RELEASE=20210427
# Tue, 27 Apr 2021 21:24:01 GMT
ARG ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
# Tue, 27 Apr 2021 21:25:13 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Apr 2021 21:25:17 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 27 Apr 2021 21:25:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Apr 2021 21:25:19 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Apr 2021 21:25:19 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Apr 2021 21:25:19 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Apr 2021 21:25:19 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Apr 2021 21:25:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Apr 2021 21:25:20 GMT
USER odoo
# Tue, 27 Apr 2021 21:25:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Apr 2021 21:25:20 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df7a8fcf45065b035b83165d399d7900a139dc5e00d9e4d6ce8699785fb5343`  
		Last Modified: Sat, 10 Apr 2021 12:41:41 GMT  
		Size: 213.2 MB (213170428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6128de947157b937143a4ca96babae9ce2e9b71d01a4b53dc0a4e1301bdaa0d4`  
		Last Modified: Sat, 10 Apr 2021 12:41:12 GMT  
		Size: 2.3 MB (2348669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963607ad2a1b5492ef59daa14209ad6d7e164abe8c9f0636566235cff0d20ade`  
		Last Modified: Sat, 10 Apr 2021 12:41:11 GMT  
		Size: 896.6 KB (896573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca57d7a391cae7292e0bc1b366c0235632ce91ec42f6ddf11e87eed7a0f78ff`  
		Last Modified: Tue, 27 Apr 2021 21:29:03 GMT  
		Size: 272.6 MB (272561198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa28544e22fad79a6ff3318efd2f9637f3e7132129a3736e6260be436d937906`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58612f6171ea665c9f2a89e0c8289ec06b8e4ba6e415be926a196da48b1f1e1`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9578101cbabb3a13af26665ba25b59d7a6db44e1215db0bdb8cb3c2e17a019ba`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc314e016235206bc8b95f020e07554a3ffa4eb36ff256201d40228290b94f47`  
		Last Modified: Tue, 27 Apr 2021 21:28:32 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:cbf4d2c87bbce86a0cae5db2d8f08debb8072222fba043ceab755b7b6c8a0e41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:5c134193f01ac4b36ead740d2cb828865f83d2ef3833dd1c298379773937fcaa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.1 MB (516118672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f97cdf3e7abe1fa762f3699ad9e1884f9c5bc9c51659ec570660deb1a6f31d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 12:30:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 10 Apr 2021 12:30:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 10 Apr 2021 12:30:54 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 12:32:34 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 10 Apr 2021 12:32:46 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:32:51 GMT
RUN npm install -g rtlcss
# Sat, 10 Apr 2021 12:32:51 GMT
ENV ODOO_VERSION=14.0
# Tue, 27 Apr 2021 21:24:01 GMT
ARG ODOO_RELEASE=20210427
# Tue, 27 Apr 2021 21:24:01 GMT
ARG ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
# Tue, 27 Apr 2021 21:25:13 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Apr 2021 21:25:17 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 27 Apr 2021 21:25:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Apr 2021 21:25:19 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Apr 2021 21:25:19 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Apr 2021 21:25:19 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Apr 2021 21:25:19 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Apr 2021 21:25:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Apr 2021 21:25:20 GMT
USER odoo
# Tue, 27 Apr 2021 21:25:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Apr 2021 21:25:20 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df7a8fcf45065b035b83165d399d7900a139dc5e00d9e4d6ce8699785fb5343`  
		Last Modified: Sat, 10 Apr 2021 12:41:41 GMT  
		Size: 213.2 MB (213170428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6128de947157b937143a4ca96babae9ce2e9b71d01a4b53dc0a4e1301bdaa0d4`  
		Last Modified: Sat, 10 Apr 2021 12:41:12 GMT  
		Size: 2.3 MB (2348669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963607ad2a1b5492ef59daa14209ad6d7e164abe8c9f0636566235cff0d20ade`  
		Last Modified: Sat, 10 Apr 2021 12:41:11 GMT  
		Size: 896.6 KB (896573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca57d7a391cae7292e0bc1b366c0235632ce91ec42f6ddf11e87eed7a0f78ff`  
		Last Modified: Tue, 27 Apr 2021 21:29:03 GMT  
		Size: 272.6 MB (272561198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa28544e22fad79a6ff3318efd2f9637f3e7132129a3736e6260be436d937906`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58612f6171ea665c9f2a89e0c8289ec06b8e4ba6e415be926a196da48b1f1e1`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9578101cbabb3a13af26665ba25b59d7a6db44e1215db0bdb8cb3c2e17a019ba`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc314e016235206bc8b95f020e07554a3ffa4eb36ff256201d40228290b94f47`  
		Last Modified: Tue, 27 Apr 2021 21:28:32 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
