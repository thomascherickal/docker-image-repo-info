## `odoo:latest`

```console
$ docker pull odoo@sha256:b41814f15b9320b60f867257608e03db75b6f9a445cd16b285dd5ba3038da7aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:702d6422b830b02fda4ee5eefa93bd32bccead17cf6b8f985cc3318a3c39611a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.3 MB (543318115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3849b0d5cca8c2dcb38c9800b9c13cf4c571d0fd460a5627792384ecf9aa052c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:41 GMT
ADD file:a2405ebb9892d98be2eb585f6121864d12b3fd983ebf15e5f0b7486e106a79c6 in / 
# Wed, 17 Nov 2021 02:20:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:10:25 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 17 Nov 2021 09:10:25 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 17 Nov 2021 09:10:25 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:11:27 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 17 Nov 2021 09:11:37 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:11:39 GMT
RUN npm install -g rtlcss
# Wed, 17 Nov 2021 09:11:39 GMT
ENV ODOO_VERSION=15.0
# Wed, 17 Nov 2021 09:11:39 GMT
ARG ODOO_RELEASE=20211110
# Wed, 17 Nov 2021 09:11:40 GMT
ARG ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
# Wed, 17 Nov 2021 09:12:57 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 17 Nov 2021 09:13:01 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 17 Nov 2021 09:13:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 17 Nov 2021 09:13:02 GMT
# ARGS: ODOO_RELEASE=20211110 ODOO_SHA=313cb2c38f939374f524aaebb017ef0e1724e375
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 17 Nov 2021 09:13:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 17 Nov 2021 09:13:03 GMT
EXPOSE 8069 8071 8072
# Wed, 17 Nov 2021 09:13:03 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 17 Nov 2021 09:13:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 17 Nov 2021 09:13:03 GMT
USER odoo
# Wed, 17 Nov 2021 09:13:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Nov 2021 09:13:04 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:eff15d958d664f0874d16aee393cc44387031ee0a68ef8542d0056c747f378e8`  
		Last Modified: Wed, 17 Nov 2021 02:25:45 GMT  
		Size: 31.4 MB (31370267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9400c757421e2063937e8b190c956fdda2687c92c013b5eff83fe1c61c0c2c8f`  
		Last Modified: Wed, 17 Nov 2021 09:20:38 GMT  
		Size: 220.3 MB (220291328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf19d1a3d79ceb0d2f1f442648da0e6ece72782b8656e052f0867231839dd0b0`  
		Last Modified: Wed, 17 Nov 2021 09:19:52 GMT  
		Size: 2.5 MB (2506093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9605eabe13664e4a62ea8056b48e7547ab78dad77c977652bc44a6e8e1e30d0`  
		Last Modified: Wed, 17 Nov 2021 09:19:51 GMT  
		Size: 724.5 KB (724479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dd0144067b9816daa2e9c5e128284a1ffb2af8ad887060057eec1740a277fc`  
		Last Modified: Wed, 17 Nov 2021 09:20:44 GMT  
		Size: 288.4 MB (288423492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d379ba2c5d0daeee7e64eab4c84ef931722ba3b61f822646e951d3d0387d9d`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acc3388effa209506493f12acfa7790bfd5bace4e945f5ee806d3abfb0e7927`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b516b6485cbad16e360552271b058caf024d336b94a638002401214546365c94`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c921df7aaf8d97bc0c7a7569b14e7078aa5fd5d2a9c7fbcb9766a709a4f676`  
		Last Modified: Wed, 17 Nov 2021 09:19:48 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
