## `odoo:latest`

```console
$ docker pull odoo@sha256:61710f0664201d2386121eeadc00758c95b8ecc017058fb3495a4a066579bcf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:ac7e6d9d796e9a3d0bb151a0459a4cefabaa8cf9f7bd29ae914ab806b5a5bda1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.5 MB (576468033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d82015409196228a91fc2d1ea067440ec82935ac0205f74c8211e5b70f95d243`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:05:17 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 20 Sep 2023 17:05:17 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 20 Sep 2023 17:05:17 GMT
ENV LANG=C.UTF-8
# Wed, 20 Sep 2023 17:06:24 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 20 Sep 2023 17:06:32 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:06:34 GMT
RUN npm install -g rtlcss
# Wed, 20 Sep 2023 17:06:34 GMT
ENV ODOO_VERSION=16.0
# Wed, 20 Sep 2023 17:06:34 GMT
ARG ODOO_RELEASE=20230908
# Wed, 20 Sep 2023 17:06:34 GMT
ARG ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
# Wed, 20 Sep 2023 17:07:55 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 20 Sep 2023 17:07:59 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 20 Sep 2023 17:07:59 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 20 Sep 2023 17:07:59 GMT
# ARGS: ODOO_RELEASE=20230908 ODOO_SHA=e8031569c375721ada05f12f4be4044f5d7bddbd
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 20 Sep 2023 17:07:59 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 20 Sep 2023 17:07:59 GMT
EXPOSE 8069 8071 8072
# Wed, 20 Sep 2023 17:08:00 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 20 Sep 2023 17:08:00 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 20 Sep 2023 17:08:00 GMT
USER odoo
# Wed, 20 Sep 2023 17:08:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Sep 2023 17:08:00 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f11206b2f0b0742a04b2e5aa673cf9bc01605b066d9fb144ce3973545531f57`  
		Last Modified: Wed, 20 Sep 2023 17:14:18 GMT  
		Size: 221.0 MB (220991931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e852d5c710cf3b695ca69683a47c0c02019debf9d920cb9cf770b83b5b466e3`  
		Last Modified: Wed, 20 Sep 2023 17:13:54 GMT  
		Size: 2.6 MB (2627315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2d84b33fdc1c69a8c227d7b0e75f038a4e81d937f06be5b99f42c6ad8c6bc9`  
		Last Modified: Wed, 20 Sep 2023 17:13:53 GMT  
		Size: 455.5 KB (455518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454e2f8c9878ee0f26e873ab2fde3b043062d669cf75f9ca3176a4c1ea816898`  
		Last Modified: Wed, 20 Sep 2023 17:14:29 GMT  
		Size: 321.0 MB (320973095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6270ab7e1c01f846a1729f620f36f2697350796bbe6b9ee038639eccd2e27a11`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b614947c683d68d6249e2c62f2b6a3544361a9ac0ecba8995af77d6ff78979`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b37a88b4fd5a1b8e6c43c9fcd1d0c19ed6e36f7e453328cc2de42069d861be`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290bb762a8ff6f3bb312f2bbaad6d634179c8047299815edd000b6034aae7ea9`  
		Last Modified: Wed, 20 Sep 2023 17:13:51 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
