<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `odoo`

-	[`odoo:11`](#odoo11)
-	[`odoo:11.0`](#odoo110)
-	[`odoo:12`](#odoo12)
-	[`odoo:12.0`](#odoo120)
-	[`odoo:13`](#odoo13)
-	[`odoo:13.0`](#odoo130)
-	[`odoo:latest`](#odoolatest)

## `odoo:11`

```console
$ docker pull odoo@sha256:79bdf03e6a795b6bf33b20764752d72e652ea1011cc7359c786ed89317535321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:11` - linux; amd64

```console
$ docker pull odoo@sha256:6ac0a14a864757f8549eaa4a530aa5c9e686f88d69f98b6630bd8a7f92a71a4c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385854800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d3e9c0e96236531c435a9d3ab497cc8371cc8c57ca6496ab127ab39c2c35df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:06:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 01 Feb 2020 19:06:33 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 19:06:34 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Sat, 01 Feb 2020 19:08:41 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 01 Feb 2020 19:08:52 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:10:34 GMT
ENV ODOO_VERSION=11.0
# Sat, 01 Feb 2020 19:10:34 GMT
ARG ODOO_RELEASE=20200121
# Sat, 01 Feb 2020 19:10:35 GMT
ARG ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
# Sat, 01 Feb 2020 19:11:44 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 01 Feb 2020 19:11:45 GMT
COPY file:cdc612ad49467417b0321c166f94e4f99b071755cb6ade071774e83d3b6ee4cb in / 
# Sat, 01 Feb 2020 19:11:46 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 01 Feb 2020 19:11:47 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 01 Feb 2020 19:11:48 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 01 Feb 2020 19:11:48 GMT
EXPOSE 8069 8071
# Sat, 01 Feb 2020 19:11:48 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 01 Feb 2020 19:11:49 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 01 Feb 2020 19:11:49 GMT
USER odoo
# Sat, 01 Feb 2020 19:11:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 01 Feb 2020 19:11:50 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6636e1389360a7dbe88a6d4b5ad58fe407b5d5febc94198e97f9da76d0db7fc`  
		Last Modified: Sat, 01 Feb 2020 19:13:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1001e4454508c0b88a62a04671fa51167d6067114ab006f54d71a63360498b59`  
		Last Modified: Sat, 01 Feb 2020 19:14:29 GMT  
		Size: 219.6 MB (219649778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93cad4ab6da49beab8b2d5308f290e586281283a633fbe52dcde9973bf0b4d`  
		Last Modified: Sat, 01 Feb 2020 19:13:27 GMT  
		Size: 2.2 MB (2246091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca141bcd9d8704f74897eb8ecf89796e452a1e712cdfd61100165ff2e8e49ba3`  
		Last Modified: Sat, 01 Feb 2020 19:15:22 GMT  
		Size: 141.4 MB (141431578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270e41372d15d79301377ae129580bb7557516da29fed6a609249bd74c13626f`  
		Last Modified: Sat, 01 Feb 2020 19:14:43 GMT  
		Size: 674.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14154ac4bf53ba51f3d9b2b7713e16eb4f65d0210bd6edaeb4edb20f3436b84`  
		Last Modified: Sat, 01 Feb 2020 19:14:43 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b65f98ed2de983646c31c4000939fd64dc521a25cd46b1c802d705bf3ba8a2`  
		Last Modified: Sat, 01 Feb 2020 19:14:43 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de928c2a2933d0a0f88dc6eef11f93df903bc71272634477703a8e6d545b698`  
		Last Modified: Sat, 01 Feb 2020 19:14:42 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:11.0`

```console
$ docker pull odoo@sha256:79bdf03e6a795b6bf33b20764752d72e652ea1011cc7359c786ed89317535321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:11.0` - linux; amd64

```console
$ docker pull odoo@sha256:6ac0a14a864757f8549eaa4a530aa5c9e686f88d69f98b6630bd8a7f92a71a4c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385854800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d3e9c0e96236531c435a9d3ab497cc8371cc8c57ca6496ab127ab39c2c35df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:06:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 01 Feb 2020 19:06:33 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 19:06:34 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Sat, 01 Feb 2020 19:08:41 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 01 Feb 2020 19:08:52 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:10:34 GMT
ENV ODOO_VERSION=11.0
# Sat, 01 Feb 2020 19:10:34 GMT
ARG ODOO_RELEASE=20200121
# Sat, 01 Feb 2020 19:10:35 GMT
ARG ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
# Sat, 01 Feb 2020 19:11:44 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 01 Feb 2020 19:11:45 GMT
COPY file:cdc612ad49467417b0321c166f94e4f99b071755cb6ade071774e83d3b6ee4cb in / 
# Sat, 01 Feb 2020 19:11:46 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 01 Feb 2020 19:11:47 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 01 Feb 2020 19:11:48 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 01 Feb 2020 19:11:48 GMT
EXPOSE 8069 8071
# Sat, 01 Feb 2020 19:11:48 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 01 Feb 2020 19:11:49 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 01 Feb 2020 19:11:49 GMT
USER odoo
# Sat, 01 Feb 2020 19:11:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 01 Feb 2020 19:11:50 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6636e1389360a7dbe88a6d4b5ad58fe407b5d5febc94198e97f9da76d0db7fc`  
		Last Modified: Sat, 01 Feb 2020 19:13:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1001e4454508c0b88a62a04671fa51167d6067114ab006f54d71a63360498b59`  
		Last Modified: Sat, 01 Feb 2020 19:14:29 GMT  
		Size: 219.6 MB (219649778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93cad4ab6da49beab8b2d5308f290e586281283a633fbe52dcde9973bf0b4d`  
		Last Modified: Sat, 01 Feb 2020 19:13:27 GMT  
		Size: 2.2 MB (2246091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca141bcd9d8704f74897eb8ecf89796e452a1e712cdfd61100165ff2e8e49ba3`  
		Last Modified: Sat, 01 Feb 2020 19:15:22 GMT  
		Size: 141.4 MB (141431578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270e41372d15d79301377ae129580bb7557516da29fed6a609249bd74c13626f`  
		Last Modified: Sat, 01 Feb 2020 19:14:43 GMT  
		Size: 674.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14154ac4bf53ba51f3d9b2b7713e16eb4f65d0210bd6edaeb4edb20f3436b84`  
		Last Modified: Sat, 01 Feb 2020 19:14:43 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b65f98ed2de983646c31c4000939fd64dc521a25cd46b1c802d705bf3ba8a2`  
		Last Modified: Sat, 01 Feb 2020 19:14:43 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de928c2a2933d0a0f88dc6eef11f93df903bc71272634477703a8e6d545b698`  
		Last Modified: Sat, 01 Feb 2020 19:14:42 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12`

```console
$ docker pull odoo@sha256:51806ba59fc3ddf3366c54e0dde1f5f944076772b1c481fee415195603eb6747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:19ee26bb6dece127e3d4ae90366b28eee5162b506648eb00c831f8b5212161f2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.8 MB (399785958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77f70f635b55918723b1f8621e0aaf864c9c71c3e7d061f116133a4cc46b39df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:06:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 01 Feb 2020 19:06:33 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 19:06:34 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Sat, 01 Feb 2020 19:08:41 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 01 Feb 2020 19:08:52 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:09:06 GMT
RUN set -x;    echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && export GNUPGHOME="$(mktemp -d)"     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:09:06 GMT
ENV ODOO_VERSION=12.0
# Sat, 01 Feb 2020 19:09:06 GMT
ARG ODOO_RELEASE=20200121
# Sat, 01 Feb 2020 19:09:07 GMT
ARG ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
# Sat, 01 Feb 2020 19:10:17 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 01 Feb 2020 19:10:19 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Sat, 01 Feb 2020 19:10:19 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 01 Feb 2020 19:10:21 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 01 Feb 2020 19:10:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 01 Feb 2020 19:10:21 GMT
EXPOSE 8069 8071
# Sat, 01 Feb 2020 19:10:22 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 01 Feb 2020 19:10:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 01 Feb 2020 19:10:22 GMT
USER odoo
# Sat, 01 Feb 2020 19:10:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 01 Feb 2020 19:10:23 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6636e1389360a7dbe88a6d4b5ad58fe407b5d5febc94198e97f9da76d0db7fc`  
		Last Modified: Sat, 01 Feb 2020 19:13:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1001e4454508c0b88a62a04671fa51167d6067114ab006f54d71a63360498b59`  
		Last Modified: Sat, 01 Feb 2020 19:14:29 GMT  
		Size: 219.6 MB (219649778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93cad4ab6da49beab8b2d5308f290e586281283a633fbe52dcde9973bf0b4d`  
		Last Modified: Sat, 01 Feb 2020 19:13:27 GMT  
		Size: 2.2 MB (2246091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696044a6246f18eb8405ae1772dec20b53cc2d0d72db48b9f0aee5c7f242b561`  
		Last Modified: Sat, 01 Feb 2020 19:13:43 GMT  
		Size: 26.6 MB (26563414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f295a9cbec4c99453d75e462481f2e163a26604575eb4fe57ce167a920f38ebd`  
		Last Modified: Sat, 01 Feb 2020 19:14:34 GMT  
		Size: 128.8 MB (128799323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b662dfe9568c3d509b3e270ed658edf671bcd0562b2c2c7fed5526871712b351`  
		Last Modified: Sat, 01 Feb 2020 19:13:25 GMT  
		Size: 673.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6046210b506c359d53b527e7cdf21a5e18d7afff881f68f72e6c28324ad49aaf`  
		Last Modified: Sat, 01 Feb 2020 19:13:25 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127800ddd18f318af62988601f77c451dd77f1be6b352c083847201aa0243b0`  
		Last Modified: Sat, 01 Feb 2020 19:13:25 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c12399acb7e4e9ac55515d77cd7ce2edac42f4fad49bfc005ccab00bb2a88a`  
		Last Modified: Sat, 01 Feb 2020 19:13:25 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:51806ba59fc3ddf3366c54e0dde1f5f944076772b1c481fee415195603eb6747
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:19ee26bb6dece127e3d4ae90366b28eee5162b506648eb00c831f8b5212161f2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.8 MB (399785958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77f70f635b55918723b1f8621e0aaf864c9c71c3e7d061f116133a4cc46b39df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:06:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 01 Feb 2020 19:06:33 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 19:06:34 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Sat, 01 Feb 2020 19:08:41 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 01 Feb 2020 19:08:52 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:09:06 GMT
RUN set -x;    echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && export GNUPGHOME="$(mktemp -d)"     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:09:06 GMT
ENV ODOO_VERSION=12.0
# Sat, 01 Feb 2020 19:09:06 GMT
ARG ODOO_RELEASE=20200121
# Sat, 01 Feb 2020 19:09:07 GMT
ARG ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
# Sat, 01 Feb 2020 19:10:17 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 01 Feb 2020 19:10:19 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Sat, 01 Feb 2020 19:10:19 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 01 Feb 2020 19:10:21 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 01 Feb 2020 19:10:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 01 Feb 2020 19:10:21 GMT
EXPOSE 8069 8071
# Sat, 01 Feb 2020 19:10:22 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 01 Feb 2020 19:10:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 01 Feb 2020 19:10:22 GMT
USER odoo
# Sat, 01 Feb 2020 19:10:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 01 Feb 2020 19:10:23 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6636e1389360a7dbe88a6d4b5ad58fe407b5d5febc94198e97f9da76d0db7fc`  
		Last Modified: Sat, 01 Feb 2020 19:13:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1001e4454508c0b88a62a04671fa51167d6067114ab006f54d71a63360498b59`  
		Last Modified: Sat, 01 Feb 2020 19:14:29 GMT  
		Size: 219.6 MB (219649778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93cad4ab6da49beab8b2d5308f290e586281283a633fbe52dcde9973bf0b4d`  
		Last Modified: Sat, 01 Feb 2020 19:13:27 GMT  
		Size: 2.2 MB (2246091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696044a6246f18eb8405ae1772dec20b53cc2d0d72db48b9f0aee5c7f242b561`  
		Last Modified: Sat, 01 Feb 2020 19:13:43 GMT  
		Size: 26.6 MB (26563414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f295a9cbec4c99453d75e462481f2e163a26604575eb4fe57ce167a920f38ebd`  
		Last Modified: Sat, 01 Feb 2020 19:14:34 GMT  
		Size: 128.8 MB (128799323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b662dfe9568c3d509b3e270ed658edf671bcd0562b2c2c7fed5526871712b351`  
		Last Modified: Sat, 01 Feb 2020 19:13:25 GMT  
		Size: 673.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6046210b506c359d53b527e7cdf21a5e18d7afff881f68f72e6c28324ad49aaf`  
		Last Modified: Sat, 01 Feb 2020 19:13:25 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5127800ddd18f318af62988601f77c451dd77f1be6b352c083847201aa0243b0`  
		Last Modified: Sat, 01 Feb 2020 19:13:25 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c12399acb7e4e9ac55515d77cd7ce2edac42f4fad49bfc005ccab00bb2a88a`  
		Last Modified: Sat, 01 Feb 2020 19:13:25 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:41c93959d1ff41266fd0d26f58bec3361120268c3f54e66958b2c12fec2083e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:f78531da1d4f264d9dcc770600d657b66f1cdbdc6fa5ed501687eca15fd30f5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.3 MB (376261515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae67748cb53b097d49b5fe66c7657537be0e2861b0874adfc22b2a95ec4726e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:03:16 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 01 Feb 2020 19:03:17 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 19:04:48 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 01 Feb 2020 19:04:59 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:05 GMT
RUN set -x;     npm install -g rtlcss
# Sat, 01 Feb 2020 19:05:06 GMT
ENV ODOO_VERSION=13.0
# Sat, 01 Feb 2020 19:05:06 GMT
ARG ODOO_RELEASE=20200121
# Sat, 01 Feb 2020 19:05:06 GMT
ARG ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
# Sat, 01 Feb 2020 19:06:16 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 01 Feb 2020 19:06:18 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Sat, 01 Feb 2020 19:06:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 01 Feb 2020 19:06:19 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 01 Feb 2020 19:06:20 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 01 Feb 2020 19:06:20 GMT
EXPOSE 8069 8071
# Sat, 01 Feb 2020 19:06:20 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 01 Feb 2020 19:06:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 01 Feb 2020 19:06:21 GMT
USER odoo
# Sat, 01 Feb 2020 19:06:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 01 Feb 2020 19:06:21 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65612bcd6c3150161603c1fd1d5aaa47db0ce71135a0deb6d213304333d3b79a`  
		Last Modified: Sat, 01 Feb 2020 19:13:07 GMT  
		Size: 203.5 MB (203544811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59b34b423f564ca69f18c9dc5722cd2f289fe2ca9c3d49b86fd110bb4ece81`  
		Last Modified: Sat, 01 Feb 2020 19:12:13 GMT  
		Size: 2.2 MB (2228753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c777e556ebc3a8c13db32b99364e7cbf7139db60cb8e14ef998a88dc68f9eb38`  
		Last Modified: Sat, 01 Feb 2020 19:12:13 GMT  
		Size: 1.1 MB (1069181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a3171af1a9b1a492efd30e7e44b0a1729f760214d834b9beeb856671bd012`  
		Last Modified: Sat, 01 Feb 2020 19:13:19 GMT  
		Size: 142.3 MB (142324108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fdba9aca9cd4ea8dcb656f9629a7497c142ea58a4843c863072cead42dbb4a`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf6028473093cbd7373cab5b706d94d841ddee4125cbf7201c0744c987e1ed6`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e56222b4392a9a4276d1d4852e6b653d76b608012a6b12ae2711fa99a24e8e`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f1ae3150fbab6a2e14e37830f152c94c56978853ae9428856baea37d2929d`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:41c93959d1ff41266fd0d26f58bec3361120268c3f54e66958b2c12fec2083e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:f78531da1d4f264d9dcc770600d657b66f1cdbdc6fa5ed501687eca15fd30f5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.3 MB (376261515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae67748cb53b097d49b5fe66c7657537be0e2861b0874adfc22b2a95ec4726e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:03:16 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 01 Feb 2020 19:03:17 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 19:04:48 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 01 Feb 2020 19:04:59 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:05 GMT
RUN set -x;     npm install -g rtlcss
# Sat, 01 Feb 2020 19:05:06 GMT
ENV ODOO_VERSION=13.0
# Sat, 01 Feb 2020 19:05:06 GMT
ARG ODOO_RELEASE=20200121
# Sat, 01 Feb 2020 19:05:06 GMT
ARG ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
# Sat, 01 Feb 2020 19:06:16 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 01 Feb 2020 19:06:18 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Sat, 01 Feb 2020 19:06:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 01 Feb 2020 19:06:19 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 01 Feb 2020 19:06:20 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 01 Feb 2020 19:06:20 GMT
EXPOSE 8069 8071
# Sat, 01 Feb 2020 19:06:20 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 01 Feb 2020 19:06:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 01 Feb 2020 19:06:21 GMT
USER odoo
# Sat, 01 Feb 2020 19:06:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 01 Feb 2020 19:06:21 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65612bcd6c3150161603c1fd1d5aaa47db0ce71135a0deb6d213304333d3b79a`  
		Last Modified: Sat, 01 Feb 2020 19:13:07 GMT  
		Size: 203.5 MB (203544811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59b34b423f564ca69f18c9dc5722cd2f289fe2ca9c3d49b86fd110bb4ece81`  
		Last Modified: Sat, 01 Feb 2020 19:12:13 GMT  
		Size: 2.2 MB (2228753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c777e556ebc3a8c13db32b99364e7cbf7139db60cb8e14ef998a88dc68f9eb38`  
		Last Modified: Sat, 01 Feb 2020 19:12:13 GMT  
		Size: 1.1 MB (1069181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a3171af1a9b1a492efd30e7e44b0a1729f760214d834b9beeb856671bd012`  
		Last Modified: Sat, 01 Feb 2020 19:13:19 GMT  
		Size: 142.3 MB (142324108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fdba9aca9cd4ea8dcb656f9629a7497c142ea58a4843c863072cead42dbb4a`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf6028473093cbd7373cab5b706d94d841ddee4125cbf7201c0744c987e1ed6`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e56222b4392a9a4276d1d4852e6b653d76b608012a6b12ae2711fa99a24e8e`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f1ae3150fbab6a2e14e37830f152c94c56978853ae9428856baea37d2929d`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:41c93959d1ff41266fd0d26f58bec3361120268c3f54e66958b2c12fec2083e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:f78531da1d4f264d9dcc770600d657b66f1cdbdc6fa5ed501687eca15fd30f5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.3 MB (376261515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae67748cb53b097d49b5fe66c7657537be0e2861b0874adfc22b2a95ec4726e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:03:16 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 01 Feb 2020 19:03:17 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 19:04:48 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 01 Feb 2020 19:04:59 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:05 GMT
RUN set -x;     npm install -g rtlcss
# Sat, 01 Feb 2020 19:05:06 GMT
ENV ODOO_VERSION=13.0
# Sat, 01 Feb 2020 19:05:06 GMT
ARG ODOO_RELEASE=20200121
# Sat, 01 Feb 2020 19:05:06 GMT
ARG ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
# Sat, 01 Feb 2020 19:06:16 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 01 Feb 2020 19:06:18 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Sat, 01 Feb 2020 19:06:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 01 Feb 2020 19:06:19 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 01 Feb 2020 19:06:20 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 01 Feb 2020 19:06:20 GMT
EXPOSE 8069 8071
# Sat, 01 Feb 2020 19:06:20 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 01 Feb 2020 19:06:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 01 Feb 2020 19:06:21 GMT
USER odoo
# Sat, 01 Feb 2020 19:06:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 01 Feb 2020 19:06:21 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65612bcd6c3150161603c1fd1d5aaa47db0ce71135a0deb6d213304333d3b79a`  
		Last Modified: Sat, 01 Feb 2020 19:13:07 GMT  
		Size: 203.5 MB (203544811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59b34b423f564ca69f18c9dc5722cd2f289fe2ca9c3d49b86fd110bb4ece81`  
		Last Modified: Sat, 01 Feb 2020 19:12:13 GMT  
		Size: 2.2 MB (2228753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c777e556ebc3a8c13db32b99364e7cbf7139db60cb8e14ef998a88dc68f9eb38`  
		Last Modified: Sat, 01 Feb 2020 19:12:13 GMT  
		Size: 1.1 MB (1069181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a3171af1a9b1a492efd30e7e44b0a1729f760214d834b9beeb856671bd012`  
		Last Modified: Sat, 01 Feb 2020 19:13:19 GMT  
		Size: 142.3 MB (142324108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fdba9aca9cd4ea8dcb656f9629a7497c142ea58a4843c863072cead42dbb4a`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf6028473093cbd7373cab5b706d94d841ddee4125cbf7201c0744c987e1ed6`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e56222b4392a9a4276d1d4852e6b653d76b608012a6b12ae2711fa99a24e8e`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f1ae3150fbab6a2e14e37830f152c94c56978853ae9428856baea37d2929d`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
