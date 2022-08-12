## `odoo:latest`

```console
$ docker pull odoo@sha256:c00026af75004041f4d0000c8dd40c5b991c8964ef73d628e0a217df918ddbef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:b8ed5a50552cf2731678668e3af69dd6e1ed55a97daae21f4cc08596e8b920bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.8 MB (557764760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf8b38c6e36f039b4c5dd882b94f262e9ed1d7c213984a60bfd0f35523328a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:36:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 02 Aug 2022 05:36:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 02 Aug 2022 05:36:10 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 05:37:09 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 02 Aug 2022 05:37:19 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:37:21 GMT
RUN npm install -g rtlcss
# Tue, 02 Aug 2022 05:37:21 GMT
ENV ODOO_VERSION=15.0
# Fri, 12 Aug 2022 20:58:01 GMT
ARG ODOO_RELEASE=20220812
# Fri, 12 Aug 2022 20:58:01 GMT
ARG ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
# Fri, 12 Aug 2022 20:59:20 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 12 Aug 2022 20:59:25 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 12 Aug 2022 20:59:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 12 Aug 2022 20:59:25 GMT
# ARGS: ODOO_RELEASE=20220812 ODOO_SHA=20c4eee998dc54c413d06bb17c59645a3d6a6e04
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 12 Aug 2022 20:59:25 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 12 Aug 2022 20:59:26 GMT
EXPOSE 8069 8071 8072
# Fri, 12 Aug 2022 20:59:26 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 12 Aug 2022 20:59:26 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 12 Aug 2022 20:59:26 GMT
USER odoo
# Fri, 12 Aug 2022 20:59:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 12 Aug 2022 20:59:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc04a644bed3d89143e2aa316af36b00716f4554c4f513da256351fe8cce70aa`  
		Last Modified: Tue, 02 Aug 2022 05:45:00 GMT  
		Size: 220.3 MB (220296597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad4934bbcf7f8f118d6cb4c9dee0e952084f336902f9279646ba728e05729cb`  
		Last Modified: Tue, 02 Aug 2022 05:44:34 GMT  
		Size: 2.5 MB (2513325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77946ee2a1b368dc2efeb7362de7ab48b80331ab4549032ab68486f60bc166ba`  
		Last Modified: Tue, 02 Aug 2022 05:44:33 GMT  
		Size: 502.0 KB (501982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2efed753a3cd370ba3d137eac4c8ccc248091d59b667ddc71801411bf4c559`  
		Last Modified: Fri, 12 Aug 2022 21:03:11 GMT  
		Size: 303.1 MB (303083638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55215f540a300038e579642dcf31d6ec9b159c715e96bd352b71318a3616ec7a`  
		Last Modified: Fri, 12 Aug 2022 21:02:40 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a970400473ae4cf1a239965d63dcf0c2c5e5cb38ccd6d21e9b8dea01219eadb`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5cd72681947ff93f98358119c7f9b078248c9c0f75efd61137874ae26d2a97`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6996b3f50e0e9ee247af79d077cbe84b012b933334c959fb1ce6d3358c6d8f6`  
		Last Modified: Fri, 12 Aug 2022 21:02:36 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
