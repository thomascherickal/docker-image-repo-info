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
$ docker pull odoo@sha256:08545371817e39f4414c3c2c9183e8eb494e983ab86ab8b0d6b1de25e13b3b4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:11` - linux; amd64

```console
$ docker pull odoo@sha256:4a4bfb161160462d8fb4a1139efcb2f0efd237db087734e94591d8a2b7ccf48e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386118334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1389f2233b6fe0ab1e25b40a0277e2de024c26159926179ec64661dbdb3940ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:50 GMT
ADD file:40f52c233aecabf572a9db7450590d54d5e125fb00ecbb4a26fecd0b71e84eb8 in / 
# Thu, 16 Apr 2020 03:27:50 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 22:36:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Mon, 20 Apr 2020 17:50:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Mon, 20 Apr 2020 17:50:43 GMT
ENV LANG=C.UTF-8
# Mon, 20 Apr 2020 17:50:44 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Mon, 20 Apr 2020 17:53:49 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 20 Apr 2020 17:54:06 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:56:17 GMT
ENV ODOO_VERSION=11.0
# Mon, 20 Apr 2020 17:56:19 GMT
ARG ODOO_RELEASE=20200417
# Mon, 20 Apr 2020 17:56:19 GMT
ARG ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
# Mon, 20 Apr 2020 17:57:35 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb        && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Apr 2020 17:57:36 GMT
COPY file:cdc612ad49467417b0321c166f94e4f99b071755cb6ade071774e83d3b6ee4cb in / 
# Mon, 20 Apr 2020 17:57:37 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Apr 2020 17:57:39 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Apr 2020 17:57:39 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Apr 2020 17:57:40 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Apr 2020 17:57:40 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Apr 2020 17:57:41 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Apr 2020 17:57:41 GMT
USER odoo
# Mon, 20 Apr 2020 17:57:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Apr 2020 17:57:42 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:5e35bd43cf7898d036f8515be74d45b2e3abd2a5534fc280de63a9c22dd175bd`  
		Last Modified: Thu, 16 Apr 2020 03:35:04 GMT  
		Size: 22.5 MB (22513476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8268d7e205b4a86bdee4fc46423b4c949689fcc8a0c0399ea26a6ca29b50776`  
		Last Modified: Mon, 20 Apr 2020 17:59:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49716de29cf293e5ffc4698d23b76ea7c270249edcaaeb97e1fcd5fe041abdd`  
		Last Modified: Mon, 20 Apr 2020 17:59:53 GMT  
		Size: 219.7 MB (219650400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2023748d1ac8b71b990e34599defa253234c2af53880a5a8cf6dea82b16490c5`  
		Last Modified: Mon, 20 Apr 2020 17:59:14 GMT  
		Size: 2.3 MB (2334795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2501339994df2a02e290cfaf9a0733a1e6238cefcb91ea24a4bda9a81b1cabd1`  
		Last Modified: Mon, 20 Apr 2020 18:00:56 GMT  
		Size: 141.6 MB (141617030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d568aba8bed1e7e6d056d6be1821fd729cdaf8cfd5df2d2ea64b1058bcd561`  
		Last Modified: Mon, 20 Apr 2020 18:00:16 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec33d96b3abd299e8722b47482f55007e41f84a355f31ad7d1588d2c059cd386`  
		Last Modified: Mon, 20 Apr 2020 18:00:15 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90857e2d6a19668143ce6b82ee2cb2127d861f5a67f319cf0ade05a66bf8a092`  
		Last Modified: Mon, 20 Apr 2020 18:00:15 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc40725c0bc659e60797b94679d884f37e716a8358237c40c7d5ea89bd5f0e2`  
		Last Modified: Mon, 20 Apr 2020 18:00:16 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:11.0`

```console
$ docker pull odoo@sha256:08545371817e39f4414c3c2c9183e8eb494e983ab86ab8b0d6b1de25e13b3b4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:11.0` - linux; amd64

```console
$ docker pull odoo@sha256:4a4bfb161160462d8fb4a1139efcb2f0efd237db087734e94591d8a2b7ccf48e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386118334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1389f2233b6fe0ab1e25b40a0277e2de024c26159926179ec64661dbdb3940ba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:50 GMT
ADD file:40f52c233aecabf572a9db7450590d54d5e125fb00ecbb4a26fecd0b71e84eb8 in / 
# Thu, 16 Apr 2020 03:27:50 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 22:36:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Mon, 20 Apr 2020 17:50:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Mon, 20 Apr 2020 17:50:43 GMT
ENV LANG=C.UTF-8
# Mon, 20 Apr 2020 17:50:44 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Mon, 20 Apr 2020 17:53:49 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 20 Apr 2020 17:54:06 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:56:17 GMT
ENV ODOO_VERSION=11.0
# Mon, 20 Apr 2020 17:56:19 GMT
ARG ODOO_RELEASE=20200417
# Mon, 20 Apr 2020 17:56:19 GMT
ARG ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
# Mon, 20 Apr 2020 17:57:35 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb        && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Apr 2020 17:57:36 GMT
COPY file:cdc612ad49467417b0321c166f94e4f99b071755cb6ade071774e83d3b6ee4cb in / 
# Mon, 20 Apr 2020 17:57:37 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Apr 2020 17:57:39 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=e21c34a263785eea09babd7a0d876ba05c841935
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Apr 2020 17:57:39 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Apr 2020 17:57:40 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Apr 2020 17:57:40 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Apr 2020 17:57:41 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Apr 2020 17:57:41 GMT
USER odoo
# Mon, 20 Apr 2020 17:57:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Apr 2020 17:57:42 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:5e35bd43cf7898d036f8515be74d45b2e3abd2a5534fc280de63a9c22dd175bd`  
		Last Modified: Thu, 16 Apr 2020 03:35:04 GMT  
		Size: 22.5 MB (22513476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8268d7e205b4a86bdee4fc46423b4c949689fcc8a0c0399ea26a6ca29b50776`  
		Last Modified: Mon, 20 Apr 2020 17:59:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49716de29cf293e5ffc4698d23b76ea7c270249edcaaeb97e1fcd5fe041abdd`  
		Last Modified: Mon, 20 Apr 2020 17:59:53 GMT  
		Size: 219.7 MB (219650400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2023748d1ac8b71b990e34599defa253234c2af53880a5a8cf6dea82b16490c5`  
		Last Modified: Mon, 20 Apr 2020 17:59:14 GMT  
		Size: 2.3 MB (2334795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2501339994df2a02e290cfaf9a0733a1e6238cefcb91ea24a4bda9a81b1cabd1`  
		Last Modified: Mon, 20 Apr 2020 18:00:56 GMT  
		Size: 141.6 MB (141617030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d568aba8bed1e7e6d056d6be1821fd729cdaf8cfd5df2d2ea64b1058bcd561`  
		Last Modified: Mon, 20 Apr 2020 18:00:16 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec33d96b3abd299e8722b47482f55007e41f84a355f31ad7d1588d2c059cd386`  
		Last Modified: Mon, 20 Apr 2020 18:00:15 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90857e2d6a19668143ce6b82ee2cb2127d861f5a67f319cf0ade05a66bf8a092`  
		Last Modified: Mon, 20 Apr 2020 18:00:15 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc40725c0bc659e60797b94679d884f37e716a8358237c40c7d5ea89bd5f0e2`  
		Last Modified: Mon, 20 Apr 2020 18:00:16 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12`

```console
$ docker pull odoo@sha256:302befeb81d306839b6e75f35beac8875342efb7c30372f91c1f8917a5ee3ccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:a56a9f95512b7b48f8738cb42c1747e1eafe759c862c80df50ebbacb6a5222b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.8 MB (395844805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1056187d8b14bd07d6cc4078169b72803fd1fd9a32ebc181260a8e1d3613c4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:50 GMT
ADD file:40f52c233aecabf572a9db7450590d54d5e125fb00ecbb4a26fecd0b71e84eb8 in / 
# Thu, 16 Apr 2020 03:27:50 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 22:36:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Mon, 20 Apr 2020 17:50:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Mon, 20 Apr 2020 17:50:43 GMT
ENV LANG=C.UTF-8
# Mon, 20 Apr 2020 17:50:44 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Mon, 20 Apr 2020 17:53:49 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 20 Apr 2020 17:54:06 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:54:22 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:54:23 GMT
ENV ODOO_VERSION=12.0
# Mon, 20 Apr 2020 17:54:23 GMT
ARG ODOO_RELEASE=20200417
# Mon, 20 Apr 2020 17:54:23 GMT
ARG ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
# Mon, 20 Apr 2020 17:55:55 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Apr 2020 17:55:59 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Mon, 20 Apr 2020 17:55:59 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Apr 2020 17:56:03 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Apr 2020 17:56:03 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Apr 2020 17:56:03 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Apr 2020 17:56:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Apr 2020 17:56:05 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Apr 2020 17:56:05 GMT
USER odoo
# Mon, 20 Apr 2020 17:56:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Apr 2020 17:56:08 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:5e35bd43cf7898d036f8515be74d45b2e3abd2a5534fc280de63a9c22dd175bd`  
		Last Modified: Thu, 16 Apr 2020 03:35:04 GMT  
		Size: 22.5 MB (22513476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8268d7e205b4a86bdee4fc46423b4c949689fcc8a0c0399ea26a6ca29b50776`  
		Last Modified: Mon, 20 Apr 2020 17:59:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49716de29cf293e5ffc4698d23b76ea7c270249edcaaeb97e1fcd5fe041abdd`  
		Last Modified: Mon, 20 Apr 2020 17:59:53 GMT  
		Size: 219.7 MB (219650400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2023748d1ac8b71b990e34599defa253234c2af53880a5a8cf6dea82b16490c5`  
		Last Modified: Mon, 20 Apr 2020 17:59:14 GMT  
		Size: 2.3 MB (2334795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bd79206267ad34a26fef6f843304a7b34f36d8d8f9bca4e6adaf4fbe7ce985`  
		Last Modified: Mon, 20 Apr 2020 17:59:22 GMT  
		Size: 22.2 MB (22228542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4a9026f3e0707520b630c0dcdad3ac589f462bd5a70d3d95430da038f95cf`  
		Last Modified: Mon, 20 Apr 2020 18:00:05 GMT  
		Size: 129.1 MB (129114955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba843987b5aab900d01be4e04a1fcdc1684730c43930eb47122a2b0de299f792`  
		Last Modified: Mon, 20 Apr 2020 17:59:11 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdfd2a0de677bee54e6ff4761219790f11469e0f0c6454eb0c60b4bf5dfb70d`  
		Last Modified: Mon, 20 Apr 2020 17:59:11 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b786ee06054e6988970810164b5af9fecde0b5dcb89b0c6d5bed7533ccbc468e`  
		Last Modified: Mon, 20 Apr 2020 17:59:12 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fe1c8808ed7208dfc0c385b28dd9e9dc226ec5ba6b3b79268f52d38d6ffc35`  
		Last Modified: Mon, 20 Apr 2020 17:59:11 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:302befeb81d306839b6e75f35beac8875342efb7c30372f91c1f8917a5ee3ccb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:a56a9f95512b7b48f8738cb42c1747e1eafe759c862c80df50ebbacb6a5222b4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.8 MB (395844805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1056187d8b14bd07d6cc4078169b72803fd1fd9a32ebc181260a8e1d3613c4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:50 GMT
ADD file:40f52c233aecabf572a9db7450590d54d5e125fb00ecbb4a26fecd0b71e84eb8 in / 
# Thu, 16 Apr 2020 03:27:50 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 22:36:40 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Mon, 20 Apr 2020 17:50:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Mon, 20 Apr 2020 17:50:43 GMT
ENV LANG=C.UTF-8
# Mon, 20 Apr 2020 17:50:44 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Mon, 20 Apr 2020 17:53:49 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 20 Apr 2020 17:54:06 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:54:22 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:54:23 GMT
ENV ODOO_VERSION=12.0
# Mon, 20 Apr 2020 17:54:23 GMT
ARG ODOO_RELEASE=20200417
# Mon, 20 Apr 2020 17:54:23 GMT
ARG ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
# Mon, 20 Apr 2020 17:55:55 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Apr 2020 17:55:59 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Mon, 20 Apr 2020 17:55:59 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Apr 2020 17:56:03 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=ca4a7485b0b75850ffe1458a8f3266839400a501
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Apr 2020 17:56:03 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Apr 2020 17:56:03 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Apr 2020 17:56:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Apr 2020 17:56:05 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Apr 2020 17:56:05 GMT
USER odoo
# Mon, 20 Apr 2020 17:56:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Apr 2020 17:56:08 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:5e35bd43cf7898d036f8515be74d45b2e3abd2a5534fc280de63a9c22dd175bd`  
		Last Modified: Thu, 16 Apr 2020 03:35:04 GMT  
		Size: 22.5 MB (22513476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8268d7e205b4a86bdee4fc46423b4c949689fcc8a0c0399ea26a6ca29b50776`  
		Last Modified: Mon, 20 Apr 2020 17:59:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49716de29cf293e5ffc4698d23b76ea7c270249edcaaeb97e1fcd5fe041abdd`  
		Last Modified: Mon, 20 Apr 2020 17:59:53 GMT  
		Size: 219.7 MB (219650400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2023748d1ac8b71b990e34599defa253234c2af53880a5a8cf6dea82b16490c5`  
		Last Modified: Mon, 20 Apr 2020 17:59:14 GMT  
		Size: 2.3 MB (2334795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bd79206267ad34a26fef6f843304a7b34f36d8d8f9bca4e6adaf4fbe7ce985`  
		Last Modified: Mon, 20 Apr 2020 17:59:22 GMT  
		Size: 22.2 MB (22228542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e4a9026f3e0707520b630c0dcdad3ac589f462bd5a70d3d95430da038f95cf`  
		Last Modified: Mon, 20 Apr 2020 18:00:05 GMT  
		Size: 129.1 MB (129114955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba843987b5aab900d01be4e04a1fcdc1684730c43930eb47122a2b0de299f792`  
		Last Modified: Mon, 20 Apr 2020 17:59:11 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdfd2a0de677bee54e6ff4761219790f11469e0f0c6454eb0c60b4bf5dfb70d`  
		Last Modified: Mon, 20 Apr 2020 17:59:11 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b786ee06054e6988970810164b5af9fecde0b5dcb89b0c6d5bed7533ccbc468e`  
		Last Modified: Mon, 20 Apr 2020 17:59:12 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fe1c8808ed7208dfc0c385b28dd9e9dc226ec5ba6b3b79268f52d38d6ffc35`  
		Last Modified: Mon, 20 Apr 2020 17:59:11 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:9cba2271d9651cb56e0ec207b1048a46b9736bd0fb743cb1336b4e5280dedb3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:26cc1a277eb50216550a82ff63cbed9771f0b123517617e533adddfda3e7b0a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.7 MB (377678377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a7dc023cb2bb62f38d6e579f18a6b347bb92ee1fa9662c3d9649dddbec8c88a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 22:33:23 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Mon, 20 Apr 2020 17:45:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Mon, 20 Apr 2020 17:45:54 GMT
ENV LANG=C.UTF-8
# Mon, 20 Apr 2020 17:47:54 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 20 Apr 2020 17:48:09 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:48:17 GMT
RUN npm install -g rtlcss
# Mon, 20 Apr 2020 17:48:18 GMT
ENV ODOO_VERSION=13.0
# Mon, 20 Apr 2020 17:48:21 GMT
ARG ODOO_RELEASE=20200417
# Mon, 20 Apr 2020 17:48:21 GMT
ARG ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
# Mon, 20 Apr 2020 17:50:11 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Apr 2020 17:50:16 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Mon, 20 Apr 2020 17:50:19 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Apr 2020 17:50:20 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Apr 2020 17:50:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Apr 2020 17:50:24 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Apr 2020 17:50:25 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Apr 2020 17:50:25 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Apr 2020 17:50:26 GMT
USER odoo
# Mon, 20 Apr 2020 17:50:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Apr 2020 17:50:27 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcb4bdf7e0fe8348ee1014f1353f95a613492dac6269ceca3a112295aa81c36`  
		Last Modified: Mon, 20 Apr 2020 17:58:35 GMT  
		Size: 203.6 MB (203560448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4373fc38d31dd8279e5dd622cae1cfee03b80f7b135f13cae7a4b6c199f30af9`  
		Last Modified: Mon, 20 Apr 2020 17:57:55 GMT  
		Size: 2.3 MB (2332582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7236448956884cff5f6ec5839c6ec8837e3f40099cf67cb0fd4102d83bbe756`  
		Last Modified: Mon, 20 Apr 2020 17:57:55 GMT  
		Size: 1.1 MB (1090230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e592c7d7ac294970e7658c0cab94468b6e5a066b99b877c8cfaa2fd98a58d0b9`  
		Last Modified: Mon, 20 Apr 2020 17:58:47 GMT  
		Size: 143.6 MB (143594562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a858abeb99315f6e442ce612d73c8b544a93d02bc5abcd877fcb3bfc0e7906`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db77bb1d9e0fc65ee5e5540078c5189e96ffe2f53ee2b5b14da5eb8c138a32b`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f838d0ef6c581b88262effbf48cbcd9f9e105f446e57e3de14b356d9ce7a5a1c`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546dfaf653d22c8d72a67262391df6a9daeb9883e9a403ef6173bd1382b8f428`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:9cba2271d9651cb56e0ec207b1048a46b9736bd0fb743cb1336b4e5280dedb3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:26cc1a277eb50216550a82ff63cbed9771f0b123517617e533adddfda3e7b0a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.7 MB (377678377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a7dc023cb2bb62f38d6e579f18a6b347bb92ee1fa9662c3d9649dddbec8c88a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 22:33:23 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Mon, 20 Apr 2020 17:45:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Mon, 20 Apr 2020 17:45:54 GMT
ENV LANG=C.UTF-8
# Mon, 20 Apr 2020 17:47:54 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 20 Apr 2020 17:48:09 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:48:17 GMT
RUN npm install -g rtlcss
# Mon, 20 Apr 2020 17:48:18 GMT
ENV ODOO_VERSION=13.0
# Mon, 20 Apr 2020 17:48:21 GMT
ARG ODOO_RELEASE=20200417
# Mon, 20 Apr 2020 17:48:21 GMT
ARG ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
# Mon, 20 Apr 2020 17:50:11 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Apr 2020 17:50:16 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Mon, 20 Apr 2020 17:50:19 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Apr 2020 17:50:20 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Apr 2020 17:50:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Apr 2020 17:50:24 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Apr 2020 17:50:25 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Apr 2020 17:50:25 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Apr 2020 17:50:26 GMT
USER odoo
# Mon, 20 Apr 2020 17:50:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Apr 2020 17:50:27 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcb4bdf7e0fe8348ee1014f1353f95a613492dac6269ceca3a112295aa81c36`  
		Last Modified: Mon, 20 Apr 2020 17:58:35 GMT  
		Size: 203.6 MB (203560448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4373fc38d31dd8279e5dd622cae1cfee03b80f7b135f13cae7a4b6c199f30af9`  
		Last Modified: Mon, 20 Apr 2020 17:57:55 GMT  
		Size: 2.3 MB (2332582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7236448956884cff5f6ec5839c6ec8837e3f40099cf67cb0fd4102d83bbe756`  
		Last Modified: Mon, 20 Apr 2020 17:57:55 GMT  
		Size: 1.1 MB (1090230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e592c7d7ac294970e7658c0cab94468b6e5a066b99b877c8cfaa2fd98a58d0b9`  
		Last Modified: Mon, 20 Apr 2020 17:58:47 GMT  
		Size: 143.6 MB (143594562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a858abeb99315f6e442ce612d73c8b544a93d02bc5abcd877fcb3bfc0e7906`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db77bb1d9e0fc65ee5e5540078c5189e96ffe2f53ee2b5b14da5eb8c138a32b`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f838d0ef6c581b88262effbf48cbcd9f9e105f446e57e3de14b356d9ce7a5a1c`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546dfaf653d22c8d72a67262391df6a9daeb9883e9a403ef6173bd1382b8f428`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:9cba2271d9651cb56e0ec207b1048a46b9736bd0fb743cb1336b4e5280dedb3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:26cc1a277eb50216550a82ff63cbed9771f0b123517617e533adddfda3e7b0a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.7 MB (377678377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a7dc023cb2bb62f38d6e579f18a6b347bb92ee1fa9662c3d9649dddbec8c88a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 22:33:23 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Mon, 20 Apr 2020 17:45:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Mon, 20 Apr 2020 17:45:54 GMT
ENV LANG=C.UTF-8
# Mon, 20 Apr 2020 17:47:54 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 20 Apr 2020 17:48:09 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Mon, 20 Apr 2020 17:48:17 GMT
RUN npm install -g rtlcss
# Mon, 20 Apr 2020 17:48:18 GMT
ENV ODOO_VERSION=13.0
# Mon, 20 Apr 2020 17:48:21 GMT
ARG ODOO_RELEASE=20200417
# Mon, 20 Apr 2020 17:48:21 GMT
ARG ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
# Mon, 20 Apr 2020 17:50:11 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 20 Apr 2020 17:50:16 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Mon, 20 Apr 2020 17:50:19 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 20 Apr 2020 17:50:20 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 20 Apr 2020 17:50:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 20 Apr 2020 17:50:24 GMT
EXPOSE 8069 8071 8072
# Mon, 20 Apr 2020 17:50:25 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 20 Apr 2020 17:50:25 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 20 Apr 2020 17:50:26 GMT
USER odoo
# Mon, 20 Apr 2020 17:50:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Apr 2020 17:50:27 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcb4bdf7e0fe8348ee1014f1353f95a613492dac6269ceca3a112295aa81c36`  
		Last Modified: Mon, 20 Apr 2020 17:58:35 GMT  
		Size: 203.6 MB (203560448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4373fc38d31dd8279e5dd622cae1cfee03b80f7b135f13cae7a4b6c199f30af9`  
		Last Modified: Mon, 20 Apr 2020 17:57:55 GMT  
		Size: 2.3 MB (2332582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7236448956884cff5f6ec5839c6ec8837e3f40099cf67cb0fd4102d83bbe756`  
		Last Modified: Mon, 20 Apr 2020 17:57:55 GMT  
		Size: 1.1 MB (1090230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e592c7d7ac294970e7658c0cab94468b6e5a066b99b877c8cfaa2fd98a58d0b9`  
		Last Modified: Mon, 20 Apr 2020 17:58:47 GMT  
		Size: 143.6 MB (143594562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a858abeb99315f6e442ce612d73c8b544a93d02bc5abcd877fcb3bfc0e7906`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db77bb1d9e0fc65ee5e5540078c5189e96ffe2f53ee2b5b14da5eb8c138a32b`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f838d0ef6c581b88262effbf48cbcd9f9e105f446e57e3de14b356d9ce7a5a1c`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546dfaf653d22c8d72a67262391df6a9daeb9883e9a403ef6173bd1382b8f428`  
		Last Modified: Mon, 20 Apr 2020 17:57:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
