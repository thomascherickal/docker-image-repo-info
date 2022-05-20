<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `odoo`

-	[`odoo:13`](#odoo13)
-	[`odoo:13.0`](#odoo130)
-	[`odoo:14`](#odoo14)
-	[`odoo:14.0`](#odoo140)
-	[`odoo:15`](#odoo15)
-	[`odoo:15.0`](#odoo150)
-	[`odoo:latest`](#odoolatest)

## `odoo:13`

```console
$ docker pull odoo@sha256:15d2bbaf49ceba96fa67e04b573a5d915cfcaa58c825513ed800024dfbca72d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:f5271e1847ec8f7169156ef88f44839168e0ab65f3f31e702f815a92f5ad3e50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.0 MB (540010646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640f96cde51243c43d8642f4d91ed7f028c4ad5a22bbcc839181cbe538c9e7fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:37:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 11 May 2022 05:37:29 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 11 May 2022 05:37:29 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:41:18 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 11 May 2022 05:41:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:41:29 GMT
RUN npm install -g rtlcss
# Wed, 11 May 2022 05:41:29 GMT
ENV ODOO_VERSION=13.0
# Fri, 20 May 2022 19:46:37 GMT
ARG ODOO_RELEASE=20220520
# Fri, 20 May 2022 19:46:37 GMT
ARG ODOO_SHA=33fd70bdad094c91ccf445753be2043c9b059b33
# Fri, 20 May 2022 19:47:49 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=33fd70bdad094c91ccf445753be2043c9b059b33
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 20 May 2022 19:47:52 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 20 May 2022 19:47:53 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 20 May 2022 19:47:53 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=33fd70bdad094c91ccf445753be2043c9b059b33
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 20 May 2022 19:47:53 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 20 May 2022 19:47:53 GMT
EXPOSE 8069 8071 8072
# Fri, 20 May 2022 19:47:53 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 20 May 2022 19:47:54 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 20 May 2022 19:47:54 GMT
USER odoo
# Fri, 20 May 2022 19:47:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 May 2022 19:47:54 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e6252588f0e6abcf931957ac7bfc2a5e5b32db2ed14dbd6b2e8a66685a5788`  
		Last Modified: Wed, 11 May 2022 05:45:17 GMT  
		Size: 207.1 MB (207143132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0b687cc39be53c1d539fc0c580160e7d11fe3a1d308058504206f40872bf99`  
		Last Modified: Wed, 11 May 2022 05:44:56 GMT  
		Size: 13.4 MB (13438332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471fc1f5680601316e623c4c30bc1211a0b42d586e9a52fd1515c2bb3f4184d5`  
		Last Modified: Wed, 11 May 2022 05:44:53 GMT  
		Size: 468.5 KB (468467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d1ebbc83efcd24cf684f7bef4a1056beb5a1f71ed0912c9e6cc84b25122a16`  
		Last Modified: Fri, 20 May 2022 19:50:11 GMT  
		Size: 291.8 MB (291817528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b2950b0f59a77271d9925df3997fdf0d43dad31d0e94ac43d84e50553b50b1`  
		Last Modified: Fri, 20 May 2022 19:49:41 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bd04a037cfcee46e424cf9d89ab3800f7f3f0877b1a1ca61f45709830a25ec`  
		Last Modified: Fri, 20 May 2022 19:49:41 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab6f8d060d2236f661d0bac47aaf6ed0288d1d9ea1996e3761bf16135769b42`  
		Last Modified: Fri, 20 May 2022 19:49:41 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cd9fddc877c36c21f24b880f44443d6f7ac214881c4593318f1a99887d686a`  
		Last Modified: Fri, 20 May 2022 19:49:41 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:15d2bbaf49ceba96fa67e04b573a5d915cfcaa58c825513ed800024dfbca72d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:f5271e1847ec8f7169156ef88f44839168e0ab65f3f31e702f815a92f5ad3e50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.0 MB (540010646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640f96cde51243c43d8642f4d91ed7f028c4ad5a22bbcc839181cbe538c9e7fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:37:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 11 May 2022 05:37:29 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 11 May 2022 05:37:29 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:41:18 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 11 May 2022 05:41:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:41:29 GMT
RUN npm install -g rtlcss
# Wed, 11 May 2022 05:41:29 GMT
ENV ODOO_VERSION=13.0
# Fri, 20 May 2022 19:46:37 GMT
ARG ODOO_RELEASE=20220520
# Fri, 20 May 2022 19:46:37 GMT
ARG ODOO_SHA=33fd70bdad094c91ccf445753be2043c9b059b33
# Fri, 20 May 2022 19:47:49 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=33fd70bdad094c91ccf445753be2043c9b059b33
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 20 May 2022 19:47:52 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 20 May 2022 19:47:53 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 20 May 2022 19:47:53 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=33fd70bdad094c91ccf445753be2043c9b059b33
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 20 May 2022 19:47:53 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 20 May 2022 19:47:53 GMT
EXPOSE 8069 8071 8072
# Fri, 20 May 2022 19:47:53 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 20 May 2022 19:47:54 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 20 May 2022 19:47:54 GMT
USER odoo
# Fri, 20 May 2022 19:47:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 May 2022 19:47:54 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e6252588f0e6abcf931957ac7bfc2a5e5b32db2ed14dbd6b2e8a66685a5788`  
		Last Modified: Wed, 11 May 2022 05:45:17 GMT  
		Size: 207.1 MB (207143132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0b687cc39be53c1d539fc0c580160e7d11fe3a1d308058504206f40872bf99`  
		Last Modified: Wed, 11 May 2022 05:44:56 GMT  
		Size: 13.4 MB (13438332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471fc1f5680601316e623c4c30bc1211a0b42d586e9a52fd1515c2bb3f4184d5`  
		Last Modified: Wed, 11 May 2022 05:44:53 GMT  
		Size: 468.5 KB (468467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d1ebbc83efcd24cf684f7bef4a1056beb5a1f71ed0912c9e6cc84b25122a16`  
		Last Modified: Fri, 20 May 2022 19:50:11 GMT  
		Size: 291.8 MB (291817528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b2950b0f59a77271d9925df3997fdf0d43dad31d0e94ac43d84e50553b50b1`  
		Last Modified: Fri, 20 May 2022 19:49:41 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bd04a037cfcee46e424cf9d89ab3800f7f3f0877b1a1ca61f45709830a25ec`  
		Last Modified: Fri, 20 May 2022 19:49:41 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab6f8d060d2236f661d0bac47aaf6ed0288d1d9ea1996e3761bf16135769b42`  
		Last Modified: Fri, 20 May 2022 19:49:41 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cd9fddc877c36c21f24b880f44443d6f7ac214881c4593318f1a99887d686a`  
		Last Modified: Fri, 20 May 2022 19:49:41 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:fa1e56e8a4b89b0be33381748041a7cc81e71073f9022f37ed37a810e50cecb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:ab1f73e539799babeb5b30c16ff52cc367f92861770fc02bb6736f2a7cc9afc6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.1 MB (530115032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a7cebdc3e96f8d1a9fed1c95e02151b9e77b25c93f65c36714e718dbb73e293`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:37:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 11 May 2022 05:37:29 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 11 May 2022 05:37:29 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:38:35 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 11 May 2022 05:38:46 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:38:49 GMT
RUN npm install -g rtlcss
# Wed, 11 May 2022 05:38:49 GMT
ENV ODOO_VERSION=14.0
# Fri, 20 May 2022 19:44:59 GMT
ARG ODOO_RELEASE=20220520
# Fri, 20 May 2022 19:44:59 GMT
ARG ODOO_SHA=f666f4a72c7ace2fa13eea01970012011c7d4828
# Fri, 20 May 2022 19:46:23 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=f666f4a72c7ace2fa13eea01970012011c7d4828
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 20 May 2022 19:46:27 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 20 May 2022 19:46:27 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 20 May 2022 19:46:27 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=f666f4a72c7ace2fa13eea01970012011c7d4828
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 20 May 2022 19:46:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 20 May 2022 19:46:28 GMT
EXPOSE 8069 8071 8072
# Fri, 20 May 2022 19:46:28 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 20 May 2022 19:46:28 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 20 May 2022 19:46:28 GMT
USER odoo
# Fri, 20 May 2022 19:46:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 May 2022 19:46:28 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18be9ffd7343938551d01a3a348c625c03ca09031fcd3e96756ea392eb19866f`  
		Last Modified: Wed, 11 May 2022 05:44:28 GMT  
		Size: 213.2 MB (213181643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bf10be0bcd5e9c9e8630aeb1c60b92f2abcdc6a0d1bc51a41f715cbff2b208`  
		Last Modified: Wed, 11 May 2022 05:44:05 GMT  
		Size: 13.4 MB (13440768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c667279c5c1e86e3868c1fe0d7a90481ceac438eefa2678773f2aeda7cb8153`  
		Last Modified: Wed, 11 May 2022 05:44:03 GMT  
		Size: 468.4 KB (468439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7964457ffd1c6ab14bff00b63c8cdcbb28f5fdb144076b5f7e6284cb620bfbc7`  
		Last Modified: Fri, 20 May 2022 19:49:31 GMT  
		Size: 275.9 MB (275881001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1637200286b38cfe13160c87d5712143eb31d42dd3eb581c76f6f580ba9112`  
		Last Modified: Fri, 20 May 2022 19:48:59 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedac79b536d59dcbdfa6808a94dd6fbd1458b753a92995afdbfee71522e8d95`  
		Last Modified: Fri, 20 May 2022 19:48:59 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3331fff77a771c7534ec4cc099f6f84e8e192eae4756a509dcead59fdcd251`  
		Last Modified: Fri, 20 May 2022 19:48:59 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196392704580e871d59edba0192bd7556b6cbba9f427af29e789bfd2796cc09d`  
		Last Modified: Fri, 20 May 2022 19:48:59 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:fa1e56e8a4b89b0be33381748041a7cc81e71073f9022f37ed37a810e50cecb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:ab1f73e539799babeb5b30c16ff52cc367f92861770fc02bb6736f2a7cc9afc6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.1 MB (530115032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a7cebdc3e96f8d1a9fed1c95e02151b9e77b25c93f65c36714e718dbb73e293`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:37:29 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 11 May 2022 05:37:29 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 11 May 2022 05:37:29 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:38:35 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 11 May 2022 05:38:46 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:38:49 GMT
RUN npm install -g rtlcss
# Wed, 11 May 2022 05:38:49 GMT
ENV ODOO_VERSION=14.0
# Fri, 20 May 2022 19:44:59 GMT
ARG ODOO_RELEASE=20220520
# Fri, 20 May 2022 19:44:59 GMT
ARG ODOO_SHA=f666f4a72c7ace2fa13eea01970012011c7d4828
# Fri, 20 May 2022 19:46:23 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=f666f4a72c7ace2fa13eea01970012011c7d4828
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 20 May 2022 19:46:27 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 20 May 2022 19:46:27 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 20 May 2022 19:46:27 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=f666f4a72c7ace2fa13eea01970012011c7d4828
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 20 May 2022 19:46:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 20 May 2022 19:46:28 GMT
EXPOSE 8069 8071 8072
# Fri, 20 May 2022 19:46:28 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 20 May 2022 19:46:28 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 20 May 2022 19:46:28 GMT
USER odoo
# Fri, 20 May 2022 19:46:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 May 2022 19:46:28 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18be9ffd7343938551d01a3a348c625c03ca09031fcd3e96756ea392eb19866f`  
		Last Modified: Wed, 11 May 2022 05:44:28 GMT  
		Size: 213.2 MB (213181643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bf10be0bcd5e9c9e8630aeb1c60b92f2abcdc6a0d1bc51a41f715cbff2b208`  
		Last Modified: Wed, 11 May 2022 05:44:05 GMT  
		Size: 13.4 MB (13440768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c667279c5c1e86e3868c1fe0d7a90481ceac438eefa2678773f2aeda7cb8153`  
		Last Modified: Wed, 11 May 2022 05:44:03 GMT  
		Size: 468.4 KB (468439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7964457ffd1c6ab14bff00b63c8cdcbb28f5fdb144076b5f7e6284cb620bfbc7`  
		Last Modified: Fri, 20 May 2022 19:49:31 GMT  
		Size: 275.9 MB (275881001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1637200286b38cfe13160c87d5712143eb31d42dd3eb581c76f6f580ba9112`  
		Last Modified: Fri, 20 May 2022 19:48:59 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedac79b536d59dcbdfa6808a94dd6fbd1458b753a92995afdbfee71522e8d95`  
		Last Modified: Fri, 20 May 2022 19:48:59 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3331fff77a771c7534ec4cc099f6f84e8e192eae4756a509dcead59fdcd251`  
		Last Modified: Fri, 20 May 2022 19:48:59 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196392704580e871d59edba0192bd7556b6cbba9f427af29e789bfd2796cc09d`  
		Last Modified: Fri, 20 May 2022 19:48:59 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:654b4410ff7956bbf646ef945733937e4b3a9e3a0949b3bf29c9ffdc424c4c96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:864cc0bce1b875d439f83c246f6df21f549494788944a6d6796853eed3b192bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **555.2 MB (555158606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ed4e47d112da9ebebc07e50b2fe743a9168b69cb6e7c8414c39dd5a09ee40c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:34:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 11 May 2022 05:34:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 11 May 2022 05:34:51 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:35:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 11 May 2022 05:35:58 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:36:00 GMT
RUN npm install -g rtlcss
# Wed, 11 May 2022 05:36:00 GMT
ENV ODOO_VERSION=15.0
# Fri, 20 May 2022 19:42:36 GMT
ARG ODOO_RELEASE=20220520
# Fri, 20 May 2022 19:42:37 GMT
ARG ODOO_SHA=0663b11f4c05c66aadfe74fbd27b14beaa9e0f07
# Fri, 20 May 2022 19:44:40 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=0663b11f4c05c66aadfe74fbd27b14beaa9e0f07
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 20 May 2022 19:44:44 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 20 May 2022 19:44:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 20 May 2022 19:44:44 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=0663b11f4c05c66aadfe74fbd27b14beaa9e0f07
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 20 May 2022 19:44:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 20 May 2022 19:44:45 GMT
EXPOSE 8069 8071 8072
# Fri, 20 May 2022 19:44:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 20 May 2022 19:44:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 20 May 2022 19:44:45 GMT
USER odoo
# Fri, 20 May 2022 19:44:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 May 2022 19:44:45 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26162ed3131197f6879615fefb5c8aa8bc5c0c135769db733a201cfb52c67be`  
		Last Modified: Wed, 11 May 2022 05:43:40 GMT  
		Size: 220.3 MB (220307699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486a4342c69cbaf3a5a1133c9f3eedbc817147246d4232cce876bd2843070a54`  
		Last Modified: Wed, 11 May 2022 05:43:14 GMT  
		Size: 2.5 MB (2510102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978adca0c78b0c610ce566793437791b380153b4ae98d4551063a87572379869`  
		Last Modified: Wed, 11 May 2022 05:43:14 GMT  
		Size: 462.1 KB (462052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680c1464667c5498ec04ad0bc4d06ea51b4b63c63130486918efe4668d991446`  
		Last Modified: Fri, 20 May 2022 19:48:45 GMT  
		Size: 300.5 MB (300496814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde8e87f076eb50ead1b59e7750d6448de5a7d21b06634e0fb79dcc31cc55816`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b63c3e2ebd1bde97ad5300d1fb586932adcb48c319839910d338333c0c0b740`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874af05fcb650d4b0a84ea2a7dcc987df26721b1ca05ae45843cd19ff36f331a`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd43c16ffc830ee559b7f39896a9a89d4b7ad76dcb2df47c1a24848dfe1d4bf`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:654b4410ff7956bbf646ef945733937e4b3a9e3a0949b3bf29c9ffdc424c4c96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:864cc0bce1b875d439f83c246f6df21f549494788944a6d6796853eed3b192bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **555.2 MB (555158606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ed4e47d112da9ebebc07e50b2fe743a9168b69cb6e7c8414c39dd5a09ee40c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:34:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 11 May 2022 05:34:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 11 May 2022 05:34:51 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:35:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 11 May 2022 05:35:58 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:36:00 GMT
RUN npm install -g rtlcss
# Wed, 11 May 2022 05:36:00 GMT
ENV ODOO_VERSION=15.0
# Fri, 20 May 2022 19:42:36 GMT
ARG ODOO_RELEASE=20220520
# Fri, 20 May 2022 19:42:37 GMT
ARG ODOO_SHA=0663b11f4c05c66aadfe74fbd27b14beaa9e0f07
# Fri, 20 May 2022 19:44:40 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=0663b11f4c05c66aadfe74fbd27b14beaa9e0f07
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 20 May 2022 19:44:44 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 20 May 2022 19:44:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 20 May 2022 19:44:44 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=0663b11f4c05c66aadfe74fbd27b14beaa9e0f07
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 20 May 2022 19:44:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 20 May 2022 19:44:45 GMT
EXPOSE 8069 8071 8072
# Fri, 20 May 2022 19:44:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 20 May 2022 19:44:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 20 May 2022 19:44:45 GMT
USER odoo
# Fri, 20 May 2022 19:44:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 May 2022 19:44:45 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26162ed3131197f6879615fefb5c8aa8bc5c0c135769db733a201cfb52c67be`  
		Last Modified: Wed, 11 May 2022 05:43:40 GMT  
		Size: 220.3 MB (220307699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486a4342c69cbaf3a5a1133c9f3eedbc817147246d4232cce876bd2843070a54`  
		Last Modified: Wed, 11 May 2022 05:43:14 GMT  
		Size: 2.5 MB (2510102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978adca0c78b0c610ce566793437791b380153b4ae98d4551063a87572379869`  
		Last Modified: Wed, 11 May 2022 05:43:14 GMT  
		Size: 462.1 KB (462052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680c1464667c5498ec04ad0bc4d06ea51b4b63c63130486918efe4668d991446`  
		Last Modified: Fri, 20 May 2022 19:48:45 GMT  
		Size: 300.5 MB (300496814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde8e87f076eb50ead1b59e7750d6448de5a7d21b06634e0fb79dcc31cc55816`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b63c3e2ebd1bde97ad5300d1fb586932adcb48c319839910d338333c0c0b740`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874af05fcb650d4b0a84ea2a7dcc987df26721b1ca05ae45843cd19ff36f331a`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd43c16ffc830ee559b7f39896a9a89d4b7ad76dcb2df47c1a24848dfe1d4bf`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:654b4410ff7956bbf646ef945733937e4b3a9e3a0949b3bf29c9ffdc424c4c96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:864cc0bce1b875d439f83c246f6df21f549494788944a6d6796853eed3b192bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **555.2 MB (555158606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ed4e47d112da9ebebc07e50b2fe743a9168b69cb6e7c8414c39dd5a09ee40c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:34:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 11 May 2022 05:34:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 11 May 2022 05:34:51 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 05:35:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 11 May 2022 05:35:58 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:36:00 GMT
RUN npm install -g rtlcss
# Wed, 11 May 2022 05:36:00 GMT
ENV ODOO_VERSION=15.0
# Fri, 20 May 2022 19:42:36 GMT
ARG ODOO_RELEASE=20220520
# Fri, 20 May 2022 19:42:37 GMT
ARG ODOO_SHA=0663b11f4c05c66aadfe74fbd27b14beaa9e0f07
# Fri, 20 May 2022 19:44:40 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=0663b11f4c05c66aadfe74fbd27b14beaa9e0f07
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 20 May 2022 19:44:44 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 20 May 2022 19:44:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 20 May 2022 19:44:44 GMT
# ARGS: ODOO_RELEASE=20220520 ODOO_SHA=0663b11f4c05c66aadfe74fbd27b14beaa9e0f07
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 20 May 2022 19:44:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 20 May 2022 19:44:45 GMT
EXPOSE 8069 8071 8072
# Fri, 20 May 2022 19:44:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 20 May 2022 19:44:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 20 May 2022 19:44:45 GMT
USER odoo
# Fri, 20 May 2022 19:44:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 May 2022 19:44:45 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26162ed3131197f6879615fefb5c8aa8bc5c0c135769db733a201cfb52c67be`  
		Last Modified: Wed, 11 May 2022 05:43:40 GMT  
		Size: 220.3 MB (220307699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486a4342c69cbaf3a5a1133c9f3eedbc817147246d4232cce876bd2843070a54`  
		Last Modified: Wed, 11 May 2022 05:43:14 GMT  
		Size: 2.5 MB (2510102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978adca0c78b0c610ce566793437791b380153b4ae98d4551063a87572379869`  
		Last Modified: Wed, 11 May 2022 05:43:14 GMT  
		Size: 462.1 KB (462052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680c1464667c5498ec04ad0bc4d06ea51b4b63c63130486918efe4668d991446`  
		Last Modified: Fri, 20 May 2022 19:48:45 GMT  
		Size: 300.5 MB (300496814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde8e87f076eb50ead1b59e7750d6448de5a7d21b06634e0fb79dcc31cc55816`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b63c3e2ebd1bde97ad5300d1fb586932adcb48c319839910d338333c0c0b740`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874af05fcb650d4b0a84ea2a7dcc987df26721b1ca05ae45843cd19ff36f331a`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd43c16ffc830ee559b7f39896a9a89d4b7ad76dcb2df47c1a24848dfe1d4bf`  
		Last Modified: Fri, 20 May 2022 19:48:11 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
