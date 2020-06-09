## `odoo:latest`

```console
$ docker pull odoo@sha256:c1ec5e4dfafe53a654676aa7d29a052570d5b05754731b6fbef5c5777840c645
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:a8ccb1708693828376a23d15cba823f172498c5c3e1232196d0be12b428c1889
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.2 MB (378208891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba0bc07b0e68f048ab24cdaef5a4d9e7f7fc09741f2be12d8407a5ab8632446`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 08:20:12 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 09 Jun 2020 08:20:12 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 09 Jun 2020 08:20:12 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 08:21:21 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends             ca-certificates             curl             dirmngr             fonts-noto-cjk             gnupg             libssl-dev             node-less             npm             python3-num2words             python3-pip             python3-phonenumbers             python3-pyldap             python3-qrcode             python3-renderpm             python3-setuptools             python3-slugify             python3-vobject             python3-watchdog             python3-xlrd             python3-xlwt             xz-utils         && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.stretch_amd64.deb         && echo '7e35a63f9db14f93ec7feeb0fce76b30c08f2057 wkhtmltox.deb' | sha1sum -c -         && apt-get install -y --no-install-recommends ./wkhtmltox.deb         && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 09 Jun 2020 08:21:31 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list         && GNUPGHOME="$(mktemp -d)"         && export GNUPGHOME         && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'         && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"         && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc         && gpgconf --kill all         && rm -rf "$GNUPGHOME"         && apt-get update          && apt-get install --no-install-recommends -y postgresql-client         && rm -f /etc/apt/sources.list.d/pgdg.list         && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 08:21:35 GMT
RUN npm install -g rtlcss
# Tue, 09 Jun 2020 08:21:35 GMT
ENV ODOO_VERSION=13.0
# Tue, 09 Jun 2020 08:21:35 GMT
ARG ODOO_RELEASE=20200417
# Tue, 09 Jun 2020 08:21:35 GMT
ARG ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
# Tue, 09 Jun 2020 08:22:43 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb         && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -         && apt-get update         && apt-get -y install --no-install-recommends ./odoo.deb         && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 09 Jun 2020 08:22:45 GMT
COPY file:172308c3aaff854a6daab6713c49c8fb84bf96ef2503f0209ef7502dd7574931 in / 
# Tue, 09 Jun 2020 08:22:45 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 09 Jun 2020 08:22:47 GMT
# ARGS: ODOO_RELEASE=20200417 ODOO_SHA=db29fbcebf63f9f656e9445f462190ac775ee533
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 09 Jun 2020 08:22:47 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 09 Jun 2020 08:22:47 GMT
EXPOSE 8069 8071 8072
# Tue, 09 Jun 2020 08:22:48 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 09 Jun 2020 08:22:48 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 09 Jun 2020 08:22:49 GMT
USER odoo
# Tue, 09 Jun 2020 08:22:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Jun 2020 08:22:49 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c38fb221c6bbb14c929d8dc9845e790d99ab77c30f35eeda6d0271790132f8f`  
		Last Modified: Tue, 09 Jun 2020 08:29:18 GMT  
		Size: 204.1 MB (204081824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fbb07c19f556a4061c1794e095cb19bde5b5853b7bbda4820e6f15d50e720e`  
		Last Modified: Tue, 09 Jun 2020 08:28:44 GMT  
		Size: 2.3 MB (2335295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f3dc70f3be0a19e54a19846ffa5cd607a2a93c5323ffc80a908f1b4b856ad4`  
		Last Modified: Tue, 09 Jun 2020 08:28:43 GMT  
		Size: 1.1 MB (1095530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541ac9da707a6f515adba0dbfb77eef7d17cac6b3f6b8fec3daf632680a06a1d`  
		Last Modified: Tue, 09 Jun 2020 08:29:19 GMT  
		Size: 143.6 MB (143595574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31217b92b7e6f8b0c121586c6d1a7498fb70793c7c61f70dd1af35a9e62f0a1e`  
		Last Modified: Tue, 09 Jun 2020 08:28:41 GMT  
		Size: 673.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a50e079c3daf4e100f10c4446a5204ce26f3560dab83e74c5afa0e41b6882`  
		Last Modified: Tue, 09 Jun 2020 08:28:42 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc685fc03600007d1974ac770446bf6781c733e978aa9267e8ba9c195b56aa34`  
		Last Modified: Tue, 09 Jun 2020 08:28:42 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d2cce46a299df5bddab5298ff1445063b10847c8dfa34bfb24364e99a801d3`  
		Last Modified: Tue, 09 Jun 2020 08:28:42 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
