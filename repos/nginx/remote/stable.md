## `nginx:stable`

```console
$ docker pull nginx@sha256:2bacdb5787f1252cc04956507f69ea5874ff0cb193f4ff6bffc22e0f6b85963a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `nginx:stable` - linux; amd64

```console
$ docker pull nginx@sha256:637488545a21a1ff771549ef65f5e3c1a8dbd92c98d360ac489d76b857021a55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53301036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:741d47c34fe04ee2b25098e547a9337b3793ae3aa26479231f90489a273a3775`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:15:17 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 15 May 2020 20:16:45 GMT
ENV NGINX_VERSION=1.18.0
# Fri, 15 May 2020 20:16:45 GMT
ENV NJS_VERSION=0.4.0
# Fri, 15 May 2020 20:16:45 GMT
ENV PKG_RELEASE=1~buster
# Fri, 15 May 2020 20:17:07 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Fri, 15 May 2020 20:17:08 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Fri, 15 May 2020 20:17:09 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Fri, 15 May 2020 20:17:09 GMT
EXPOSE 80
# Fri, 15 May 2020 20:17:09 GMT
STOPSIGNAL SIGTERM
# Fri, 15 May 2020 20:17:09 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e231683bfde7f6cdb860dcaf855c8aaf8a4cdb83ab8dd345ab35e8d5a2e421a`  
		Last Modified: Fri, 15 May 2020 20:18:46 GMT  
		Size: 26.2 MB (26201443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511e2efefada0b20168024e58d73b3c5dcaa71383f77461c4be74d742838f5df`  
		Last Modified: Fri, 15 May 2020 20:18:39 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fd0ec105c9a0ba769b2357195c0842fddf670c55f9e6a4a5f55d6fa61311d5`  
		Last Modified: Fri, 15 May 2020 20:18:39 GMT  
		Size: 635.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; arm variant v7

```console
$ docker pull nginx@sha256:68bc48771b541fe22a485f533fbe7b7d44241429258abad6ada1d8022bc91e36
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47006660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:881df77f54aae4b098f01aa4bac8c9e894afb02a9b70df001d0eb878f6a63c60`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:03:38 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 15 May 2020 11:16:27 GMT
ENV NGINX_VERSION=1.18.0
# Fri, 15 May 2020 11:16:28 GMT
ENV NJS_VERSION=0.4.0
# Fri, 15 May 2020 11:16:29 GMT
ENV PKG_RELEASE=1~buster
# Fri, 15 May 2020 11:22:15 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Fri, 15 May 2020 11:22:18 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Fri, 15 May 2020 11:22:20 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Fri, 15 May 2020 11:22:21 GMT
EXPOSE 80
# Fri, 15 May 2020 11:22:21 GMT
STOPSIGNAL SIGTERM
# Fri, 15 May 2020 11:22:22 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b813a80a71ff84fbd570f7689dd2cb51971e43278e1a67ff11385d2096875985`  
		Last Modified: Fri, 15 May 2020 11:30:06 GMT  
		Size: 24.3 MB (24299895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9231303c4a788cccd88a1193480aee03d45b31f2011bed3f27e6515587b969bc`  
		Last Modified: Fri, 15 May 2020 11:29:59 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0629cd7159130370cb7c316cbd3ba96f7e236748863d6c4a3afebcf1e33586`  
		Last Modified: Fri, 15 May 2020 11:29:59 GMT  
		Size: 636.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:0fadadf3afe8d2f13065a9503659ad8f66a1c0c338c76f3a59820360969c7530
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52041650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cefed706feb990b52ab0c766249cfc46dc70291a82408fef0b9cffb5ecfbb627`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 22:21:42 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 15 May 2020 22:42:13 GMT
ENV NGINX_VERSION=1.18.0
# Fri, 15 May 2020 22:42:22 GMT
ENV NJS_VERSION=0.4.0
# Fri, 15 May 2020 22:42:33 GMT
ENV PKG_RELEASE=1~buster
# Fri, 15 May 2020 22:49:59 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Fri, 15 May 2020 22:50:14 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Fri, 15 May 2020 22:50:21 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Fri, 15 May 2020 22:51:27 GMT
EXPOSE 80
# Fri, 15 May 2020 22:51:52 GMT
STOPSIGNAL SIGTERM
# Fri, 15 May 2020 22:52:24 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c5df0018cf998028ce92658c3f6bb2ed719aba04125c19eeeab501b66b98ea`  
		Last Modified: Fri, 15 May 2020 23:02:50 GMT  
		Size: 26.2 MB (26183612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a69f01e71255d861a7a5bce9bc8ea708d2644ea5b6c23b49b5f1566b493ee0c`  
		Last Modified: Fri, 15 May 2020 23:02:44 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48604f1285e0eb6b75408bf83d8f84b2bef9bdb6b019d390d334cf404785014`  
		Last Modified: Fri, 15 May 2020 23:02:44 GMT  
		Size: 640.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; 386

```console
$ docker pull nginx@sha256:457e3302a9e44da6076d9d6d11e050db25ae4a144c97b908d512938abef296b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54771443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a044d2b554e5c47d8c44f5c77b40be9ba2ef29166975b3d02b96fd7b9935233`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:49 GMT
ADD file:9fb8fd8bf970c4134f555964fe485a3baa84f1d4c91c5aa35276c24404de9d5d in / 
# Tue, 09 Jun 2020 01:39:49 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:05:05 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 09 Jun 2020 02:06:21 GMT
ENV NGINX_VERSION=1.18.0
# Tue, 09 Jun 2020 02:06:21 GMT
ENV NJS_VERSION=0.4.0
# Tue, 09 Jun 2020 02:06:21 GMT
ENV PKG_RELEASE=1~buster
# Tue, 09 Jun 2020 02:06:47 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Tue, 09 Jun 2020 02:06:47 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Tue, 09 Jun 2020 02:06:48 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Tue, 09 Jun 2020 02:06:49 GMT
EXPOSE 80
# Tue, 09 Jun 2020 02:06:49 GMT
STOPSIGNAL SIGTERM
# Tue, 09 Jun 2020 02:06:49 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:860f8957d8be856e2235a28e49fc4dca17254951e0eb67d760769755656f5cad`  
		Last Modified: Tue, 09 Jun 2020 01:45:01 GMT  
		Size: 27.8 MB (27754909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dab8728e0c15e6338dbe35a5725bba91c74c66b6915405ce3b5591255896091`  
		Last Modified: Tue, 09 Jun 2020 02:08:37 GMT  
		Size: 27.0 MB (27015697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b419eb6dcc8f410441f8587e4f3b60c537e808f38d89a598dc157377315c31f`  
		Last Modified: Tue, 09 Jun 2020 02:08:31 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de035da832d4a0a732010b3797c177abee8fa6d278a29d81689cd65b5661af09`  
		Last Modified: Tue, 09 Jun 2020 02:08:31 GMT  
		Size: 637.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; ppc64le

```console
$ docker pull nginx@sha256:fb2b5f9f9b64ab4657d765494aec6544aab35f82fed8ccd37a37168e403ddad2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.7 MB (58719670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c19142a97f0602922ee66494cc76a62e1ca0912b0a4b745fb3575c7902f7583`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Fri, 29 May 2020 22:02:25 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 29 May 2020 22:24:13 GMT
ENV NGINX_VERSION=1.18.0
# Fri, 29 May 2020 22:24:15 GMT
ENV NJS_VERSION=0.4.0
# Fri, 29 May 2020 22:24:17 GMT
ENV PKG_RELEASE=1~buster
# Fri, 29 May 2020 22:34:10 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Fri, 29 May 2020 22:34:17 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Fri, 29 May 2020 22:34:21 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Fri, 29 May 2020 22:34:24 GMT
EXPOSE 80
# Fri, 29 May 2020 22:34:25 GMT
STOPSIGNAL SIGTERM
# Fri, 29 May 2020 22:34:27 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f52a25fba07dc2e40e248b22cf52f59dbcd25ffe415ab2e7fac55f0d71aa36`  
		Last Modified: Fri, 29 May 2020 23:09:06 GMT  
		Size: 28.2 MB (28194372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cbaf13d25b513e336917cbae68db25e5f289fdfe417f762e9e8ec8ca1ac309`  
		Last Modified: Fri, 29 May 2020 23:08:58 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70594219fbc033749cc828da5a06da1e66551d37a3cbaa0233dc7229a724aa9`  
		Last Modified: Fri, 29 May 2020 23:08:58 GMT  
		Size: 640.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; s390x

```console
$ docker pull nginx@sha256:c5c5e1fdd9760833e917ac26a45671ea63ee8a5790a53c2b774a3ca52cae90e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51543984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7922e6ee495a261f9412de1cd934c48bf9e0793b30bace1c8cb2ad5bd7d834a`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Thu, 14 May 2020 23:06:40 GMT
ADD file:a29e647b8dccf726d8610d8c599d6727d6145426f9374720b985fc9be9ac906c in / 
# Thu, 14 May 2020 23:06:41 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:45:39 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 15 May 2020 04:50:56 GMT
ENV NGINX_VERSION=1.18.0
# Fri, 15 May 2020 04:50:56 GMT
ENV NJS_VERSION=0.4.0
# Fri, 15 May 2020 04:50:57 GMT
ENV PKG_RELEASE=1~buster
# Fri, 15 May 2020 04:53:05 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Fri, 15 May 2020 04:53:07 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Fri, 15 May 2020 04:53:07 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Fri, 15 May 2020 04:53:08 GMT
EXPOSE 80
# Fri, 15 May 2020 04:53:08 GMT
STOPSIGNAL SIGTERM
# Fri, 15 May 2020 04:53:08 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:bdb298e230dde60bfce8a476ae8ea8988828f7ec9f5452f38f46102a609f57c1`  
		Last Modified: Thu, 14 May 2020 23:11:24 GMT  
		Size: 25.7 MB (25712933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f380deb3fa09bc60740aa5cc6bde74b2774d1533dff6f68594e1efb5fdb1580e`  
		Last Modified: Fri, 15 May 2020 04:56:57 GMT  
		Size: 25.8 MB (25830214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d622918d933a41aa8856212964dfb09e744b61554e75c5d6628ce462be1d8d36`  
		Last Modified: Fri, 15 May 2020 04:56:53 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29b3d739661ded33d68c469a377b9848586197d4d6d398eb22b88b93fc7f24f`  
		Last Modified: Fri, 15 May 2020 04:56:59 GMT  
		Size: 635.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
