## `odoo:latest`

```console
$ docker pull odoo@sha256:8c2881cd6f13eb85e0086d237b8c39b1ac9c23a4b592d132714308cac651439b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:cae06b02083470ecc8814c739263b951faff8762cb8121d82454b44b3f5939bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.5 MB (551544020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03dbbe9108c28ef2cc4ff02c8f3eeaa5cd70613b0f7630e6bcd1055965095ce1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:59:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 29 Mar 2022 18:59:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 29 Mar 2022 18:59:21 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 19:00:20 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 29 Mar 2022 19:00:31 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 19:00:32 GMT
RUN npm install -g rtlcss
# Tue, 29 Mar 2022 19:00:32 GMT
ENV ODOO_VERSION=15.0
# Tue, 29 Mar 2022 19:00:33 GMT
ARG ODOO_RELEASE=20220325
# Tue, 29 Mar 2022 19:00:33 GMT
ARG ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
# Tue, 29 Mar 2022 19:02:19 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 29 Mar 2022 19:02:23 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 29 Mar 2022 19:02:23 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 29 Mar 2022 19:02:23 GMT
# ARGS: ODOO_RELEASE=20220325 ODOO_SHA=3d498c38022150b5e3907f2d72346cefe3e16809
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 29 Mar 2022 19:02:23 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 29 Mar 2022 19:02:23 GMT
EXPOSE 8069 8071 8072
# Tue, 29 Mar 2022 19:02:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 29 Mar 2022 19:02:24 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 29 Mar 2022 19:02:24 GMT
USER odoo
# Tue, 29 Mar 2022 19:02:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 19:02:24 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c747a1fa386d9308d1e2f9baef9efced0ce497e52e37fa9688ddc2a83779205`  
		Last Modified: Tue, 29 Mar 2022 19:08:26 GMT  
		Size: 220.3 MB (220306192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26df123c00088a4376eaafc17e8c006c7c47cc1dfa794ff5663dd160dba57157`  
		Last Modified: Tue, 29 Mar 2022 19:07:59 GMT  
		Size: 2.5 MB (2510070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff3bdf6129a4fe206bdf15ab252ebd5569b0f3efff6f8c7e2be9a0e0479b1cc`  
		Last Modified: Tue, 29 Mar 2022 19:07:58 GMT  
		Size: 450.8 KB (450767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01aec3f70f62afe7b3b91a5ffed9b81566e20857fa753e1f8fca00c2d8a76d5b`  
		Last Modified: Tue, 29 Mar 2022 19:08:32 GMT  
		Size: 296.9 MB (296896072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50e8b4b5551815104a61e8c9c95c7725ed5f2183a3b2d64dda20557595e6399`  
		Last Modified: Tue, 29 Mar 2022 19:07:57 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bfc2abf2008b8b202a10511cf9d03ccc2e2343a207f8a37f9d42e29c5f28d8`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf54e7361a0a8e603c294cd65b5257820b5bfe537a9f3898aa8a11bb2887ef1c`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52e6f0a41f3ba62d5cb85b997e04aa6a02aa721736275a8bbe9d772ce125df7`  
		Last Modified: Tue, 29 Mar 2022 19:07:56 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
