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
$ docker pull odoo@sha256:659b9b42c5975544bb860c5ba51308f289b2368354b57af7750934c9b2903267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:fec84a50464b308d0c4841056f03ccd6463c06290a22f46214f70075cc50aaf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.3 MB (540341959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be2f242c990ee0c331cb476428f03eb80675b24f4eb0e7d8d20864b054c61385`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:20:42 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 Aug 2022 04:20:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 Aug 2022 04:20:42 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 04:24:34 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 Aug 2022 04:24:43 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:24:46 GMT
RUN npm install -g rtlcss
# Tue, 23 Aug 2022 04:24:46 GMT
ENV ODOO_VERSION=13.0
# Fri, 02 Sep 2022 20:36:10 GMT
ARG ODOO_RELEASE=20220902
# Fri, 02 Sep 2022 20:36:10 GMT
ARG ODOO_SHA=d4da6396aed6e32579f525a45a22a5d4edfd3629
# Fri, 02 Sep 2022 20:37:23 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=d4da6396aed6e32579f525a45a22a5d4edfd3629
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Sep 2022 20:37:27 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 02 Sep 2022 20:37:27 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Sep 2022 20:37:28 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=d4da6396aed6e32579f525a45a22a5d4edfd3629
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Sep 2022 20:37:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Sep 2022 20:37:28 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Sep 2022 20:37:28 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Sep 2022 20:37:28 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Sep 2022 20:37:28 GMT
USER odoo
# Fri, 02 Sep 2022 20:37:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:37:28 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bc659c82c5df3ceed5b594b12d2276649ddada6c21fc27a2f70b40a9e475a9`  
		Last Modified: Tue, 23 Aug 2022 04:28:26 GMT  
		Size: 207.1 MB (207143904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf9beead154e3aab7df26112ce7e2825e3fad4784b1e5c98c8c19370334c1e1`  
		Last Modified: Tue, 23 Aug 2022 04:28:05 GMT  
		Size: 13.4 MB (13442806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f765d64561bd0be0eaa52035b4ec790b19e63dae6849f79cc86644fb84b6b`  
		Last Modified: Tue, 23 Aug 2022 04:28:02 GMT  
		Size: 454.2 KB (454230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adf1f2d0ef0cd4695b4cab8a54b7b7af63b7927ae42b1132c58f8f00f0354f1`  
		Last Modified: Fri, 02 Sep 2022 20:39:45 GMT  
		Size: 292.2 MB (292160225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d93bf4ee48b3290ea949d909fa8c87b52ac53249cb240da479c810a5e70b9`  
		Last Modified: Fri, 02 Sep 2022 20:39:14 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075db1aceabd7f42628c5fc3d955e8579d3060b0735ceb949a49f5da3a75ce73`  
		Last Modified: Fri, 02 Sep 2022 20:39:14 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffb64ed8e3152744d6a654eae72c79b8531139c3d7f190be7cdb4c1e2c0c6f1`  
		Last Modified: Fri, 02 Sep 2022 20:39:14 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9421f12879b54df7797d0a6b0551dd6a095af11a0d39898b04586bac1940ff8f`  
		Last Modified: Fri, 02 Sep 2022 20:39:14 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:659b9b42c5975544bb860c5ba51308f289b2368354b57af7750934c9b2903267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:fec84a50464b308d0c4841056f03ccd6463c06290a22f46214f70075cc50aaf5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.3 MB (540341959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be2f242c990ee0c331cb476428f03eb80675b24f4eb0e7d8d20864b054c61385`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:20:42 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 Aug 2022 04:20:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 Aug 2022 04:20:42 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 04:24:34 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 Aug 2022 04:24:43 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:24:46 GMT
RUN npm install -g rtlcss
# Tue, 23 Aug 2022 04:24:46 GMT
ENV ODOO_VERSION=13.0
# Fri, 02 Sep 2022 20:36:10 GMT
ARG ODOO_RELEASE=20220902
# Fri, 02 Sep 2022 20:36:10 GMT
ARG ODOO_SHA=d4da6396aed6e32579f525a45a22a5d4edfd3629
# Fri, 02 Sep 2022 20:37:23 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=d4da6396aed6e32579f525a45a22a5d4edfd3629
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Sep 2022 20:37:27 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 02 Sep 2022 20:37:27 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Sep 2022 20:37:28 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=d4da6396aed6e32579f525a45a22a5d4edfd3629
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Sep 2022 20:37:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Sep 2022 20:37:28 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Sep 2022 20:37:28 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Sep 2022 20:37:28 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Sep 2022 20:37:28 GMT
USER odoo
# Fri, 02 Sep 2022 20:37:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:37:28 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bc659c82c5df3ceed5b594b12d2276649ddada6c21fc27a2f70b40a9e475a9`  
		Last Modified: Tue, 23 Aug 2022 04:28:26 GMT  
		Size: 207.1 MB (207143904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf9beead154e3aab7df26112ce7e2825e3fad4784b1e5c98c8c19370334c1e1`  
		Last Modified: Tue, 23 Aug 2022 04:28:05 GMT  
		Size: 13.4 MB (13442806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f765d64561bd0be0eaa52035b4ec790b19e63dae6849f79cc86644fb84b6b`  
		Last Modified: Tue, 23 Aug 2022 04:28:02 GMT  
		Size: 454.2 KB (454230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adf1f2d0ef0cd4695b4cab8a54b7b7af63b7927ae42b1132c58f8f00f0354f1`  
		Last Modified: Fri, 02 Sep 2022 20:39:45 GMT  
		Size: 292.2 MB (292160225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159d93bf4ee48b3290ea949d909fa8c87b52ac53249cb240da479c810a5e70b9`  
		Last Modified: Fri, 02 Sep 2022 20:39:14 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075db1aceabd7f42628c5fc3d955e8579d3060b0735ceb949a49f5da3a75ce73`  
		Last Modified: Fri, 02 Sep 2022 20:39:14 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffb64ed8e3152744d6a654eae72c79b8531139c3d7f190be7cdb4c1e2c0c6f1`  
		Last Modified: Fri, 02 Sep 2022 20:39:14 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9421f12879b54df7797d0a6b0551dd6a095af11a0d39898b04586bac1940ff8f`  
		Last Modified: Fri, 02 Sep 2022 20:39:14 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:eb4e019156768203c5f435fe31e3502cdfc987e8b684fb6c6768a7f88703deae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:22bb883d654c3fd2478bccd5370757f21110ca25ea6bab5fce58dce4c28c1c9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.8 MB (530846752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b64df4e7279ce1bfd2203c611150b3bdccfb1c4102453294d95022eebe8137`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:20:42 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 Aug 2022 04:20:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 Aug 2022 04:20:42 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 04:21:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 Aug 2022 04:21:59 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:22:02 GMT
RUN npm install -g rtlcss
# Tue, 23 Aug 2022 04:22:02 GMT
ENV ODOO_VERSION=14.0
# Fri, 02 Sep 2022 20:34:47 GMT
ARG ODOO_RELEASE=20220902
# Fri, 02 Sep 2022 20:34:47 GMT
ARG ODOO_SHA=5dd3ba425de996c22c1f34383c8897f3c5930c0c
# Fri, 02 Sep 2022 20:36:00 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=5dd3ba425de996c22c1f34383c8897f3c5930c0c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Sep 2022 20:36:04 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 02 Sep 2022 20:36:04 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Sep 2022 20:36:05 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=5dd3ba425de996c22c1f34383c8897f3c5930c0c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Sep 2022 20:36:05 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Sep 2022 20:36:05 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Sep 2022 20:36:05 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Sep 2022 20:36:05 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Sep 2022 20:36:06 GMT
USER odoo
# Fri, 02 Sep 2022 20:36:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:36:06 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7a659d0e2ab4fe22a3e85e8063766519e98d39e86af6b71909b51058e7bb4d`  
		Last Modified: Tue, 23 Aug 2022 04:27:42 GMT  
		Size: 213.2 MB (213182299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13632be899adb63dd5166f35d4195b362d0c1be609d4dcabac13530b04d03fd1`  
		Last Modified: Tue, 23 Aug 2022 04:27:19 GMT  
		Size: 13.4 MB (13444767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed89ec81fb9348e6b4f6a91ae54dbad2d7fea55f2b1ee189efcbf42d3825a51a`  
		Last Modified: Tue, 23 Aug 2022 04:27:17 GMT  
		Size: 454.2 KB (454214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c7353738ce3513186bc3caf8662a1a4215614974dc9ca5b92fede28715eb98`  
		Last Modified: Fri, 02 Sep 2022 20:39:04 GMT  
		Size: 276.6 MB (276624678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c907eebf41b7508d3c9533a35c9da1bc20207059f4d8e8c605862d93d9b5a4df`  
		Last Modified: Fri, 02 Sep 2022 20:38:31 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99ab57007e272373d8e3925c4b7f8c1a2564a947788f511f8f6355ecca1c8c8`  
		Last Modified: Fri, 02 Sep 2022 20:38:31 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a8f8ec50f3223fae894542bf9540ade85a6f7f273323dfd20793c85a09ba5e`  
		Last Modified: Fri, 02 Sep 2022 20:38:32 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a995c1f0f1777d35e65a9b71cf089fe0820d78f46d06594fa452033ad061c3`  
		Last Modified: Fri, 02 Sep 2022 20:38:32 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:eb4e019156768203c5f435fe31e3502cdfc987e8b684fb6c6768a7f88703deae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:22bb883d654c3fd2478bccd5370757f21110ca25ea6bab5fce58dce4c28c1c9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.8 MB (530846752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b64df4e7279ce1bfd2203c611150b3bdccfb1c4102453294d95022eebe8137`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:20:42 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 Aug 2022 04:20:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 Aug 2022 04:20:42 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 04:21:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 Aug 2022 04:21:59 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:22:02 GMT
RUN npm install -g rtlcss
# Tue, 23 Aug 2022 04:22:02 GMT
ENV ODOO_VERSION=14.0
# Fri, 02 Sep 2022 20:34:47 GMT
ARG ODOO_RELEASE=20220902
# Fri, 02 Sep 2022 20:34:47 GMT
ARG ODOO_SHA=5dd3ba425de996c22c1f34383c8897f3c5930c0c
# Fri, 02 Sep 2022 20:36:00 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=5dd3ba425de996c22c1f34383c8897f3c5930c0c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Sep 2022 20:36:04 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 02 Sep 2022 20:36:04 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Sep 2022 20:36:05 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=5dd3ba425de996c22c1f34383c8897f3c5930c0c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Sep 2022 20:36:05 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Sep 2022 20:36:05 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Sep 2022 20:36:05 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Sep 2022 20:36:05 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Sep 2022 20:36:06 GMT
USER odoo
# Fri, 02 Sep 2022 20:36:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:36:06 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7a659d0e2ab4fe22a3e85e8063766519e98d39e86af6b71909b51058e7bb4d`  
		Last Modified: Tue, 23 Aug 2022 04:27:42 GMT  
		Size: 213.2 MB (213182299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13632be899adb63dd5166f35d4195b362d0c1be609d4dcabac13530b04d03fd1`  
		Last Modified: Tue, 23 Aug 2022 04:27:19 GMT  
		Size: 13.4 MB (13444767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed89ec81fb9348e6b4f6a91ae54dbad2d7fea55f2b1ee189efcbf42d3825a51a`  
		Last Modified: Tue, 23 Aug 2022 04:27:17 GMT  
		Size: 454.2 KB (454214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c7353738ce3513186bc3caf8662a1a4215614974dc9ca5b92fede28715eb98`  
		Last Modified: Fri, 02 Sep 2022 20:39:04 GMT  
		Size: 276.6 MB (276624678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c907eebf41b7508d3c9533a35c9da1bc20207059f4d8e8c605862d93d9b5a4df`  
		Last Modified: Fri, 02 Sep 2022 20:38:31 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99ab57007e272373d8e3925c4b7f8c1a2564a947788f511f8f6355ecca1c8c8`  
		Last Modified: Fri, 02 Sep 2022 20:38:31 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a8f8ec50f3223fae894542bf9540ade85a6f7f273323dfd20793c85a09ba5e`  
		Last Modified: Fri, 02 Sep 2022 20:38:32 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a995c1f0f1777d35e65a9b71cf089fe0820d78f46d06594fa452033ad061c3`  
		Last Modified: Fri, 02 Sep 2022 20:38:32 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:cbe6492fe757397bab65ec6ece72f0c794d38dafe943a96dcd331320320761b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:bdea66c1d2b4e1599b733733dd865586fb0333c03501c792192292b4b8a099e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.8 MB (557829847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2118e49c208a17684684db783216dedfcb485671c517ef90218c7eacaf4c474c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:18:04 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 Aug 2022 04:18:04 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 Aug 2022 04:18:04 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 04:19:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 Aug 2022 04:19:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:19:14 GMT
RUN npm install -g rtlcss
# Tue, 23 Aug 2022 04:19:15 GMT
ENV ODOO_VERSION=15.0
# Fri, 02 Sep 2022 20:33:08 GMT
ARG ODOO_RELEASE=20220902
# Fri, 02 Sep 2022 20:33:09 GMT
ARG ODOO_SHA=f08078727fff11b2e0778627c476e7b95cbebdea
# Fri, 02 Sep 2022 20:34:26 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=f08078727fff11b2e0778627c476e7b95cbebdea
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Sep 2022 20:34:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 02 Sep 2022 20:34:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Sep 2022 20:34:31 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=f08078727fff11b2e0778627c476e7b95cbebdea
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Sep 2022 20:34:31 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Sep 2022 20:34:32 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Sep 2022 20:34:32 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Sep 2022 20:34:32 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Sep 2022 20:34:32 GMT
USER odoo
# Fri, 02 Sep 2022 20:34:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:34:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb8f3073d7aa12b590bbcfb6b670ff30bdce9db379f2ebccdd4349cd3d1b17`  
		Last Modified: Tue, 23 Aug 2022 04:26:53 GMT  
		Size: 220.3 MB (220296783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b432e5a5fa86f6c173d9d8614889a638ff0891c38a9c08f7fa5cdf9e9a63b044`  
		Last Modified: Tue, 23 Aug 2022 04:26:27 GMT  
		Size: 2.5 MB (2514624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdd6ff1405cad92ef01a751c4193873ed8078e06ba52d718c300386c2189830`  
		Last Modified: Tue, 23 Aug 2022 04:26:27 GMT  
		Size: 449.9 KB (449883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c439bce7a6ec33dd8e1153f7e7a0e2c931eaced8acba7f5db513083b03efe031`  
		Last Modified: Fri, 02 Sep 2022 20:38:19 GMT  
		Size: 303.2 MB (303184614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda1cadc2434672447709ab0f2375d26ea44a34a5abc0fb576d9a7800ae7d7cc`  
		Last Modified: Fri, 02 Sep 2022 20:37:43 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff67f4127ee62a6fad3766cca28569a2b06680f36d15d192f04314e1e70c0faf`  
		Last Modified: Fri, 02 Sep 2022 20:37:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e15e1366f5cc3efc4b38fd2ff464a5551df9775619841aeb5d56f39384f985e`  
		Last Modified: Fri, 02 Sep 2022 20:37:44 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5fa1a4ba7d32891c644f1f402f1b33aefecb74cf7683d9773cada86a123d67`  
		Last Modified: Fri, 02 Sep 2022 20:37:43 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:cbe6492fe757397bab65ec6ece72f0c794d38dafe943a96dcd331320320761b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:bdea66c1d2b4e1599b733733dd865586fb0333c03501c792192292b4b8a099e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.8 MB (557829847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2118e49c208a17684684db783216dedfcb485671c517ef90218c7eacaf4c474c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:18:04 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 Aug 2022 04:18:04 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 Aug 2022 04:18:04 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 04:19:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 Aug 2022 04:19:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:19:14 GMT
RUN npm install -g rtlcss
# Tue, 23 Aug 2022 04:19:15 GMT
ENV ODOO_VERSION=15.0
# Fri, 02 Sep 2022 20:33:08 GMT
ARG ODOO_RELEASE=20220902
# Fri, 02 Sep 2022 20:33:09 GMT
ARG ODOO_SHA=f08078727fff11b2e0778627c476e7b95cbebdea
# Fri, 02 Sep 2022 20:34:26 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=f08078727fff11b2e0778627c476e7b95cbebdea
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Sep 2022 20:34:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 02 Sep 2022 20:34:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Sep 2022 20:34:31 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=f08078727fff11b2e0778627c476e7b95cbebdea
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Sep 2022 20:34:31 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Sep 2022 20:34:32 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Sep 2022 20:34:32 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Sep 2022 20:34:32 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Sep 2022 20:34:32 GMT
USER odoo
# Fri, 02 Sep 2022 20:34:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:34:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb8f3073d7aa12b590bbcfb6b670ff30bdce9db379f2ebccdd4349cd3d1b17`  
		Last Modified: Tue, 23 Aug 2022 04:26:53 GMT  
		Size: 220.3 MB (220296783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b432e5a5fa86f6c173d9d8614889a638ff0891c38a9c08f7fa5cdf9e9a63b044`  
		Last Modified: Tue, 23 Aug 2022 04:26:27 GMT  
		Size: 2.5 MB (2514624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdd6ff1405cad92ef01a751c4193873ed8078e06ba52d718c300386c2189830`  
		Last Modified: Tue, 23 Aug 2022 04:26:27 GMT  
		Size: 449.9 KB (449883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c439bce7a6ec33dd8e1153f7e7a0e2c931eaced8acba7f5db513083b03efe031`  
		Last Modified: Fri, 02 Sep 2022 20:38:19 GMT  
		Size: 303.2 MB (303184614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda1cadc2434672447709ab0f2375d26ea44a34a5abc0fb576d9a7800ae7d7cc`  
		Last Modified: Fri, 02 Sep 2022 20:37:43 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff67f4127ee62a6fad3766cca28569a2b06680f36d15d192f04314e1e70c0faf`  
		Last Modified: Fri, 02 Sep 2022 20:37:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e15e1366f5cc3efc4b38fd2ff464a5551df9775619841aeb5d56f39384f985e`  
		Last Modified: Fri, 02 Sep 2022 20:37:44 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5fa1a4ba7d32891c644f1f402f1b33aefecb74cf7683d9773cada86a123d67`  
		Last Modified: Fri, 02 Sep 2022 20:37:43 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:cbe6492fe757397bab65ec6ece72f0c794d38dafe943a96dcd331320320761b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:bdea66c1d2b4e1599b733733dd865586fb0333c03501c792192292b4b8a099e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.8 MB (557829847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2118e49c208a17684684db783216dedfcb485671c517ef90218c7eacaf4c474c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:18:04 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 23 Aug 2022 04:18:04 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 23 Aug 2022 04:18:04 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 04:19:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 23 Aug 2022 04:19:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 04:19:14 GMT
RUN npm install -g rtlcss
# Tue, 23 Aug 2022 04:19:15 GMT
ENV ODOO_VERSION=15.0
# Fri, 02 Sep 2022 20:33:08 GMT
ARG ODOO_RELEASE=20220902
# Fri, 02 Sep 2022 20:33:09 GMT
ARG ODOO_SHA=f08078727fff11b2e0778627c476e7b95cbebdea
# Fri, 02 Sep 2022 20:34:26 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=f08078727fff11b2e0778627c476e7b95cbebdea
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 02 Sep 2022 20:34:31 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 02 Sep 2022 20:34:31 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 02 Sep 2022 20:34:31 GMT
# ARGS: ODOO_RELEASE=20220902 ODOO_SHA=f08078727fff11b2e0778627c476e7b95cbebdea
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 02 Sep 2022 20:34:31 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 02 Sep 2022 20:34:32 GMT
EXPOSE 8069 8071 8072
# Fri, 02 Sep 2022 20:34:32 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 02 Sep 2022 20:34:32 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 02 Sep 2022 20:34:32 GMT
USER odoo
# Fri, 02 Sep 2022 20:34:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 02 Sep 2022 20:34:32 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bb8f3073d7aa12b590bbcfb6b670ff30bdce9db379f2ebccdd4349cd3d1b17`  
		Last Modified: Tue, 23 Aug 2022 04:26:53 GMT  
		Size: 220.3 MB (220296783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b432e5a5fa86f6c173d9d8614889a638ff0891c38a9c08f7fa5cdf9e9a63b044`  
		Last Modified: Tue, 23 Aug 2022 04:26:27 GMT  
		Size: 2.5 MB (2514624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdd6ff1405cad92ef01a751c4193873ed8078e06ba52d718c300386c2189830`  
		Last Modified: Tue, 23 Aug 2022 04:26:27 GMT  
		Size: 449.9 KB (449883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c439bce7a6ec33dd8e1153f7e7a0e2c931eaced8acba7f5db513083b03efe031`  
		Last Modified: Fri, 02 Sep 2022 20:38:19 GMT  
		Size: 303.2 MB (303184614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda1cadc2434672447709ab0f2375d26ea44a34a5abc0fb576d9a7800ae7d7cc`  
		Last Modified: Fri, 02 Sep 2022 20:37:43 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff67f4127ee62a6fad3766cca28569a2b06680f36d15d192f04314e1e70c0faf`  
		Last Modified: Fri, 02 Sep 2022 20:37:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e15e1366f5cc3efc4b38fd2ff464a5551df9775619841aeb5d56f39384f985e`  
		Last Modified: Fri, 02 Sep 2022 20:37:44 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5fa1a4ba7d32891c644f1f402f1b33aefecb74cf7683d9773cada86a123d67`  
		Last Modified: Fri, 02 Sep 2022 20:37:43 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
