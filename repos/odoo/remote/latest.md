## `odoo:latest`

```console
$ docker pull odoo@sha256:15820ddae9c880f2f4e0885469a4ed52b675e36b6bffbd22f2f1c92e6f639e62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:9f3285245b8cafa3537ad422b73a5a37054dc15377cdc882f15d9b8d1980c31f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.3 MB (551278571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2d50b63355fbcb5995a68839b79d45665c30bc4ade0e741b080e8bc09a1a9fc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 14:04:27 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 01 Mar 2022 14:04:27 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 01 Mar 2022 14:04:27 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 14:05:42 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 01 Mar 2022 14:06:28 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:06:30 GMT
RUN npm install -g rtlcss
# Tue, 01 Mar 2022 14:06:30 GMT
ENV ODOO_VERSION=15.0
# Mon, 07 Mar 2022 19:46:53 GMT
ARG ODOO_RELEASE=20220307
# Mon, 07 Mar 2022 19:46:53 GMT
ARG ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
# Mon, 07 Mar 2022 19:48:07 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Mon, 07 Mar 2022 19:48:11 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Mon, 07 Mar 2022 19:48:11 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Mon, 07 Mar 2022 19:48:12 GMT
# ARGS: ODOO_RELEASE=20220307 ODOO_SHA=460e9c91ac6d5d8a9c22dffae95247cd8ed61d55
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Mon, 07 Mar 2022 19:48:12 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Mon, 07 Mar 2022 19:48:12 GMT
EXPOSE 8069 8071 8072
# Mon, 07 Mar 2022 19:48:12 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Mon, 07 Mar 2022 19:48:12 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Mon, 07 Mar 2022 19:48:12 GMT
USER odoo
# Mon, 07 Mar 2022 19:48:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Mar 2022 19:48:12 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a163ebeb0494c6130a80754f29b68a5c07419748988cf37afb9630747c41c69`  
		Last Modified: Tue, 01 Mar 2022 14:17:16 GMT  
		Size: 220.3 MB (220298373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2966b8e28ea8e47acbcca748753c937ef05bfde069cd7bfd2f70252b765fea99`  
		Last Modified: Tue, 01 Mar 2022 14:16:39 GMT  
		Size: 2.5 MB (2510056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9cf6997d2b0f369d91a2ce39d67ba3e78767956bd3cfdfc8d4287600b5389d`  
		Last Modified: Tue, 01 Mar 2022 14:16:38 GMT  
		Size: 447.3 KB (447285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a00db9ec98d74309ff4179c1227d6d2fef69862ff23de7e21984c3f67b479a0`  
		Last Modified: Mon, 07 Mar 2022 19:51:45 GMT  
		Size: 296.7 MB (296654000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493b4385630dec4e8162af9df1c6d4df55714493efc51596eb4a164c4eb63f49`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e655a91665cca257ae7d1746494a821d078d3d91e4ad4e20bcf1949dcb603d79`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d79ec5bcc003281f0154def0c30ec11a3b5baba4bbe5d1a53805e44c4d1d39`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a035624d232c158962c533e416ba594597e913d645f5a84a3f7e65f1ec01c76`  
		Last Modified: Mon, 07 Mar 2022 19:51:12 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
