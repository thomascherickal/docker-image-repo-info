## `odoo:latest`

```console
$ docker pull odoo@sha256:cbf4d2c87bbce86a0cae5db2d8f08debb8072222fba043ceab755b7b6c8a0e41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:5c134193f01ac4b36ead740d2cb828865f83d2ef3833dd1c298379773937fcaa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **516.1 MB (516118672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f97cdf3e7abe1fa762f3699ad9e1884f9c5bc9c51659ec570660deb1a6f31d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 12:30:53 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 10 Apr 2021 12:30:53 GMT
SHELL [/bin/bash -xo pipefail -c]
# Sat, 10 Apr 2021 12:30:54 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 12:32:34 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 10 Apr 2021 12:32:46 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:32:51 GMT
RUN npm install -g rtlcss
# Sat, 10 Apr 2021 12:32:51 GMT
ENV ODOO_VERSION=14.0
# Tue, 27 Apr 2021 21:24:01 GMT
ARG ODOO_RELEASE=20210427
# Tue, 27 Apr 2021 21:24:01 GMT
ARG ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
# Tue, 27 Apr 2021 21:25:13 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 27 Apr 2021 21:25:17 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 27 Apr 2021 21:25:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 27 Apr 2021 21:25:19 GMT
# ARGS: ODOO_RELEASE=20210427 ODOO_SHA=9d8e8038d5589bc8f4f5f012773dba4deefd3adc
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 27 Apr 2021 21:25:19 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 27 Apr 2021 21:25:19 GMT
EXPOSE 8069 8071 8072
# Tue, 27 Apr 2021 21:25:19 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 27 Apr 2021 21:25:19 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 27 Apr 2021 21:25:20 GMT
USER odoo
# Tue, 27 Apr 2021 21:25:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Apr 2021 21:25:20 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df7a8fcf45065b035b83165d399d7900a139dc5e00d9e4d6ce8699785fb5343`  
		Last Modified: Sat, 10 Apr 2021 12:41:41 GMT  
		Size: 213.2 MB (213170428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6128de947157b937143a4ca96babae9ce2e9b71d01a4b53dc0a4e1301bdaa0d4`  
		Last Modified: Sat, 10 Apr 2021 12:41:12 GMT  
		Size: 2.3 MB (2348669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963607ad2a1b5492ef59daa14209ad6d7e164abe8c9f0636566235cff0d20ade`  
		Last Modified: Sat, 10 Apr 2021 12:41:11 GMT  
		Size: 896.6 KB (896573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca57d7a391cae7292e0bc1b366c0235632ce91ec42f6ddf11e87eed7a0f78ff`  
		Last Modified: Tue, 27 Apr 2021 21:29:03 GMT  
		Size: 272.6 MB (272561198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa28544e22fad79a6ff3318efd2f9637f3e7132129a3736e6260be436d937906`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58612f6171ea665c9f2a89e0c8289ec06b8e4ba6e415be926a196da48b1f1e1`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9578101cbabb3a13af26665ba25b59d7a6db44e1215db0bdb8cb3c2e17a019ba`  
		Last Modified: Tue, 27 Apr 2021 21:28:31 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc314e016235206bc8b95f020e07554a3ffa4eb36ff256201d40228290b94f47`  
		Last Modified: Tue, 27 Apr 2021 21:28:32 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
