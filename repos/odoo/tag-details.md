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
$ docker pull odoo@sha256:c6c6093954ce36bc84fa044239db56ecc850cdd97de916ce0c6f92a7bca2fc4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:6d55c964231e238435432f52ecf2c3a6df9337b82e571efd546b449880f97fe8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.3 MB (540325179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb880a9394743bd242d123ef14775da1d195657bbce0e2eed5129c9d910b2164`
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
# Fri, 26 Aug 2022 19:27:27 GMT
ARG ODOO_RELEASE=20220826
# Fri, 26 Aug 2022 19:27:27 GMT
ARG ODOO_SHA=cf27da2394eaa4732b382482eb9733d09172a915
# Fri, 26 Aug 2022 19:28:40 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=cf27da2394eaa4732b382482eb9733d09172a915
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Aug 2022 19:28:44 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 26 Aug 2022 19:28:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Aug 2022 19:28:44 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=cf27da2394eaa4732b382482eb9733d09172a915
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Aug 2022 19:28:44 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Aug 2022 19:28:45 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Aug 2022 19:28:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Aug 2022 19:28:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Aug 2022 19:28:45 GMT
USER odoo
# Fri, 26 Aug 2022 19:28:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Aug 2022 19:28:45 GMT
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
	-	`sha256:579110ec86c28c137fc578141f01ae94cb6b44f215c9bea398b34379763eb6f1`  
		Last Modified: Fri, 26 Aug 2022 19:31:03 GMT  
		Size: 292.1 MB (292143448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5fb7485b4de117e031281a53a8ef96dec832b75fe3b60e0af2f3785373b415`  
		Last Modified: Fri, 26 Aug 2022 19:30:32 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a02c0b6ae935d07fda8f258dff997814c843b03ef2e277e31995b42cca4585a`  
		Last Modified: Fri, 26 Aug 2022 19:30:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acd806c075d872a8a9b858f479a09b771da3385877973b4048317c02fb0c012`  
		Last Modified: Fri, 26 Aug 2022 19:30:32 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dad058468a58e90280fe2ff468abbbcdb366832e13eb11e3e98f2ab061a1fab`  
		Last Modified: Fri, 26 Aug 2022 19:30:32 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:c6c6093954ce36bc84fa044239db56ecc850cdd97de916ce0c6f92a7bca2fc4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:6d55c964231e238435432f52ecf2c3a6df9337b82e571efd546b449880f97fe8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.3 MB (540325179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb880a9394743bd242d123ef14775da1d195657bbce0e2eed5129c9d910b2164`
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
# Fri, 26 Aug 2022 19:27:27 GMT
ARG ODOO_RELEASE=20220826
# Fri, 26 Aug 2022 19:27:27 GMT
ARG ODOO_SHA=cf27da2394eaa4732b382482eb9733d09172a915
# Fri, 26 Aug 2022 19:28:40 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=cf27da2394eaa4732b382482eb9733d09172a915
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Aug 2022 19:28:44 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 26 Aug 2022 19:28:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Aug 2022 19:28:44 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=cf27da2394eaa4732b382482eb9733d09172a915
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Aug 2022 19:28:44 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Aug 2022 19:28:45 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Aug 2022 19:28:45 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Aug 2022 19:28:45 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Aug 2022 19:28:45 GMT
USER odoo
# Fri, 26 Aug 2022 19:28:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Aug 2022 19:28:45 GMT
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
	-	`sha256:579110ec86c28c137fc578141f01ae94cb6b44f215c9bea398b34379763eb6f1`  
		Last Modified: Fri, 26 Aug 2022 19:31:03 GMT  
		Size: 292.1 MB (292143448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5fb7485b4de117e031281a53a8ef96dec832b75fe3b60e0af2f3785373b415`  
		Last Modified: Fri, 26 Aug 2022 19:30:32 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a02c0b6ae935d07fda8f258dff997814c843b03ef2e277e31995b42cca4585a`  
		Last Modified: Fri, 26 Aug 2022 19:30:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acd806c075d872a8a9b858f479a09b771da3385877973b4048317c02fb0c012`  
		Last Modified: Fri, 26 Aug 2022 19:30:32 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dad058468a58e90280fe2ff468abbbcdb366832e13eb11e3e98f2ab061a1fab`  
		Last Modified: Fri, 26 Aug 2022 19:30:32 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:8ef55cbb53aba957d817ed2ca285bae046cc9f9089f39b3d3952b407c74da91f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:bfaa3e371dcc72ea788aeb69d58a7118950d1d1f246ad000d58c90ce6a16a73f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.8 MB (530822499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:975dfd1b320cc7de7bf3cce743209927ce7149ed4f0ed31492591005be96d6d1`
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
# Fri, 26 Aug 2022 19:26:04 GMT
ARG ODOO_RELEASE=20220826
# Fri, 26 Aug 2022 19:26:04 GMT
ARG ODOO_SHA=fe6467ecb51a5b5bf831a2c1021e77b2a890a01d
# Fri, 26 Aug 2022 19:27:17 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=fe6467ecb51a5b5bf831a2c1021e77b2a890a01d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Aug 2022 19:27:21 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 26 Aug 2022 19:27:21 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Aug 2022 19:27:22 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=fe6467ecb51a5b5bf831a2c1021e77b2a890a01d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Aug 2022 19:27:22 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Aug 2022 19:27:22 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Aug 2022 19:27:22 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Aug 2022 19:27:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Aug 2022 19:27:22 GMT
USER odoo
# Fri, 26 Aug 2022 19:27:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Aug 2022 19:27:23 GMT
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
	-	`sha256:673608430b7979329fe3f494f75e0cbeb0b5ecd07ef30ae03a24ba920517f72a`  
		Last Modified: Fri, 26 Aug 2022 19:30:22 GMT  
		Size: 276.6 MB (276600426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb23ac1816abadc2d1f0fe92b4c15af23fbb291ee3769f0e412d8688213b6829`  
		Last Modified: Fri, 26 Aug 2022 19:29:49 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0110a9466722ead205ea19b4529918b9b3f9ed420594814ec7ba22d02e2b58d`  
		Last Modified: Fri, 26 Aug 2022 19:29:49 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96582cadafcfaed88d438e72eac6ee638de039cbd0c0d8b1e6398eb4fb736ac`  
		Last Modified: Fri, 26 Aug 2022 19:29:49 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502b65c1cb3ab7f68a55d530fbe503f7295940a2d2f0e4f0cd34b7668dd1a346`  
		Last Modified: Fri, 26 Aug 2022 19:29:49 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:8ef55cbb53aba957d817ed2ca285bae046cc9f9089f39b3d3952b407c74da91f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:bfaa3e371dcc72ea788aeb69d58a7118950d1d1f246ad000d58c90ce6a16a73f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.8 MB (530822499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:975dfd1b320cc7de7bf3cce743209927ce7149ed4f0ed31492591005be96d6d1`
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
# Fri, 26 Aug 2022 19:26:04 GMT
ARG ODOO_RELEASE=20220826
# Fri, 26 Aug 2022 19:26:04 GMT
ARG ODOO_SHA=fe6467ecb51a5b5bf831a2c1021e77b2a890a01d
# Fri, 26 Aug 2022 19:27:17 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=fe6467ecb51a5b5bf831a2c1021e77b2a890a01d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Aug 2022 19:27:21 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 26 Aug 2022 19:27:21 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Aug 2022 19:27:22 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=fe6467ecb51a5b5bf831a2c1021e77b2a890a01d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Aug 2022 19:27:22 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Aug 2022 19:27:22 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Aug 2022 19:27:22 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Aug 2022 19:27:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Aug 2022 19:27:22 GMT
USER odoo
# Fri, 26 Aug 2022 19:27:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Aug 2022 19:27:23 GMT
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
	-	`sha256:673608430b7979329fe3f494f75e0cbeb0b5ecd07ef30ae03a24ba920517f72a`  
		Last Modified: Fri, 26 Aug 2022 19:30:22 GMT  
		Size: 276.6 MB (276600426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb23ac1816abadc2d1f0fe92b4c15af23fbb291ee3769f0e412d8688213b6829`  
		Last Modified: Fri, 26 Aug 2022 19:29:49 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0110a9466722ead205ea19b4529918b9b3f9ed420594814ec7ba22d02e2b58d`  
		Last Modified: Fri, 26 Aug 2022 19:29:49 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96582cadafcfaed88d438e72eac6ee638de039cbd0c0d8b1e6398eb4fb736ac`  
		Last Modified: Fri, 26 Aug 2022 19:29:49 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502b65c1cb3ab7f68a55d530fbe503f7295940a2d2f0e4f0cd34b7668dd1a346`  
		Last Modified: Fri, 26 Aug 2022 19:29:49 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:1dddb0b820fc78692760052c7f5056fb6ec4a313e5e9d4ec0d957d39f34fdcac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:7be6ab8688e83d309d716bbb60090de40fd11e4e3b8fb4569cf637e09b6c717e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.8 MB (557786122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a844f3a4a8287e42a6eaf55443a978d45e580a8691230fe1b23eba50a5e9345`
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
# Fri, 26 Aug 2022 19:24:26 GMT
ARG ODOO_RELEASE=20220826
# Fri, 26 Aug 2022 19:24:26 GMT
ARG ODOO_SHA=e7155bae1d34b75cc34624e83b9b15992eab6b44
# Fri, 26 Aug 2022 19:25:44 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=e7155bae1d34b75cc34624e83b9b15992eab6b44
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Aug 2022 19:25:48 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 26 Aug 2022 19:25:48 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Aug 2022 19:25:49 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=e7155bae1d34b75cc34624e83b9b15992eab6b44
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Aug 2022 19:25:49 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Aug 2022 19:25:49 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Aug 2022 19:25:49 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Aug 2022 19:25:49 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Aug 2022 19:25:49 GMT
USER odoo
# Fri, 26 Aug 2022 19:25:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Aug 2022 19:25:49 GMT
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
	-	`sha256:529b16c7c79d6b3cf712751dc8a624969400094d4b26a7c5103d4d61a76f4ae1`  
		Last Modified: Fri, 26 Aug 2022 19:29:35 GMT  
		Size: 303.1 MB (303140887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ad11d807af551c7a7bfe6c85661bca2c7f7a26b714bd7e769922210fed54f`  
		Last Modified: Fri, 26 Aug 2022 19:29:00 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133473b86894ac02295db163c328b58978050021cd7f319b92e812f2340a7f2f`  
		Last Modified: Fri, 26 Aug 2022 19:29:00 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3276c5522698ea9125496f63da76c7b419de550206d5e2524b63f7deca8cdf2d`  
		Last Modified: Fri, 26 Aug 2022 19:29:01 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbcabca1fadd68e1de55b66b6ad27c6dd5f21a64c6477f4f2e8f34aef3b0e8b`  
		Last Modified: Fri, 26 Aug 2022 19:29:00 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:1dddb0b820fc78692760052c7f5056fb6ec4a313e5e9d4ec0d957d39f34fdcac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:7be6ab8688e83d309d716bbb60090de40fd11e4e3b8fb4569cf637e09b6c717e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.8 MB (557786122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a844f3a4a8287e42a6eaf55443a978d45e580a8691230fe1b23eba50a5e9345`
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
# Fri, 26 Aug 2022 19:24:26 GMT
ARG ODOO_RELEASE=20220826
# Fri, 26 Aug 2022 19:24:26 GMT
ARG ODOO_SHA=e7155bae1d34b75cc34624e83b9b15992eab6b44
# Fri, 26 Aug 2022 19:25:44 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=e7155bae1d34b75cc34624e83b9b15992eab6b44
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Aug 2022 19:25:48 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 26 Aug 2022 19:25:48 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Aug 2022 19:25:49 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=e7155bae1d34b75cc34624e83b9b15992eab6b44
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Aug 2022 19:25:49 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Aug 2022 19:25:49 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Aug 2022 19:25:49 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Aug 2022 19:25:49 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Aug 2022 19:25:49 GMT
USER odoo
# Fri, 26 Aug 2022 19:25:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Aug 2022 19:25:49 GMT
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
	-	`sha256:529b16c7c79d6b3cf712751dc8a624969400094d4b26a7c5103d4d61a76f4ae1`  
		Last Modified: Fri, 26 Aug 2022 19:29:35 GMT  
		Size: 303.1 MB (303140887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ad11d807af551c7a7bfe6c85661bca2c7f7a26b714bd7e769922210fed54f`  
		Last Modified: Fri, 26 Aug 2022 19:29:00 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133473b86894ac02295db163c328b58978050021cd7f319b92e812f2340a7f2f`  
		Last Modified: Fri, 26 Aug 2022 19:29:00 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3276c5522698ea9125496f63da76c7b419de550206d5e2524b63f7deca8cdf2d`  
		Last Modified: Fri, 26 Aug 2022 19:29:01 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbcabca1fadd68e1de55b66b6ad27c6dd5f21a64c6477f4f2e8f34aef3b0e8b`  
		Last Modified: Fri, 26 Aug 2022 19:29:00 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:1dddb0b820fc78692760052c7f5056fb6ec4a313e5e9d4ec0d957d39f34fdcac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:7be6ab8688e83d309d716bbb60090de40fd11e4e3b8fb4569cf637e09b6c717e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.8 MB (557786122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a844f3a4a8287e42a6eaf55443a978d45e580a8691230fe1b23eba50a5e9345`
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
# Fri, 26 Aug 2022 19:24:26 GMT
ARG ODOO_RELEASE=20220826
# Fri, 26 Aug 2022 19:24:26 GMT
ARG ODOO_SHA=e7155bae1d34b75cc34624e83b9b15992eab6b44
# Fri, 26 Aug 2022 19:25:44 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=e7155bae1d34b75cc34624e83b9b15992eab6b44
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Aug 2022 19:25:48 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 26 Aug 2022 19:25:48 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Aug 2022 19:25:49 GMT
# ARGS: ODOO_RELEASE=20220826 ODOO_SHA=e7155bae1d34b75cc34624e83b9b15992eab6b44
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Aug 2022 19:25:49 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Aug 2022 19:25:49 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Aug 2022 19:25:49 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Aug 2022 19:25:49 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Aug 2022 19:25:49 GMT
USER odoo
# Fri, 26 Aug 2022 19:25:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Aug 2022 19:25:49 GMT
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
	-	`sha256:529b16c7c79d6b3cf712751dc8a624969400094d4b26a7c5103d4d61a76f4ae1`  
		Last Modified: Fri, 26 Aug 2022 19:29:35 GMT  
		Size: 303.1 MB (303140887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0ad11d807af551c7a7bfe6c85661bca2c7f7a26b714bd7e769922210fed54f`  
		Last Modified: Fri, 26 Aug 2022 19:29:00 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133473b86894ac02295db163c328b58978050021cd7f319b92e812f2340a7f2f`  
		Last Modified: Fri, 26 Aug 2022 19:29:00 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3276c5522698ea9125496f63da76c7b419de550206d5e2524b63f7deca8cdf2d`  
		Last Modified: Fri, 26 Aug 2022 19:29:01 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbcabca1fadd68e1de55b66b6ad27c6dd5f21a64c6477f4f2e8f34aef3b0e8b`  
		Last Modified: Fri, 26 Aug 2022 19:29:00 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
