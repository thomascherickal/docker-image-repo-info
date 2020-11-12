## `odoo:latest`

```console
$ docker pull odoo@sha256:a34cf6b6fb0f96039d9c1aaadf0d3840b01700a8fba427b779b3ed36290b0849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:74b2fd8ed7e4ba6ba815a25aa08074cea518bed95d7ddf9cdb2c252951c56424
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.1 MB (402071237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa9ee392a4951c09b82024803109dd6ed8c5ff3a7754f8667da81fc76b042b68`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 17:49:10 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 13 Oct 2020 17:49:10 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 13 Oct 2020 17:49:11 GMT
ENV LANG=C.UTF-8
# Mon, 26 Oct 2020 17:45:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Mon, 26 Oct 2020 17:45:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Oct 2020 17:45:21 GMT
RUN npm install -g rtlcss
# Mon, 26 Oct 2020 17:45:21 GMT
ENV ODOO_VERSION=14.0
# Thu, 12 Nov 2020 19:22:09 GMT
ARG ODOO_RELEASE=20201112
# Thu, 12 Nov 2020 19:22:10 GMT
ARG ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
# Thu, 12 Nov 2020 19:22:59 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Nov 2020 19:23:00 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Thu, 12 Nov 2020 19:23:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Nov 2020 19:23:02 GMT
# ARGS: ODOO_RELEASE=20201112 ODOO_SHA=1ab9abfb9193486aed1886146fe253af6d18d601
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Nov 2020 19:23:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Nov 2020 19:23:02 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Nov 2020 19:23:02 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Nov 2020 19:23:02 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Nov 2020 19:23:03 GMT
USER odoo
# Thu, 12 Nov 2020 19:23:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Nov 2020 19:23:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c69f32ce0e0b8c40da731c837dc4af71c91d64af3a383306b1998b87065248f`  
		Last Modified: Mon, 26 Oct 2020 17:51:27 GMT  
		Size: 213.1 MB (213119031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79914c2df80be97bf35af10e222d03a9673bdb70868542859f4ca306713ea83f`  
		Last Modified: Mon, 26 Oct 2020 17:50:46 GMT  
		Size: 2.4 MB (2435820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64083ae2108cec48181a94003bae0b8399a4a7b6471f1e2d1be462f3b80856bf`  
		Last Modified: Mon, 26 Oct 2020 17:50:45 GMT  
		Size: 1.1 MB (1118509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01edfe5d1f72ce612c1c5cc8c8fd1c632d466f9ae9a7c2b687f7dfe1a9db52bf`  
		Last Modified: Thu, 12 Nov 2020 19:26:01 GMT  
		Size: 158.3 MB (158303244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1469ce57930f123780015a29d2181ecca47034ed282d389c1c16a9b48f2a`  
		Last Modified: Thu, 12 Nov 2020 19:25:30 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c91fa07954c1f88edd13bc7da55c82ad466f6a17046cbed153cdd1193545ea9`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13f72919012cc465c0c6fbdf95426594bfe9f624ecea38f6006f33ee6b7e416`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25543eac24aeaf3949be246262ab118f76d0eb6e61fde74ab56951d58fe7383d`  
		Last Modified: Thu, 12 Nov 2020 19:25:31 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
