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
$ docker pull odoo@sha256:b5f2b7391c4d5b6130bef56779aa315b9561017f5e6aa410649b4ae99bd9775c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:86067b097c9d6a6ae185939c8c0f6ba1d4a222d47e013c3d614b3fbcc3118358
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.6 MB (539563181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:028146da6806c525a4f7fe3b65ce91517389a05e03599380af107e2e97976afe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:04:36 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:04:36 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:04:37 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:09:43 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:09:56 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:10:00 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:10:00 GMT
ENV ODOO_VERSION=13.0
# Tue, 12 Oct 2021 12:10:00 GMT
ARG ODOO_RELEASE=20211007
# Tue, 12 Oct 2021 12:10:00 GMT
ARG ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
# Tue, 12 Oct 2021 12:12:38 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 12 Oct 2021 12:12:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 12 Oct 2021 12:12:42 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 12 Oct 2021 12:12:43 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 12 Oct 2021 12:12:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 12 Oct 2021 12:12:44 GMT
EXPOSE 8069 8071 8072
# Tue, 12 Oct 2021 12:12:44 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 12 Oct 2021 12:12:44 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 12 Oct 2021 12:12:44 GMT
USER odoo
# Tue, 12 Oct 2021 12:12:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 12:12:45 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45015eb54192c2e0c507396977810d7fddab577041c6c02a5758bcbf4d855326`  
		Last Modified: Tue, 12 Oct 2021 12:15:15 GMT  
		Size: 207.1 MB (207130926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8865fe285493c649f819eb839e1553c90a3bb6ef50521345f499df0337d093`  
		Last Modified: Tue, 12 Oct 2021 12:14:51 GMT  
		Size: 13.4 MB (13433045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788061f0dbd60660f54795fdbec83e425330c41bd36f2514ddf332ca7304796e`  
		Last Modified: Tue, 12 Oct 2021 12:14:47 GMT  
		Size: 864.8 KB (864751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98206d1f603f7c1e6228217bb4258ed3434cdf5fe3c27cd4213236a82a9545c8`  
		Last Modified: Tue, 12 Oct 2021 12:15:23 GMT  
		Size: 291.0 MB (290992483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9473fd62cbf129d38324209cf251b76537222384ab77e9435ddec120e829b4f`  
		Last Modified: Tue, 12 Oct 2021 12:14:44 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb905b54884173c8b587861f3b143a999407653af91e956a702f73a7ff9daf3`  
		Last Modified: Tue, 12 Oct 2021 12:14:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf88a9dcc63d8f26459ae6a89daa151a57d09c82f18bc10a974ed69dceb5fa2b`  
		Last Modified: Tue, 12 Oct 2021 12:14:44 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f38b1d63e582efa8480128d8dcf519cf55b72fb81d67238b5ddde028798461`  
		Last Modified: Tue, 12 Oct 2021 12:14:44 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:b5f2b7391c4d5b6130bef56779aa315b9561017f5e6aa410649b4ae99bd9775c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:86067b097c9d6a6ae185939c8c0f6ba1d4a222d47e013c3d614b3fbcc3118358
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.6 MB (539563181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:028146da6806c525a4f7fe3b65ce91517389a05e03599380af107e2e97976afe`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:04:36 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:04:36 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:04:37 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:09:43 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:09:56 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:10:00 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:10:00 GMT
ENV ODOO_VERSION=13.0
# Tue, 12 Oct 2021 12:10:00 GMT
ARG ODOO_RELEASE=20211007
# Tue, 12 Oct 2021 12:10:00 GMT
ARG ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
# Tue, 12 Oct 2021 12:12:38 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 12 Oct 2021 12:12:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 12 Oct 2021 12:12:42 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 12 Oct 2021 12:12:43 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=5761202ca3dea1f89ad2e67a0f4111c5291f20e3
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 12 Oct 2021 12:12:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 12 Oct 2021 12:12:44 GMT
EXPOSE 8069 8071 8072
# Tue, 12 Oct 2021 12:12:44 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 12 Oct 2021 12:12:44 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 12 Oct 2021 12:12:44 GMT
USER odoo
# Tue, 12 Oct 2021 12:12:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 12:12:45 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45015eb54192c2e0c507396977810d7fddab577041c6c02a5758bcbf4d855326`  
		Last Modified: Tue, 12 Oct 2021 12:15:15 GMT  
		Size: 207.1 MB (207130926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8865fe285493c649f819eb839e1553c90a3bb6ef50521345f499df0337d093`  
		Last Modified: Tue, 12 Oct 2021 12:14:51 GMT  
		Size: 13.4 MB (13433045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788061f0dbd60660f54795fdbec83e425330c41bd36f2514ddf332ca7304796e`  
		Last Modified: Tue, 12 Oct 2021 12:14:47 GMT  
		Size: 864.8 KB (864751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98206d1f603f7c1e6228217bb4258ed3434cdf5fe3c27cd4213236a82a9545c8`  
		Last Modified: Tue, 12 Oct 2021 12:15:23 GMT  
		Size: 291.0 MB (290992483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9473fd62cbf129d38324209cf251b76537222384ab77e9435ddec120e829b4f`  
		Last Modified: Tue, 12 Oct 2021 12:14:44 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb905b54884173c8b587861f3b143a999407653af91e956a702f73a7ff9daf3`  
		Last Modified: Tue, 12 Oct 2021 12:14:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf88a9dcc63d8f26459ae6a89daa151a57d09c82f18bc10a974ed69dceb5fa2b`  
		Last Modified: Tue, 12 Oct 2021 12:14:44 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f38b1d63e582efa8480128d8dcf519cf55b72fb81d67238b5ddde028798461`  
		Last Modified: Tue, 12 Oct 2021 12:14:44 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:61c36f10a03757388bfc84046caabacc551b0de6b7abf7b04c72ab5c40b3b2e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:691cf5f657479f792061cb2b697bfb1cef1e3e707644bcf5dfd608b453d05638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.1 MB (528139657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d0d72d770c26849ca799c669ad98582a6f0e8f9381550a155fae68a86fa198c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:04:36 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:04:36 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:04:37 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:05:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:06:18 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:06:25 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:06:25 GMT
ENV ODOO_VERSION=14.0
# Tue, 12 Oct 2021 12:06:25 GMT
ARG ODOO_RELEASE=20211007
# Tue, 12 Oct 2021 12:06:26 GMT
ARG ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
# Tue, 12 Oct 2021 12:08:23 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 12 Oct 2021 12:08:27 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 12 Oct 2021 12:08:27 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 12 Oct 2021 12:08:28 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 12 Oct 2021 12:08:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 12 Oct 2021 12:08:28 GMT
EXPOSE 8069 8071 8072
# Tue, 12 Oct 2021 12:08:29 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 12 Oct 2021 12:08:29 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 12 Oct 2021 12:08:29 GMT
USER odoo
# Tue, 12 Oct 2021 12:08:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 12:08:29 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a690652210adb99f7736fa4e78f5c15ebd7443f1779c0f4df93f3ede9b7242f4`  
		Last Modified: Tue, 12 Oct 2021 12:14:26 GMT  
		Size: 213.2 MB (213173260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f39d77a6b54dadd4be888e4329319568a8c6910b227f9968b18b3f32b7e5b8c`  
		Last Modified: Tue, 12 Oct 2021 12:14:00 GMT  
		Size: 13.4 MB (13435702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a022bb6719132cde437ae6e8500998624cebc5c7cfc5a5c69157cb1eeb54eb1`  
		Last Modified: Tue, 12 Oct 2021 12:13:56 GMT  
		Size: 864.7 KB (864743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d18df483e9cde65541667ed57b7cb8e5310e0f09285e41cc4f0a54491fdc82`  
		Last Modified: Tue, 12 Oct 2021 12:14:34 GMT  
		Size: 273.5 MB (273523977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14fadd6357054f83e67319c5835f958f5956456362c56d380a5b98d896369c1`  
		Last Modified: Tue, 12 Oct 2021 12:13:54 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a422c7ed0251616edb589f5b554b24df9ec4972c0e1ea5bd603762afb4cba07f`  
		Last Modified: Tue, 12 Oct 2021 12:13:54 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1337036f9f1a076346bb76db8584df7bafb0addf6c592054e422cc5b1fba08a`  
		Last Modified: Tue, 12 Oct 2021 12:13:54 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3449d0ce9accbd40fd7533bc7269366472b5e4b8a14193e4c4470aa00ba895`  
		Last Modified: Tue, 12 Oct 2021 12:13:54 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:61c36f10a03757388bfc84046caabacc551b0de6b7abf7b04c72ab5c40b3b2e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:691cf5f657479f792061cb2b697bfb1cef1e3e707644bcf5dfd608b453d05638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.1 MB (528139657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d0d72d770c26849ca799c669ad98582a6f0e8f9381550a155fae68a86fa198c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:04:36 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:04:36 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:04:37 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:05:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:06:18 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:06:25 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:06:25 GMT
ENV ODOO_VERSION=14.0
# Tue, 12 Oct 2021 12:06:25 GMT
ARG ODOO_RELEASE=20211007
# Tue, 12 Oct 2021 12:06:26 GMT
ARG ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
# Tue, 12 Oct 2021 12:08:23 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 12 Oct 2021 12:08:27 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 12 Oct 2021 12:08:27 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 12 Oct 2021 12:08:28 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=183bc4f2d640b53d5e2fb8fc06a1915a432c9ac7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 12 Oct 2021 12:08:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 12 Oct 2021 12:08:28 GMT
EXPOSE 8069 8071 8072
# Tue, 12 Oct 2021 12:08:29 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 12 Oct 2021 12:08:29 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 12 Oct 2021 12:08:29 GMT
USER odoo
# Tue, 12 Oct 2021 12:08:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 12:08:29 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a690652210adb99f7736fa4e78f5c15ebd7443f1779c0f4df93f3ede9b7242f4`  
		Last Modified: Tue, 12 Oct 2021 12:14:26 GMT  
		Size: 213.2 MB (213173260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f39d77a6b54dadd4be888e4329319568a8c6910b227f9968b18b3f32b7e5b8c`  
		Last Modified: Tue, 12 Oct 2021 12:14:00 GMT  
		Size: 13.4 MB (13435702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a022bb6719132cde437ae6e8500998624cebc5c7cfc5a5c69157cb1eeb54eb1`  
		Last Modified: Tue, 12 Oct 2021 12:13:56 GMT  
		Size: 864.7 KB (864743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d18df483e9cde65541667ed57b7cb8e5310e0f09285e41cc4f0a54491fdc82`  
		Last Modified: Tue, 12 Oct 2021 12:14:34 GMT  
		Size: 273.5 MB (273523977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14fadd6357054f83e67319c5835f958f5956456362c56d380a5b98d896369c1`  
		Last Modified: Tue, 12 Oct 2021 12:13:54 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a422c7ed0251616edb589f5b554b24df9ec4972c0e1ea5bd603762afb4cba07f`  
		Last Modified: Tue, 12 Oct 2021 12:13:54 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1337036f9f1a076346bb76db8584df7bafb0addf6c592054e422cc5b1fba08a`  
		Last Modified: Tue, 12 Oct 2021 12:13:54 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3449d0ce9accbd40fd7533bc7269366472b5e4b8a14193e4c4470aa00ba895`  
		Last Modified: Tue, 12 Oct 2021 12:13:54 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:0213aee3dfe28cd256de75aff0158eb5e32b61dba734d4e9b2f33d74e49b4346
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:5bb85850eb0153dcc94c8ae3a9b8e0188a2d43d5d754aa74a32cc4e56c618263
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539738896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c10d473b9d29aadc474e0e868b2afc7ad001a9493e47d4a914b49d2b59aefb24`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:01:12 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:01:12 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:01:12 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:02:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         gsfonts         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-openssl         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:02:30 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:02:33 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:02:33 GMT
ENV ODOO_VERSION=15.0
# Tue, 12 Oct 2021 12:02:33 GMT
ARG ODOO_RELEASE=20211007
# Tue, 12 Oct 2021 12:02:33 GMT
ARG ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
# Tue, 12 Oct 2021 12:04:23 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 12 Oct 2021 12:04:27 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 12 Oct 2021 12:04:27 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 12 Oct 2021 12:04:28 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 12 Oct 2021 12:04:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 12 Oct 2021 12:04:28 GMT
EXPOSE 8069 8071 8072
# Tue, 12 Oct 2021 12:04:29 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 12 Oct 2021 12:04:29 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 12 Oct 2021 12:04:30 GMT
USER odoo
# Tue, 12 Oct 2021 12:04:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 12:04:30 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38726de5ed2ec7e468afd026f502bdc97f591e43c0bc8e09ba8b0657c238ac0a`  
		Last Modified: Tue, 12 Oct 2021 12:13:37 GMT  
		Size: 223.8 MB (223816542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f220056c49310bef49e54a44fb6626222df0b73def08a56e1e145c3414d3f1f`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 2.5 MB (2506151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3854229348d451d83ddbf604aba25bf82021f5d0b001918068b73a3d4f6103ad`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 853.4 KB (853380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea2bfdca89e700f653480da6333235a6971ec8e4b88b1225ea7883eb53f751c`  
		Last Modified: Tue, 12 Oct 2021 12:13:41 GMT  
		Size: 281.2 MB (281203050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f054aa5cd4d43921b6e69ec2af6e5f597f7c4e95664aafa7a706d11e48e33`  
		Last Modified: Tue, 12 Oct 2021 12:13:03 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfd2a463ca346249d7315cc74986f9219e6cbc3972fe820a2a23f1991cadb13`  
		Last Modified: Tue, 12 Oct 2021 12:13:04 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad8e3215bb7862cdfe8d91ab9393148ded6877222625d5550b545f02110137b`  
		Last Modified: Tue, 12 Oct 2021 12:13:03 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c4afdf4017e08010365bc34d323657826a7cf6538d86f0425eb12475c34a9e`  
		Last Modified: Tue, 12 Oct 2021 12:13:03 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:0213aee3dfe28cd256de75aff0158eb5e32b61dba734d4e9b2f33d74e49b4346
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:5bb85850eb0153dcc94c8ae3a9b8e0188a2d43d5d754aa74a32cc4e56c618263
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539738896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c10d473b9d29aadc474e0e868b2afc7ad001a9493e47d4a914b49d2b59aefb24`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:01:12 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:01:12 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:01:12 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:02:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         gsfonts         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-openssl         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:02:30 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:02:33 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:02:33 GMT
ENV ODOO_VERSION=15.0
# Tue, 12 Oct 2021 12:02:33 GMT
ARG ODOO_RELEASE=20211007
# Tue, 12 Oct 2021 12:02:33 GMT
ARG ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
# Tue, 12 Oct 2021 12:04:23 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 12 Oct 2021 12:04:27 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 12 Oct 2021 12:04:27 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 12 Oct 2021 12:04:28 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 12 Oct 2021 12:04:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 12 Oct 2021 12:04:28 GMT
EXPOSE 8069 8071 8072
# Tue, 12 Oct 2021 12:04:29 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 12 Oct 2021 12:04:29 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 12 Oct 2021 12:04:30 GMT
USER odoo
# Tue, 12 Oct 2021 12:04:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 12:04:30 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38726de5ed2ec7e468afd026f502bdc97f591e43c0bc8e09ba8b0657c238ac0a`  
		Last Modified: Tue, 12 Oct 2021 12:13:37 GMT  
		Size: 223.8 MB (223816542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f220056c49310bef49e54a44fb6626222df0b73def08a56e1e145c3414d3f1f`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 2.5 MB (2506151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3854229348d451d83ddbf604aba25bf82021f5d0b001918068b73a3d4f6103ad`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 853.4 KB (853380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea2bfdca89e700f653480da6333235a6971ec8e4b88b1225ea7883eb53f751c`  
		Last Modified: Tue, 12 Oct 2021 12:13:41 GMT  
		Size: 281.2 MB (281203050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f054aa5cd4d43921b6e69ec2af6e5f597f7c4e95664aafa7a706d11e48e33`  
		Last Modified: Tue, 12 Oct 2021 12:13:03 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfd2a463ca346249d7315cc74986f9219e6cbc3972fe820a2a23f1991cadb13`  
		Last Modified: Tue, 12 Oct 2021 12:13:04 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad8e3215bb7862cdfe8d91ab9393148ded6877222625d5550b545f02110137b`  
		Last Modified: Tue, 12 Oct 2021 12:13:03 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c4afdf4017e08010365bc34d323657826a7cf6538d86f0425eb12475c34a9e`  
		Last Modified: Tue, 12 Oct 2021 12:13:03 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:0213aee3dfe28cd256de75aff0158eb5e32b61dba734d4e9b2f33d74e49b4346
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:5bb85850eb0153dcc94c8ae3a9b8e0188a2d43d5d754aa74a32cc4e56c618263
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539738896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c10d473b9d29aadc474e0e868b2afc7ad001a9493e47d4a914b49d2b59aefb24`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:01:12 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 12 Oct 2021 12:01:12 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 12 Oct 2021 12:01:12 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 12:02:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         gsfonts         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-openssl         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 12 Oct 2021 12:02:30 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:02:33 GMT
RUN npm install -g rtlcss
# Tue, 12 Oct 2021 12:02:33 GMT
ENV ODOO_VERSION=15.0
# Tue, 12 Oct 2021 12:02:33 GMT
ARG ODOO_RELEASE=20211007
# Tue, 12 Oct 2021 12:02:33 GMT
ARG ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
# Tue, 12 Oct 2021 12:04:23 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 12 Oct 2021 12:04:27 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 12 Oct 2021 12:04:27 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 12 Oct 2021 12:04:28 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 12 Oct 2021 12:04:28 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 12 Oct 2021 12:04:28 GMT
EXPOSE 8069 8071 8072
# Tue, 12 Oct 2021 12:04:29 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 12 Oct 2021 12:04:29 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 12 Oct 2021 12:04:30 GMT
USER odoo
# Tue, 12 Oct 2021 12:04:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 12 Oct 2021 12:04:30 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38726de5ed2ec7e468afd026f502bdc97f591e43c0bc8e09ba8b0657c238ac0a`  
		Last Modified: Tue, 12 Oct 2021 12:13:37 GMT  
		Size: 223.8 MB (223816542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f220056c49310bef49e54a44fb6626222df0b73def08a56e1e145c3414d3f1f`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 2.5 MB (2506151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3854229348d451d83ddbf604aba25bf82021f5d0b001918068b73a3d4f6103ad`  
		Last Modified: Tue, 12 Oct 2021 12:13:06 GMT  
		Size: 853.4 KB (853380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea2bfdca89e700f653480da6333235a6971ec8e4b88b1225ea7883eb53f751c`  
		Last Modified: Tue, 12 Oct 2021 12:13:41 GMT  
		Size: 281.2 MB (281203050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f054aa5cd4d43921b6e69ec2af6e5f597f7c4e95664aafa7a706d11e48e33`  
		Last Modified: Tue, 12 Oct 2021 12:13:03 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfd2a463ca346249d7315cc74986f9219e6cbc3972fe820a2a23f1991cadb13`  
		Last Modified: Tue, 12 Oct 2021 12:13:04 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad8e3215bb7862cdfe8d91ab9393148ded6877222625d5550b545f02110137b`  
		Last Modified: Tue, 12 Oct 2021 12:13:03 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c4afdf4017e08010365bc34d323657826a7cf6538d86f0425eb12475c34a9e`  
		Last Modified: Tue, 12 Oct 2021 12:13:03 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
