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
$ docker pull odoo@sha256:b3f9a56365a9ac0ac2e86502374d2e30e8dca0153addeb945afa139185e467d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:0f466e71449ba7af7df342c76305f6027639e7cbda31dfb24d5e7b9351e97a77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.6 MB (539632522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e8d902642082e10e97e844e6ec2189c26f306b5f9846472b98d89d2b9c1a29c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:08:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 01 Mar 2022 14:08:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 01 Mar 2022 14:08:35 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 14:13:55 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 01 Mar 2022 14:14:27 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:14:32 GMT
RUN npm install -g rtlcss
# Tue, 01 Mar 2022 14:14:32 GMT
ENV ODOO_VERSION=13.0
# Mon, 07 Mar 2022 19:49:39 GMT
ARG ODOO_RELEASE=20220307
# Mon, 07 Mar 2022 19:49:39 GMT
ARG ODOO_SHA=63fac7c528d28de8df554f15c0a99a9efaa63ff5
# Mon, 07 Mar 2022 19:50:49 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=63fac7c528d28de8df554f15c0a99a9efaa63ff5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 07 Mar 2022 19:50:53 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 07 Mar 2022 19:50:53 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 07 Mar 2022 19:50:54 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=63fac7c528d28de8df554f15c0a99a9efaa63ff5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 07 Mar 2022 19:50:54 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 07 Mar 2022 19:50:54 GMT
EXPOSE 8069 8071 8072
# Mon, 07 Mar 2022 19:50:54 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 07 Mar 2022 19:50:54 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 07 Mar 2022 19:50:54 GMT
USER odoo
# Mon, 07 Mar 2022 19:50:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Mar 2022 19:50:54 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51d7a5019b187d246e9ae3da10053fb1cfc762a66834ca03e4a95d4f22f6c7c`  
		Last Modified: Tue, 01 Mar 2022 14:19:18 GMT  
		Size: 207.1 MB (207134366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f774b6ab8a9647a0abef7a9cafee8664e94673b07fc70cb6f1dc847a1a8ef6b3`  
		Last Modified: Tue, 01 Mar 2022 14:18:53 GMT  
		Size: 13.4 MB (13438497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92100f15afab684a47d277389605f2ec7c5eee252fd7f30b7d61e621e62ca89`  
		Last Modified: Tue, 01 Mar 2022 14:18:49 GMT  
		Size: 454.1 KB (454054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90edbc21af9a68ec13060cd5e4ea9efcdda82adfda8fd17f20147041f590c0bd`  
		Last Modified: Mon, 07 Mar 2022 19:53:10 GMT  
		Size: 291.4 MB (291449405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a1dd58a118c99c68c75c59111826352c822c08320fe9a8037c101576bd2d81`  
		Last Modified: Mon, 07 Mar 2022 19:52:40 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21841547e2491bee5f9b2a2bbbc5775905676955a3776f6bf275abbc12b390fb`  
		Last Modified: Mon, 07 Mar 2022 19:52:39 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8b281d60ca74c9bfbd4cec62051fdf5f5674298201612aaf3f40d33285eeb0`  
		Last Modified: Mon, 07 Mar 2022 19:52:39 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b81b12074905376256aa21be6052629e8b6eb61453509ae1f4b72fb1ee4f0a`  
		Last Modified: Mon, 07 Mar 2022 19:52:39 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:b3f9a56365a9ac0ac2e86502374d2e30e8dca0153addeb945afa139185e467d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:0f466e71449ba7af7df342c76305f6027639e7cbda31dfb24d5e7b9351e97a77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.6 MB (539632522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e8d902642082e10e97e844e6ec2189c26f306b5f9846472b98d89d2b9c1a29c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:08:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 01 Mar 2022 14:08:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 01 Mar 2022 14:08:35 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 14:13:55 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 01 Mar 2022 14:14:27 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:14:32 GMT
RUN npm install -g rtlcss
# Tue, 01 Mar 2022 14:14:32 GMT
ENV ODOO_VERSION=13.0
# Mon, 07 Mar 2022 19:49:39 GMT
ARG ODOO_RELEASE=20220307
# Mon, 07 Mar 2022 19:49:39 GMT
ARG ODOO_SHA=63fac7c528d28de8df554f15c0a99a9efaa63ff5
# Mon, 07 Mar 2022 19:50:49 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=63fac7c528d28de8df554f15c0a99a9efaa63ff5
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 07 Mar 2022 19:50:53 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 07 Mar 2022 19:50:53 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 07 Mar 2022 19:50:54 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=63fac7c528d28de8df554f15c0a99a9efaa63ff5
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 07 Mar 2022 19:50:54 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 07 Mar 2022 19:50:54 GMT
EXPOSE 8069 8071 8072
# Mon, 07 Mar 2022 19:50:54 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 07 Mar 2022 19:50:54 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 07 Mar 2022 19:50:54 GMT
USER odoo
# Mon, 07 Mar 2022 19:50:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Mar 2022 19:50:54 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51d7a5019b187d246e9ae3da10053fb1cfc762a66834ca03e4a95d4f22f6c7c`  
		Last Modified: Tue, 01 Mar 2022 14:19:18 GMT  
		Size: 207.1 MB (207134366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f774b6ab8a9647a0abef7a9cafee8664e94673b07fc70cb6f1dc847a1a8ef6b3`  
		Last Modified: Tue, 01 Mar 2022 14:18:53 GMT  
		Size: 13.4 MB (13438497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92100f15afab684a47d277389605f2ec7c5eee252fd7f30b7d61e621e62ca89`  
		Last Modified: Tue, 01 Mar 2022 14:18:49 GMT  
		Size: 454.1 KB (454054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90edbc21af9a68ec13060cd5e4ea9efcdda82adfda8fd17f20147041f590c0bd`  
		Last Modified: Mon, 07 Mar 2022 19:53:10 GMT  
		Size: 291.4 MB (291449405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a1dd58a118c99c68c75c59111826352c822c08320fe9a8037c101576bd2d81`  
		Last Modified: Mon, 07 Mar 2022 19:52:40 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21841547e2491bee5f9b2a2bbbc5775905676955a3776f6bf275abbc12b390fb`  
		Last Modified: Mon, 07 Mar 2022 19:52:39 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8b281d60ca74c9bfbd4cec62051fdf5f5674298201612aaf3f40d33285eeb0`  
		Last Modified: Mon, 07 Mar 2022 19:52:39 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b81b12074905376256aa21be6052629e8b6eb61453509ae1f4b72fb1ee4f0a`  
		Last Modified: Mon, 07 Mar 2022 19:52:39 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:b14dca8ed46d08f44eb6ad61ad44a7670b99e7350bf094ba85cd01b9ca852921
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:7fce683962590bad5695792b43c2ab7ff72a0c293ee6d4d08fb6e5901a398821
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.5 MB (529461761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe69d309472acdb6571aa5066f423df26c9be3dd265624f2e96af647464f962`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:08:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 01 Mar 2022 14:08:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 01 Mar 2022 14:08:35 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 14:10:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 01 Mar 2022 14:10:44 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:10:47 GMT
RUN npm install -g rtlcss
# Tue, 01 Mar 2022 14:10:47 GMT
ENV ODOO_VERSION=14.0
# Mon, 07 Mar 2022 19:48:16 GMT
ARG ODOO_RELEASE=20220307
# Mon, 07 Mar 2022 19:48:16 GMT
ARG ODOO_SHA=4260081fc3a7712e6e2627289673ac586adedbd7
# Mon, 07 Mar 2022 19:49:25 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=4260081fc3a7712e6e2627289673ac586adedbd7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 07 Mar 2022 19:49:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 07 Mar 2022 19:49:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 07 Mar 2022 19:49:30 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=4260081fc3a7712e6e2627289673ac586adedbd7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 07 Mar 2022 19:49:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 07 Mar 2022 19:49:30 GMT
EXPOSE 8069 8071 8072
# Mon, 07 Mar 2022 19:49:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 07 Mar 2022 19:49:30 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 07 Mar 2022 19:49:30 GMT
USER odoo
# Mon, 07 Mar 2022 19:49:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Mar 2022 19:49:30 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f744a3eb8faa9c53b9214156a1731a3f54041ba4452fda20403c4a974d7833c5`  
		Last Modified: Tue, 01 Mar 2022 14:18:29 GMT  
		Size: 213.2 MB (213175223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65e732c75de0a0623a3815cfbf17f73b6c4a96a58458b08bffb71d148e34f`  
		Last Modified: Tue, 01 Mar 2022 14:17:48 GMT  
		Size: 13.4 MB (13440948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c0506bf3aadc634c05ab579f7616d756a1e9542e0d9eb8d0ef50b95334dc04`  
		Last Modified: Tue, 01 Mar 2022 14:17:42 GMT  
		Size: 453.9 KB (453933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54742b7c1f24de89d5ac36de780237c6250c4327a8e6503103027095242afe4a`  
		Last Modified: Mon, 07 Mar 2022 19:52:30 GMT  
		Size: 275.2 MB (275235462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5410f2ced9a21b5e025a3f3eec6971af29e222e16f07ae3322c78922e87fe9a`  
		Last Modified: Mon, 07 Mar 2022 19:51:58 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9767845354712cf41c6efb8afa8971cefaec2785b409987e18c24fcc398d43`  
		Last Modified: Mon, 07 Mar 2022 19:51:58 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366ea98ba868076821b2b941f295e353e92aef90e36006e3f3f8d7cd3ac5f507`  
		Last Modified: Mon, 07 Mar 2022 19:51:58 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb83ca07811727e5d9dc033450778bc1afcf48737c49a9c528de760ba12bc4ef`  
		Last Modified: Mon, 07 Mar 2022 19:51:58 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:b14dca8ed46d08f44eb6ad61ad44a7670b99e7350bf094ba85cd01b9ca852921
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:7fce683962590bad5695792b43c2ab7ff72a0c293ee6d4d08fb6e5901a398821
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.5 MB (529461761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe69d309472acdb6571aa5066f423df26c9be3dd265624f2e96af647464f962`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:08:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 01 Mar 2022 14:08:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 01 Mar 2022 14:08:35 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 14:10:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 01 Mar 2022 14:10:44 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:10:47 GMT
RUN npm install -g rtlcss
# Tue, 01 Mar 2022 14:10:47 GMT
ENV ODOO_VERSION=14.0
# Mon, 07 Mar 2022 19:48:16 GMT
ARG ODOO_RELEASE=20220307
# Mon, 07 Mar 2022 19:48:16 GMT
ARG ODOO_SHA=4260081fc3a7712e6e2627289673ac586adedbd7
# Mon, 07 Mar 2022 19:49:25 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=4260081fc3a7712e6e2627289673ac586adedbd7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 07 Mar 2022 19:49:29 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 07 Mar 2022 19:49:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 07 Mar 2022 19:49:30 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=4260081fc3a7712e6e2627289673ac586adedbd7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 07 Mar 2022 19:49:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 07 Mar 2022 19:49:30 GMT
EXPOSE 8069 8071 8072
# Mon, 07 Mar 2022 19:49:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 07 Mar 2022 19:49:30 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 07 Mar 2022 19:49:30 GMT
USER odoo
# Mon, 07 Mar 2022 19:49:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Mar 2022 19:49:30 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f744a3eb8faa9c53b9214156a1731a3f54041ba4452fda20403c4a974d7833c5`  
		Last Modified: Tue, 01 Mar 2022 14:18:29 GMT  
		Size: 213.2 MB (213175223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e65e732c75de0a0623a3815cfbf17f73b6c4a96a58458b08bffb71d148e34f`  
		Last Modified: Tue, 01 Mar 2022 14:17:48 GMT  
		Size: 13.4 MB (13440948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c0506bf3aadc634c05ab579f7616d756a1e9542e0d9eb8d0ef50b95334dc04`  
		Last Modified: Tue, 01 Mar 2022 14:17:42 GMT  
		Size: 453.9 KB (453933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54742b7c1f24de89d5ac36de780237c6250c4327a8e6503103027095242afe4a`  
		Last Modified: Mon, 07 Mar 2022 19:52:30 GMT  
		Size: 275.2 MB (275235462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5410f2ced9a21b5e025a3f3eec6971af29e222e16f07ae3322c78922e87fe9a`  
		Last Modified: Mon, 07 Mar 2022 19:51:58 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9767845354712cf41c6efb8afa8971cefaec2785b409987e18c24fcc398d43`  
		Last Modified: Mon, 07 Mar 2022 19:51:58 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366ea98ba868076821b2b941f295e353e92aef90e36006e3f3f8d7cd3ac5f507`  
		Last Modified: Mon, 07 Mar 2022 19:51:58 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb83ca07811727e5d9dc033450778bc1afcf48737c49a9c528de760ba12bc4ef`  
		Last Modified: Mon, 07 Mar 2022 19:51:58 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:15820ddae9c880f2f4e0885469a4ed52b675e36b6bffbd22f2f1c92e6f639e62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:9f3285245b8cafa3537ad422b73a5a37054dc15377cdc882f15d9b8d1980c31f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.3 MB (551278571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2d50b63355fbcb5995a68839b79d45665c30bc4ade0e741b080e8bc09a1a9fc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:04:27 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 01 Mar 2022 14:04:27 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 01 Mar 2022 14:04:27 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 14:05:42 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 01 Mar 2022 14:06:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:06:30 GMT
RUN npm install -g rtlcss
# Tue, 01 Mar 2022 14:06:30 GMT
ENV ODOO_VERSION=15.0
# Mon, 07 Mar 2022 19:46:53 GMT
ARG ODOO_RELEASE=20220307
# Mon, 07 Mar 2022 19:46:53 GMT
ARG ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
# Mon, 07 Mar 2022 19:48:07 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 07 Mar 2022 19:48:11 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 07 Mar 2022 19:48:11 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 07 Mar 2022 19:48:12 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 07 Mar 2022 19:48:12 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 07 Mar 2022 19:48:12 GMT
EXPOSE 8069 8071 8072
# Mon, 07 Mar 2022 19:48:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 07 Mar 2022 19:48:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 07 Mar 2022 19:48:12 GMT
USER odoo
# Mon, 07 Mar 2022 19:48:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Mar 2022 19:48:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a163ebeb0494c6130a80754f29b68a5c07419748988cf37afb9630747c41c69`  
		Last Modified: Tue, 01 Mar 2022 14:17:16 GMT  
		Size: 220.3 MB (220298373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2966b8e28ea8e47acbcca748753c937ef05bfde069cd7bfd2f70252b765fea99`  
		Last Modified: Tue, 01 Mar 2022 14:16:39 GMT  
		Size: 2.5 MB (2510056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9cf6997d2b0f369d91a2ce39d67ba3e78767956bd3cfdfc8d4287600b5389d`  
		Last Modified: Tue, 01 Mar 2022 14:16:38 GMT  
		Size: 447.3 KB (447285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a00db9ec98d74309ff4179c1227d6d2fef69862ff23de7e21984c3f67b479a0`  
		Last Modified: Mon, 07 Mar 2022 19:51:45 GMT  
		Size: 296.7 MB (296654000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493b4385630dec4e8162af9df1c6d4df55714493efc51596eb4a164c4eb63f49`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e655a91665cca257ae7d1746494a821d078d3d91e4ad4e20bcf1949dcb603d79`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d79ec5bcc003281f0154def0c30ec11a3b5baba4bbe5d1a53805e44c4d1d39`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a035624d232c158962c533e416ba594597e913d645f5a84a3f7e65f1ec01c76`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:15820ddae9c880f2f4e0885469a4ed52b675e36b6bffbd22f2f1c92e6f639e62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:9f3285245b8cafa3537ad422b73a5a37054dc15377cdc882f15d9b8d1980c31f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.3 MB (551278571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2d50b63355fbcb5995a68839b79d45665c30bc4ade0e741b080e8bc09a1a9fc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:04:27 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 01 Mar 2022 14:04:27 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 01 Mar 2022 14:04:27 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 14:05:42 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 01 Mar 2022 14:06:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:06:30 GMT
RUN npm install -g rtlcss
# Tue, 01 Mar 2022 14:06:30 GMT
ENV ODOO_VERSION=15.0
# Mon, 07 Mar 2022 19:46:53 GMT
ARG ODOO_RELEASE=20220307
# Mon, 07 Mar 2022 19:46:53 GMT
ARG ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
# Mon, 07 Mar 2022 19:48:07 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 07 Mar 2022 19:48:11 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 07 Mar 2022 19:48:11 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 07 Mar 2022 19:48:12 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 07 Mar 2022 19:48:12 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 07 Mar 2022 19:48:12 GMT
EXPOSE 8069 8071 8072
# Mon, 07 Mar 2022 19:48:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 07 Mar 2022 19:48:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 07 Mar 2022 19:48:12 GMT
USER odoo
# Mon, 07 Mar 2022 19:48:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Mar 2022 19:48:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a163ebeb0494c6130a80754f29b68a5c07419748988cf37afb9630747c41c69`  
		Last Modified: Tue, 01 Mar 2022 14:17:16 GMT  
		Size: 220.3 MB (220298373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2966b8e28ea8e47acbcca748753c937ef05bfde069cd7bfd2f70252b765fea99`  
		Last Modified: Tue, 01 Mar 2022 14:16:39 GMT  
		Size: 2.5 MB (2510056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9cf6997d2b0f369d91a2ce39d67ba3e78767956bd3cfdfc8d4287600b5389d`  
		Last Modified: Tue, 01 Mar 2022 14:16:38 GMT  
		Size: 447.3 KB (447285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a00db9ec98d74309ff4179c1227d6d2fef69862ff23de7e21984c3f67b479a0`  
		Last Modified: Mon, 07 Mar 2022 19:51:45 GMT  
		Size: 296.7 MB (296654000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493b4385630dec4e8162af9df1c6d4df55714493efc51596eb4a164c4eb63f49`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e655a91665cca257ae7d1746494a821d078d3d91e4ad4e20bcf1949dcb603d79`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d79ec5bcc003281f0154def0c30ec11a3b5baba4bbe5d1a53805e44c4d1d39`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a035624d232c158962c533e416ba594597e913d645f5a84a3f7e65f1ec01c76`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:15820ddae9c880f2f4e0885469a4ed52b675e36b6bffbd22f2f1c92e6f639e62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:9f3285245b8cafa3537ad422b73a5a37054dc15377cdc882f15d9b8d1980c31f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.3 MB (551278571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2d50b63355fbcb5995a68839b79d45665c30bc4ade0e741b080e8bc09a1a9fc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:04:27 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 01 Mar 2022 14:04:27 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 01 Mar 2022 14:04:27 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 14:05:42 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 01 Mar 2022 14:06:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:06:30 GMT
RUN npm install -g rtlcss
# Tue, 01 Mar 2022 14:06:30 GMT
ENV ODOO_VERSION=15.0
# Mon, 07 Mar 2022 19:46:53 GMT
ARG ODOO_RELEASE=20220307
# Mon, 07 Mar 2022 19:46:53 GMT
ARG ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
# Mon, 07 Mar 2022 19:48:07 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 07 Mar 2022 19:48:11 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 07 Mar 2022 19:48:11 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 07 Mar 2022 19:48:12 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 07 Mar 2022 19:48:12 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 07 Mar 2022 19:48:12 GMT
EXPOSE 8069 8071 8072
# Mon, 07 Mar 2022 19:48:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 07 Mar 2022 19:48:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 07 Mar 2022 19:48:12 GMT
USER odoo
# Mon, 07 Mar 2022 19:48:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Mar 2022 19:48:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a163ebeb0494c6130a80754f29b68a5c07419748988cf37afb9630747c41c69`  
		Last Modified: Tue, 01 Mar 2022 14:17:16 GMT  
		Size: 220.3 MB (220298373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2966b8e28ea8e47acbcca748753c937ef05bfde069cd7bfd2f70252b765fea99`  
		Last Modified: Tue, 01 Mar 2022 14:16:39 GMT  
		Size: 2.5 MB (2510056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9cf6997d2b0f369d91a2ce39d67ba3e78767956bd3cfdfc8d4287600b5389d`  
		Last Modified: Tue, 01 Mar 2022 14:16:38 GMT  
		Size: 447.3 KB (447285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a00db9ec98d74309ff4179c1227d6d2fef69862ff23de7e21984c3f67b479a0`  
		Last Modified: Mon, 07 Mar 2022 19:51:45 GMT  
		Size: 296.7 MB (296654000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493b4385630dec4e8162af9df1c6d4df55714493efc51596eb4a164c4eb63f49`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e655a91665cca257ae7d1746494a821d078d3d91e4ad4e20bcf1949dcb603d79`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d79ec5bcc003281f0154def0c30ec11a3b5baba4bbe5d1a53805e44c4d1d39`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a035624d232c158962c533e416ba594597e913d645f5a84a3f7e65f1ec01c76`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
