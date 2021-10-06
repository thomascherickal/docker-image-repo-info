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
$ docker pull odoo@sha256:0bf34470208c49c4292adec3230f9a2d2ff94ff3362a2a0f5d69d3612190c6da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:6521005019c9f11e83f1c5419aab961f7e6a4f9757347df2ff0e103024e96b73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538443157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924cffb9717b73f420a5946149606fe114d6938126de0f5e7aa1e696a20f20cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:30 GMT
ADD file:c7a3b8a1e87bedfb6605855ad703321050112d02c9925ece42f4111d7a42cdd0 in / 
# Tue, 28 Sep 2021 01:25:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:04:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 28 Sep 2021 09:04:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 28 Sep 2021 09:04:53 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:04:54 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 28 Sep 2021 09:07:07 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 28 Sep 2021 09:07:29 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:07:46 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:07:46 GMT
ENV ODOO_VERSION=12.0
# Wed, 06 Oct 2021 18:24:28 GMT
ARG ODOO_RELEASE=20211006
# Wed, 06 Oct 2021 18:24:29 GMT
ARG ODOO_SHA=f32dcd82b04e9a93e17a7d4b3ab471dc20408253
# Wed, 06 Oct 2021 18:25:36 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=f32dcd82b04e9a93e17a7d4b3ab471dc20408253
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 06 Oct 2021 18:25:39 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 06 Oct 2021 18:25:40 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 06 Oct 2021 18:25:40 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=f32dcd82b04e9a93e17a7d4b3ab471dc20408253
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 06 Oct 2021 18:25:41 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 06 Oct 2021 18:25:41 GMT
EXPOSE 8069 8071 8072
# Wed, 06 Oct 2021 18:25:41 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 06 Oct 2021 18:25:41 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 06 Oct 2021 18:25:41 GMT
USER odoo
# Wed, 06 Oct 2021 18:25:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Oct 2021 18:25:42 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:36d925ed8e305498a951c3b56d100d153ae3babf046b88e2d00899105fe81c31`  
		Last Modified: Tue, 28 Sep 2021 01:32:51 GMT  
		Size: 22.5 MB (22527699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5788ecc3532a07db45efea6a2c973faee8385402c0498b6cd805140e3ff3aa`  
		Last Modified: Tue, 28 Sep 2021 09:11:45 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d29df4b5fe46f143c4fcdd612f91cb00e025018292c0e2ea4f4aa8fb40b628c`  
		Last Modified: Tue, 28 Sep 2021 09:12:29 GMT  
		Size: 219.7 MB (219657423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa757125f4784d18e2db094bd9c15892e1e3a68f8405c3cfd6e44f57dfd10b5`  
		Last Modified: Tue, 28 Sep 2021 09:11:46 GMT  
		Size: 2.2 MB (2227263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999e75deb22b82657afe043a6b3b90c7531f3f68e0b794caa5a715a2656cc863`  
		Last Modified: Tue, 28 Sep 2021 09:11:54 GMT  
		Size: 22.0 MB (22019278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66d27d56f6793d5a1afe5f66f7c3af6786b87945b847e2b3db1e0401435a74e`  
		Last Modified: Wed, 06 Oct 2021 18:27:58 GMT  
		Size: 272.0 MB (272008802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245b8e1b96a304af8bf8cf3ae168a143796c4c97c3e611febbeda59ff66f66d3`  
		Last Modified: Wed, 06 Oct 2021 18:27:31 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542be52c4dfe61d73fb7d6484cf99ca1d03547b6e2fe332278e816b71ca23e67`  
		Last Modified: Wed, 06 Oct 2021 18:27:31 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386c0455b25b5ad3ae285e0cc43346bf653b33b098642e5686cfb2cbacff7564`  
		Last Modified: Wed, 06 Oct 2021 18:27:31 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc917cc806609fefcee591b902f6a83ed09d887a3866d3c8103b9c6e848e386d`  
		Last Modified: Wed, 06 Oct 2021 18:27:31 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:0bf34470208c49c4292adec3230f9a2d2ff94ff3362a2a0f5d69d3612190c6da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:6521005019c9f11e83f1c5419aab961f7e6a4f9757347df2ff0e103024e96b73
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **538.4 MB (538443157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924cffb9717b73f420a5946149606fe114d6938126de0f5e7aa1e696a20f20cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:30 GMT
ADD file:c7a3b8a1e87bedfb6605855ad703321050112d02c9925ece42f4111d7a42cdd0 in / 
# Tue, 28 Sep 2021 01:25:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 09:04:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 28 Sep 2021 09:04:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 28 Sep 2021 09:04:53 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:04:54 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 28 Sep 2021 09:07:07 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 28 Sep 2021 09:07:29 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:07:46 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:07:46 GMT
ENV ODOO_VERSION=12.0
# Wed, 06 Oct 2021 18:24:28 GMT
ARG ODOO_RELEASE=20211006
# Wed, 06 Oct 2021 18:24:29 GMT
ARG ODOO_SHA=f32dcd82b04e9a93e17a7d4b3ab471dc20408253
# Wed, 06 Oct 2021 18:25:36 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=f32dcd82b04e9a93e17a7d4b3ab471dc20408253
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 06 Oct 2021 18:25:39 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 06 Oct 2021 18:25:40 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 06 Oct 2021 18:25:40 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=f32dcd82b04e9a93e17a7d4b3ab471dc20408253
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 06 Oct 2021 18:25:41 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 06 Oct 2021 18:25:41 GMT
EXPOSE 8069 8071 8072
# Wed, 06 Oct 2021 18:25:41 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 06 Oct 2021 18:25:41 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 06 Oct 2021 18:25:41 GMT
USER odoo
# Wed, 06 Oct 2021 18:25:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Oct 2021 18:25:42 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:36d925ed8e305498a951c3b56d100d153ae3babf046b88e2d00899105fe81c31`  
		Last Modified: Tue, 28 Sep 2021 01:32:51 GMT  
		Size: 22.5 MB (22527699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5788ecc3532a07db45efea6a2c973faee8385402c0498b6cd805140e3ff3aa`  
		Last Modified: Tue, 28 Sep 2021 09:11:45 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d29df4b5fe46f143c4fcdd612f91cb00e025018292c0e2ea4f4aa8fb40b628c`  
		Last Modified: Tue, 28 Sep 2021 09:12:29 GMT  
		Size: 219.7 MB (219657423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa757125f4784d18e2db094bd9c15892e1e3a68f8405c3cfd6e44f57dfd10b5`  
		Last Modified: Tue, 28 Sep 2021 09:11:46 GMT  
		Size: 2.2 MB (2227263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999e75deb22b82657afe043a6b3b90c7531f3f68e0b794caa5a715a2656cc863`  
		Last Modified: Tue, 28 Sep 2021 09:11:54 GMT  
		Size: 22.0 MB (22019278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66d27d56f6793d5a1afe5f66f7c3af6786b87945b847e2b3db1e0401435a74e`  
		Last Modified: Wed, 06 Oct 2021 18:27:58 GMT  
		Size: 272.0 MB (272008802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245b8e1b96a304af8bf8cf3ae168a143796c4c97c3e611febbeda59ff66f66d3`  
		Last Modified: Wed, 06 Oct 2021 18:27:31 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542be52c4dfe61d73fb7d6484cf99ca1d03547b6e2fe332278e816b71ca23e67`  
		Last Modified: Wed, 06 Oct 2021 18:27:31 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386c0455b25b5ad3ae285e0cc43346bf653b33b098642e5686cfb2cbacff7564`  
		Last Modified: Wed, 06 Oct 2021 18:27:31 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc917cc806609fefcee591b902f6a83ed09d887a3866d3c8103b9c6e848e386d`  
		Last Modified: Wed, 06 Oct 2021 18:27:31 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:1b9dd4ba01b1d8cde59c3a2f3e55e80ad2b362d2bb0747e66cbdb121dac11d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:6092a42e0507311eb2be92dc11e4a663c107378688beb8acbcf8ad61296ef49c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.5 MB (528495283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca957e6c35d40c03c5f943f3151c64211bc2d3590143d6af24909b4734cdbb0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 08:57:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 28 Sep 2021 08:57:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 28 Sep 2021 08:57:31 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:02:35 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 28 Sep 2021 09:02:51 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:02:55 GMT
RUN npm install -g rtlcss
# Tue, 28 Sep 2021 09:02:55 GMT
ENV ODOO_VERSION=13.0
# Wed, 06 Oct 2021 18:23:03 GMT
ARG ODOO_RELEASE=20211006
# Wed, 06 Oct 2021 18:23:03 GMT
ARG ODOO_SHA=b3545e9d1a28c5955c3fc95d5dbe726807ed70f6
# Wed, 06 Oct 2021 18:24:16 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=b3545e9d1a28c5955c3fc95d5dbe726807ed70f6
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 06 Oct 2021 18:24:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 06 Oct 2021 18:24:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 06 Oct 2021 18:24:21 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=b3545e9d1a28c5955c3fc95d5dbe726807ed70f6
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 06 Oct 2021 18:24:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 06 Oct 2021 18:24:21 GMT
EXPOSE 8069 8071 8072
# Wed, 06 Oct 2021 18:24:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 06 Oct 2021 18:24:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 06 Oct 2021 18:24:22 GMT
USER odoo
# Wed, 06 Oct 2021 18:24:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Oct 2021 18:24:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c839a5f094fb26110db82ce8478b2716b5ae4a3b1f4787dcf4e42a3ee806fa7`  
		Last Modified: Tue, 28 Sep 2021 09:11:24 GMT  
		Size: 207.1 MB (207131178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9702631183b797e14e02f699e03b5970d762468d09fdf90f68293fa1d190b699`  
		Last Modified: Tue, 28 Sep 2021 09:10:56 GMT  
		Size: 2.3 MB (2347886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d624dc0f4f384ddbee9fa140b492064255415e389bc2188ab634fc3f01234b`  
		Last Modified: Tue, 28 Sep 2021 09:10:56 GMT  
		Size: 882.8 KB (882781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384122c895c86c5de041a316f4e683afbaf700a8bd46ba80c4c7353c027fd707`  
		Last Modified: Wed, 06 Oct 2021 18:27:20 GMT  
		Size: 291.0 MB (290984979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09942985fe3486e6a006ebfaf8647cd4124e501783ebdb5f12d526a34a1047ef`  
		Last Modified: Wed, 06 Oct 2021 18:26:50 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211b30b01985a07c05f9fdc24013f61f99e975007d1480f5603cd35584e9f6a6`  
		Last Modified: Wed, 06 Oct 2021 18:26:50 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a28cd5d377a73ec89f37784c71b53a3573b25ff3f675481c2a5f3a4f5956574`  
		Last Modified: Wed, 06 Oct 2021 18:26:50 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568a9504a603d4ef8bb6be73d254572db190d14b0ddc46708af33bd3b01401a2`  
		Last Modified: Wed, 06 Oct 2021 18:26:50 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:1b9dd4ba01b1d8cde59c3a2f3e55e80ad2b362d2bb0747e66cbdb121dac11d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:6092a42e0507311eb2be92dc11e4a663c107378688beb8acbcf8ad61296ef49c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.5 MB (528495283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca957e6c35d40c03c5f943f3151c64211bc2d3590143d6af24909b4734cdbb0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 08:57:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 28 Sep 2021 08:57:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 28 Sep 2021 08:57:31 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 09:02:35 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 28 Sep 2021 09:02:51 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 09:02:55 GMT
RUN npm install -g rtlcss
# Tue, 28 Sep 2021 09:02:55 GMT
ENV ODOO_VERSION=13.0
# Wed, 06 Oct 2021 18:23:03 GMT
ARG ODOO_RELEASE=20211006
# Wed, 06 Oct 2021 18:23:03 GMT
ARG ODOO_SHA=b3545e9d1a28c5955c3fc95d5dbe726807ed70f6
# Wed, 06 Oct 2021 18:24:16 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=b3545e9d1a28c5955c3fc95d5dbe726807ed70f6
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 06 Oct 2021 18:24:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 06 Oct 2021 18:24:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 06 Oct 2021 18:24:21 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=b3545e9d1a28c5955c3fc95d5dbe726807ed70f6
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 06 Oct 2021 18:24:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 06 Oct 2021 18:24:21 GMT
EXPOSE 8069 8071 8072
# Wed, 06 Oct 2021 18:24:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 06 Oct 2021 18:24:22 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 06 Oct 2021 18:24:22 GMT
USER odoo
# Wed, 06 Oct 2021 18:24:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Oct 2021 18:24:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c839a5f094fb26110db82ce8478b2716b5ae4a3b1f4787dcf4e42a3ee806fa7`  
		Last Modified: Tue, 28 Sep 2021 09:11:24 GMT  
		Size: 207.1 MB (207131178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9702631183b797e14e02f699e03b5970d762468d09fdf90f68293fa1d190b699`  
		Last Modified: Tue, 28 Sep 2021 09:10:56 GMT  
		Size: 2.3 MB (2347886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d624dc0f4f384ddbee9fa140b492064255415e389bc2188ab634fc3f01234b`  
		Last Modified: Tue, 28 Sep 2021 09:10:56 GMT  
		Size: 882.8 KB (882781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384122c895c86c5de041a316f4e683afbaf700a8bd46ba80c4c7353c027fd707`  
		Last Modified: Wed, 06 Oct 2021 18:27:20 GMT  
		Size: 291.0 MB (290984979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09942985fe3486e6a006ebfaf8647cd4124e501783ebdb5f12d526a34a1047ef`  
		Last Modified: Wed, 06 Oct 2021 18:26:50 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211b30b01985a07c05f9fdc24013f61f99e975007d1480f5603cd35584e9f6a6`  
		Last Modified: Wed, 06 Oct 2021 18:26:50 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a28cd5d377a73ec89f37784c71b53a3573b25ff3f675481c2a5f3a4f5956574`  
		Last Modified: Wed, 06 Oct 2021 18:26:50 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568a9504a603d4ef8bb6be73d254572db190d14b0ddc46708af33bd3b01401a2`  
		Last Modified: Wed, 06 Oct 2021 18:26:50 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:155d4ac2e63711ec81bdec2da293dada04473a3daa04419a19b5d54d33fc0fa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:0d01c9391fb84f3da9bb31f056482ef94b03b9657aa1dac18d0d6fcf0698a355
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **517.1 MB (517069631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f2ca467f9ebde283f3b1ddb06c3578e51b965d72bbdd694cb5496cddb4fb1b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 08:57:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 28 Sep 2021 08:57:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 28 Sep 2021 08:57:31 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 08:59:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 28 Sep 2021 08:59:19 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 08:59:24 GMT
RUN npm install -g rtlcss
# Tue, 28 Sep 2021 08:59:24 GMT
ENV ODOO_VERSION=14.0
# Wed, 06 Oct 2021 18:21:37 GMT
ARG ODOO_RELEASE=20211006
# Wed, 06 Oct 2021 18:21:38 GMT
ARG ODOO_SHA=468f467ce89e39b9aa735bbc70412000bd99b2c2
# Wed, 06 Oct 2021 18:22:52 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=468f467ce89e39b9aa735bbc70412000bd99b2c2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 06 Oct 2021 18:22:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 06 Oct 2021 18:22:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 06 Oct 2021 18:22:57 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=468f467ce89e39b9aa735bbc70412000bd99b2c2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 06 Oct 2021 18:22:57 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 06 Oct 2021 18:22:57 GMT
EXPOSE 8069 8071 8072
# Wed, 06 Oct 2021 18:22:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 06 Oct 2021 18:22:57 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 06 Oct 2021 18:22:58 GMT
USER odoo
# Wed, 06 Oct 2021 18:22:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Oct 2021 18:22:58 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202cc4801528046f1295d1e9fde12d1ca51922bb3bbb78f28414392e496affb`  
		Last Modified: Tue, 28 Sep 2021 09:10:33 GMT  
		Size: 213.2 MB (213172416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f9940244ebdbb6e2808ac61f977f7a881c116cf6b1a5ff5400656affb2122`  
		Last Modified: Tue, 28 Sep 2021 09:10:05 GMT  
		Size: 2.4 MB (2350586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e07d3bb02ae4b65c91447226f5c9402577d6f42a0cc8060e112b073485266a8`  
		Last Modified: Tue, 28 Sep 2021 09:10:05 GMT  
		Size: 882.7 KB (882660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecf74ff761664d7582a8116116f478b7603d9c074f6444fbc7c6524daff9b5c`  
		Last Modified: Wed, 06 Oct 2021 18:26:37 GMT  
		Size: 273.5 MB (273515514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12ad090856f79106d3711b32bd612da86f3d0ebd0dd878f07b55db69876d356`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf68f36b396626eb481d5916d575d517aa7451a7bba69b8c4623c8737a21875`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36578e51156a34aec1d27c7ab25c5d5ca51b1a8c06a755c17296fbacdde1ca07`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b5b4a2b197bce1aeacdadb4b7dae8d2a9f837ade3ed3d61f690524ad69184a`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:155d4ac2e63711ec81bdec2da293dada04473a3daa04419a19b5d54d33fc0fa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:0d01c9391fb84f3da9bb31f056482ef94b03b9657aa1dac18d0d6fcf0698a355
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **517.1 MB (517069631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f2ca467f9ebde283f3b1ddb06c3578e51b965d72bbdd694cb5496cddb4fb1b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 08:57:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 28 Sep 2021 08:57:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 28 Sep 2021 08:57:31 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 08:59:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 28 Sep 2021 08:59:19 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 08:59:24 GMT
RUN npm install -g rtlcss
# Tue, 28 Sep 2021 08:59:24 GMT
ENV ODOO_VERSION=14.0
# Wed, 06 Oct 2021 18:21:37 GMT
ARG ODOO_RELEASE=20211006
# Wed, 06 Oct 2021 18:21:38 GMT
ARG ODOO_SHA=468f467ce89e39b9aa735bbc70412000bd99b2c2
# Wed, 06 Oct 2021 18:22:52 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=468f467ce89e39b9aa735bbc70412000bd99b2c2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 06 Oct 2021 18:22:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 06 Oct 2021 18:22:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 06 Oct 2021 18:22:57 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=468f467ce89e39b9aa735bbc70412000bd99b2c2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 06 Oct 2021 18:22:57 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 06 Oct 2021 18:22:57 GMT
EXPOSE 8069 8071 8072
# Wed, 06 Oct 2021 18:22:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 06 Oct 2021 18:22:57 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 06 Oct 2021 18:22:58 GMT
USER odoo
# Wed, 06 Oct 2021 18:22:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Oct 2021 18:22:58 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202cc4801528046f1295d1e9fde12d1ca51922bb3bbb78f28414392e496affb`  
		Last Modified: Tue, 28 Sep 2021 09:10:33 GMT  
		Size: 213.2 MB (213172416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f9940244ebdbb6e2808ac61f977f7a881c116cf6b1a5ff5400656affb2122`  
		Last Modified: Tue, 28 Sep 2021 09:10:05 GMT  
		Size: 2.4 MB (2350586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e07d3bb02ae4b65c91447226f5c9402577d6f42a0cc8060e112b073485266a8`  
		Last Modified: Tue, 28 Sep 2021 09:10:05 GMT  
		Size: 882.7 KB (882660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecf74ff761664d7582a8116116f478b7603d9c074f6444fbc7c6524daff9b5c`  
		Last Modified: Wed, 06 Oct 2021 18:26:37 GMT  
		Size: 273.5 MB (273515514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12ad090856f79106d3711b32bd612da86f3d0ebd0dd878f07b55db69876d356`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf68f36b396626eb481d5916d575d517aa7451a7bba69b8c4623c8737a21875`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36578e51156a34aec1d27c7ab25c5d5ca51b1a8c06a755c17296fbacdde1ca07`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b5b4a2b197bce1aeacdadb4b7dae8d2a9f837ade3ed3d61f690524ad69184a`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:155d4ac2e63711ec81bdec2da293dada04473a3daa04419a19b5d54d33fc0fa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:0d01c9391fb84f3da9bb31f056482ef94b03b9657aa1dac18d0d6fcf0698a355
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **517.1 MB (517069631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f2ca467f9ebde283f3b1ddb06c3578e51b965d72bbdd694cb5496cddb4fb1b2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 08:57:30 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 28 Sep 2021 08:57:30 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 28 Sep 2021 08:57:31 GMT
ENV LANG=C.UTF-8
# Tue, 28 Sep 2021 08:59:02 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 28 Sep 2021 08:59:19 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 08:59:24 GMT
RUN npm install -g rtlcss
# Tue, 28 Sep 2021 08:59:24 GMT
ENV ODOO_VERSION=14.0
# Wed, 06 Oct 2021 18:21:37 GMT
ARG ODOO_RELEASE=20211006
# Wed, 06 Oct 2021 18:21:38 GMT
ARG ODOO_SHA=468f467ce89e39b9aa735bbc70412000bd99b2c2
# Wed, 06 Oct 2021 18:22:52 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=468f467ce89e39b9aa735bbc70412000bd99b2c2
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 06 Oct 2021 18:22:56 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 06 Oct 2021 18:22:56 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 06 Oct 2021 18:22:57 GMT
# ARGS: ODOO_RELEASE=20211006 ODOO_SHA=468f467ce89e39b9aa735bbc70412000bd99b2c2
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 06 Oct 2021 18:22:57 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 06 Oct 2021 18:22:57 GMT
EXPOSE 8069 8071 8072
# Wed, 06 Oct 2021 18:22:57 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 06 Oct 2021 18:22:57 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 06 Oct 2021 18:22:58 GMT
USER odoo
# Wed, 06 Oct 2021 18:22:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 06 Oct 2021 18:22:58 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202cc4801528046f1295d1e9fde12d1ca51922bb3bbb78f28414392e496affb`  
		Last Modified: Tue, 28 Sep 2021 09:10:33 GMT  
		Size: 213.2 MB (213172416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f9940244ebdbb6e2808ac61f977f7a881c116cf6b1a5ff5400656affb2122`  
		Last Modified: Tue, 28 Sep 2021 09:10:05 GMT  
		Size: 2.4 MB (2350586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e07d3bb02ae4b65c91447226f5c9402577d6f42a0cc8060e112b073485266a8`  
		Last Modified: Tue, 28 Sep 2021 09:10:05 GMT  
		Size: 882.7 KB (882660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecf74ff761664d7582a8116116f478b7603d9c074f6444fbc7c6524daff9b5c`  
		Last Modified: Wed, 06 Oct 2021 18:26:37 GMT  
		Size: 273.5 MB (273515514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12ad090856f79106d3711b32bd612da86f3d0ebd0dd878f07b55db69876d356`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf68f36b396626eb481d5916d575d517aa7451a7bba69b8c4623c8737a21875`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36578e51156a34aec1d27c7ab25c5d5ca51b1a8c06a755c17296fbacdde1ca07`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b5b4a2b197bce1aeacdadb4b7dae8d2a9f837ade3ed3d61f690524ad69184a`  
		Last Modified: Wed, 06 Oct 2021 18:26:06 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
