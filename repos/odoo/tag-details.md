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
$ docker pull odoo@sha256:487514270bff6f4a37cfb7532a2f513cfca7ea4ce996f628c6d9edd4502be2a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13` - linux; amd64

```console
$ docker pull odoo@sha256:1ff1503a157dd7af6bd63f165a270fde7f8e69b4fced636f68589ec9497a5697
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.4 MB (540389313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1c9323e40597bf7e5636f57b70fc176e09c8668239b940181fe9cb0c9fe653`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 12:50:50 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Oct 2022 12:50:50 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Oct 2022 12:50:50 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 12:56:08 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Oct 2022 12:56:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 12:56:19 GMT
RUN npm install -g rtlcss
# Wed, 05 Oct 2022 12:56:19 GMT
ENV ODOO_VERSION=13.0
# Thu, 06 Oct 2022 09:08:53 GMT
ARG ODOO_RELEASE=20221005
# Thu, 06 Oct 2022 09:08:53 GMT
ARG ODOO_SHA=2971414babd77550e662238e94d12142bcf07abf
# Thu, 06 Oct 2022 09:10:06 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=2971414babd77550e662238e94d12142bcf07abf
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 06 Oct 2022 09:10:09 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 06 Oct 2022 09:10:09 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 06 Oct 2022 09:10:10 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=2971414babd77550e662238e94d12142bcf07abf
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 06 Oct 2022 09:10:10 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 06 Oct 2022 09:10:10 GMT
EXPOSE 8069 8071 8072
# Thu, 06 Oct 2022 09:10:10 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 06 Oct 2022 09:10:10 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 06 Oct 2022 09:10:10 GMT
USER odoo
# Thu, 06 Oct 2022 09:10:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 09:10:11 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48e0856975f76bb58e407130d28eea0df88e55a11bc6a9d7bc162d04dd88e60`  
		Last Modified: Wed, 05 Oct 2022 13:00:00 GMT  
		Size: 207.1 MB (207144790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1abf53b046e1d759a453376e0b7546577865ef1e31341fe1b27d7619589da5`  
		Last Modified: Wed, 05 Oct 2022 12:59:38 GMT  
		Size: 13.4 MB (13442511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ec5fffb811e900b540def18663ab415a936770b612d0d52999ebd0ceeee9c3`  
		Last Modified: Wed, 05 Oct 2022 12:59:35 GMT  
		Size: 453.2 KB (453230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dd8a4cacf271b03869f36804f81411994051b9fe969df9a2f32feafc9c79e2`  
		Last Modified: Thu, 06 Oct 2022 09:12:27 GMT  
		Size: 292.2 MB (292208271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049a1caaa08bf845648e64044fde7ab263617ba058c971e865c831598b12225d`  
		Last Modified: Thu, 06 Oct 2022 09:11:56 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78120c93f6b7943f4231ef6633e8aa5dddd3fe6111ef6d913c7af287d4291bee`  
		Last Modified: Thu, 06 Oct 2022 09:11:56 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b1dfee18d3f33d717d94aaa712e236596ce1018fdb0b0e5f47eacf8c897b4f`  
		Last Modified: Thu, 06 Oct 2022 09:11:56 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e05601aeb83e7612edaf9e8a7946efb8e2d5c5650e23da08200d9449fd8ec1`  
		Last Modified: Thu, 06 Oct 2022 09:11:56 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:13.0`

```console
$ docker pull odoo@sha256:487514270bff6f4a37cfb7532a2f513cfca7ea4ce996f628c6d9edd4502be2a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:13.0` - linux; amd64

```console
$ docker pull odoo@sha256:1ff1503a157dd7af6bd63f165a270fde7f8e69b4fced636f68589ec9497a5697
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.4 MB (540389313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1c9323e40597bf7e5636f57b70fc176e09c8668239b940181fe9cb0c9fe653`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 12:50:50 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Oct 2022 12:50:50 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Oct 2022 12:50:50 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 12:56:08 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb         && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Oct 2022 12:56:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 12:56:19 GMT
RUN npm install -g rtlcss
# Wed, 05 Oct 2022 12:56:19 GMT
ENV ODOO_VERSION=13.0
# Thu, 06 Oct 2022 09:08:53 GMT
ARG ODOO_RELEASE=20221005
# Thu, 06 Oct 2022 09:08:53 GMT
ARG ODOO_SHA=2971414babd77550e662238e94d12142bcf07abf
# Thu, 06 Oct 2022 09:10:06 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=2971414babd77550e662238e94d12142bcf07abf
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 06 Oct 2022 09:10:09 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 06 Oct 2022 09:10:09 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 06 Oct 2022 09:10:10 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=2971414babd77550e662238e94d12142bcf07abf
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 06 Oct 2022 09:10:10 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 06 Oct 2022 09:10:10 GMT
EXPOSE 8069 8071 8072
# Thu, 06 Oct 2022 09:10:10 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 06 Oct 2022 09:10:10 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 06 Oct 2022 09:10:10 GMT
USER odoo
# Thu, 06 Oct 2022 09:10:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 09:10:11 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48e0856975f76bb58e407130d28eea0df88e55a11bc6a9d7bc162d04dd88e60`  
		Last Modified: Wed, 05 Oct 2022 13:00:00 GMT  
		Size: 207.1 MB (207144790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1abf53b046e1d759a453376e0b7546577865ef1e31341fe1b27d7619589da5`  
		Last Modified: Wed, 05 Oct 2022 12:59:38 GMT  
		Size: 13.4 MB (13442511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ec5fffb811e900b540def18663ab415a936770b612d0d52999ebd0ceeee9c3`  
		Last Modified: Wed, 05 Oct 2022 12:59:35 GMT  
		Size: 453.2 KB (453230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dd8a4cacf271b03869f36804f81411994051b9fe969df9a2f32feafc9c79e2`  
		Last Modified: Thu, 06 Oct 2022 09:12:27 GMT  
		Size: 292.2 MB (292208271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049a1caaa08bf845648e64044fde7ab263617ba058c971e865c831598b12225d`  
		Last Modified: Thu, 06 Oct 2022 09:11:56 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78120c93f6b7943f4231ef6633e8aa5dddd3fe6111ef6d913c7af287d4291bee`  
		Last Modified: Thu, 06 Oct 2022 09:11:56 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b1dfee18d3f33d717d94aaa712e236596ce1018fdb0b0e5f47eacf8c897b4f`  
		Last Modified: Thu, 06 Oct 2022 09:11:56 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e05601aeb83e7612edaf9e8a7946efb8e2d5c5650e23da08200d9449fd8ec1`  
		Last Modified: Thu, 06 Oct 2022 09:11:56 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14`

```console
$ docker pull odoo@sha256:7a3adde9bb2997508d522a2730e6516a7baed23743334306fa258324158e26a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:1161750deed785205949a468d3c2782fc473085ffea3d5dac5399c61e7bed415
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.0 MB (530963258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a19f9183accea49ed1635884d355395635e4de8e176ebee85a40369db51317`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 12:50:50 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Oct 2022 12:50:50 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Oct 2022 12:50:50 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 12:52:20 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Oct 2022 12:52:32 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 12:52:35 GMT
RUN npm install -g rtlcss
# Wed, 05 Oct 2022 12:52:35 GMT
ENV ODOO_VERSION=14.0
# Thu, 06 Oct 2022 09:07:15 GMT
ARG ODOO_RELEASE=20221005
# Thu, 06 Oct 2022 09:07:15 GMT
ARG ODOO_SHA=0b73069923e9be8f293b0344baacf39282bf2eb7
# Thu, 06 Oct 2022 09:08:35 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=0b73069923e9be8f293b0344baacf39282bf2eb7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 06 Oct 2022 09:08:39 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 06 Oct 2022 09:08:39 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 06 Oct 2022 09:08:39 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=0b73069923e9be8f293b0344baacf39282bf2eb7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 06 Oct 2022 09:08:40 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 06 Oct 2022 09:08:40 GMT
EXPOSE 8069 8071 8072
# Thu, 06 Oct 2022 09:08:40 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 06 Oct 2022 09:08:40 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 06 Oct 2022 09:08:40 GMT
USER odoo
# Thu, 06 Oct 2022 09:08:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 09:08:40 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73991209e36bf89d51fca585d2b4242c0cb80cbfd84e98fe6314e9b7c0d1dde1`  
		Last Modified: Wed, 05 Oct 2022 12:59:16 GMT  
		Size: 213.2 MB (213182348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073b040c0568df4c7a36beaffa7b2957e709200877eb8d18ce95049f470d8381`  
		Last Modified: Wed, 05 Oct 2022 12:58:54 GMT  
		Size: 13.4 MB (13443968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101df339f0e4711374ae94bdfc877da10ab15e76776311e1cc4ea61abed09c22`  
		Last Modified: Wed, 05 Oct 2022 12:58:51 GMT  
		Size: 453.2 KB (453236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7b0c7587297e66be4eb5eddae1059d07563788abb3b371c43994555aac624c`  
		Last Modified: Thu, 06 Oct 2022 09:11:46 GMT  
		Size: 276.7 MB (276743199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7fd943878fab5761d606525e797a82983dce28ea6cfaba2022c1f0f593e3be`  
		Last Modified: Thu, 06 Oct 2022 09:11:13 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411b3b6eef6e2d9b370b7e334dffe97effc0e9137933248e4bbd1876fef4d9c1`  
		Last Modified: Thu, 06 Oct 2022 09:11:13 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855dde5dd5be653f2a6c125692ee33897df99b2356ea90b5444028c162d43f87`  
		Last Modified: Thu, 06 Oct 2022 09:11:13 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cfcd0d166cc50edf0b32043987a06fd70063fac3e02e78cc5e35a86244bb74`  
		Last Modified: Thu, 06 Oct 2022 09:11:14 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:7a3adde9bb2997508d522a2730e6516a7baed23743334306fa258324158e26a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:1161750deed785205949a468d3c2782fc473085ffea3d5dac5399c61e7bed415
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **531.0 MB (530963258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a19f9183accea49ed1635884d355395635e4de8e176ebee85a40369db51317`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 12:50:50 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Oct 2022 12:50:50 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Oct 2022 12:50:50 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 12:52:20 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Oct 2022 12:52:32 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 12:52:35 GMT
RUN npm install -g rtlcss
# Wed, 05 Oct 2022 12:52:35 GMT
ENV ODOO_VERSION=14.0
# Thu, 06 Oct 2022 09:07:15 GMT
ARG ODOO_RELEASE=20221005
# Thu, 06 Oct 2022 09:07:15 GMT
ARG ODOO_SHA=0b73069923e9be8f293b0344baacf39282bf2eb7
# Thu, 06 Oct 2022 09:08:35 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=0b73069923e9be8f293b0344baacf39282bf2eb7
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 06 Oct 2022 09:08:39 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 06 Oct 2022 09:08:39 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 06 Oct 2022 09:08:39 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=0b73069923e9be8f293b0344baacf39282bf2eb7
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 06 Oct 2022 09:08:40 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 06 Oct 2022 09:08:40 GMT
EXPOSE 8069 8071 8072
# Thu, 06 Oct 2022 09:08:40 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 06 Oct 2022 09:08:40 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 06 Oct 2022 09:08:40 GMT
USER odoo
# Thu, 06 Oct 2022 09:08:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 09:08:40 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73991209e36bf89d51fca585d2b4242c0cb80cbfd84e98fe6314e9b7c0d1dde1`  
		Last Modified: Wed, 05 Oct 2022 12:59:16 GMT  
		Size: 213.2 MB (213182348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073b040c0568df4c7a36beaffa7b2957e709200877eb8d18ce95049f470d8381`  
		Last Modified: Wed, 05 Oct 2022 12:58:54 GMT  
		Size: 13.4 MB (13443968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101df339f0e4711374ae94bdfc877da10ab15e76776311e1cc4ea61abed09c22`  
		Last Modified: Wed, 05 Oct 2022 12:58:51 GMT  
		Size: 453.2 KB (453236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7b0c7587297e66be4eb5eddae1059d07563788abb3b371c43994555aac624c`  
		Last Modified: Thu, 06 Oct 2022 09:11:46 GMT  
		Size: 276.7 MB (276743199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7fd943878fab5761d606525e797a82983dce28ea6cfaba2022c1f0f593e3be`  
		Last Modified: Thu, 06 Oct 2022 09:11:13 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411b3b6eef6e2d9b370b7e334dffe97effc0e9137933248e4bbd1876fef4d9c1`  
		Last Modified: Thu, 06 Oct 2022 09:11:13 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855dde5dd5be653f2a6c125692ee33897df99b2356ea90b5444028c162d43f87`  
		Last Modified: Thu, 06 Oct 2022 09:11:13 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cfcd0d166cc50edf0b32043987a06fd70063fac3e02e78cc5e35a86244bb74`  
		Last Modified: Thu, 06 Oct 2022 09:11:14 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:29090c572197859c2be870b6518a2861fa39e8b066df7d706f0fc05240c19cc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:01705db3d5920758c2cb62a62b3d8144cd5eb4b6f6a0be1f00ac9bad8e756523
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **558.3 MB (558288362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3920c91920260922db0305f3cf2d69342607706259f29924b3c1c69e4c858d3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 12:47:42 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Oct 2022 12:47:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Oct 2022 12:47:42 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 12:48:54 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Oct 2022 12:49:04 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 12:49:05 GMT
RUN npm install -g rtlcss
# Wed, 05 Oct 2022 12:49:05 GMT
ENV ODOO_VERSION=15.0
# Thu, 06 Oct 2022 09:05:37 GMT
ARG ODOO_RELEASE=20221005
# Thu, 06 Oct 2022 09:05:37 GMT
ARG ODOO_SHA=60bdd7c9073b1d4252e081dfbdb33b741fef623d
# Thu, 06 Oct 2022 09:06:59 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=60bdd7c9073b1d4252e081dfbdb33b741fef623d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 06 Oct 2022 09:07:03 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 06 Oct 2022 09:07:03 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 06 Oct 2022 09:07:04 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=60bdd7c9073b1d4252e081dfbdb33b741fef623d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 06 Oct 2022 09:07:04 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 06 Oct 2022 09:07:04 GMT
EXPOSE 8069 8071 8072
# Thu, 06 Oct 2022 09:07:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 06 Oct 2022 09:07:04 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 06 Oct 2022 09:07:05 GMT
USER odoo
# Thu, 06 Oct 2022 09:07:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 09:07:05 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1eb84e6e02a853d9decd11a159b54a0995b7293fa476df2fec218d33b1df6d`  
		Last Modified: Wed, 05 Oct 2022 12:58:29 GMT  
		Size: 220.3 MB (220296502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e514ed12a4b7e196251756d20aa16acbeaf5a3a34f67005bd99c3faa6bf6cfba`  
		Last Modified: Wed, 05 Oct 2022 12:58:02 GMT  
		Size: 2.5 MB (2513557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bec1ca6984d8b904d4439a7f235c18d3ab647da175de5faa8ba74a9c232cb8`  
		Last Modified: Wed, 05 Oct 2022 12:58:02 GMT  
		Size: 449.2 KB (449160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaf720e8b109312658ea7e951d0ebd852a43aa5c6b105f0c06af236ff22dc1f`  
		Last Modified: Thu, 06 Oct 2022 09:11:01 GMT  
		Size: 303.6 MB (303606578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c798263a75de76fc1dd1448876ba720c7f19aca44e00333a430fa316cd22e92`  
		Last Modified: Thu, 06 Oct 2022 09:10:26 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e117c903aa429f47d0f1a1060af812aa99236b976ff8dfe65863876d223711`  
		Last Modified: Thu, 06 Oct 2022 09:10:27 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fe834a3b9e590328109bb706095e30e8dc8b021d2d16b4956221e9755d466a`  
		Last Modified: Thu, 06 Oct 2022 09:10:27 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933641ca1d2b6f70303dfef43e6445336ccec82a518b127e53adbf873c2621c5`  
		Last Modified: Thu, 06 Oct 2022 09:10:27 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:29090c572197859c2be870b6518a2861fa39e8b066df7d706f0fc05240c19cc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:01705db3d5920758c2cb62a62b3d8144cd5eb4b6f6a0be1f00ac9bad8e756523
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **558.3 MB (558288362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3920c91920260922db0305f3cf2d69342607706259f29924b3c1c69e4c858d3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 12:47:42 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Oct 2022 12:47:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Oct 2022 12:47:42 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 12:48:54 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Oct 2022 12:49:04 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 12:49:05 GMT
RUN npm install -g rtlcss
# Wed, 05 Oct 2022 12:49:05 GMT
ENV ODOO_VERSION=15.0
# Thu, 06 Oct 2022 09:05:37 GMT
ARG ODOO_RELEASE=20221005
# Thu, 06 Oct 2022 09:05:37 GMT
ARG ODOO_SHA=60bdd7c9073b1d4252e081dfbdb33b741fef623d
# Thu, 06 Oct 2022 09:06:59 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=60bdd7c9073b1d4252e081dfbdb33b741fef623d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 06 Oct 2022 09:07:03 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 06 Oct 2022 09:07:03 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 06 Oct 2022 09:07:04 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=60bdd7c9073b1d4252e081dfbdb33b741fef623d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 06 Oct 2022 09:07:04 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 06 Oct 2022 09:07:04 GMT
EXPOSE 8069 8071 8072
# Thu, 06 Oct 2022 09:07:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 06 Oct 2022 09:07:04 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 06 Oct 2022 09:07:05 GMT
USER odoo
# Thu, 06 Oct 2022 09:07:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 09:07:05 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1eb84e6e02a853d9decd11a159b54a0995b7293fa476df2fec218d33b1df6d`  
		Last Modified: Wed, 05 Oct 2022 12:58:29 GMT  
		Size: 220.3 MB (220296502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e514ed12a4b7e196251756d20aa16acbeaf5a3a34f67005bd99c3faa6bf6cfba`  
		Last Modified: Wed, 05 Oct 2022 12:58:02 GMT  
		Size: 2.5 MB (2513557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bec1ca6984d8b904d4439a7f235c18d3ab647da175de5faa8ba74a9c232cb8`  
		Last Modified: Wed, 05 Oct 2022 12:58:02 GMT  
		Size: 449.2 KB (449160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaf720e8b109312658ea7e951d0ebd852a43aa5c6b105f0c06af236ff22dc1f`  
		Last Modified: Thu, 06 Oct 2022 09:11:01 GMT  
		Size: 303.6 MB (303606578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c798263a75de76fc1dd1448876ba720c7f19aca44e00333a430fa316cd22e92`  
		Last Modified: Thu, 06 Oct 2022 09:10:26 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e117c903aa429f47d0f1a1060af812aa99236b976ff8dfe65863876d223711`  
		Last Modified: Thu, 06 Oct 2022 09:10:27 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fe834a3b9e590328109bb706095e30e8dc8b021d2d16b4956221e9755d466a`  
		Last Modified: Thu, 06 Oct 2022 09:10:27 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933641ca1d2b6f70303dfef43e6445336ccec82a518b127e53adbf873c2621c5`  
		Last Modified: Thu, 06 Oct 2022 09:10:27 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:29090c572197859c2be870b6518a2861fa39e8b066df7d706f0fc05240c19cc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:01705db3d5920758c2cb62a62b3d8144cd5eb4b6f6a0be1f00ac9bad8e756523
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **558.3 MB (558288362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3920c91920260922db0305f3cf2d69342607706259f29924b3c1c69e4c858d3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 12:47:42 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Oct 2022 12:47:42 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Oct 2022 12:47:42 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 12:48:54 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Oct 2022 12:49:04 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 12:49:05 GMT
RUN npm install -g rtlcss
# Wed, 05 Oct 2022 12:49:05 GMT
ENV ODOO_VERSION=15.0
# Thu, 06 Oct 2022 09:05:37 GMT
ARG ODOO_RELEASE=20221005
# Thu, 06 Oct 2022 09:05:37 GMT
ARG ODOO_SHA=60bdd7c9073b1d4252e081dfbdb33b741fef623d
# Thu, 06 Oct 2022 09:06:59 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=60bdd7c9073b1d4252e081dfbdb33b741fef623d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 06 Oct 2022 09:07:03 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 06 Oct 2022 09:07:03 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 06 Oct 2022 09:07:04 GMT
# ARGS: ODOO_RELEASE=20221005 ODOO_SHA=60bdd7c9073b1d4252e081dfbdb33b741fef623d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 06 Oct 2022 09:07:04 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 06 Oct 2022 09:07:04 GMT
EXPOSE 8069 8071 8072
# Thu, 06 Oct 2022 09:07:04 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 06 Oct 2022 09:07:04 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 06 Oct 2022 09:07:05 GMT
USER odoo
# Thu, 06 Oct 2022 09:07:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 09:07:05 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1eb84e6e02a853d9decd11a159b54a0995b7293fa476df2fec218d33b1df6d`  
		Last Modified: Wed, 05 Oct 2022 12:58:29 GMT  
		Size: 220.3 MB (220296502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e514ed12a4b7e196251756d20aa16acbeaf5a3a34f67005bd99c3faa6bf6cfba`  
		Last Modified: Wed, 05 Oct 2022 12:58:02 GMT  
		Size: 2.5 MB (2513557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bec1ca6984d8b904d4439a7f235c18d3ab647da175de5faa8ba74a9c232cb8`  
		Last Modified: Wed, 05 Oct 2022 12:58:02 GMT  
		Size: 449.2 KB (449160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaf720e8b109312658ea7e951d0ebd852a43aa5c6b105f0c06af236ff22dc1f`  
		Last Modified: Thu, 06 Oct 2022 09:11:01 GMT  
		Size: 303.6 MB (303606578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c798263a75de76fc1dd1448876ba720c7f19aca44e00333a430fa316cd22e92`  
		Last Modified: Thu, 06 Oct 2022 09:10:26 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e117c903aa429f47d0f1a1060af812aa99236b976ff8dfe65863876d223711`  
		Last Modified: Thu, 06 Oct 2022 09:10:27 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fe834a3b9e590328109bb706095e30e8dc8b021d2d16b4956221e9755d466a`  
		Last Modified: Thu, 06 Oct 2022 09:10:27 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933641ca1d2b6f70303dfef43e6445336ccec82a518b127e53adbf873c2621c5`  
		Last Modified: Thu, 06 Oct 2022 09:10:27 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
