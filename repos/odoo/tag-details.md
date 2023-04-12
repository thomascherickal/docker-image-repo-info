<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `odoo`

-	[`odoo:14`](#odoo14)
-	[`odoo:14.0`](#odoo140)
-	[`odoo:15`](#odoo15)
-	[`odoo:15.0`](#odoo150)
-	[`odoo:16`](#odoo16)
-	[`odoo:16.0`](#odoo160)
-	[`odoo:latest`](#odoolatest)

## `odoo:14`

```console
$ docker pull odoo@sha256:db6397343e7ed816e5c95d523ce451951b8bf5ad921361e8a224d98cb009c917
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14` - linux; amd64

```console
$ docker pull odoo@sha256:623746dd6ab46a0f70316b90b03b927a4fc3edc21f619c93a5f59a74056c5394
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.1 MB (532143852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99f6cec307759c7e61b973e1e1184f24b3dc71711c67c4834d2fc95cfaa9388`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:25 GMT
ADD file:e614539607055bdbde0cc1a94ef9783fe3627c8553ef1b21071ecb5c27ea27e4 in / 
# Wed, 12 Apr 2023 00:20:26 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:58:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:58:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:58:51 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 09:00:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 09:00:27 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:00:29 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 09:00:30 GMT
ENV ODOO_VERSION=14.0
# Wed, 12 Apr 2023 09:00:30 GMT
ARG ODOO_RELEASE=20230329
# Wed, 12 Apr 2023 09:00:30 GMT
ARG ODOO_SHA=940676f897cf2e7cf056ce665ebea9385c80dfcb
# Wed, 12 Apr 2023 09:01:49 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=940676f897cf2e7cf056ce665ebea9385c80dfcb
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 12 Apr 2023 09:01:53 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 12 Apr 2023 09:01:53 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 12 Apr 2023 09:01:54 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=940676f897cf2e7cf056ce665ebea9385c80dfcb
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 12 Apr 2023 09:01:54 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 12 Apr 2023 09:01:54 GMT
EXPOSE 8069 8071 8072
# Wed, 12 Apr 2023 09:01:54 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 12 Apr 2023 09:01:54 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 12 Apr 2023 09:01:54 GMT
USER odoo
# Wed, 12 Apr 2023 09:01:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 09:01:54 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9fbefa3370776b7ec7633cf07efc14cc24e0c0cd53893ad0e7e3f44ffdc1bedb`  
		Last Modified: Wed, 12 Apr 2023 00:24:22 GMT  
		Size: 27.1 MB (27138920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00d75581d1741b260047f82ac192a761c24b6c2d68e527e4a0de334335aa31`  
		Last Modified: Wed, 12 Apr 2023 09:04:00 GMT  
		Size: 213.2 MB (213203787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41383b72b69d61dc58305cf803eb49130c28b9c3978783268058f107ef8f2c35`  
		Last Modified: Wed, 12 Apr 2023 09:03:39 GMT  
		Size: 13.5 MB (13517731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6cb4d73ac452284f4e76b99129bce0d2ad7863d895cfd103f629d01b3b1e38`  
		Last Modified: Wed, 12 Apr 2023 09:03:37 GMT  
		Size: 453.9 KB (453862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cafcc2e5cdf6fbfb61bbc97c4be48373492c19e0fc9eef7c2e4cf2855ba864`  
		Last Modified: Wed, 12 Apr 2023 09:04:07 GMT  
		Size: 277.8 MB (277827092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bc7d5ee82869d3698cc8f3dc4b3cba9b1b7d396da5656b44833e14cd10d2f3`  
		Last Modified: Wed, 12 Apr 2023 09:03:35 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1c453aa8a019e4bb3ab38b45b16c65b0edf750eecbb0963ea99cc666a2af67`  
		Last Modified: Wed, 12 Apr 2023 09:03:35 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2966bda7e14cb79b6e21a62ba2e0948dcae063e5afc1b1a8837a2614b48d5c6d`  
		Last Modified: Wed, 12 Apr 2023 09:03:35 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3023a35cc558f7584d74886abb4b2fc86814f8d6f6f20a37fc2e0d9f6962285`  
		Last Modified: Wed, 12 Apr 2023 09:03:35 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:14.0`

```console
$ docker pull odoo@sha256:db6397343e7ed816e5c95d523ce451951b8bf5ad921361e8a224d98cb009c917
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:14.0` - linux; amd64

```console
$ docker pull odoo@sha256:623746dd6ab46a0f70316b90b03b927a4fc3edc21f619c93a5f59a74056c5394
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.1 MB (532143852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99f6cec307759c7e61b973e1e1184f24b3dc71711c67c4834d2fc95cfaa9388`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:25 GMT
ADD file:e614539607055bdbde0cc1a94ef9783fe3627c8553ef1b21071ecb5c27ea27e4 in / 
# Wed, 12 Apr 2023 00:20:26 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:58:51 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:58:51 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:58:51 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 09:00:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 09:00:27 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 09:00:29 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 09:00:30 GMT
ENV ODOO_VERSION=14.0
# Wed, 12 Apr 2023 09:00:30 GMT
ARG ODOO_RELEASE=20230329
# Wed, 12 Apr 2023 09:00:30 GMT
ARG ODOO_SHA=940676f897cf2e7cf056ce665ebea9385c80dfcb
# Wed, 12 Apr 2023 09:01:49 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=940676f897cf2e7cf056ce665ebea9385c80dfcb
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 12 Apr 2023 09:01:53 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 12 Apr 2023 09:01:53 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 12 Apr 2023 09:01:54 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=940676f897cf2e7cf056ce665ebea9385c80dfcb
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 12 Apr 2023 09:01:54 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 12 Apr 2023 09:01:54 GMT
EXPOSE 8069 8071 8072
# Wed, 12 Apr 2023 09:01:54 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 12 Apr 2023 09:01:54 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 12 Apr 2023 09:01:54 GMT
USER odoo
# Wed, 12 Apr 2023 09:01:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 09:01:54 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:9fbefa3370776b7ec7633cf07efc14cc24e0c0cd53893ad0e7e3f44ffdc1bedb`  
		Last Modified: Wed, 12 Apr 2023 00:24:22 GMT  
		Size: 27.1 MB (27138920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00d75581d1741b260047f82ac192a761c24b6c2d68e527e4a0de334335aa31`  
		Last Modified: Wed, 12 Apr 2023 09:04:00 GMT  
		Size: 213.2 MB (213203787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41383b72b69d61dc58305cf803eb49130c28b9c3978783268058f107ef8f2c35`  
		Last Modified: Wed, 12 Apr 2023 09:03:39 GMT  
		Size: 13.5 MB (13517731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6cb4d73ac452284f4e76b99129bce0d2ad7863d895cfd103f629d01b3b1e38`  
		Last Modified: Wed, 12 Apr 2023 09:03:37 GMT  
		Size: 453.9 KB (453862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cafcc2e5cdf6fbfb61bbc97c4be48373492c19e0fc9eef7c2e4cf2855ba864`  
		Last Modified: Wed, 12 Apr 2023 09:04:07 GMT  
		Size: 277.8 MB (277827092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bc7d5ee82869d3698cc8f3dc4b3cba9b1b7d396da5656b44833e14cd10d2f3`  
		Last Modified: Wed, 12 Apr 2023 09:03:35 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1c453aa8a019e4bb3ab38b45b16c65b0edf750eecbb0963ea99cc666a2af67`  
		Last Modified: Wed, 12 Apr 2023 09:03:35 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2966bda7e14cb79b6e21a62ba2e0948dcae063e5afc1b1a8837a2614b48d5c6d`  
		Last Modified: Wed, 12 Apr 2023 09:03:35 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3023a35cc558f7584d74886abb4b2fc86814f8d6f6f20a37fc2e0d9f6962285`  
		Last Modified: Wed, 12 Apr 2023 09:03:35 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15`

```console
$ docker pull odoo@sha256:76e130222a0a0d33e7273c6c12f78f080e69b12f6c76424813163fefe33369f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15` - linux; amd64

```console
$ docker pull odoo@sha256:a0de958a6135431d66ecef7fe13e38e2d68d0f4851e7e89d1977431514f371d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **560.5 MB (560473548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:210214f8f1c333849c5e23ff6b33ab984713e34c58154c5e8d614b7db1bf10e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:54:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:54:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:54:35 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:55:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 08:55:53 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:55:54 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 08:57:28 GMT
ENV ODOO_VERSION=15.0
# Wed, 12 Apr 2023 08:57:28 GMT
ARG ODOO_RELEASE=20230329
# Wed, 12 Apr 2023 08:57:28 GMT
ARG ODOO_SHA=6e714b334c69b3ed396ce5f5c5a87603736bce80
# Wed, 12 Apr 2023 08:58:41 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=6e714b334c69b3ed396ce5f5c5a87603736bce80
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 12 Apr 2023 08:58:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 12 Apr 2023 08:58:42 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 12 Apr 2023 08:58:43 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=6e714b334c69b3ed396ce5f5c5a87603736bce80
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 12 Apr 2023 08:58:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 12 Apr 2023 08:58:43 GMT
EXPOSE 8069 8071 8072
# Wed, 12 Apr 2023 08:58:43 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 12 Apr 2023 08:58:43 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 12 Apr 2023 08:58:43 GMT
USER odoo
# Wed, 12 Apr 2023 08:58:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 08:58:44 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc072a51e9ff1e113fd7d7e6e812f69acee46b65fdb5e60e6a6977ab04867f8f`  
		Last Modified: Wed, 12 Apr 2023 09:02:33 GMT  
		Size: 220.3 MB (220298412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea2cf4d76c14443a63296eecd70cd09a9af720ca062d516b3f41535b435edf2`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 2.6 MB (2575214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfcc7225c9d8a7756bbe895737596be4bb564e0e7223b89b59cd40b96d7735b`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 449.3 KB (449266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f74922f04f327b9a6046848439d6742f909071f90d31f8af7bdbb6449b65920`  
		Last Modified: Wed, 12 Apr 2023 09:03:26 GMT  
		Size: 305.7 MB (305729965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8883a6515f1d1f122c05ba96638358a986ccd0cc21c130a8b911ef12d3c69d17`  
		Last Modified: Wed, 12 Apr 2023 09:02:53 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0507a76502f6fbed70acd68d84cb30f459a066403d79d832b66046010ac6742`  
		Last Modified: Wed, 12 Apr 2023 09:02:53 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ca80536777f344c877df0f7f0aa951c90028e5668927d0cb8222fd4d7b906`  
		Last Modified: Wed, 12 Apr 2023 09:02:53 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b562b5f29738f43792f62d33c4e5367be06ffe9b7e6a7a4fb8d730e6ed00d9`  
		Last Modified: Wed, 12 Apr 2023 09:02:54 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:15.0`

```console
$ docker pull odoo@sha256:76e130222a0a0d33e7273c6c12f78f080e69b12f6c76424813163fefe33369f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:15.0` - linux; amd64

```console
$ docker pull odoo@sha256:a0de958a6135431d66ecef7fe13e38e2d68d0f4851e7e89d1977431514f371d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **560.5 MB (560473548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:210214f8f1c333849c5e23ff6b33ab984713e34c58154c5e8d614b7db1bf10e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:54:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:54:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:54:35 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:55:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 08:55:53 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:55:54 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 08:57:28 GMT
ENV ODOO_VERSION=15.0
# Wed, 12 Apr 2023 08:57:28 GMT
ARG ODOO_RELEASE=20230329
# Wed, 12 Apr 2023 08:57:28 GMT
ARG ODOO_SHA=6e714b334c69b3ed396ce5f5c5a87603736bce80
# Wed, 12 Apr 2023 08:58:41 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=6e714b334c69b3ed396ce5f5c5a87603736bce80
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 12 Apr 2023 08:58:42 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 12 Apr 2023 08:58:42 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 12 Apr 2023 08:58:43 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=6e714b334c69b3ed396ce5f5c5a87603736bce80
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 12 Apr 2023 08:58:43 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 12 Apr 2023 08:58:43 GMT
EXPOSE 8069 8071 8072
# Wed, 12 Apr 2023 08:58:43 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 12 Apr 2023 08:58:43 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 12 Apr 2023 08:58:43 GMT
USER odoo
# Wed, 12 Apr 2023 08:58:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 08:58:44 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc072a51e9ff1e113fd7d7e6e812f69acee46b65fdb5e60e6a6977ab04867f8f`  
		Last Modified: Wed, 12 Apr 2023 09:02:33 GMT  
		Size: 220.3 MB (220298412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea2cf4d76c14443a63296eecd70cd09a9af720ca062d516b3f41535b435edf2`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 2.6 MB (2575214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfcc7225c9d8a7756bbe895737596be4bb564e0e7223b89b59cd40b96d7735b`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 449.3 KB (449266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f74922f04f327b9a6046848439d6742f909071f90d31f8af7bdbb6449b65920`  
		Last Modified: Wed, 12 Apr 2023 09:03:26 GMT  
		Size: 305.7 MB (305729965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8883a6515f1d1f122c05ba96638358a986ccd0cc21c130a8b911ef12d3c69d17`  
		Last Modified: Wed, 12 Apr 2023 09:02:53 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0507a76502f6fbed70acd68d84cb30f459a066403d79d832b66046010ac6742`  
		Last Modified: Wed, 12 Apr 2023 09:02:53 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ca80536777f344c877df0f7f0aa951c90028e5668927d0cb8222fd4d7b906`  
		Last Modified: Wed, 12 Apr 2023 09:02:53 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b562b5f29738f43792f62d33c4e5367be06ffe9b7e6a7a4fb8d730e6ed00d9`  
		Last Modified: Wed, 12 Apr 2023 09:02:54 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16`

```console
$ docker pull odoo@sha256:4111b36648969a6a43c9e17612ececed985ed8b5f2526eefab684f8ae6cc3415
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16` - linux; amd64

```console
$ docker pull odoo@sha256:c6f093c34db08c9c7798a05920b046633a73bf6be94f9a46d88d6cc16e4621ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **568.9 MB (568871031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f303c3d14637ef24dfbf448f5f6b775f5d4b7dbb797c771cf1e020b5e3ce0abb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:54:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:54:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:54:35 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:55:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 08:55:53 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:55:54 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 08:55:54 GMT
ENV ODOO_VERSION=16.0
# Wed, 12 Apr 2023 08:55:54 GMT
ARG ODOO_RELEASE=20230329
# Wed, 12 Apr 2023 08:55:54 GMT
ARG ODOO_SHA=21ec62a768439b5a2ce736aba6899801e73073a6
# Wed, 12 Apr 2023 08:57:20 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=21ec62a768439b5a2ce736aba6899801e73073a6
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 12 Apr 2023 08:57:25 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 12 Apr 2023 08:57:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 12 Apr 2023 08:57:26 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=21ec62a768439b5a2ce736aba6899801e73073a6
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 12 Apr 2023 08:57:26 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 12 Apr 2023 08:57:26 GMT
EXPOSE 8069 8071 8072
# Wed, 12 Apr 2023 08:57:26 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 12 Apr 2023 08:57:26 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 12 Apr 2023 08:57:26 GMT
USER odoo
# Wed, 12 Apr 2023 08:57:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 08:57:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc072a51e9ff1e113fd7d7e6e812f69acee46b65fdb5e60e6a6977ab04867f8f`  
		Last Modified: Wed, 12 Apr 2023 09:02:33 GMT  
		Size: 220.3 MB (220298412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea2cf4d76c14443a63296eecd70cd09a9af720ca062d516b3f41535b435edf2`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 2.6 MB (2575214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfcc7225c9d8a7756bbe895737596be4bb564e0e7223b89b59cd40b96d7735b`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 449.3 KB (449266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2828024293968186beb972cb0505a0d832700fac39c59f48edee81567ffb4b33`  
		Last Modified: Wed, 12 Apr 2023 09:02:43 GMT  
		Size: 314.1 MB (314127449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483cdb247c4d9bd0ad2d87628ac97a24ceed6d199b9eab4b32682aa323fc708`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b9d748f4ab566cbb1743e6bf339ce65762322028c851c67f3571ad33829a7`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78f1b4c1ad6a240d6fd2bf8f9cf5e457be600aa9d4f7006995c0f0fc7614b3a`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e235538e13ff7c3e1b50cd136825be4af1b9e422f99e61a7ee94deed32c39d`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:16.0`

```console
$ docker pull odoo@sha256:4111b36648969a6a43c9e17612ececed985ed8b5f2526eefab684f8ae6cc3415
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:16.0` - linux; amd64

```console
$ docker pull odoo@sha256:c6f093c34db08c9c7798a05920b046633a73bf6be94f9a46d88d6cc16e4621ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **568.9 MB (568871031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f303c3d14637ef24dfbf448f5f6b775f5d4b7dbb797c771cf1e020b5e3ce0abb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:54:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:54:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:54:35 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:55:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 08:55:53 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:55:54 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 08:55:54 GMT
ENV ODOO_VERSION=16.0
# Wed, 12 Apr 2023 08:55:54 GMT
ARG ODOO_RELEASE=20230329
# Wed, 12 Apr 2023 08:55:54 GMT
ARG ODOO_SHA=21ec62a768439b5a2ce736aba6899801e73073a6
# Wed, 12 Apr 2023 08:57:20 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=21ec62a768439b5a2ce736aba6899801e73073a6
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 12 Apr 2023 08:57:25 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 12 Apr 2023 08:57:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 12 Apr 2023 08:57:26 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=21ec62a768439b5a2ce736aba6899801e73073a6
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 12 Apr 2023 08:57:26 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 12 Apr 2023 08:57:26 GMT
EXPOSE 8069 8071 8072
# Wed, 12 Apr 2023 08:57:26 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 12 Apr 2023 08:57:26 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 12 Apr 2023 08:57:26 GMT
USER odoo
# Wed, 12 Apr 2023 08:57:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 08:57:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc072a51e9ff1e113fd7d7e6e812f69acee46b65fdb5e60e6a6977ab04867f8f`  
		Last Modified: Wed, 12 Apr 2023 09:02:33 GMT  
		Size: 220.3 MB (220298412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea2cf4d76c14443a63296eecd70cd09a9af720ca062d516b3f41535b435edf2`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 2.6 MB (2575214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfcc7225c9d8a7756bbe895737596be4bb564e0e7223b89b59cd40b96d7735b`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 449.3 KB (449266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2828024293968186beb972cb0505a0d832700fac39c59f48edee81567ffb4b33`  
		Last Modified: Wed, 12 Apr 2023 09:02:43 GMT  
		Size: 314.1 MB (314127449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483cdb247c4d9bd0ad2d87628ac97a24ceed6d199b9eab4b32682aa323fc708`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b9d748f4ab566cbb1743e6bf339ce65762322028c851c67f3571ad33829a7`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78f1b4c1ad6a240d6fd2bf8f9cf5e457be600aa9d4f7006995c0f0fc7614b3a`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e235538e13ff7c3e1b50cd136825be4af1b9e422f99e61a7ee94deed32c39d`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `odoo:latest`

```console
$ docker pull odoo@sha256:4111b36648969a6a43c9e17612ececed985ed8b5f2526eefab684f8ae6cc3415
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:c6f093c34db08c9c7798a05920b046633a73bf6be94f9a46d88d6cc16e4621ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **568.9 MB (568871031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f303c3d14637ef24dfbf448f5f6b775f5d4b7dbb797c771cf1e020b5e3ce0abb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:54:35 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Wed, 12 Apr 2023 08:54:35 GMT
SHELL [/bin/bash -xo pipefail -c]
# Wed, 12 Apr 2023 08:54:35 GMT
ENV LANG=C.UTF-8
# Wed, 12 Apr 2023 08:55:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-num2words         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/wkhtmltopdf/releases/download/0.12.5/wkhtmltox_0.12.5-1.buster_amd64.deb     && echo 'ea8277df4297afc507c61122f3c349af142f31e5 wkhtmltox.deb' | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Wed, 12 Apr 2023 08:55:53 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 08:55:54 GMT
RUN npm install -g rtlcss
# Wed, 12 Apr 2023 08:55:54 GMT
ENV ODOO_VERSION=16.0
# Wed, 12 Apr 2023 08:55:54 GMT
ARG ODOO_RELEASE=20230329
# Wed, 12 Apr 2023 08:55:54 GMT
ARG ODOO_SHA=21ec62a768439b5a2ce736aba6899801e73073a6
# Wed, 12 Apr 2023 08:57:20 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=21ec62a768439b5a2ce736aba6899801e73073a6
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Wed, 12 Apr 2023 08:57:25 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Wed, 12 Apr 2023 08:57:25 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Wed, 12 Apr 2023 08:57:26 GMT
# ARGS: ODOO_RELEASE=20230329 ODOO_SHA=21ec62a768439b5a2ce736aba6899801e73073a6
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Wed, 12 Apr 2023 08:57:26 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Wed, 12 Apr 2023 08:57:26 GMT
EXPOSE 8069 8071 8072
# Wed, 12 Apr 2023 08:57:26 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Wed, 12 Apr 2023 08:57:26 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Wed, 12 Apr 2023 08:57:26 GMT
USER odoo
# Wed, 12 Apr 2023 08:57:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Apr 2023 08:57:26 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc072a51e9ff1e113fd7d7e6e812f69acee46b65fdb5e60e6a6977ab04867f8f`  
		Last Modified: Wed, 12 Apr 2023 09:02:33 GMT  
		Size: 220.3 MB (220298412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea2cf4d76c14443a63296eecd70cd09a9af720ca062d516b3f41535b435edf2`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 2.6 MB (2575214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfcc7225c9d8a7756bbe895737596be4bb564e0e7223b89b59cd40b96d7735b`  
		Last Modified: Wed, 12 Apr 2023 09:02:09 GMT  
		Size: 449.3 KB (449266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2828024293968186beb972cb0505a0d832700fac39c59f48edee81567ffb4b33`  
		Last Modified: Wed, 12 Apr 2023 09:02:43 GMT  
		Size: 314.1 MB (314127449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483cdb247c4d9bd0ad2d87628ac97a24ceed6d199b9eab4b32682aa323fc708`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b9d748f4ab566cbb1743e6bf339ce65762322028c851c67f3571ad33829a7`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78f1b4c1ad6a240d6fd2bf8f9cf5e457be600aa9d4f7006995c0f0fc7614b3a`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e235538e13ff7c3e1b50cd136825be4af1b9e422f99e61a7ee94deed32c39d`  
		Last Modified: Wed, 12 Apr 2023 09:02:07 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
