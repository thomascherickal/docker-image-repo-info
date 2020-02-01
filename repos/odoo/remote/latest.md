## `odoo:latest`

```console
$ docker pull odoo@sha256:41c93959d1ff41266fd0d26f58bec3361120268c3f54e66958b2c12fec2083e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:f78531da1d4f264d9dcc770600d657b66f1cdbdc6fa5ed501687eca15fd30f5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.3 MB (376261515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae67748cb53b097d49b5fe66c7657537be0e2861b0874adfc22b2a95ec4726e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:03:16 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Sat, 01 Feb 2020 19:03:17 GMT
ENV LANG=C.UTF-8
# Sat, 01 Feb 2020 19:04:48 GMT
RUN set -x;         apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Sat, 01 Feb 2020 19:04:59 GMT
RUN set -x;         echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && export GNUPGHOME="$(mktemp -d)"         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install -y postgresql-client         && rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:05 GMT
RUN set -x;     npm install -g rtlcss
# Sat, 01 Feb 2020 19:05:06 GMT
ENV ODOO_VERSION=13.0
# Sat, 01 Feb 2020 19:05:06 GMT
ARG ODOO_RELEASE=20200121
# Sat, 01 Feb 2020 19:05:06 GMT
ARG ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
# Sat, 01 Feb 2020 19:06:16 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN set -x;         curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && dpkg --force-depends -i odoo.deb         && apt-get update         && apt-get -y install -f --no-install-recommends         && rm -rf /var/lib/apt/lists/* odoo.deb
# Sat, 01 Feb 2020 19:06:18 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Sat, 01 Feb 2020 19:06:18 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Sat, 01 Feb 2020 19:06:19 GMT
# ARGS: ODOO_RELEASE=20200121 ODOO_SHA=770d71cfafb9a8f8419b88f8033b964d5742ad57
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Sat, 01 Feb 2020 19:06:20 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Sat, 01 Feb 2020 19:06:20 GMT
EXPOSE 8069 8071
# Sat, 01 Feb 2020 19:06:20 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Sat, 01 Feb 2020 19:06:21 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Sat, 01 Feb 2020 19:06:21 GMT
USER odoo
# Sat, 01 Feb 2020 19:06:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 01 Feb 2020 19:06:21 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65612bcd6c3150161603c1fd1d5aaa47db0ce71135a0deb6d213304333d3b79a`  
		Last Modified: Sat, 01 Feb 2020 19:13:07 GMT  
		Size: 203.5 MB (203544811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59b34b423f564ca69f18c9dc5722cd2f289fe2ca9c3d49b86fd110bb4ece81`  
		Last Modified: Sat, 01 Feb 2020 19:12:13 GMT  
		Size: 2.2 MB (2228753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c777e556ebc3a8c13db32b99364e7cbf7139db60cb8e14ef998a88dc68f9eb38`  
		Last Modified: Sat, 01 Feb 2020 19:12:13 GMT  
		Size: 1.1 MB (1069181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82a3171af1a9b1a492efd30e7e44b0a1729f760214d834b9beeb856671bd012`  
		Last Modified: Sat, 01 Feb 2020 19:13:19 GMT  
		Size: 142.3 MB (142324108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fdba9aca9cd4ea8dcb656f9629a7497c142ea58a4843c863072cead42dbb4a`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf6028473093cbd7373cab5b706d94d841ddee4125cbf7201c0744c987e1ed6`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e56222b4392a9a4276d1d4852e6b653d76b608012a6b12ae2711fa99a24e8e`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 593.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424f1ae3150fbab6a2e14e37830f152c94c56978853ae9428856baea37d2929d`  
		Last Modified: Sat, 01 Feb 2020 19:12:11 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
