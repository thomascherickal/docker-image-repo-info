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
$ docker pull odoo@sha256:a114dab2efd2f24194958e0de50afebb95d530392a951019c506f454745eb112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:11` - linux; amd64

```console
$ docker pull odoo@sha256:056620c5060e87e06bb2c6809c1e2e09a118a3739df8af1f9bc2d69981d46ec3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385941787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9312c97536320863d6e79f914d8ad37fb15b8f0c5003a2e499127015448b215`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:50:04 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Feb 2020 11:50:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 11:50:06 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 26 Feb 2020 11:52:58 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Feb 2020 11:53:13 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:54:49 GMT
ENV ODOO_VERSION=11.0
# Wed, 26 Feb 2020 11:54:50 GMT
ARG ODOO_RELEASE=20200121
# Wed, 26 Feb 2020 11:54:50 GMT
ARG ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
# Wed, 26 Feb 2020 11:55:41 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 26 Feb 2020 11:55:43 GMT
COPY file:cdc612ad49467417b0321c166f94e4f99b071755cb6ade071774e83d3b6ee4cb in / 
# Wed, 26 Feb 2020 11:55:43 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 26 Feb 2020 11:55:44 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 26 Feb 2020 11:55:44 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 26 Feb 2020 11:55:44 GMT
EXPOSE 8069 8071
# Wed, 26 Feb 2020 11:55:44 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 26 Feb 2020 11:55:44 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 26 Feb 2020 11:55:45 GMT
USER odoo
# Wed, 26 Feb 2020 11:55:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 11:55:45 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78c4af8acbddd5d359e0c129ec40ccfe8bc37428fcda883968c8b58971bc310`  
		Last Modified: Wed, 26 Feb 2020 11:56:49 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5dd0fe2807848725c0a11ec9ff26c4e338007ba55f5b7277aaf7df33165548`  
		Last Modified: Wed, 26 Feb 2020 11:57:23 GMT  
		Size: 219.7 MB (219650402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb36e7e760103c8a1d36f57d24809105ae6d421e44e218890ed502660abd7570`  
		Last Modified: Wed, 26 Feb 2020 11:56:50 GMT  
		Size: 2.3 MB (2346347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0e942a05f6e9e8aa2e1becfed9f9f1b85aa98533ca84d8805633b42261ba2c`  
		Last Modified: Wed, 26 Feb 2020 11:57:56 GMT  
		Size: 141.4 MB (141429043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588c48495ce84d909c22713eaeba11a66a0e16e3612caaa35fe0b16ff80668dd`  
		Last Modified: Wed, 26 Feb 2020 11:57:28 GMT  
		Size: 674.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc829b14ccdc4836074475c3ace359109913feaaa23fb626cb3bdebbeb5463db`  
		Last Modified: Wed, 26 Feb 2020 11:57:28 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecededdb8afea8a2a5c4f50b98630f909f73c7c55472c85ccc3e4eb39395b88d`  
		Last Modified: Wed, 26 Feb 2020 11:57:28 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea5ade042a5a0f02e6398c3df19509748205374b1cf1734b4aa76ddc0864cd2`  
		Last Modified: Wed, 26 Feb 2020 11:57:28 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:11.0`

```console
$ docker pull odoo@sha256:a114dab2efd2f24194958e0de50afebb95d530392a951019c506f454745eb112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:11.0` - linux; amd64

```console
$ docker pull odoo@sha256:056620c5060e87e06bb2c6809c1e2e09a118a3739df8af1f9bc2d69981d46ec3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385941787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9312c97536320863d6e79f914d8ad37fb15b8f0c5003a2e499127015448b215`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:50:04 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Feb 2020 11:50:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 11:50:06 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 26 Feb 2020 11:52:58 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Feb 2020 11:53:13 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:54:49 GMT
ENV ODOO_VERSION=11.0
# Wed, 26 Feb 2020 11:54:50 GMT
ARG ODOO_RELEASE=20200121
# Wed, 26 Feb 2020 11:54:50 GMT
ARG ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
# Wed, 26 Feb 2020 11:55:41 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 26 Feb 2020 11:55:43 GMT
COPY file:cdc612ad49467417b0321c166f94e4f99b071755cb6ade071774e83d3b6ee4cb in / 
# Wed, 26 Feb 2020 11:55:43 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 26 Feb 2020 11:55:44 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=13f30434cb4fb28b11d78fd4e7c616d03362f779
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 26 Feb 2020 11:55:44 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 26 Feb 2020 11:55:44 GMT
EXPOSE 8069 8071
# Wed, 26 Feb 2020 11:55:44 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 26 Feb 2020 11:55:44 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 26 Feb 2020 11:55:45 GMT
USER odoo
# Wed, 26 Feb 2020 11:55:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 11:55:45 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78c4af8acbddd5d359e0c129ec40ccfe8bc37428fcda883968c8b58971bc310`  
		Last Modified: Wed, 26 Feb 2020 11:56:49 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5dd0fe2807848725c0a11ec9ff26c4e338007ba55f5b7277aaf7df33165548`  
		Last Modified: Wed, 26 Feb 2020 11:57:23 GMT  
		Size: 219.7 MB (219650402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb36e7e760103c8a1d36f57d24809105ae6d421e44e218890ed502660abd7570`  
		Last Modified: Wed, 26 Feb 2020 11:56:50 GMT  
		Size: 2.3 MB (2346347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0e942a05f6e9e8aa2e1becfed9f9f1b85aa98533ca84d8805633b42261ba2c`  
		Last Modified: Wed, 26 Feb 2020 11:57:56 GMT  
		Size: 141.4 MB (141429043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588c48495ce84d909c22713eaeba11a66a0e16e3612caaa35fe0b16ff80668dd`  
		Last Modified: Wed, 26 Feb 2020 11:57:28 GMT  
		Size: 674.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc829b14ccdc4836074475c3ace359109913feaaa23fb626cb3bdebbeb5463db`  
		Last Modified: Wed, 26 Feb 2020 11:57:28 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecededdb8afea8a2a5c4f50b98630f909f73c7c55472c85ccc3e4eb39395b88d`  
		Last Modified: Wed, 26 Feb 2020 11:57:28 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea5ade042a5a0f02e6398c3df19509748205374b1cf1734b4aa76ddc0864cd2`  
		Last Modified: Wed, 26 Feb 2020 11:57:28 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12`

```console
$ docker pull odoo@sha256:ee1ebe74dfb1ca27dd73f88c5afafe86be52b5eeb2731c16153fe4b005fe94cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:755b20cf8794df72871dddf9d32af376bc47238ade12577467667d29bf9ae2e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.9 MB (399876090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71e0dcc27c109cb59b941531f057a575d3fe986177b9a7e12a6f672a38a59fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:50:04 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Feb 2020 11:50:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 11:50:06 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 26 Feb 2020 11:52:58 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Feb 2020 11:53:13 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:53:35 GMT
RUN set -x;    echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && export GNUPGHOME="$(mktemp -d)"     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:53:35 GMT
ENV ODOO_VERSION=12.0
# Wed, 26 Feb 2020 11:53:36 GMT
ARG ODOO_RELEASE=20200121
# Wed, 26 Feb 2020 11:53:36 GMT
ARG ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
# Wed, 26 Feb 2020 11:54:32 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 26 Feb 2020 11:54:33 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 26 Feb 2020 11:54:33 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 26 Feb 2020 11:54:34 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 26 Feb 2020 11:54:34 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 26 Feb 2020 11:54:34 GMT
EXPOSE 8069 8071
# Wed, 26 Feb 2020 11:54:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 26 Feb 2020 11:54:35 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 26 Feb 2020 11:54:35 GMT
USER odoo
# Wed, 26 Feb 2020 11:54:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 11:54:35 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78c4af8acbddd5d359e0c129ec40ccfe8bc37428fcda883968c8b58971bc310`  
		Last Modified: Wed, 26 Feb 2020 11:56:49 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5dd0fe2807848725c0a11ec9ff26c4e338007ba55f5b7277aaf7df33165548`  
		Last Modified: Wed, 26 Feb 2020 11:57:23 GMT  
		Size: 219.7 MB (219650402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb36e7e760103c8a1d36f57d24809105ae6d421e44e218890ed502660abd7570`  
		Last Modified: Wed, 26 Feb 2020 11:56:50 GMT  
		Size: 2.3 MB (2346347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fc0110971cb28d05f0f1fc8f852c52a7ca806b1f3c1688979a91ef997c03a5`  
		Last Modified: Wed, 26 Feb 2020 11:56:58 GMT  
		Size: 26.6 MB (26566008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5994e5dd377dd7be708dcf4a0de2bb5c6fc4b7b4b78c96627ba588e3a5fa241`  
		Last Modified: Wed, 26 Feb 2020 11:57:22 GMT  
		Size: 128.8 MB (128797337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825f7550156112daebec168dc7f4a2e6b8b68e7a074d641982dd15cc39ea587a`  
		Last Modified: Wed, 26 Feb 2020 11:56:48 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fe1cc441a0f78d23611ab6800ce59bc410ce36c45539db9c6895097027939b`  
		Last Modified: Wed, 26 Feb 2020 11:56:48 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d562381983fca50ec0a250c0af234aabaf06eace18ef8b3250ac45bf2d7df82b`  
		Last Modified: Wed, 26 Feb 2020 11:56:48 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2cc4e4dc305aa948d15d53da5bb52703c1807397248a5dfe59041e38b0a65b`  
		Last Modified: Wed, 26 Feb 2020 11:56:48 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:ee1ebe74dfb1ca27dd73f88c5afafe86be52b5eeb2731c16153fe4b005fe94cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:755b20cf8794df72871dddf9d32af376bc47238ade12577467667d29bf9ae2e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.9 MB (399876090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a71e0dcc27c109cb59b941531f057a575d3fe986177b9a7e12a6f672a38a59fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:50:04 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Feb 2020 11:50:05 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 11:50:06 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 26 Feb 2020 11:52:58 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Feb 2020 11:53:13 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:53:35 GMT
RUN set -x;    echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && export GNUPGHOME="$(mktemp -d)"     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:53:35 GMT
ENV ODOO_VERSION=12.0
# Wed, 26 Feb 2020 11:53:36 GMT
ARG ODOO_RELEASE=20200121
# Wed, 26 Feb 2020 11:53:36 GMT
ARG ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
# Wed, 26 Feb 2020 11:54:32 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 26 Feb 2020 11:54:33 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 26 Feb 2020 11:54:33 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 26 Feb 2020 11:54:34 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=cb0bcb5d239983468c2e3b3f7cf17f58df820b1c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 26 Feb 2020 11:54:34 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 26 Feb 2020 11:54:34 GMT
EXPOSE 8069 8071
# Wed, 26 Feb 2020 11:54:34 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 26 Feb 2020 11:54:35 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 26 Feb 2020 11:54:35 GMT
USER odoo
# Wed, 26 Feb 2020 11:54:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 11:54:35 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78c4af8acbddd5d359e0c129ec40ccfe8bc37428fcda883968c8b58971bc310`  
		Last Modified: Wed, 26 Feb 2020 11:56:49 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5dd0fe2807848725c0a11ec9ff26c4e338007ba55f5b7277aaf7df33165548`  
		Last Modified: Wed, 26 Feb 2020 11:57:23 GMT  
		Size: 219.7 MB (219650402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb36e7e760103c8a1d36f57d24809105ae6d421e44e218890ed502660abd7570`  
		Last Modified: Wed, 26 Feb 2020 11:56:50 GMT  
		Size: 2.3 MB (2346347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fc0110971cb28d05f0f1fc8f852c52a7ca806b1f3c1688979a91ef997c03a5`  
		Last Modified: Wed, 26 Feb 2020 11:56:58 GMT  
		Size: 26.6 MB (26566008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5994e5dd377dd7be708dcf4a0de2bb5c6fc4b7b4b78c96627ba588e3a5fa241`  
		Last Modified: Wed, 26 Feb 2020 11:57:22 GMT  
		Size: 128.8 MB (128797337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825f7550156112daebec168dc7f4a2e6b8b68e7a074d641982dd15cc39ea587a`  
		Last Modified: Wed, 26 Feb 2020 11:56:48 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fe1cc441a0f78d23611ab6800ce59bc410ce36c45539db9c6895097027939b`  
		Last Modified: Wed, 26 Feb 2020 11:56:48 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d562381983fca50ec0a250c0af234aabaf06eace18ef8b3250ac45bf2d7df82b`  
		Last Modified: Wed, 26 Feb 2020 11:56:48 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2cc4e4dc305aa948d15d53da5bb52703c1807397248a5dfe59041e38b0a65b`  
		Last Modified: Wed, 26 Feb 2020 11:56:48 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:d4960fde390072f14b197f45775770b7cafc43d3afea60882766ce7d2004aa00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:6f63cbf4d2aff5fd4dadc8532d1aeec8855f72f0733e7a1ea3d9a4d54f134b12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.4 MB (376386122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de33ddfad71fb4a96b94931e9a237b66e68f2456854011db98999f44ea5a8731`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:46:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Feb 2020 11:46:48 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 11:48:05 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Feb 2020 11:48:18 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:48:25 GMT
RUN set -x;     npm install -g rtlcss
# Wed, 26 Feb 2020 11:48:25 GMT
ENV ODOO_VERSION=13.0
# Wed, 26 Feb 2020 11:48:25 GMT
ARG ODOO_RELEASE=20200121
# Wed, 26 Feb 2020 11:48:26 GMT
ARG ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
# Wed, 26 Feb 2020 11:49:48 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 26 Feb 2020 11:49:50 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 26 Feb 2020 11:49:50 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 26 Feb 2020 11:49:51 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 26 Feb 2020 11:49:51 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 26 Feb 2020 11:49:51 GMT
EXPOSE 8069 8071
# Wed, 26 Feb 2020 11:49:51 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 26 Feb 2020 11:49:51 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 26 Feb 2020 11:49:52 GMT
USER odoo
# Wed, 26 Feb 2020 11:49:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 11:49:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48753109c62917fdcbb60e49017f827aadd9db2aafc74641cca81ab7c1e98e3`  
		Last Modified: Wed, 26 Feb 2020 11:56:39 GMT  
		Size: 203.6 MB (203558059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a384f9e9149f8a0838e04217c4368771d4672a0eeb966324183ca0d44cde7163`  
		Last Modified: Wed, 26 Feb 2020 11:55:59 GMT  
		Size: 2.3 MB (2332407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d11f83d09d07bc5cab163d63ee721c0256c800cc5f75b9453581a8649b17a5`  
		Last Modified: Wed, 26 Feb 2020 11:55:59 GMT  
		Size: 1.1 MB (1076580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c916f95d325b2b6de54d687822dafd94df1f20682565b2846099ff00692eff7e`  
		Last Modified: Wed, 26 Feb 2020 11:56:33 GMT  
		Size: 142.3 MB (142324858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26cd439482bfeb213dbcbe102be68f9572c8b7428f35952af8a25f775b09b46`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71d823cb2f5a3775f9d4f4abe804d2b91c46359eda93a0dad08ebd94a34d728`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cbedafc91c1846b9b86bf5a071f5bf8bbe5cbb3540c9537aab2bb9dba9b246`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0757eb646574bd972f7eccbebf8e69d80ed4e334de00cd1dc21df1e8ef2d2c8c`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:d4960fde390072f14b197f45775770b7cafc43d3afea60882766ce7d2004aa00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:6f63cbf4d2aff5fd4dadc8532d1aeec8855f72f0733e7a1ea3d9a4d54f134b12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.4 MB (376386122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de33ddfad71fb4a96b94931e9a237b66e68f2456854011db98999f44ea5a8731`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:46:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Feb 2020 11:46:48 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 11:48:05 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Feb 2020 11:48:18 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:48:25 GMT
RUN set -x;     npm install -g rtlcss
# Wed, 26 Feb 2020 11:48:25 GMT
ENV ODOO_VERSION=13.0
# Wed, 26 Feb 2020 11:48:25 GMT
ARG ODOO_RELEASE=20200121
# Wed, 26 Feb 2020 11:48:26 GMT
ARG ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
# Wed, 26 Feb 2020 11:49:48 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 26 Feb 2020 11:49:50 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 26 Feb 2020 11:49:50 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 26 Feb 2020 11:49:51 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 26 Feb 2020 11:49:51 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 26 Feb 2020 11:49:51 GMT
EXPOSE 8069 8071
# Wed, 26 Feb 2020 11:49:51 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 26 Feb 2020 11:49:51 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 26 Feb 2020 11:49:52 GMT
USER odoo
# Wed, 26 Feb 2020 11:49:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 11:49:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48753109c62917fdcbb60e49017f827aadd9db2aafc74641cca81ab7c1e98e3`  
		Last Modified: Wed, 26 Feb 2020 11:56:39 GMT  
		Size: 203.6 MB (203558059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a384f9e9149f8a0838e04217c4368771d4672a0eeb966324183ca0d44cde7163`  
		Last Modified: Wed, 26 Feb 2020 11:55:59 GMT  
		Size: 2.3 MB (2332407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d11f83d09d07bc5cab163d63ee721c0256c800cc5f75b9453581a8649b17a5`  
		Last Modified: Wed, 26 Feb 2020 11:55:59 GMT  
		Size: 1.1 MB (1076580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c916f95d325b2b6de54d687822dafd94df1f20682565b2846099ff00692eff7e`  
		Last Modified: Wed, 26 Feb 2020 11:56:33 GMT  
		Size: 142.3 MB (142324858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26cd439482bfeb213dbcbe102be68f9572c8b7428f35952af8a25f775b09b46`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71d823cb2f5a3775f9d4f4abe804d2b91c46359eda93a0dad08ebd94a34d728`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cbedafc91c1846b9b86bf5a071f5bf8bbe5cbb3540c9537aab2bb9dba9b246`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0757eb646574bd972f7eccbebf8e69d80ed4e334de00cd1dc21df1e8ef2d2c8c`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:d4960fde390072f14b197f45775770b7cafc43d3afea60882766ce7d2004aa00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:6f63cbf4d2aff5fd4dadc8532d1aeec8855f72f0733e7a1ea3d9a4d54f134b12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.4 MB (376386122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de33ddfad71fb4a96b94931e9a237b66e68f2456854011db98999f44ea5a8731`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:46:48 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 26 Feb 2020 11:46:48 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 11:48:05 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 26 Feb 2020 11:48:18 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:48:25 GMT
RUN set -x;     npm install -g rtlcss
# Wed, 26 Feb 2020 11:48:25 GMT
ENV ODOO_VERSION=13.0
# Wed, 26 Feb 2020 11:48:25 GMT
ARG ODOO_RELEASE=20200121
# Wed, 26 Feb 2020 11:48:26 GMT
ARG ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
# Wed, 26 Feb 2020 11:49:48 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 26 Feb 2020 11:49:50 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 26 Feb 2020 11:49:50 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 26 Feb 2020 11:49:51 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 26 Feb 2020 11:49:51 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 26 Feb 2020 11:49:51 GMT
EXPOSE 8069 8071
# Wed, 26 Feb 2020 11:49:51 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 26 Feb 2020 11:49:51 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 26 Feb 2020 11:49:52 GMT
USER odoo
# Wed, 26 Feb 2020 11:49:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 11:49:52 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48753109c62917fdcbb60e49017f827aadd9db2aafc74641cca81ab7c1e98e3`  
		Last Modified: Wed, 26 Feb 2020 11:56:39 GMT  
		Size: 203.6 MB (203558059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a384f9e9149f8a0838e04217c4368771d4672a0eeb966324183ca0d44cde7163`  
		Last Modified: Wed, 26 Feb 2020 11:55:59 GMT  
		Size: 2.3 MB (2332407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d11f83d09d07bc5cab163d63ee721c0256c800cc5f75b9453581a8649b17a5`  
		Last Modified: Wed, 26 Feb 2020 11:55:59 GMT  
		Size: 1.1 MB (1076580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c916f95d325b2b6de54d687822dafd94df1f20682565b2846099ff00692eff7e`  
		Last Modified: Wed, 26 Feb 2020 11:56:33 GMT  
		Size: 142.3 MB (142324858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26cd439482bfeb213dbcbe102be68f9572c8b7428f35952af8a25f775b09b46`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71d823cb2f5a3775f9d4f4abe804d2b91c46359eda93a0dad08ebd94a34d728`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cbedafc91c1846b9b86bf5a071f5bf8bbe5cbb3540c9537aab2bb9dba9b246`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0757eb646574bd972f7eccbebf8e69d80ed4e334de00cd1dc21df1e8ef2d2c8c`  
		Last Modified: Wed, 26 Feb 2020 11:55:57 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
