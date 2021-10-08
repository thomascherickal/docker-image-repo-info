## `odoo:latest`

```console
$ docker pull odoo@sha256:31e6b45ce74bf5b90264ca63f7a4d72283ba64b86d930c1482490e38c4a1504d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:7e222384ad337934b7c86db7d7220ac1a44cb58c1ac8e5f012abb7cff5455bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **539.7 MB (539745637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ff6a85ce52eb4d58c33e35cc098b6962cbd03b8062e279eb0d3f10e2e19a032`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Fri, 08 Oct 2021 17:20:31 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Fri, 08 Oct 2021 17:20:31 GMT
SHELL [/bin/bash -xo pipefail -c]
# Fri, 08 Oct 2021 17:20:31 GMT
ENV LANG=C.UTF-8
# Fri, 08 Oct 2021 17:21:31 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         gsfonts         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-openssl         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Fri, 08 Oct 2021 17:21:48 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Oct 2021 17:21:51 GMT
RUN npm install -g rtlcss
# Fri, 08 Oct 2021 17:21:51 GMT
ENV ODOO_VERSION=15.0
# Fri, 08 Oct 2021 17:21:51 GMT
ARG ODOO_RELEASE=20211007
# Fri, 08 Oct 2021 17:21:51 GMT
ARG ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
# Fri, 08 Oct 2021 17:23:06 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Fri, 08 Oct 2021 17:23:10 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Fri, 08 Oct 2021 17:23:10 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Fri, 08 Oct 2021 17:23:11 GMT
# ARGS: ODOO_RELEASE=20211007 ODOO_SHA=aee026f813f334400aa49dc857d4043719f8f395
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Fri, 08 Oct 2021 17:23:11 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Fri, 08 Oct 2021 17:23:11 GMT
EXPOSE 8069 8071 8072
# Fri, 08 Oct 2021 17:23:11 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Fri, 08 Oct 2021 17:23:11 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Fri, 08 Oct 2021 17:23:12 GMT
USER odoo
# Fri, 08 Oct 2021 17:23:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Oct 2021 17:23:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be52707944e2c459c0a114bfbec35c0aec482356baed8e15f747658fcdca6e6`  
		Last Modified: Fri, 08 Oct 2021 17:27:01 GMT  
		Size: 223.8 MB (223814497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c397d8744aa1d4eb6230a18250d33169abf2ae6ab30f09fa5f287c7950bd2`  
		Last Modified: Fri, 08 Oct 2021 17:26:34 GMT  
		Size: 2.5 MB (2506003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4435dbe6255c1f833427223a7e5f73ef0624514d7afece7954d674711d2193e7`  
		Last Modified: Fri, 08 Oct 2021 17:26:33 GMT  
		Size: 853.2 KB (853224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1db7ace550d5156b967f291a8e4c7e6ced71811122cf63105218f1fec0765c`  
		Last Modified: Fri, 08 Oct 2021 17:27:05 GMT  
		Size: 281.2 MB (281200538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fabbe06bcdde04e0b7ef2e9e1501599c3011214e12419e881aae211be58850c`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93d2bb6236506da7b29e172c991710872da38e9ab70ad4c3ff2132756456116`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3682eb88f77b41507ca9c8b7bc2958f0f07845f3b825be6ca9bd2217cb78ff`  
		Last Modified: Fri, 08 Oct 2021 17:26:31 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90658b550a295730b105270faa8854a617aaa7d765cb3d9dfcec69d7e3c15e1`  
		Last Modified: Fri, 08 Oct 2021 17:26:30 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
