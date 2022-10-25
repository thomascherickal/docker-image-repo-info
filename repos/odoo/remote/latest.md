## `odoo:latest`

```console
$ docker pull odoo@sha256:debb8b4ec6741a3a0e986b819557de0b9e8f9c4de16908b317e34838bf43dee2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:4110198fd60c6cd326c532ce27ad431b063476933da7610139264d76c6177ab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.0 MB (548958774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d82a3f7d3864c1046e5967342796f9e92ae7171e363f6baf239765ebb1ae9a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:17:27 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 25 Oct 2022 04:17:27 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 25 Oct 2022 04:17:27 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 04:18:41 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 25 Oct 2022 04:18:52 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:18:54 GMT
RUN npm install -g rtlcss
# Tue, 25 Oct 2022 04:18:54 GMT
ENV ODOO_VERSION=16.0
# Tue, 25 Oct 2022 04:18:54 GMT
ARG ODOO_RELEASE=20221012
# Tue, 25 Oct 2022 04:18:54 GMT
ARG ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
# Tue, 25 Oct 2022 04:20:19 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 25 Oct 2022 04:20:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 25 Oct 2022 04:20:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 25 Oct 2022 04:20:23 GMT
# ARGS: ODOO_RELEASE=20221012 ODOO_SHA=f34bc089609c2a7da65f25f29cf4e0218c7af464
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 25 Oct 2022 04:20:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 25 Oct 2022 04:20:24 GMT
EXPOSE 8069 8071 8072
# Tue, 25 Oct 2022 04:20:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 25 Oct 2022 04:20:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 25 Oct 2022 04:20:24 GMT
USER odoo
# Tue, 25 Oct 2022 04:20:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 25 Oct 2022 04:20:24 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f207492967abb893017aed63de26947bc26869c41cb3ae43d047964a3f68abbe`  
		Last Modified: Tue, 25 Oct 2022 04:26:18 GMT  
		Size: 220.3 MB (220299448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034ca3be8a4120921abf777d526b8d64a15bfde37777c39a62f8c4934362a209`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 2.6 MB (2582213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260a86372800d03191e4df8077b594ccd6ea0f53bbc9f7f306cd191796d9f641`  
		Last Modified: Tue, 25 Oct 2022 04:25:51 GMT  
		Size: 449.8 KB (449767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caa33c4d9d34d3a1e72d460dd6b8bd8be65cc719f5a02804d1af4e98574057c`  
		Last Modified: Tue, 25 Oct 2022 04:26:24 GMT  
		Size: 294.2 MB (294204843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6358514a760e4cc3729bac9a4cc44e967c069888c1a866cd427aed6503874a6e`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6e9d3885e34085b18fefbb2a05774dcdfa809089a9284d3761b480fc6814a`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475015701f8f26b0872f8e93222391d601d1419113047f71266cfc6c525f48ca`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f872f3bdb2d2e38d871218c914ca1b81c885636aa66f098e5531929878facb`  
		Last Modified: Tue, 25 Oct 2022 04:25:48 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
