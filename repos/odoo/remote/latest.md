## `odoo:latest`

```console
$ docker pull odoo@sha256:7889037d626ee226e21b956474b9b0c04ab3aa7d9a01228fed08062ee58f45d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:ac884a5f7166600a3cecf7fd95aa6ffbacd989e98a0483ff59f0e542c6a84f76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.3 MB (403277844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8363e01420b14f57c3634d1998a67fd98e5fa7df68eb4c5d210f5b14772efbc1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:26:23 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 18 Nov 2020 06:26:24 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 18 Nov 2020 06:26:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 06:28:04 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 18 Nov 2020 06:28:17 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 06:28:24 GMT
RUN npm install -g rtlcss
# Wed, 18 Nov 2020 06:28:24 GMT
ENV ODOO_VERSION=14.0
# Tue, 24 Nov 2020 00:50:28 GMT
ARG ODOO_RELEASE=20201123
# Tue, 24 Nov 2020 00:50:28 GMT
ARG ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
# Tue, 24 Nov 2020 00:51:24 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 24 Nov 2020 00:51:25 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 24 Nov 2020 00:51:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 24 Nov 2020 00:51:26 GMT
# ARGS: ODOO_RELEASE=20201123 ODOO_SHA=bbcefc0cd5b5aa2285a577118f918742bac670c4
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 24 Nov 2020 00:51:27 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 24 Nov 2020 00:51:27 GMT
EXPOSE 8069 8071 8072
# Tue, 24 Nov 2020 00:51:27 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 24 Nov 2020 00:51:27 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 24 Nov 2020 00:51:27 GMT
USER odoo
# Tue, 24 Nov 2020 00:51:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 24 Nov 2020 00:51:28 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9f15f1287f3c33a7386fc4db89367a1bf2b0176e5652a9f2528a8a0db43473`  
		Last Modified: Wed, 18 Nov 2020 06:38:20 GMT  
		Size: 213.1 MB (213118132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de1b21a1ad400a20f2ccf8539b0c965f9d2762f4de39c4646b95b631b52066d`  
		Last Modified: Wed, 18 Nov 2020 06:37:42 GMT  
		Size: 2.3 MB (2346385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fe648d082dcfa3a00b257cade6256af02e9e4f2f070eb8fa3f124fd9d4de40`  
		Last Modified: Wed, 18 Nov 2020 06:37:41 GMT  
		Size: 1.1 MB (1123493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dda9173147ac3ce3f76bc56a583c24691348f936b9bfc96f55013f2339351d`  
		Last Modified: Tue, 24 Nov 2020 00:54:32 GMT  
		Size: 159.6 MB (159581948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020e9ea6a75b592d63282cf7b751fd15b99a0be5eec6b6e69dd0efd0e32f8324`  
		Last Modified: Tue, 24 Nov 2020 00:53:58 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a205c7662c9bedcb581b00da4ff7b25122c74ec41b5f9ed1f65c064bb73aadb9`  
		Last Modified: Tue, 24 Nov 2020 00:53:59 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b3e944bdd34743c74f801f9033426547493bdfb0e6d5e1f9afc34210a34d2b`  
		Last Modified: Tue, 24 Nov 2020 00:53:59 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bafa32d6e7a434c652194a541f4d3516409542bea9eb2b4db3a5168f839b70`  
		Last Modified: Tue, 24 Nov 2020 00:53:58 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
