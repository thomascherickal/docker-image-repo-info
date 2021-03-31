## `odoo:latest`

```console
$ docker pull odoo@sha256:2ecb515f376e3d4e70fe6553825d1a2e7103751b0711f6969ac04361a2cfddc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:597518465b4b472c487bd444d7fb22766f282840dcba49d99ec38d8a089e7be7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.8 MB (515795602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ba433d24bc66371eb98f141ebd811166f5c08994ad18bf44a04dba978e4e22`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:28:28 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 31 Mar 2021 05:28:28 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 31 Mar 2021 05:28:29 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 05:29:34 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 31 Mar 2021 05:29:44 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:29:47 GMT
RUN npm install -g rtlcss
# Wed, 31 Mar 2021 05:29:48 GMT
ENV ODOO_VERSION=14.0
# Wed, 31 Mar 2021 05:29:48 GMT
ARG ODOO_RELEASE=20210330
# Wed, 31 Mar 2021 05:29:48 GMT
ARG ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
# Wed, 31 Mar 2021 05:30:59 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 31 Mar 2021 05:31:01 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 31 Mar 2021 05:31:01 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 31 Mar 2021 05:31:02 GMT
# ARGS: ODOO_RELEASE=20210330 ODOO_SHA=0a0ebf50846a5e5131a6725795c3fc59d511262d
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 31 Mar 2021 05:31:02 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 31 Mar 2021 05:31:02 GMT
EXPOSE 8069 8071 8072
# Wed, 31 Mar 2021 05:31:03 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 31 Mar 2021 05:31:03 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 31 Mar 2021 05:31:03 GMT
USER odoo
# Wed, 31 Mar 2021 05:31:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 31 Mar 2021 05:31:03 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891b8c13a6557e87341fe3dae2cacc445b84d3061c83b252ca743c338d64cc83`  
		Last Modified: Wed, 31 Mar 2021 05:37:46 GMT  
		Size: 213.2 MB (213169537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acf2c1161bac7f6d917df1dab741f4f98b3d7d9bb4994d7fd1913385578875e`  
		Last Modified: Wed, 31 Mar 2021 05:37:18 GMT  
		Size: 2.3 MB (2348508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16b52e489bcfae111683bd0dc94749af43d9ea55931a3c2a703c8c3ff3dfb6e`  
		Last Modified: Wed, 31 Mar 2021 05:37:16 GMT  
		Size: 894.0 KB (894018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c12fc10a65fc5cc749140f39858c24345a40cd3a5c65cb1bd16564562f5863`  
		Last Modified: Wed, 31 Mar 2021 05:37:52 GMT  
		Size: 272.2 MB (272241819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99f91ee63f5d119d59cfb65a6bffadf64bde3db9e62735ca33afbf4059f9300`  
		Last Modified: Wed, 31 Mar 2021 05:37:13 GMT  
		Size: 671.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71b71de0f7f0c0868631d2ab856a984a6096b6eeae599564aa6a8ad7d4e440b`  
		Last Modified: Wed, 31 Mar 2021 05:37:13 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a363c38a84e7a64fe52ba04fa47a29eda88f5c223718f31032b258fcc191ea4`  
		Last Modified: Wed, 31 Mar 2021 05:37:14 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee9192eeed425ce8c67b4d2d92154b2082eb4838c326615ef35167d38cefbfd`  
		Last Modified: Wed, 31 Mar 2021 05:37:14 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
