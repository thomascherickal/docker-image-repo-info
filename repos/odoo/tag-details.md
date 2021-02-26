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
$ docker pull odoo@sha256:addf1982602d3fd520fa5d2d926bc28dbdf9f2fb6b3e52abdd8f08439f261908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:a7827bf62bc18775059903d554fae0fd1730c313170783878080df95ff36aefe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.1 MB (541078043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b1681c76ae5c43455d520e0b45ab83ec115e128fb8be02650aad1259881bba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:33:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 09 Feb 2021 17:33:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 09 Feb 2021 17:33:49 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 17:33:50 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 09 Feb 2021 17:35:51 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 09 Feb 2021 17:36:01 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:36:16 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:36:17 GMT
ENV ODOO_VERSION=12.0
# Fri, 26 Feb 2021 22:53:40 GMT
ARG ODOO_RELEASE=20210226
# Fri, 26 Feb 2021 22:53:41 GMT
ARG ODOO_SHA=7d580c67928ca5fbb1beb49221b11c6513f8a6ed
# Fri, 26 Feb 2021 22:54:43 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=7d580c67928ca5fbb1beb49221b11c6513f8a6ed
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Feb 2021 22:54:44 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 26 Feb 2021 22:54:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Feb 2021 22:54:45 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=7d580c67928ca5fbb1beb49221b11c6513f8a6ed
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Feb 2021 22:54:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Feb 2021 22:54:45 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Feb 2021 22:54:46 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Feb 2021 22:54:46 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Feb 2021 22:54:46 GMT
USER odoo
# Fri, 26 Feb 2021 22:54:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Feb 2021 22:54:46 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1cabf5609130f825def08a86940a9a06f7025505559b2c7e652b60a9e05005`  
		Last Modified: Tue, 09 Feb 2021 17:40:43 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23230155ecde52cbc43dbfe8141ef3dcbfaa6a5e242654c5ff6071e727f0a9`  
		Last Modified: Tue, 09 Feb 2021 17:41:19 GMT  
		Size: 219.6 MB (219611261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666ff187134bcc9d0cf0a66450af847efce4bd9dc973a88ae485acff4a4b3df1`  
		Last Modified: Tue, 09 Feb 2021 17:40:43 GMT  
		Size: 2.2 MB (2222432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e5ca9709c7ca8d1819e6f5e6a2a15591eb75f5cf82ba48c2825cde329116c8`  
		Last Modified: Tue, 09 Feb 2021 17:41:01 GMT  
		Size: 22.1 MB (22055467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0e735779acf6a6defe816bbebebc23d958f56b2556eba64b9ca6d640e2bb88`  
		Last Modified: Fri, 26 Feb 2021 22:57:10 GMT  
		Size: 274.7 MB (274657650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c46fd1f5ed93988fc3f5c22ce61ce10bb31b01e9daf78d667e5cae4de3c28f`  
		Last Modified: Fri, 26 Feb 2021 22:56:37 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ea8e1aad2271971025bd86df13238e2888a39f3430231b8b26d36aa7ff285`  
		Last Modified: Fri, 26 Feb 2021 22:56:36 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e6bf4992364ccd7e6680e17bd3666abecd8c51b58d49e25f17cc127d13fbbb`  
		Last Modified: Fri, 26 Feb 2021 22:56:36 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cf7aa0537883a59e6ca3302c9bd39a4e33f5de4e2cd8aad1124830b8318533`  
		Last Modified: Fri, 26 Feb 2021 22:56:37 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:addf1982602d3fd520fa5d2d926bc28dbdf9f2fb6b3e52abdd8f08439f261908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:a7827bf62bc18775059903d554fae0fd1730c313170783878080df95ff36aefe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.1 MB (541078043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6b1681c76ae5c43455d520e0b45ab83ec115e128fb8be02650aad1259881bba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:33:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 09 Feb 2021 17:33:48 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 09 Feb 2021 17:33:49 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 17:33:50 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 09 Feb 2021 17:35:51 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 09 Feb 2021 17:36:01 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:36:16 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:36:17 GMT
ENV ODOO_VERSION=12.0
# Fri, 26 Feb 2021 22:53:40 GMT
ARG ODOO_RELEASE=20210226
# Fri, 26 Feb 2021 22:53:41 GMT
ARG ODOO_SHA=7d580c67928ca5fbb1beb49221b11c6513f8a6ed
# Fri, 26 Feb 2021 22:54:43 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=7d580c67928ca5fbb1beb49221b11c6513f8a6ed
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Feb 2021 22:54:44 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 26 Feb 2021 22:54:44 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Feb 2021 22:54:45 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=7d580c67928ca5fbb1beb49221b11c6513f8a6ed
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Feb 2021 22:54:45 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Feb 2021 22:54:45 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Feb 2021 22:54:46 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Feb 2021 22:54:46 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Feb 2021 22:54:46 GMT
USER odoo
# Fri, 26 Feb 2021 22:54:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Feb 2021 22:54:46 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1cabf5609130f825def08a86940a9a06f7025505559b2c7e652b60a9e05005`  
		Last Modified: Tue, 09 Feb 2021 17:40:43 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23230155ecde52cbc43dbfe8141ef3dcbfaa6a5e242654c5ff6071e727f0a9`  
		Last Modified: Tue, 09 Feb 2021 17:41:19 GMT  
		Size: 219.6 MB (219611261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666ff187134bcc9d0cf0a66450af847efce4bd9dc973a88ae485acff4a4b3df1`  
		Last Modified: Tue, 09 Feb 2021 17:40:43 GMT  
		Size: 2.2 MB (2222432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e5ca9709c7ca8d1819e6f5e6a2a15591eb75f5cf82ba48c2825cde329116c8`  
		Last Modified: Tue, 09 Feb 2021 17:41:01 GMT  
		Size: 22.1 MB (22055467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0e735779acf6a6defe816bbebebc23d958f56b2556eba64b9ca6d640e2bb88`  
		Last Modified: Fri, 26 Feb 2021 22:57:10 GMT  
		Size: 274.7 MB (274657650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c46fd1f5ed93988fc3f5c22ce61ce10bb31b01e9daf78d667e5cae4de3c28f`  
		Last Modified: Fri, 26 Feb 2021 22:56:37 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8ea8e1aad2271971025bd86df13238e2888a39f3430231b8b26d36aa7ff285`  
		Last Modified: Fri, 26 Feb 2021 22:56:36 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e6bf4992364ccd7e6680e17bd3666abecd8c51b58d49e25f17cc127d13fbbb`  
		Last Modified: Fri, 26 Feb 2021 22:56:36 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cf7aa0537883a59e6ca3302c9bd39a4e33f5de4e2cd8aad1124830b8318533`  
		Last Modified: Fri, 26 Feb 2021 22:56:37 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:c943e83eaa8b55608dedf7932a2a9e06fd0e60e27d5f95ba2361cbab15cca6c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:abe75cb75a4a2cc97d9ff7321a527018efe78fe1bd5c9b57b7c29fe4f0540a4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.6 MB (530565441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71206964dd68f1fd5129d77f5565ad5c34aff0d1d5191731224c211aed4ee1ed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:27:28 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 09 Feb 2021 17:27:28 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 09 Feb 2021 17:27:29 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 17:32:01 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 09 Feb 2021 17:32:08 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:32:12 GMT
RUN npm install -g rtlcss
# Tue, 09 Feb 2021 17:32:12 GMT
ENV ODOO_VERSION=13.0
# Fri, 26 Feb 2021 22:52:10 GMT
ARG ODOO_RELEASE=20210226
# Fri, 26 Feb 2021 22:52:10 GMT
ARG ODOO_SHA=a3a1561cda391d5ec771e0b228ea50ff31949a0a
# Fri, 26 Feb 2021 22:53:24 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=a3a1561cda391d5ec771e0b228ea50ff31949a0a
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Feb 2021 22:53:25 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 26 Feb 2021 22:53:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Feb 2021 22:53:26 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=a3a1561cda391d5ec771e0b228ea50ff31949a0a
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Feb 2021 22:53:27 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Feb 2021 22:53:27 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Feb 2021 22:53:27 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Feb 2021 22:53:27 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Feb 2021 22:53:27 GMT
USER odoo
# Fri, 26 Feb 2021 22:53:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Feb 2021 22:53:28 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df63def913e7acc2a8ee5bbdb8dac5f2449993c30e7aff862b1f01f485f5f2`  
		Last Modified: Tue, 09 Feb 2021 17:40:15 GMT  
		Size: 207.1 MB (207097574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ab203da2fb5d30f709e95af58f20d98a184b7fbc9e8611a5d91717a5fbe1c9`  
		Last Modified: Tue, 09 Feb 2021 17:39:37 GMT  
		Size: 2.3 MB (2343915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16975ddc87358fae6e7b7b9c3809881bdaaf4a63f75c307a3d344c92852557f5`  
		Last Modified: Tue, 09 Feb 2021 17:39:36 GMT  
		Size: 909.0 KB (909031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5265198e7818b99c00250b113fd86f6f4a1f12f66df10e584cd419f5b2bd861a`  
		Last Modified: Fri, 26 Feb 2021 22:56:32 GMT  
		Size: 293.1 MB (293117373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e06bfe0997405a57d30e1d0b2679bd5b125785d31ae250c3fb19977374cfbb`  
		Last Modified: Fri, 26 Feb 2021 22:55:55 GMT  
		Size: 673.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd6446508c2696c22e3eaab5d0c4720cb0e5472bac5d973ad737e732e946137`  
		Last Modified: Fri, 26 Feb 2021 22:55:55 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9f423248de7126dd46387296c351bb4487418aef8360317c0733a782f53e90`  
		Last Modified: Fri, 26 Feb 2021 22:55:55 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577964de6b21bfc1fc76989c5faea13b28d6f131fdbbaee5189af5df77fe65a2`  
		Last Modified: Fri, 26 Feb 2021 22:55:55 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:c943e83eaa8b55608dedf7932a2a9e06fd0e60e27d5f95ba2361cbab15cca6c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:abe75cb75a4a2cc97d9ff7321a527018efe78fe1bd5c9b57b7c29fe4f0540a4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **530.6 MB (530565441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71206964dd68f1fd5129d77f5565ad5c34aff0d1d5191731224c211aed4ee1ed`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:27:28 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 09 Feb 2021 17:27:28 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 09 Feb 2021 17:27:29 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 17:32:01 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 09 Feb 2021 17:32:08 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:32:12 GMT
RUN npm install -g rtlcss
# Tue, 09 Feb 2021 17:32:12 GMT
ENV ODOO_VERSION=13.0
# Fri, 26 Feb 2021 22:52:10 GMT
ARG ODOO_RELEASE=20210226
# Fri, 26 Feb 2021 22:52:10 GMT
ARG ODOO_SHA=a3a1561cda391d5ec771e0b228ea50ff31949a0a
# Fri, 26 Feb 2021 22:53:24 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=a3a1561cda391d5ec771e0b228ea50ff31949a0a
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Feb 2021 22:53:25 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 26 Feb 2021 22:53:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Feb 2021 22:53:26 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=a3a1561cda391d5ec771e0b228ea50ff31949a0a
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Feb 2021 22:53:27 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Feb 2021 22:53:27 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Feb 2021 22:53:27 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Feb 2021 22:53:27 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Feb 2021 22:53:27 GMT
USER odoo
# Fri, 26 Feb 2021 22:53:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Feb 2021 22:53:28 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df63def913e7acc2a8ee5bbdb8dac5f2449993c30e7aff862b1f01f485f5f2`  
		Last Modified: Tue, 09 Feb 2021 17:40:15 GMT  
		Size: 207.1 MB (207097574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ab203da2fb5d30f709e95af58f20d98a184b7fbc9e8611a5d91717a5fbe1c9`  
		Last Modified: Tue, 09 Feb 2021 17:39:37 GMT  
		Size: 2.3 MB (2343915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16975ddc87358fae6e7b7b9c3809881bdaaf4a63f75c307a3d344c92852557f5`  
		Last Modified: Tue, 09 Feb 2021 17:39:36 GMT  
		Size: 909.0 KB (909031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5265198e7818b99c00250b113fd86f6f4a1f12f66df10e584cd419f5b2bd861a`  
		Last Modified: Fri, 26 Feb 2021 22:56:32 GMT  
		Size: 293.1 MB (293117373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e06bfe0997405a57d30e1d0b2679bd5b125785d31ae250c3fb19977374cfbb`  
		Last Modified: Fri, 26 Feb 2021 22:55:55 GMT  
		Size: 673.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd6446508c2696c22e3eaab5d0c4720cb0e5472bac5d973ad737e732e946137`  
		Last Modified: Fri, 26 Feb 2021 22:55:55 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9f423248de7126dd46387296c351bb4487418aef8360317c0733a782f53e90`  
		Last Modified: Fri, 26 Feb 2021 22:55:55 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577964de6b21bfc1fc76989c5faea13b28d6f131fdbbaee5189af5df77fe65a2`  
		Last Modified: Fri, 26 Feb 2021 22:55:55 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:897664c60243356b75278a42be15bb9b4803f208125c64285f006de2e444b30e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:fb89f2854bfc7e4081bc51fc3c6ac80e00fb794870c020dcf8c6e999d44deb80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **513.1 MB (513062598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ec4f9b29b7a3ddb79b9dba98d4eaa6f29190bfe9acd24ab2e28da949c23a8c1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:27:28 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 09 Feb 2021 17:27:28 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 09 Feb 2021 17:27:29 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 17:29:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 09 Feb 2021 17:29:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:29:17 GMT
RUN npm install -g rtlcss
# Tue, 09 Feb 2021 17:29:17 GMT
ENV ODOO_VERSION=14.0
# Fri, 26 Feb 2021 22:50:53 GMT
ARG ODOO_RELEASE=20210226
# Fri, 26 Feb 2021 22:50:54 GMT
ARG ODOO_SHA=b0b9309d5156ae171d6f0213d3b15005b9257c47
# Fri, 26 Feb 2021 22:52:01 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=b0b9309d5156ae171d6f0213d3b15005b9257c47
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Feb 2021 22:52:02 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 26 Feb 2021 22:52:02 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Feb 2021 22:52:03 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=b0b9309d5156ae171d6f0213d3b15005b9257c47
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Feb 2021 22:52:04 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Feb 2021 22:52:04 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Feb 2021 22:52:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Feb 2021 22:52:04 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Feb 2021 22:52:04 GMT
USER odoo
# Fri, 26 Feb 2021 22:52:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Feb 2021 22:52:05 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f01c0c02d487d167e4440bbc1f9f7d18aef702f607a4f4d53ed03fa8d789738`  
		Last Modified: Tue, 09 Feb 2021 17:39:00 GMT  
		Size: 213.2 MB (213152252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e328a5fa7db6c9ddcf2128f44c9e8e1644ea40f1e250a7427dd00dc2b19700`  
		Last Modified: Tue, 09 Feb 2021 17:37:49 GMT  
		Size: 2.3 MB (2346601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241913ecf51f6d0a8e68d705ef3d58c1745fbbbca4089277a75bd244831b5247`  
		Last Modified: Tue, 09 Feb 2021 17:37:51 GMT  
		Size: 908.6 KB (908573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02d954142c172caef5e15f9149a84e3c67177976cba20ac4cccb809421b1458`  
		Last Modified: Fri, 26 Feb 2021 22:55:43 GMT  
		Size: 269.6 MB (269557626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b62491dd7b39816c85e2375fd1f504876585f1bddf3e271b1c04f184665915`  
		Last Modified: Fri, 26 Feb 2021 22:55:06 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989821e7c976ba19d887b194119c990e6b3f6fc7ed66b14a2f454ce2ece3e89c`  
		Last Modified: Fri, 26 Feb 2021 22:55:06 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb474d1fd84dd993b96eae0acb7c667d2f26e1691094c077a89f9950039aa6e7`  
		Last Modified: Fri, 26 Feb 2021 22:55:05 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5817d57603203c69e3e1273e33c1677bbfc2d9ed836806b7ae5079b2c743440d`  
		Last Modified: Fri, 26 Feb 2021 22:55:05 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:897664c60243356b75278a42be15bb9b4803f208125c64285f006de2e444b30e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:fb89f2854bfc7e4081bc51fc3c6ac80e00fb794870c020dcf8c6e999d44deb80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **513.1 MB (513062598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ec4f9b29b7a3ddb79b9dba98d4eaa6f29190bfe9acd24ab2e28da949c23a8c1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:27:28 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 09 Feb 2021 17:27:28 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 09 Feb 2021 17:27:29 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 17:29:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 09 Feb 2021 17:29:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:29:17 GMT
RUN npm install -g rtlcss
# Tue, 09 Feb 2021 17:29:17 GMT
ENV ODOO_VERSION=14.0
# Fri, 26 Feb 2021 22:50:53 GMT
ARG ODOO_RELEASE=20210226
# Fri, 26 Feb 2021 22:50:54 GMT
ARG ODOO_SHA=b0b9309d5156ae171d6f0213d3b15005b9257c47
# Fri, 26 Feb 2021 22:52:01 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=b0b9309d5156ae171d6f0213d3b15005b9257c47
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Feb 2021 22:52:02 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 26 Feb 2021 22:52:02 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Feb 2021 22:52:03 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=b0b9309d5156ae171d6f0213d3b15005b9257c47
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Feb 2021 22:52:04 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Feb 2021 22:52:04 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Feb 2021 22:52:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Feb 2021 22:52:04 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Feb 2021 22:52:04 GMT
USER odoo
# Fri, 26 Feb 2021 22:52:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Feb 2021 22:52:05 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f01c0c02d487d167e4440bbc1f9f7d18aef702f607a4f4d53ed03fa8d789738`  
		Last Modified: Tue, 09 Feb 2021 17:39:00 GMT  
		Size: 213.2 MB (213152252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e328a5fa7db6c9ddcf2128f44c9e8e1644ea40f1e250a7427dd00dc2b19700`  
		Last Modified: Tue, 09 Feb 2021 17:37:49 GMT  
		Size: 2.3 MB (2346601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241913ecf51f6d0a8e68d705ef3d58c1745fbbbca4089277a75bd244831b5247`  
		Last Modified: Tue, 09 Feb 2021 17:37:51 GMT  
		Size: 908.6 KB (908573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02d954142c172caef5e15f9149a84e3c67177976cba20ac4cccb809421b1458`  
		Last Modified: Fri, 26 Feb 2021 22:55:43 GMT  
		Size: 269.6 MB (269557626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b62491dd7b39816c85e2375fd1f504876585f1bddf3e271b1c04f184665915`  
		Last Modified: Fri, 26 Feb 2021 22:55:06 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989821e7c976ba19d887b194119c990e6b3f6fc7ed66b14a2f454ce2ece3e89c`  
		Last Modified: Fri, 26 Feb 2021 22:55:06 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb474d1fd84dd993b96eae0acb7c667d2f26e1691094c077a89f9950039aa6e7`  
		Last Modified: Fri, 26 Feb 2021 22:55:05 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5817d57603203c69e3e1273e33c1677bbfc2d9ed836806b7ae5079b2c743440d`  
		Last Modified: Fri, 26 Feb 2021 22:55:05 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:897664c60243356b75278a42be15bb9b4803f208125c64285f006de2e444b30e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:fb89f2854bfc7e4081bc51fc3c6ac80e00fb794870c020dcf8c6e999d44deb80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **513.1 MB (513062598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ec4f9b29b7a3ddb79b9dba98d4eaa6f29190bfe9acd24ab2e28da949c23a8c1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:27:28 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 09 Feb 2021 17:27:28 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 09 Feb 2021 17:27:29 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 17:29:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 09 Feb 2021 17:29:13 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:29:17 GMT
RUN npm install -g rtlcss
# Tue, 09 Feb 2021 17:29:17 GMT
ENV ODOO_VERSION=14.0
# Fri, 26 Feb 2021 22:50:53 GMT
ARG ODOO_RELEASE=20210226
# Fri, 26 Feb 2021 22:50:54 GMT
ARG ODOO_SHA=b0b9309d5156ae171d6f0213d3b15005b9257c47
# Fri, 26 Feb 2021 22:52:01 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=b0b9309d5156ae171d6f0213d3b15005b9257c47
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 26 Feb 2021 22:52:02 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Fri, 26 Feb 2021 22:52:02 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 26 Feb 2021 22:52:03 GMT
# ARGS: ODOO_RELEASE=20210226 ODOO_SHA=b0b9309d5156ae171d6f0213d3b15005b9257c47
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 26 Feb 2021 22:52:04 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 26 Feb 2021 22:52:04 GMT
EXPOSE 8069 8071 8072
# Fri, 26 Feb 2021 22:52:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 26 Feb 2021 22:52:04 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 26 Feb 2021 22:52:04 GMT
USER odoo
# Fri, 26 Feb 2021 22:52:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Feb 2021 22:52:05 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f01c0c02d487d167e4440bbc1f9f7d18aef702f607a4f4d53ed03fa8d789738`  
		Last Modified: Tue, 09 Feb 2021 17:39:00 GMT  
		Size: 213.2 MB (213152252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e328a5fa7db6c9ddcf2128f44c9e8e1644ea40f1e250a7427dd00dc2b19700`  
		Last Modified: Tue, 09 Feb 2021 17:37:49 GMT  
		Size: 2.3 MB (2346601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241913ecf51f6d0a8e68d705ef3d58c1745fbbbca4089277a75bd244831b5247`  
		Last Modified: Tue, 09 Feb 2021 17:37:51 GMT  
		Size: 908.6 KB (908573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02d954142c172caef5e15f9149a84e3c67177976cba20ac4cccb809421b1458`  
		Last Modified: Fri, 26 Feb 2021 22:55:43 GMT  
		Size: 269.6 MB (269557626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b62491dd7b39816c85e2375fd1f504876585f1bddf3e271b1c04f184665915`  
		Last Modified: Fri, 26 Feb 2021 22:55:06 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989821e7c976ba19d887b194119c990e6b3f6fc7ed66b14a2f454ce2ece3e89c`  
		Last Modified: Fri, 26 Feb 2021 22:55:06 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb474d1fd84dd993b96eae0acb7c667d2f26e1691094c077a89f9950039aa6e7`  
		Last Modified: Fri, 26 Feb 2021 22:55:05 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5817d57603203c69e3e1273e33c1677bbfc2d9ed836806b7ae5079b2c743440d`  
		Last Modified: Fri, 26 Feb 2021 22:55:05 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
