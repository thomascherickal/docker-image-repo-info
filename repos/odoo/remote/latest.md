## `odoo:latest`

```console
$ docker pull odoo@sha256:eaf77eff4341a0ca9c22da268a6260141f35f2a7f6b7a2096b600e9872798f1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `odoo:latest` - linux; amd64

```console
$ docker pull odoo@sha256:a7f60b1963ab43824ea42c1af5b42b4c52db8d65ec7af41a4f9e69a646b6ba62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.6 MB (592612047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7170d39c241047d94ec39e68cea318800116523bcfa6077f5524a0c8a3180eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Tue, 14 Nov 2023 01:38:22 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 14 Nov 2023 01:38:22 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 14 Nov 2023 01:38:22 GMT
ENV LANG=en_US.UTF-8
# Tue, 14 Nov 2023 01:38:22 GMT
ARG TARGETARCH
# Tue, 14 Nov 2023 01:40:32 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 14 Nov 2023 01:43:12 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 14 Nov 2023 01:43:14 GMT
RUN npm install -g rtlcss
# Tue, 14 Nov 2023 01:43:14 GMT
ENV ODOO_VERSION=17.0
# Tue, 14 Nov 2023 01:43:14 GMT
ARG ODOO_RELEASE=20231113
# Tue, 14 Nov 2023 01:43:14 GMT
ARG ODOO_SHA=b72a32e3356084adb637334b45b110cdedc8ab0c
# Tue, 14 Nov 2023 01:45:02 GMT
# ARGS: ODOO_RELEASE=20231113 ODOO_SHA=b72a32e3356084adb637334b45b110cdedc8ab0c
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 14 Nov 2023 01:45:04 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 14 Nov 2023 01:45:04 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 14 Nov 2023 01:45:05 GMT
# ARGS: ODOO_RELEASE=20231113 ODOO_SHA=b72a32e3356084adb637334b45b110cdedc8ab0c
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 14 Nov 2023 01:45:05 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 14 Nov 2023 01:45:05 GMT
EXPOSE 8069 8071 8072
# Tue, 14 Nov 2023 01:45:05 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 14 Nov 2023 01:45:05 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 14 Nov 2023 01:45:05 GMT
USER odoo
# Tue, 14 Nov 2023 01:45:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Nov 2023 01:45:05 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb3c31d88935a4bd21fe72cde4d10cf70f938ed370d1589f5afe78de8e9d5ef`  
		Last Modified: Tue, 14 Nov 2023 01:48:55 GMT  
		Size: 236.0 MB (236000929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1635e6cd9216147592a4196f3bd6dbd96074a19264c7ec0d1ebca064d6810ba5`  
		Last Modified: Tue, 14 Nov 2023 01:48:28 GMT  
		Size: 2.5 MB (2526404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ce7265beed021294fe7c29a3a1bc47a0ccdcda030d1d53cbc088171441d3a8`  
		Last Modified: Tue, 14 Nov 2023 01:48:28 GMT  
		Size: 460.6 KB (460559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491ed2407f72c50f82b88a57800e72be5c1af72ca4e45cc484dfae6634cd0030`  
		Last Modified: Tue, 14 Nov 2023 01:49:03 GMT  
		Size: 323.2 MB (323182579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543221c1238d6ee3186b24846b8c7e021f8bd44f3958d7454dfa4999d7cdea95`  
		Last Modified: Tue, 14 Nov 2023 01:48:26 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d25bfe6e40b514a7fd70cade9dc301affe022bde8ef3eaa213a722bc9129f1`  
		Last Modified: Tue, 14 Nov 2023 01:48:26 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338da5921028da41ae6a32bd5b0c01eac9bbef08954048427d0557332acab111`  
		Last Modified: Tue, 14 Nov 2023 01:48:26 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9683ec1a4254f4c829b1dd646c10b6d49dd3945a537dfad7f990c292207feb90`  
		Last Modified: Tue, 14 Nov 2023 01:48:26 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:latest` - linux; arm64 variant v8

```console
$ docker pull odoo@sha256:081e643c5b1d024db510b0c7b35b43a07b0eb08674a4478ecbe7d3e690c79535
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **589.3 MB (589252116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8213f8ac42992be9d7b335deb14e4cdcdf6332ab64b8112eb3c0e9011525a3d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Tue, 14 Nov 2023 00:50:55 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 14 Nov 2023 00:50:55 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 14 Nov 2023 00:50:55 GMT
ENV LANG=en_US.UTF-8
# Tue, 14 Nov 2023 00:50:56 GMT
ARG TARGETARCH
# Tue, 14 Nov 2023 00:53:29 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 14 Nov 2023 00:53:43 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 14 Nov 2023 00:53:44 GMT
RUN npm install -g rtlcss
# Tue, 14 Nov 2023 00:53:44 GMT
ENV ODOO_VERSION=17.0
# Tue, 21 Nov 2023 04:07:16 GMT
ARG ODOO_RELEASE=20231120
# Tue, 21 Nov 2023 04:07:16 GMT
ARG ODOO_SHA=57b836de2901c4ec5e3de433eb9258024701d255
# Tue, 21 Nov 2023 04:09:26 GMT
# ARGS: ODOO_RELEASE=20231120 ODOO_SHA=57b836de2901c4ec5e3de433eb9258024701d255
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 21 Nov 2023 04:09:35 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 21 Nov 2023 04:09:35 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 21 Nov 2023 04:09:35 GMT
# ARGS: ODOO_RELEASE=20231120 ODOO_SHA=57b836de2901c4ec5e3de433eb9258024701d255
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 21 Nov 2023 04:09:35 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 21 Nov 2023 04:09:35 GMT
EXPOSE 8069 8071 8072
# Tue, 21 Nov 2023 04:09:35 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 21 Nov 2023 04:09:35 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 21 Nov 2023 04:09:35 GMT
USER odoo
# Tue, 21 Nov 2023 04:09:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 04:09:36 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab1126a28686b8ed5fe7ce9c231b2feaf2464bfdd4c69292a490627f6d3e9e`  
		Last Modified: Tue, 14 Nov 2023 00:57:54 GMT  
		Size: 233.2 MB (233245340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac61d67d73d062d91830915181a68ab467f4aec863686610d5655f2baa622d55`  
		Last Modified: Tue, 14 Nov 2023 00:57:35 GMT  
		Size: 2.5 MB (2520327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50a0b71d2c501c8759efe323740bae5ad9e3440515f38b9963427218127ac5b`  
		Last Modified: Tue, 14 Nov 2023 00:57:35 GMT  
		Size: 460.5 KB (460530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0b61a08606390fbb30208a1c7ecb8e9f362c2e67348e7ca4e0a137f155bfdc`  
		Last Modified: Tue, 21 Nov 2023 04:11:53 GMT  
		Size: 324.6 MB (324631518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cadee43b1bf171bcee8f8a922aaacf7780d1bc3f22ffb8753b6026dedad8f6`  
		Last Modified: Tue, 21 Nov 2023 04:11:24 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618075eb4ae57747ac5d18886eb478e1bde106ce7c8ffdb4ee962e649342551e`  
		Last Modified: Tue, 21 Nov 2023 04:11:24 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a97278fdc7005daaf7f7481fbaf2ad6650a52d3727b57952d0ec091e402d89`  
		Last Modified: Tue, 21 Nov 2023 04:11:24 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66f192450018011ce8cedb344714cdbafaa778844b51ca83c7bd59b6c3d6018`  
		Last Modified: Tue, 21 Nov 2023 04:11:24 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `odoo:latest` - linux; ppc64le

```console
$ docker pull odoo@sha256:b7851ec4705b5e2f2dcec02962bd3a42780532177776f54b1142571adc4d25aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **611.7 MB (611662048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:affaaac65f413cdf81476af3f1f0da82fcf20ee50c65def7443bbc7daef30c95`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["odoo"]`
-	`SHELL`: `["\/bin\/bash","-xo","pipefail","-c"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
# Tue, 14 Nov 2023 01:16:47 GMT
MAINTAINER Odoo S.A. <info@odoo.com>
# Tue, 14 Nov 2023 01:16:47 GMT
SHELL [/bin/bash -xo pipefail -c]
# Tue, 14 Nov 2023 01:16:48 GMT
ENV LANG=en_US.UTF-8
# Tue, 14 Nov 2023 01:16:49 GMT
ARG TARGETARCH
# Tue, 14 Nov 2023 01:21:28 GMT
RUN apt-get update &&     DEBIAN_FRONTEND=noninteractive     apt-get install -y --no-install-recommends         ca-certificates         curl         dirmngr         fonts-noto-cjk         gnupg         libssl-dev         node-less         npm         python3-magic         python3-num2words         python3-odf         python3-pdfminer         python3-pip         python3-phonenumbers         python3-pyldap         python3-qrcode         python3-renderpm         python3-setuptools         python3-slugify         python3-vobject         python3-watchdog         python3-xlrd         python3-xlwt         xz-utils &&     if [ -z "${TARGETARCH}" ]; then         TARGETARCH="$(dpkg --print-architecture)";     fi;     WKHTMLTOPDF_ARCH=${TARGETARCH} &&     case ${TARGETARCH} in     "amd64") WKHTMLTOPDF_ARCH=amd64 && WKHTMLTOPDF_SHA=967390a759707337b46d1c02452e2bb6b2dc6d59  ;;     "arm64")  WKHTMLTOPDF_SHA=90f6e69896d51ef77339d3f3a20f8582bdf496cc  ;;     "ppc64le" | "ppc64el") WKHTMLTOPDF_ARCH=ppc64el && WKHTMLTOPDF_SHA=5312d7d34a25b321282929df82e3574319aed25c  ;;     esac     && curl -o wkhtmltox.deb -sSL https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-3/wkhtmltox_0.12.6.1-3.jammy_${WKHTMLTOPDF_ARCH}.deb     && echo ${WKHTMLTOPDF_SHA} wkhtmltox.deb | sha1sum -c -     && apt-get install -y --no-install-recommends ./wkhtmltox.deb     && rm -rf /var/lib/apt/lists/* wkhtmltox.deb
# Tue, 14 Nov 2023 01:21:50 GMT
RUN echo 'deb http://apt.postgresql.org/pub/repos/apt/ jammy-pgdg main' > /etc/apt/sources.list.d/pgdg.list     && GNUPGHOME="$(mktemp -d)"     && export GNUPGHOME     && repokey='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'     && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "${repokey}"     && gpg --batch --armor --export "${repokey}" > /etc/apt/trusted.gpg.d/pgdg.gpg.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && apt-get update      && apt-get install --no-install-recommends -y postgresql-client     && rm -f /etc/apt/sources.list.d/pgdg.list     && rm -rf /var/lib/apt/lists/*
# Tue, 14 Nov 2023 01:21:53 GMT
RUN npm install -g rtlcss
# Tue, 14 Nov 2023 01:21:54 GMT
ENV ODOO_VERSION=17.0
# Tue, 21 Nov 2023 04:34:09 GMT
ARG ODOO_RELEASE=20231120
# Tue, 21 Nov 2023 04:34:09 GMT
ARG ODOO_SHA=57b836de2901c4ec5e3de433eb9258024701d255
# Tue, 21 Nov 2023 04:37:08 GMT
# ARGS: ODOO_RELEASE=20231120 ODOO_SHA=57b836de2901c4ec5e3de433eb9258024701d255
RUN curl -o odoo.deb -sSL http://nightly.odoo.com/${ODOO_VERSION}/nightly/deb/odoo_${ODOO_VERSION}.${ODOO_RELEASE}_all.deb     && echo "${ODOO_SHA} odoo.deb" | sha1sum -c -     && apt-get update     && apt-get -y install --no-install-recommends ./odoo.deb     && rm -rf /var/lib/apt/lists/* odoo.deb
# Tue, 21 Nov 2023 04:37:21 GMT
COPY file:cbe34bc5236465e4ed439e0c8f6504d2d221f79f7c70b37fe62b56662bd0ab6d in / 
# Tue, 21 Nov 2023 04:37:22 GMT
COPY file:1e7209cce5525d270c422815db614f496d4d0da4820de1ab0000e9e592223235 in /etc/odoo/ 
# Tue, 21 Nov 2023 04:37:23 GMT
# ARGS: ODOO_RELEASE=20231120 ODOO_SHA=57b836de2901c4ec5e3de433eb9258024701d255
RUN chown odoo /etc/odoo/odoo.conf     && mkdir -p /mnt/extra-addons     && chown -R odoo /mnt/extra-addons
# Tue, 21 Nov 2023 04:37:24 GMT
VOLUME [/var/lib/odoo /mnt/extra-addons]
# Tue, 21 Nov 2023 04:37:24 GMT
EXPOSE 8069 8071 8072
# Tue, 21 Nov 2023 04:37:24 GMT
ENV ODOO_RC=/etc/odoo/odoo.conf
# Tue, 21 Nov 2023 04:37:26 GMT
COPY file:0bc771c66dfeb517d19d13ea2699a0d3cbbbba684c8851640e6b87fe85b40619 in /usr/local/bin/wait-for-psql.py 
# Tue, 21 Nov 2023 04:37:27 GMT
USER odoo
# Tue, 21 Nov 2023 04:37:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 04:37:29 GMT
CMD ["odoo"]
```

-	Layers:
	-	`sha256:589c4cce1daa100afadbdbeda96025d02f85c117e0e60b70801af41b4e618668`  
		Last Modified: Fri, 13 Oct 2023 06:13:20 GMT  
		Size: 35.7 MB (35682793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff961ccf5729ac1f3c5d8b7806dd42fa9a9fbc4083f43b7d5bc3b9bbc166edbd`  
		Last Modified: Tue, 14 Nov 2023 01:28:59 GMT  
		Size: 245.9 MB (245927069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f6d3d2526a589659b9a531e4540bfd3bd343c49e9845f1409f5d7b12f7cca3`  
		Last Modified: Tue, 14 Nov 2023 01:28:17 GMT  
		Size: 2.8 MB (2803243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bc659a5b58234fbb32ee9ced616e815875a88f93489359a4f37bacad64bf54`  
		Last Modified: Tue, 14 Nov 2023 01:28:16 GMT  
		Size: 460.5 KB (460495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa87a1e6855f7991bb0b852407c1259aecc287aaa92688747b0a83a5914051`  
		Last Modified: Tue, 21 Nov 2023 04:44:03 GMT  
		Size: 326.8 MB (326785980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38fb051d6a2636dff68e579dd6d331587b6b1fd93ae93749396e6cc146d95f8`  
		Last Modified: Tue, 21 Nov 2023 04:43:20 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a545be1ff4fa26725caea8d93009850670d90b06669c660fdae6f5cbf6c66fb`  
		Last Modified: Tue, 21 Nov 2023 04:43:20 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8b650a97009bfa1a8feff40fe14603e739226de430d8e283f5c353279aff92`  
		Last Modified: Tue, 21 Nov 2023 04:43:20 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0565f9098b3ad31dd9b67f2af817bf716ca6c4d258d4f0f4a1a616e190f59df0`  
		Last Modified: Tue, 21 Nov 2023 04:43:20 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
