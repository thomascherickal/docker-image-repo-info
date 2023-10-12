## `odoo:latest`

```console
$ docker pull odoo@sha256:01697e5fbab426474004fa6b8c49f0af7554b1fafe2d5c10d68f52461fccf490
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:d84d0d713e8fc33126f97f0706df092f67f8d5e32bc7fb88083003cc40bf64f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **576.8 MB (576806934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f6ec0d61e8b356ed4c1422c3263ce2743dbc67a9973af9dd417ad90a8be6c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:19:57 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Thu, 12 Oct 2023 00:19:57 GMT
SHELL [/bin/bash -xo pipefail -c]
# Thu, 12 Oct 2023 00:19:57 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 00:21:05 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Thu, 12 Oct 2023 00:21:15 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:21:16 GMT
RUN npm install -g rtlcss
# Thu, 12 Oct 2023 00:21:16 GMT
ENV ODOO_VERSION=16.0
# Thu, 12 Oct 2023 00:21:17 GMT
ARG ODOO_RELEASE=20230925
# Thu, 12 Oct 2023 00:21:17 GMT
ARG ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
# Thu, 12 Oct 2023 00:22:49 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Thu, 12 Oct 2023 00:22:54 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Thu, 12 Oct 2023 00:22:54 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Thu, 12 Oct 2023 00:22:54 GMT
# ARGS: ODOO_RELEASE=20230925 ODOO_SHA=c258ecd198cbd079fe1a271dcba23930820eb12f
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Thu, 12 Oct 2023 00:22:54 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Thu, 12 Oct 2023 00:22:54 GMT
EXPOSE 8069 8071 8072
# Thu, 12 Oct 2023 00:22:54 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Thu, 12 Oct 2023 00:22:55 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Thu, 12 Oct 2023 00:22:55 GMT
USER odoo
# Thu, 12 Oct 2023 00:22:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 00:22:55 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d361645e6e1ccf35842cd5eecba0ebc49b323a1b5620e333fcc753bae4d5fbc3`  
		Last Modified: Thu, 12 Oct 2023 00:29:13 GMT  
		Size: 221.0 MB (220990725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5302d28554bbcd79d6bf767cc6e8b48a0c1339264f4448085ff4cc3417f501f`  
		Last Modified: Thu, 12 Oct 2023 00:28:49 GMT  
		Size: 2.6 MB (2628048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d21d45cc4a63b48a65b85f9c014fd7d7af6a43a3571071f582c2bc334ad175`  
		Last Modified: Thu, 12 Oct 2023 00:28:49 GMT  
		Size: 457.2 KB (457194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef9674e55780baea497534673da1655f08144b64a962d71dd05909b03d673ec`  
		Last Modified: Thu, 12 Oct 2023 00:29:24 GMT  
		Size: 321.3 MB (321310642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89b0de0a7ef60c87a76e0d30dcc4ebf776d7050ca3f31dc56f3bd6f92460c1c`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2f302451ec2da5f3f57cf9a2370f276f5d0f43711d1ab57914828866f7f3ac`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0c51ea4877caa63c5e0e87e3d6da150114ba3fb4fb7bd2aebc49bc57985b35`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc2566bf1e44b6707a1ffb37669b2b252eb8bf4fa9e3b738cec1bd7469f5cf8`  
		Last Modified: Thu, 12 Oct 2023 00:28:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
