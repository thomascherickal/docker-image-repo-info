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
$ docker pull odoo@sha256:a1a0de46952de7ebb02934f8de177dafa41158485f118eb074e77f8523a8f4d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:11` - linux; amd64

```console
$ docker pull odoo@sha256:32a49004cc8818f2079d87d269f68cb852d0acf1da2d931aa8af26227359af42
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386142892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62d2bacdc9d1d37a1363cbae06dd369d34ddba652af2cf8728dc3f363056b3b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:32:37 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Aug 2020 00:32:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Aug 2020 00:32:38 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:32:39 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 05 Aug 2020 00:34:16 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Aug 2020 00:34:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:36:25 GMT
ENV ODOO_VERSION=11.0
# Wed, 05 Aug 2020 00:36:25 GMT
ARG ODOO_RELEASE=20200629
# Wed, 05 Aug 2020 00:36:26 GMT
ARG ODOO_SHA=3c9c5bb32d7d878b246624a4dfc233080a2b5888
# Wed, 05 Aug 2020 00:37:08 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=3c9c5bb32d7d878b246624a4dfc233080a2b5888
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb        && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 05 Aug 2020 00:37:09 GMT
COPY file:cdc612ad49467417b0321c166f94e4f99b071755cb6ade071774e83d3b6ee4cb in / 
# Wed, 05 Aug 2020 00:37:09 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 05 Aug 2020 00:37:10 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=3c9c5bb32d7d878b246624a4dfc233080a2b5888
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 05 Aug 2020 00:37:10 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 05 Aug 2020 00:37:10 GMT
EXPOSE 8069 8071 8072
# Wed, 05 Aug 2020 00:37:10 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 05 Aug 2020 00:37:11 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 05 Aug 2020 00:37:11 GMT
USER odoo
# Wed, 05 Aug 2020 00:37:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Aug 2020 00:37:11 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad5c506d50e1dbcc214e3afec29f06e82b7ab2fbfdaa83b7dbe492de47ea5b2`  
		Last Modified: Wed, 05 Aug 2020 00:38:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d430b9279d73c5bcf9ccf812287316870750b3e4e81298ba96b22b66cac9dc7d`  
		Last Modified: Wed, 05 Aug 2020 00:38:36 GMT  
		Size: 219.6 MB (219609743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc34cd5c920e05f814ee9bb94e8cb32c206e1a643d3def70a9a36e63174b3f11`  
		Last Modified: Wed, 05 Aug 2020 00:38:06 GMT  
		Size: 2.3 MB (2336276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce64a2a59a6f4bae6d754d61da5660d827df96e8f66294b17b2caa7c304e3a82`  
		Last Modified: Wed, 05 Aug 2020 00:39:38 GMT  
		Size: 141.7 MB (141671965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1263f1049e0a96df900065b56933038c203d183239e5e6fc77ae3e9789f4d9`  
		Last Modified: Wed, 05 Aug 2020 00:38:40 GMT  
		Size: 674.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af148bb412c1c7189a5a6b8aab64d7e2a4cdc18064974af0e8daf06b06a4f4`  
		Last Modified: Wed, 05 Aug 2020 00:38:40 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a416e47edea3b8e42ef37ba245990229959d5efccc9e3da4313747fbfebcc0`  
		Last Modified: Wed, 05 Aug 2020 00:38:40 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d34330c98b3e22f874d0c32fbc3d597affba42ea0971c85f4f88906c476282`  
		Last Modified: Wed, 05 Aug 2020 00:38:41 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:11.0`

```console
$ docker pull odoo@sha256:a1a0de46952de7ebb02934f8de177dafa41158485f118eb074e77f8523a8f4d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:11.0` - linux; amd64

```console
$ docker pull odoo@sha256:32a49004cc8818f2079d87d269f68cb852d0acf1da2d931aa8af26227359af42
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386142892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62d2bacdc9d1d37a1363cbae06dd369d34ddba652af2cf8728dc3f363056b3b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:32:37 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Aug 2020 00:32:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Aug 2020 00:32:38 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:32:39 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 05 Aug 2020 00:34:16 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Aug 2020 00:34:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:36:25 GMT
ENV ODOO_VERSION=11.0
# Wed, 05 Aug 2020 00:36:25 GMT
ARG ODOO_RELEASE=20200629
# Wed, 05 Aug 2020 00:36:26 GMT
ARG ODOO_SHA=3c9c5bb32d7d878b246624a4dfc233080a2b5888
# Wed, 05 Aug 2020 00:37:08 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=3c9c5bb32d7d878b246624a4dfc233080a2b5888
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb        && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 05 Aug 2020 00:37:09 GMT
COPY file:cdc612ad49467417b0321c166f94e4f99b071755cb6ade071774e83d3b6ee4cb in / 
# Wed, 05 Aug 2020 00:37:09 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 05 Aug 2020 00:37:10 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=3c9c5bb32d7d878b246624a4dfc233080a2b5888
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 05 Aug 2020 00:37:10 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 05 Aug 2020 00:37:10 GMT
EXPOSE 8069 8071 8072
# Wed, 05 Aug 2020 00:37:10 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 05 Aug 2020 00:37:11 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 05 Aug 2020 00:37:11 GMT
USER odoo
# Wed, 05 Aug 2020 00:37:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Aug 2020 00:37:11 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad5c506d50e1dbcc214e3afec29f06e82b7ab2fbfdaa83b7dbe492de47ea5b2`  
		Last Modified: Wed, 05 Aug 2020 00:38:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d430b9279d73c5bcf9ccf812287316870750b3e4e81298ba96b22b66cac9dc7d`  
		Last Modified: Wed, 05 Aug 2020 00:38:36 GMT  
		Size: 219.6 MB (219609743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc34cd5c920e05f814ee9bb94e8cb32c206e1a643d3def70a9a36e63174b3f11`  
		Last Modified: Wed, 05 Aug 2020 00:38:06 GMT  
		Size: 2.3 MB (2336276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce64a2a59a6f4bae6d754d61da5660d827df96e8f66294b17b2caa7c304e3a82`  
		Last Modified: Wed, 05 Aug 2020 00:39:38 GMT  
		Size: 141.7 MB (141671965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1263f1049e0a96df900065b56933038c203d183239e5e6fc77ae3e9789f4d9`  
		Last Modified: Wed, 05 Aug 2020 00:38:40 GMT  
		Size: 674.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1af148bb412c1c7189a5a6b8aab64d7e2a4cdc18064974af0e8daf06b06a4f4`  
		Last Modified: Wed, 05 Aug 2020 00:38:40 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a416e47edea3b8e42ef37ba245990229959d5efccc9e3da4313747fbfebcc0`  
		Last Modified: Wed, 05 Aug 2020 00:38:40 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d34330c98b3e22f874d0c32fbc3d597affba42ea0971c85f4f88906c476282`  
		Last Modified: Wed, 05 Aug 2020 00:38:41 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12`

```console
$ docker pull odoo@sha256:25e9dcf77f4223abf444b5c1f033dc033ccde7287c0ad75890ef7d51bd4739d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12` - linux; amd64

```console
$ docker pull odoo@sha256:a59ca51e209bd079d0f5bb61cdb5a7a12c6d59da765adaec50fcf3d7e5e707ce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396144370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29da3adecc88cd9cbc33978b03715d41a34ad41be2d9432f59a8ba6d619b9b83`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:32:37 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Aug 2020 00:32:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Aug 2020 00:32:38 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:32:39 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 05 Aug 2020 00:34:16 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Aug 2020 00:34:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:35:10 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:35:10 GMT
ENV ODOO_VERSION=12.0
# Wed, 05 Aug 2020 00:35:10 GMT
ARG ODOO_RELEASE=20200629
# Wed, 05 Aug 2020 00:35:10 GMT
ARG ODOO_SHA=3c334ba4178b346839679895468ca786bcce9b5f
# Wed, 05 Aug 2020 00:36:04 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=3c334ba4178b346839679895468ca786bcce9b5f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 05 Aug 2020 00:36:05 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 05 Aug 2020 00:36:06 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 05 Aug 2020 00:36:06 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=3c334ba4178b346839679895468ca786bcce9b5f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 05 Aug 2020 00:36:07 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 05 Aug 2020 00:36:07 GMT
EXPOSE 8069 8071 8072
# Wed, 05 Aug 2020 00:36:07 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 05 Aug 2020 00:36:07 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 05 Aug 2020 00:36:07 GMT
USER odoo
# Wed, 05 Aug 2020 00:36:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Aug 2020 00:36:08 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad5c506d50e1dbcc214e3afec29f06e82b7ab2fbfdaa83b7dbe492de47ea5b2`  
		Last Modified: Wed, 05 Aug 2020 00:38:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d430b9279d73c5bcf9ccf812287316870750b3e4e81298ba96b22b66cac9dc7d`  
		Last Modified: Wed, 05 Aug 2020 00:38:36 GMT  
		Size: 219.6 MB (219609743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc34cd5c920e05f814ee9bb94e8cb32c206e1a643d3def70a9a36e63174b3f11`  
		Last Modified: Wed, 05 Aug 2020 00:38:06 GMT  
		Size: 2.3 MB (2336276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2464addedb0e8016754c0bb4efc785d8712c63bfdb8e1f931c16b7cc7f7387b7`  
		Last Modified: Wed, 05 Aug 2020 00:38:11 GMT  
		Size: 22.2 MB (22241349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e651c7cce30a2641b77197a95679acabd1daf3d7baa3f29d1af2e898107caf`  
		Last Modified: Wed, 05 Aug 2020 00:38:35 GMT  
		Size: 129.4 MB (129432091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdf40ba8b427045f8a5b91046ce08ef3ab5ff6d281b8646dcd9a43a9efcc135`  
		Last Modified: Wed, 05 Aug 2020 00:38:04 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d47db41a534db9cad529c95fee4bef5b2636d4215d00fdcbef81b96daeb8696`  
		Last Modified: Wed, 05 Aug 2020 00:38:05 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb39fb9ca983764489010f3e2efef715a522a844e44d42a6a439889883d1c18`  
		Last Modified: Wed, 05 Aug 2020 00:38:04 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005b1fdbdc5dc8a081945166e7a79d521190c66e3ba7c9431e161c16ffc7757d`  
		Last Modified: Wed, 05 Aug 2020 00:38:04 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:12.0`

```console
$ docker pull odoo@sha256:25e9dcf77f4223abf444b5c1f033dc033ccde7287c0ad75890ef7d51bd4739d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:12.0` - linux; amd64

```console
$ docker pull odoo@sha256:a59ca51e209bd079d0f5bb61cdb5a7a12c6d59da765adaec50fcf3d7e5e707ce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396144370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29da3adecc88cd9cbc33978b03715d41a34ad41be2d9432f59a8ba6d619b9b83`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:32:37 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Aug 2020 00:32:38 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Aug 2020 00:32:38 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:32:39 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
# Wed, 05 Aug 2020 00:34:16 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl1.0-dev             node-less             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Aug 2020 00:34:26 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:35:10 GMT
RUN echo "deb http://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='9FD3B784BC1C6FC31A8A0A1C1655A0AB68576280'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/nodejs.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update     && apt-get install --no-install-recommends -y nodejs     && npm install -g rtlcss     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:35:10 GMT
ENV ODOO_VERSION=12.0
# Wed, 05 Aug 2020 00:35:10 GMT
ARG ODOO_RELEASE=20200629
# Wed, 05 Aug 2020 00:35:10 GMT
ARG ODOO_SHA=3c334ba4178b346839679895468ca786bcce9b5f
# Wed, 05 Aug 2020 00:36:04 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=3c334ba4178b346839679895468ca786bcce9b5f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 05 Aug 2020 00:36:05 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 05 Aug 2020 00:36:06 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 05 Aug 2020 00:36:06 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=3c334ba4178b346839679895468ca786bcce9b5f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 05 Aug 2020 00:36:07 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 05 Aug 2020 00:36:07 GMT
EXPOSE 8069 8071 8072
# Wed, 05 Aug 2020 00:36:07 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 05 Aug 2020 00:36:07 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 05 Aug 2020 00:36:07 GMT
USER odoo
# Wed, 05 Aug 2020 00:36:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Aug 2020 00:36:08 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad5c506d50e1dbcc214e3afec29f06e82b7ab2fbfdaa83b7dbe492de47ea5b2`  
		Last Modified: Wed, 05 Aug 2020 00:38:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d430b9279d73c5bcf9ccf812287316870750b3e4e81298ba96b22b66cac9dc7d`  
		Last Modified: Wed, 05 Aug 2020 00:38:36 GMT  
		Size: 219.6 MB (219609743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc34cd5c920e05f814ee9bb94e8cb32c206e1a643d3def70a9a36e63174b3f11`  
		Last Modified: Wed, 05 Aug 2020 00:38:06 GMT  
		Size: 2.3 MB (2336276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2464addedb0e8016754c0bb4efc785d8712c63bfdb8e1f931c16b7cc7f7387b7`  
		Last Modified: Wed, 05 Aug 2020 00:38:11 GMT  
		Size: 22.2 MB (22241349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e651c7cce30a2641b77197a95679acabd1daf3d7baa3f29d1af2e898107caf`  
		Last Modified: Wed, 05 Aug 2020 00:38:35 GMT  
		Size: 129.4 MB (129432091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdf40ba8b427045f8a5b91046ce08ef3ab5ff6d281b8646dcd9a43a9efcc135`  
		Last Modified: Wed, 05 Aug 2020 00:38:04 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d47db41a534db9cad529c95fee4bef5b2636d4215d00fdcbef81b96daeb8696`  
		Last Modified: Wed, 05 Aug 2020 00:38:05 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb39fb9ca983764489010f3e2efef715a522a844e44d42a6a439889883d1c18`  
		Last Modified: Wed, 05 Aug 2020 00:38:04 GMT  
		Size: 594.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005b1fdbdc5dc8a081945166e7a79d521190c66e3ba7c9431e161c16ffc7757d`  
		Last Modified: Wed, 05 Aug 2020 00:38:04 GMT  
		Size: 592.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13`

```console
$ docker pull odoo@sha256:a0a1f89921d66751b8f94042f4bd291d4761858ef4f4262a0b27de8cf70b74d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:59167b0e03ba9139a54a9652ec2cab21771904c9e99f48ff01f0710f1c356cd1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.8 MB (381845371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3576ec790ae798d19836433fb6209fecad869412e3a171c8c8c5ce15591eca43`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:30:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Aug 2020 00:30:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Aug 2020 00:30:22 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:31:24 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Aug 2020 00:31:32 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:31:36 GMT
RUN npm install -g rtlcss
# Wed, 05 Aug 2020 00:31:36 GMT
ENV ODOO_VERSION=13.0
# Wed, 05 Aug 2020 00:31:36 GMT
ARG ODOO_RELEASE=20200629
# Wed, 05 Aug 2020 00:31:37 GMT
ARG ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
# Wed, 05 Aug 2020 00:32:28 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 05 Aug 2020 00:32:29 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 05 Aug 2020 00:32:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 05 Aug 2020 00:32:30 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 05 Aug 2020 00:32:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 05 Aug 2020 00:32:30 GMT
EXPOSE 8069 8071 8072
# Wed, 05 Aug 2020 00:32:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 05 Aug 2020 00:32:30 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 05 Aug 2020 00:32:31 GMT
USER odoo
# Wed, 05 Aug 2020 00:32:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Aug 2020 00:32:31 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa677b64d95abed08a2d9cb947cd9851cd4dbaea538dfbf571254ad7d5c149fb`  
		Last Modified: Wed, 05 Aug 2020 00:37:57 GMT  
		Size: 204.1 MB (204058599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd4309767ba7ebc1ba1cd04b4b96d90fa8ce3b88c6e27e0a2655d5c1139c19c`  
		Last Modified: Wed, 05 Aug 2020 00:37:26 GMT  
		Size: 2.3 MB (2335315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbc48d26ec0e852866cadfb5a0162007485f8f4c60d28986a74f205ba47bc2`  
		Last Modified: Wed, 05 Aug 2020 00:37:25 GMT  
		Size: 1.1 MB (1096042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4cbbe7cdff82a1d0dbb02c329c3f8009198132899824d41a0218823c524bd`  
		Last Modified: Wed, 05 Aug 2020 00:37:58 GMT  
		Size: 147.3 MB (147260894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338ad56bea8cd87880b09d2eecced8151c18f0c5c3c256860d8075442d71ab8c`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c8b032695828e1c2e06e5df52eb8e671361c9365b7e188414cd28ccedd6659`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd5f5f6c87c23e570d53fc7224dbed24b73ba9e03d9a2313934fd98f3544861`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ccac12380488556781d0d580556b28808b535a0cc878a150a32b02250e7187`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:a0a1f89921d66751b8f94042f4bd291d4761858ef4f4262a0b27de8cf70b74d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:59167b0e03ba9139a54a9652ec2cab21771904c9e99f48ff01f0710f1c356cd1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.8 MB (381845371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3576ec790ae798d19836433fb6209fecad869412e3a171c8c8c5ce15591eca43`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:30:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Aug 2020 00:30:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Aug 2020 00:30:22 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:31:24 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Aug 2020 00:31:32 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:31:36 GMT
RUN npm install -g rtlcss
# Wed, 05 Aug 2020 00:31:36 GMT
ENV ODOO_VERSION=13.0
# Wed, 05 Aug 2020 00:31:36 GMT
ARG ODOO_RELEASE=20200629
# Wed, 05 Aug 2020 00:31:37 GMT
ARG ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
# Wed, 05 Aug 2020 00:32:28 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 05 Aug 2020 00:32:29 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 05 Aug 2020 00:32:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 05 Aug 2020 00:32:30 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 05 Aug 2020 00:32:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 05 Aug 2020 00:32:30 GMT
EXPOSE 8069 8071 8072
# Wed, 05 Aug 2020 00:32:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 05 Aug 2020 00:32:30 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 05 Aug 2020 00:32:31 GMT
USER odoo
# Wed, 05 Aug 2020 00:32:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Aug 2020 00:32:31 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa677b64d95abed08a2d9cb947cd9851cd4dbaea538dfbf571254ad7d5c149fb`  
		Last Modified: Wed, 05 Aug 2020 00:37:57 GMT  
		Size: 204.1 MB (204058599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd4309767ba7ebc1ba1cd04b4b96d90fa8ce3b88c6e27e0a2655d5c1139c19c`  
		Last Modified: Wed, 05 Aug 2020 00:37:26 GMT  
		Size: 2.3 MB (2335315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbc48d26ec0e852866cadfb5a0162007485f8f4c60d28986a74f205ba47bc2`  
		Last Modified: Wed, 05 Aug 2020 00:37:25 GMT  
		Size: 1.1 MB (1096042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4cbbe7cdff82a1d0dbb02c329c3f8009198132899824d41a0218823c524bd`  
		Last Modified: Wed, 05 Aug 2020 00:37:58 GMT  
		Size: 147.3 MB (147260894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338ad56bea8cd87880b09d2eecced8151c18f0c5c3c256860d8075442d71ab8c`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c8b032695828e1c2e06e5df52eb8e671361c9365b7e188414cd28ccedd6659`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd5f5f6c87c23e570d53fc7224dbed24b73ba9e03d9a2313934fd98f3544861`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ccac12380488556781d0d580556b28808b535a0cc878a150a32b02250e7187`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:a0a1f89921d66751b8f94042f4bd291d4761858ef4f4262a0b27de8cf70b74d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:59167b0e03ba9139a54a9652ec2cab21771904c9e99f48ff01f0710f1c356cd1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.8 MB (381845371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3576ec790ae798d19836433fb6209fecad869412e3a171c8c8c5ce15591eca43`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:30:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Aug 2020 00:30:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Aug 2020 00:30:22 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:31:24 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Aug 2020 00:31:32 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:31:36 GMT
RUN npm install -g rtlcss
# Wed, 05 Aug 2020 00:31:36 GMT
ENV ODOO_VERSION=13.0
# Wed, 05 Aug 2020 00:31:36 GMT
ARG ODOO_RELEASE=20200629
# Wed, 05 Aug 2020 00:31:37 GMT
ARG ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
# Wed, 05 Aug 2020 00:32:28 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 05 Aug 2020 00:32:29 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 05 Aug 2020 00:32:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 05 Aug 2020 00:32:30 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 05 Aug 2020 00:32:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 05 Aug 2020 00:32:30 GMT
EXPOSE 8069 8071 8072
# Wed, 05 Aug 2020 00:32:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 05 Aug 2020 00:32:30 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 05 Aug 2020 00:32:31 GMT
USER odoo
# Wed, 05 Aug 2020 00:32:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Aug 2020 00:32:31 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa677b64d95abed08a2d9cb947cd9851cd4dbaea538dfbf571254ad7d5c149fb`  
		Last Modified: Wed, 05 Aug 2020 00:37:57 GMT  
		Size: 204.1 MB (204058599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd4309767ba7ebc1ba1cd04b4b96d90fa8ce3b88c6e27e0a2655d5c1139c19c`  
		Last Modified: Wed, 05 Aug 2020 00:37:26 GMT  
		Size: 2.3 MB (2335315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbc48d26ec0e852866cadfb5a0162007485f8f4c60d28986a74f205ba47bc2`  
		Last Modified: Wed, 05 Aug 2020 00:37:25 GMT  
		Size: 1.1 MB (1096042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4cbbe7cdff82a1d0dbb02c329c3f8009198132899824d41a0218823c524bd`  
		Last Modified: Wed, 05 Aug 2020 00:37:58 GMT  
		Size: 147.3 MB (147260894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338ad56bea8cd87880b09d2eecced8151c18f0c5c3c256860d8075442d71ab8c`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c8b032695828e1c2e06e5df52eb8e671361c9365b7e188414cd28ccedd6659`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd5f5f6c87c23e570d53fc7224dbed24b73ba9e03d9a2313934fd98f3544861`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ccac12380488556781d0d580556b28808b535a0cc878a150a32b02250e7187`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
