## `odoo:latest`

```console
$ docker pull odoo@sha256:a0a1f89921d66751b8f94042f4bd291d4761858ef4f4262a0b27de8cf70b74d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:59167b0e03ba9139a54a9652ec2cab21771904c9e99f48ff01f0710f1c356cd1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.8 MB (381845371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3576ec790ae798d19836433fb6209fecad869412e3a171c8c8c5ce15591eca43`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:30:21 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 05 Aug 2020 00:30:21 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 05 Aug 2020 00:30:22 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:31:24 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 05 Aug 2020 00:31:32 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:31:36 GMT
RUN npm install -g rtlcss
# Wed, 05 Aug 2020 00:31:36 GMT
ENV ODOO_VERSION=13.0
# Wed, 05 Aug 2020 00:31:36 GMT
ARG ODOO_RELEASE=20200629
# Wed, 05 Aug 2020 00:31:37 GMT
ARG ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
# Wed, 05 Aug 2020 00:32:28 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 05 Aug 2020 00:32:29 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Wed, 05 Aug 2020 00:32:29 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 05 Aug 2020 00:32:30 GMT
# ARGS: ODOO_RELEASE=20200629 ODOO_SHA=1d86e2728a65ed2c9f6ea9b6b893df878f75599e
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 05 Aug 2020 00:32:30 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 05 Aug 2020 00:32:30 GMT
EXPOSE 8069 8071 8072
# Wed, 05 Aug 2020 00:32:30 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 05 Aug 2020 00:32:30 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 05 Aug 2020 00:32:31 GMT
USER odoo
# Wed, 05 Aug 2020 00:32:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Aug 2020 00:32:31 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa677b64d95abed08a2d9cb947cd9851cd4dbaea538dfbf571254ad7d5c149fb`  
		Last Modified: Wed, 05 Aug 2020 00:37:57 GMT  
		Size: 204.1 MB (204058599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd4309767ba7ebc1ba1cd04b4b96d90fa8ce3b88c6e27e0a2655d5c1139c19c`  
		Last Modified: Wed, 05 Aug 2020 00:37:26 GMT  
		Size: 2.3 MB (2335315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ffbc48d26ec0e852866cadfb5a0162007485f8f4c60d28986a74f205ba47bc2`  
		Last Modified: Wed, 05 Aug 2020 00:37:25 GMT  
		Size: 1.1 MB (1096042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4cbbe7cdff82a1d0dbb02c329c3f8009198132899824d41a0218823c524bd`  
		Last Modified: Wed, 05 Aug 2020 00:37:58 GMT  
		Size: 147.3 MB (147260894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338ad56bea8cd87880b09d2eecced8151c18f0c5c3c256860d8075442d71ab8c`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c8b032695828e1c2e06e5df52eb8e671361c9365b7e188414cd28ccedd6659`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd5f5f6c87c23e570d53fc7224dbed24b73ba9e03d9a2313934fd98f3544861`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ccac12380488556781d0d580556b28808b535a0cc878a150a32b02250e7187`  
		Last Modified: Wed, 05 Aug 2020 00:37:24 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
