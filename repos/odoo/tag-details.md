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
$ docker pull odoo@sha256:b208f780fe9f5455c8cb18a01aa18fda3121d0ee564db74b9aefbd9184b77fa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:46b1c877d767c5174032a7bd7f6c379b1c221a654b5a06e93fa16baee2990a4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539655416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4fa0b6a0790f3ce28814d758ef60b014e29792b64cd0a4711f8c9a06f43162`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:43:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 18 Mar 2022 08:43:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 18 Mar 2022 08:43:33 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 08:47:38 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 18 Mar 2022 08:48:20 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:48:23 GMT
RUN npm install -g rtlcss
# Fri, 18 Mar 2022 08:48:23 GMT
ENV ODOO_VERSION=13.0
# Fri, 18 Mar 2022 08:48:23 GMT
ARG ODOO_RELEASE=20220317
# Fri, 18 Mar 2022 08:48:23 GMT
ARG ODOO_SHA=2dc6ad8b50d9f3b9ec3b7b5e24d66e1f9cc57bfd
# Fri, 18 Mar 2022 08:49:35 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=2dc6ad8b50d9f3b9ec3b7b5e24d66e1f9cc57bfd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Mar 2022 08:49:39 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Mar 2022 08:49:39 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Mar 2022 08:49:40 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=2dc6ad8b50d9f3b9ec3b7b5e24d66e1f9cc57bfd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Mar 2022 08:49:40 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Mar 2022 08:49:40 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Mar 2022 08:49:40 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Mar 2022 08:49:40 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Mar 2022 08:49:40 GMT
USER odoo
# Fri, 18 Mar 2022 08:49:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 08:49:40 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af34b027e523073c7675ff12f9ad5be8103e416da025f5404332e3cf0db43f35`  
		Last Modified: Fri, 18 Mar 2022 08:52:07 GMT  
		Size: 207.1 MB (207134258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13e5ae8a871168ea464816a7e582d1a276372a2c52ad4800bac7bd56a6fb924`  
		Last Modified: Fri, 18 Mar 2022 08:51:45 GMT  
		Size: 13.4 MB (13438629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74509aad15ce51f9c500e5e3c2954a378c94d498decc206e5111c2639add3dcf`  
		Last Modified: Fri, 18 Mar 2022 08:51:42 GMT  
		Size: 457.3 KB (457251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2efbd08f1909fc1bcc34285fc27131f088e3358829fc7da201b2ea1b4a8870`  
		Last Modified: Fri, 18 Mar 2022 08:52:13 GMT  
		Size: 291.5 MB (291468984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff9505990d355eef25bf877d371e95a611fd3825943090c459cbd30cccc5ac3`  
		Last Modified: Fri, 18 Mar 2022 08:51:39 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d770ad423b225498d490f3cf283b133a92f613f15194b96f0673725815b438a3`  
		Last Modified: Fri, 18 Mar 2022 08:51:40 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03278d35fd9a69fdf339097291c86f372e1dc19202a7d5bd98a830fc1bb0a9`  
		Last Modified: Fri, 18 Mar 2022 08:51:39 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9810fdc39083401260d1fcca9fce3c7581849e448b42166803f6d56a1b6e66`  
		Last Modified: Fri, 18 Mar 2022 08:51:39 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:b208f780fe9f5455c8cb18a01aa18fda3121d0ee564db74b9aefbd9184b77fa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:46b1c877d767c5174032a7bd7f6c379b1c221a654b5a06e93fa16baee2990a4d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539655416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4fa0b6a0790f3ce28814d758ef60b014e29792b64cd0a4711f8c9a06f43162`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:43:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 18 Mar 2022 08:43:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 18 Mar 2022 08:43:33 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 08:47:38 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 18 Mar 2022 08:48:20 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:48:23 GMT
RUN npm install -g rtlcss
# Fri, 18 Mar 2022 08:48:23 GMT
ENV ODOO_VERSION=13.0
# Fri, 18 Mar 2022 08:48:23 GMT
ARG ODOO_RELEASE=20220317
# Fri, 18 Mar 2022 08:48:23 GMT
ARG ODOO_SHA=2dc6ad8b50d9f3b9ec3b7b5e24d66e1f9cc57bfd
# Fri, 18 Mar 2022 08:49:35 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=2dc6ad8b50d9f3b9ec3b7b5e24d66e1f9cc57bfd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Mar 2022 08:49:39 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Mar 2022 08:49:39 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Mar 2022 08:49:40 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=2dc6ad8b50d9f3b9ec3b7b5e24d66e1f9cc57bfd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Mar 2022 08:49:40 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Mar 2022 08:49:40 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Mar 2022 08:49:40 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Mar 2022 08:49:40 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Mar 2022 08:49:40 GMT
USER odoo
# Fri, 18 Mar 2022 08:49:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 08:49:40 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af34b027e523073c7675ff12f9ad5be8103e416da025f5404332e3cf0db43f35`  
		Last Modified: Fri, 18 Mar 2022 08:52:07 GMT  
		Size: 207.1 MB (207134258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13e5ae8a871168ea464816a7e582d1a276372a2c52ad4800bac7bd56a6fb924`  
		Last Modified: Fri, 18 Mar 2022 08:51:45 GMT  
		Size: 13.4 MB (13438629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74509aad15ce51f9c500e5e3c2954a378c94d498decc206e5111c2639add3dcf`  
		Last Modified: Fri, 18 Mar 2022 08:51:42 GMT  
		Size: 457.3 KB (457251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2efbd08f1909fc1bcc34285fc27131f088e3358829fc7da201b2ea1b4a8870`  
		Last Modified: Fri, 18 Mar 2022 08:52:13 GMT  
		Size: 291.5 MB (291468984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff9505990d355eef25bf877d371e95a611fd3825943090c459cbd30cccc5ac3`  
		Last Modified: Fri, 18 Mar 2022 08:51:39 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d770ad423b225498d490f3cf283b133a92f613f15194b96f0673725815b438a3`  
		Last Modified: Fri, 18 Mar 2022 08:51:40 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03278d35fd9a69fdf339097291c86f372e1dc19202a7d5bd98a830fc1bb0a9`  
		Last Modified: Fri, 18 Mar 2022 08:51:39 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9810fdc39083401260d1fcca9fce3c7581849e448b42166803f6d56a1b6e66`  
		Last Modified: Fri, 18 Mar 2022 08:51:39 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:cb370cf1857384b3e9b0f72ae056d98368352e3c74e8f22cb2eaad2ba8c51a62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:3995b7b73b34c9ea25228ed76fda1e09863a1c1433f8bee8a37acf5413b9b946
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.5 MB (529508651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:892631e4706e756326c249b50aa39168983f0c5362f85c64b54cd9480d6899ef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:43:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 18 Mar 2022 08:43:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 18 Mar 2022 08:43:33 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 08:44:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 18 Mar 2022 08:45:05 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:45:09 GMT
RUN npm install -g rtlcss
# Fri, 18 Mar 2022 08:45:09 GMT
ENV ODOO_VERSION=14.0
# Fri, 18 Mar 2022 08:45:09 GMT
ARG ODOO_RELEASE=20220317
# Fri, 18 Mar 2022 08:45:09 GMT
ARG ODOO_SHA=7afef5494a9b74a63d30532aa9b86dcf8268e8c1
# Fri, 18 Mar 2022 08:46:20 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=7afef5494a9b74a63d30532aa9b86dcf8268e8c1
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Mar 2022 08:46:24 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Mar 2022 08:46:24 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Mar 2022 08:46:24 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=7afef5494a9b74a63d30532aa9b86dcf8268e8c1
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Mar 2022 08:46:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Mar 2022 08:46:24 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Mar 2022 08:46:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Mar 2022 08:46:25 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Mar 2022 08:46:25 GMT
USER odoo
# Fri, 18 Mar 2022 08:46:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 08:46:25 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0faaa559017c2d6ff94384d09ad315a52f26cb01e5870bf721605cc8546508`  
		Last Modified: Fri, 18 Mar 2022 08:51:23 GMT  
		Size: 213.2 MB (213174285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ead5a3160839dfe6d7a3807c708dee7ce4bbdcc2a8d84878c88da20dee986d`  
		Last Modified: Fri, 18 Mar 2022 08:50:59 GMT  
		Size: 13.4 MB (13440836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38508374ad87df6acc92d697d514235f01e68121874d684a3662d65aed523024`  
		Last Modified: Fri, 18 Mar 2022 08:50:56 GMT  
		Size: 457.3 KB (457280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca12f73800adfdcc0b707da110743ad7838b3e7fb3c92afe3296fe54b87fc91`  
		Last Modified: Fri, 18 Mar 2022 08:51:30 GMT  
		Size: 275.3 MB (275279963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f63b0c944b889f16819b73b8553ffdc2cbf364c7bff11571bcdbcf4478e14b`  
		Last Modified: Fri, 18 Mar 2022 08:50:53 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921639dd182f2b9a80f9a95318ebfd1b0d59c73cab5c65ecec320aae18b1b775`  
		Last Modified: Fri, 18 Mar 2022 08:50:53 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdb4815fc79e469ee2a3490d22e0e06176e037e8cf6de37440f7f5bdaf7cadc`  
		Last Modified: Fri, 18 Mar 2022 08:50:53 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e03ece0369d8ce5238ce0da522de5c72c2237e8f16621b8c6fc57b823a3955c`  
		Last Modified: Fri, 18 Mar 2022 08:50:53 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:cb370cf1857384b3e9b0f72ae056d98368352e3c74e8f22cb2eaad2ba8c51a62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:3995b7b73b34c9ea25228ed76fda1e09863a1c1433f8bee8a37acf5413b9b946
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **529.5 MB (529508651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:892631e4706e756326c249b50aa39168983f0c5362f85c64b54cd9480d6899ef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:43:33 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 18 Mar 2022 08:43:33 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 18 Mar 2022 08:43:33 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 08:44:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 18 Mar 2022 08:45:05 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:45:09 GMT
RUN npm install -g rtlcss
# Fri, 18 Mar 2022 08:45:09 GMT
ENV ODOO_VERSION=14.0
# Fri, 18 Mar 2022 08:45:09 GMT
ARG ODOO_RELEASE=20220317
# Fri, 18 Mar 2022 08:45:09 GMT
ARG ODOO_SHA=7afef5494a9b74a63d30532aa9b86dcf8268e8c1
# Fri, 18 Mar 2022 08:46:20 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=7afef5494a9b74a63d30532aa9b86dcf8268e8c1
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Mar 2022 08:46:24 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Mar 2022 08:46:24 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Mar 2022 08:46:24 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=7afef5494a9b74a63d30532aa9b86dcf8268e8c1
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Mar 2022 08:46:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Mar 2022 08:46:24 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Mar 2022 08:46:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Mar 2022 08:46:25 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Mar 2022 08:46:25 GMT
USER odoo
# Fri, 18 Mar 2022 08:46:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 08:46:25 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0faaa559017c2d6ff94384d09ad315a52f26cb01e5870bf721605cc8546508`  
		Last Modified: Fri, 18 Mar 2022 08:51:23 GMT  
		Size: 213.2 MB (213174285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ead5a3160839dfe6d7a3807c708dee7ce4bbdcc2a8d84878c88da20dee986d`  
		Last Modified: Fri, 18 Mar 2022 08:50:59 GMT  
		Size: 13.4 MB (13440836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38508374ad87df6acc92d697d514235f01e68121874d684a3662d65aed523024`  
		Last Modified: Fri, 18 Mar 2022 08:50:56 GMT  
		Size: 457.3 KB (457280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca12f73800adfdcc0b707da110743ad7838b3e7fb3c92afe3296fe54b87fc91`  
		Last Modified: Fri, 18 Mar 2022 08:51:30 GMT  
		Size: 275.3 MB (275279963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f63b0c944b889f16819b73b8553ffdc2cbf364c7bff11571bcdbcf4478e14b`  
		Last Modified: Fri, 18 Mar 2022 08:50:53 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921639dd182f2b9a80f9a95318ebfd1b0d59c73cab5c65ecec320aae18b1b775`  
		Last Modified: Fri, 18 Mar 2022 08:50:53 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdb4815fc79e469ee2a3490d22e0e06176e037e8cf6de37440f7f5bdaf7cadc`  
		Last Modified: Fri, 18 Mar 2022 08:50:53 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e03ece0369d8ce5238ce0da522de5c72c2237e8f16621b8c6fc57b823a3955c`  
		Last Modified: Fri, 18 Mar 2022 08:50:53 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:a9cfd098f97472b2c29928625c3272c77d2dc539a3076d14429fb9f0008c0182
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:b0f192017179f7ddcba260f0a47bf146b509c4b561c551ef23c4f1ea9206f294
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.5 MB (551457341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e10f87fbc3414906293dd932836006cdfad1fffbfce96208464ec01eb3e4b07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:40:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 18 Mar 2022 08:40:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 18 Mar 2022 08:40:10 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 08:41:10 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 18 Mar 2022 08:41:58 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:42:00 GMT
RUN npm install -g rtlcss
# Fri, 18 Mar 2022 08:42:00 GMT
ENV ODOO_VERSION=15.0
# Fri, 18 Mar 2022 08:42:00 GMT
ARG ODOO_RELEASE=20220317
# Fri, 18 Mar 2022 08:42:00 GMT
ARG ODOO_SHA=8b4480787cd1016c5e083210401b37c87c67863d
# Fri, 18 Mar 2022 08:43:16 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=8b4480787cd1016c5e083210401b37c87c67863d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Mar 2022 08:43:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Mar 2022 08:43:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Mar 2022 08:43:21 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=8b4480787cd1016c5e083210401b37c87c67863d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Mar 2022 08:43:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Mar 2022 08:43:21 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Mar 2022 08:43:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Mar 2022 08:43:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Mar 2022 08:43:21 GMT
USER odoo
# Fri, 18 Mar 2022 08:43:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 08:43:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b017bd0f3af794ea97d29bea01710b0112b2dd1193ae49ba1f535e87d7bf27`  
		Last Modified: Fri, 18 Mar 2022 08:50:35 GMT  
		Size: 220.3 MB (220298052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f81dd0cadac34bb3b184c1c920982bd6981304e625e5ad01b9dce5f2bc784d6`  
		Last Modified: Fri, 18 Mar 2022 08:50:04 GMT  
		Size: 2.5 MB (2509910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc845e3739ad670483a172d5d1497e8da58b94a3d5c68a7f2d7eb5f7baab7c`  
		Last Modified: Fri, 18 Mar 2022 08:50:03 GMT  
		Size: 450.8 KB (450836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9459325649e8e137cb1f43e9136faa99e91cfa428b1e67fd2f265a2e58d82755`  
		Last Modified: Fri, 18 Mar 2022 08:50:40 GMT  
		Size: 296.8 MB (296819509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9f67f685162b2ba2e29842c2c6dfdfe25c290a35ec1c87875fe7a8f3adaad1`  
		Last Modified: Fri, 18 Mar 2022 08:50:01 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b0068d4c4713080d21e60f33432e3fb3d9d54012c6ba09663c04ef89f7130c`  
		Last Modified: Fri, 18 Mar 2022 08:50:00 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910f94a02c2dd1f53f74bcee1e39dd93b4fd43514c583b6d6cc3690edadc6447`  
		Last Modified: Fri, 18 Mar 2022 08:50:00 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145617aaffb5c1f1f915f69c8afb27af2a3209cc3f9f61b1934fd14789e5fb6c`  
		Last Modified: Fri, 18 Mar 2022 08:50:00 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:a9cfd098f97472b2c29928625c3272c77d2dc539a3076d14429fb9f0008c0182
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:b0f192017179f7ddcba260f0a47bf146b509c4b561c551ef23c4f1ea9206f294
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.5 MB (551457341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e10f87fbc3414906293dd932836006cdfad1fffbfce96208464ec01eb3e4b07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:40:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 18 Mar 2022 08:40:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 18 Mar 2022 08:40:10 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 08:41:10 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 18 Mar 2022 08:41:58 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:42:00 GMT
RUN npm install -g rtlcss
# Fri, 18 Mar 2022 08:42:00 GMT
ENV ODOO_VERSION=15.0
# Fri, 18 Mar 2022 08:42:00 GMT
ARG ODOO_RELEASE=20220317
# Fri, 18 Mar 2022 08:42:00 GMT
ARG ODOO_SHA=8b4480787cd1016c5e083210401b37c87c67863d
# Fri, 18 Mar 2022 08:43:16 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=8b4480787cd1016c5e083210401b37c87c67863d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Mar 2022 08:43:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Mar 2022 08:43:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Mar 2022 08:43:21 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=8b4480787cd1016c5e083210401b37c87c67863d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Mar 2022 08:43:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Mar 2022 08:43:21 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Mar 2022 08:43:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Mar 2022 08:43:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Mar 2022 08:43:21 GMT
USER odoo
# Fri, 18 Mar 2022 08:43:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 08:43:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b017bd0f3af794ea97d29bea01710b0112b2dd1193ae49ba1f535e87d7bf27`  
		Last Modified: Fri, 18 Mar 2022 08:50:35 GMT  
		Size: 220.3 MB (220298052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f81dd0cadac34bb3b184c1c920982bd6981304e625e5ad01b9dce5f2bc784d6`  
		Last Modified: Fri, 18 Mar 2022 08:50:04 GMT  
		Size: 2.5 MB (2509910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc845e3739ad670483a172d5d1497e8da58b94a3d5c68a7f2d7eb5f7baab7c`  
		Last Modified: Fri, 18 Mar 2022 08:50:03 GMT  
		Size: 450.8 KB (450836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9459325649e8e137cb1f43e9136faa99e91cfa428b1e67fd2f265a2e58d82755`  
		Last Modified: Fri, 18 Mar 2022 08:50:40 GMT  
		Size: 296.8 MB (296819509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9f67f685162b2ba2e29842c2c6dfdfe25c290a35ec1c87875fe7a8f3adaad1`  
		Last Modified: Fri, 18 Mar 2022 08:50:01 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b0068d4c4713080d21e60f33432e3fb3d9d54012c6ba09663c04ef89f7130c`  
		Last Modified: Fri, 18 Mar 2022 08:50:00 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910f94a02c2dd1f53f74bcee1e39dd93b4fd43514c583b6d6cc3690edadc6447`  
		Last Modified: Fri, 18 Mar 2022 08:50:00 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145617aaffb5c1f1f915f69c8afb27af2a3209cc3f9f61b1934fd14789e5fb6c`  
		Last Modified: Fri, 18 Mar 2022 08:50:00 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:a9cfd098f97472b2c29928625c3272c77d2dc539a3076d14429fb9f0008c0182
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:b0f192017179f7ddcba260f0a47bf146b509c4b561c551ef23c4f1ea9206f294
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.5 MB (551457341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e10f87fbc3414906293dd932836006cdfad1fffbfce96208464ec01eb3e4b07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:40:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 18 Mar 2022 08:40:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 18 Mar 2022 08:40:10 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 08:41:10 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 18 Mar 2022 08:41:58 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:42:00 GMT
RUN npm install -g rtlcss
# Fri, 18 Mar 2022 08:42:00 GMT
ENV ODOO_VERSION=15.0
# Fri, 18 Mar 2022 08:42:00 GMT
ARG ODOO_RELEASE=20220317
# Fri, 18 Mar 2022 08:42:00 GMT
ARG ODOO_SHA=8b4480787cd1016c5e083210401b37c87c67863d
# Fri, 18 Mar 2022 08:43:16 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=8b4480787cd1016c5e083210401b37c87c67863d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 18 Mar 2022 08:43:20 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 18 Mar 2022 08:43:20 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 18 Mar 2022 08:43:21 GMT
# ARGS: ODOO_RELEASE=20220317 ODOO_SHA=8b4480787cd1016c5e083210401b37c87c67863d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 18 Mar 2022 08:43:21 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 18 Mar 2022 08:43:21 GMT
EXPOSE 8069 8071 8072
# Fri, 18 Mar 2022 08:43:21 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 18 Mar 2022 08:43:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 18 Mar 2022 08:43:21 GMT
USER odoo
# Fri, 18 Mar 2022 08:43:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Mar 2022 08:43:22 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b017bd0f3af794ea97d29bea01710b0112b2dd1193ae49ba1f535e87d7bf27`  
		Last Modified: Fri, 18 Mar 2022 08:50:35 GMT  
		Size: 220.3 MB (220298052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f81dd0cadac34bb3b184c1c920982bd6981304e625e5ad01b9dce5f2bc784d6`  
		Last Modified: Fri, 18 Mar 2022 08:50:04 GMT  
		Size: 2.5 MB (2509910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fc845e3739ad670483a172d5d1497e8da58b94a3d5c68a7f2d7eb5f7baab7c`  
		Last Modified: Fri, 18 Mar 2022 08:50:03 GMT  
		Size: 450.8 KB (450836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9459325649e8e137cb1f43e9136faa99e91cfa428b1e67fd2f265a2e58d82755`  
		Last Modified: Fri, 18 Mar 2022 08:50:40 GMT  
		Size: 296.8 MB (296819509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9f67f685162b2ba2e29842c2c6dfdfe25c290a35ec1c87875fe7a8f3adaad1`  
		Last Modified: Fri, 18 Mar 2022 08:50:01 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b0068d4c4713080d21e60f33432e3fb3d9d54012c6ba09663c04ef89f7130c`  
		Last Modified: Fri, 18 Mar 2022 08:50:00 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910f94a02c2dd1f53f74bcee1e39dd93b4fd43514c583b6d6cc3690edadc6447`  
		Last Modified: Fri, 18 Mar 2022 08:50:00 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145617aaffb5c1f1f915f69c8afb27af2a3209cc3f9f61b1934fd14789e5fb6c`  
		Last Modified: Fri, 18 Mar 2022 08:50:00 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
