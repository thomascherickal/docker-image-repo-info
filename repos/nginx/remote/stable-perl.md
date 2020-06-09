## `nginx:stable-perl`

```console
$ docker pull nginx@sha256:b0fb0a3930343d9ebf3028ebc583f7e6974393ece20f495e1c383f26c6725a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `nginx:stable-perl` - linux; amd64

```console
$ docker pull nginx@sha256:4394b79fa1101a3c9eada8cbd65900c8d1a3fae423f09cddd3af0b066e0b78a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64246950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf56628552802d2b3c6c2d72f9f58c75126ce2c04ea7cfce8f6f65aba33fc2de`
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
# Fri, 15 May 2020 20:17:39 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Fri, 15 May 2020 20:17:40 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Fri, 15 May 2020 20:17:41 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Fri, 15 May 2020 20:17:41 GMT
EXPOSE 80
# Fri, 15 May 2020 20:17:41 GMT
STOPSIGNAL SIGTERM
# Fri, 15 May 2020 20:17:41 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861715223014d2410669601bacc67bc9e62c549a6d442d07acbaa8c5f85ab964`  
		Last Modified: Fri, 15 May 2020 20:19:01 GMT  
		Size: 37.1 MB (37147354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2990a0810be84544b132f8fa81ad323a1f2f4abf95b308546534ddac8a1c2133`  
		Last Modified: Fri, 15 May 2020 20:18:51 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c1f5db361d868f08a74f00a06ad2351b97d838135a8eb5eb736949fb565b67`  
		Last Modified: Fri, 15 May 2020 20:18:51 GMT  
		Size: 637.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; arm variant v7

```console
$ docker pull nginx@sha256:2dbc63667390ea3d03a1d38576a49fc4fb09515e863e927ef6fbbc1695a664d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (57014157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc111855d375b687fd843338a4bc972fceb3c23b7f8eec4f7bb69f98c4841d56`
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
# Fri, 15 May 2020 11:28:51 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Fri, 15 May 2020 11:28:56 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Fri, 15 May 2020 11:28:58 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Fri, 15 May 2020 11:28:58 GMT
EXPOSE 80
# Fri, 15 May 2020 11:28:59 GMT
STOPSIGNAL SIGTERM
# Fri, 15 May 2020 11:29:00 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51baeb0f2fb042ae85810b4246cc56fb5349244a47d043262c4f80bdf36ee354`  
		Last Modified: Fri, 15 May 2020 11:30:25 GMT  
		Size: 34.3 MB (34307390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107eeec2d5398f149099626d46087d3304288c986928e54a6fa627e3d03be021`  
		Last Modified: Fri, 15 May 2020 11:30:13 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4deefe67563eb310d0a7f0625e4f49b43076759c0299655978d4c63d5fa95a`  
		Last Modified: Fri, 15 May 2020 11:30:13 GMT  
		Size: 639.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:6f2d61a858e2af04f936a2432c34dce5ab579f701b6d178999f7c2dc5c0cc914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.9 MB (62914269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d156eb012b25374d30fe544e64d195772e6e903a056a30194b76b97602f3c0a7`
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
# Fri, 15 May 2020 23:01:09 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Fri, 15 May 2020 23:01:14 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Fri, 15 May 2020 23:01:17 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Fri, 15 May 2020 23:01:18 GMT
EXPOSE 80
# Fri, 15 May 2020 23:01:18 GMT
STOPSIGNAL SIGTERM
# Fri, 15 May 2020 23:01:19 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee59fb3a5cf74e364e6830d4ee9b7ecd1c7e12959dd59064407003c3705dd43`  
		Last Modified: Fri, 15 May 2020 23:03:11 GMT  
		Size: 37.1 MB (37056234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecea4d8bb236884b22d6330a04d98d4f58e1bff9f028fbb4d4f15af346f15bd1`  
		Last Modified: Fri, 15 May 2020 23:02:58 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85de8fbf8ba3aa8dbf225f45d22a2670d2f3d1891722b296afd459619a1ee81a`  
		Last Modified: Fri, 15 May 2020 23:02:57 GMT  
		Size: 639.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; 386

```console
$ docker pull nginx@sha256:9b45a0d7eceaf21fc37ff2c40be4d241ce34ecba7c94857e73a081dc8f6465d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65212494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24364b5a2a6952343aa868b2b69f7234305b3347ba4ca6583ec2f791f5c672f9`
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
# Tue, 09 Jun 2020 02:07:24 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Tue, 09 Jun 2020 02:07:25 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Tue, 09 Jun 2020 02:07:26 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Tue, 09 Jun 2020 02:07:26 GMT
EXPOSE 80
# Tue, 09 Jun 2020 02:07:26 GMT
STOPSIGNAL SIGTERM
# Tue, 09 Jun 2020 02:07:26 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:860f8957d8be856e2235a28e49fc4dca17254951e0eb67d760769755656f5cad`  
		Last Modified: Tue, 09 Jun 2020 01:45:01 GMT  
		Size: 27.8 MB (27754909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f855f6075cdd5480883088e3d13a19211698bd8bc4eb17f932c4639f3c6c2f`  
		Last Modified: Tue, 09 Jun 2020 02:08:50 GMT  
		Size: 37.5 MB (37456748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688a952628da7b7d501723b20a9c67a8452271715bb13835cd308f14e8b86fec`  
		Last Modified: Tue, 09 Jun 2020 02:08:42 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f036475ac07620edba09293bddea3ed744272e5ebe7a5ef9b72bc89808b5b59`  
		Last Modified: Tue, 09 Jun 2020 02:08:41 GMT  
		Size: 636.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; ppc64le

```console
$ docker pull nginx@sha256:9d9d6dcd8b8f6274b55c5167a6e72d25d9b16d08c21aaa9d65d6ef49fb46680d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69907466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b98161d2351a77a2b6016d305c7702e0a99548b70d3ae497690fea58dc6486`
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
# Fri, 29 May 2020 23:06:23 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Fri, 29 May 2020 23:06:37 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Fri, 29 May 2020 23:06:50 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Fri, 29 May 2020 23:06:54 GMT
EXPOSE 80
# Fri, 29 May 2020 23:07:00 GMT
STOPSIGNAL SIGTERM
# Fri, 29 May 2020 23:07:10 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac756470c454d151887972a3f77415687a4a18aeffd7686b2c4f37b90e664ee`  
		Last Modified: Fri, 29 May 2020 23:09:38 GMT  
		Size: 39.4 MB (39382165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f5a27f094ec742bfdd63e5910574110f95e94f4c0129d37aecf334f64b2c5c`  
		Last Modified: Fri, 29 May 2020 23:09:20 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8cf363f9be9d1ed0329d9d66a5cbb50cc218c774fb04ae432f7fe9eef01e75`  
		Last Modified: Fri, 29 May 2020 23:09:20 GMT  
		Size: 640.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; s390x

```console
$ docker pull nginx@sha256:081961c231a06a5a636da4cf616ff9b40f79c6dd8278127ca657083d3662688c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62794478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4f89199c7b732c628f57b145e6d7053a1e0f31a22049960998919e367d2a66`
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
# Fri, 15 May 2020 04:55:34 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi
# Fri, 15 May 2020 04:55:37 GMT
RUN ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log
# Fri, 15 May 2020 04:55:37 GMT
RUN sed -i -E 's,listen       80;,listen       80;\n    listen  [::]:80;,'         /etc/nginx/conf.d/default.conf
# Fri, 15 May 2020 04:55:37 GMT
EXPOSE 80
# Fri, 15 May 2020 04:55:38 GMT
STOPSIGNAL SIGTERM
# Fri, 15 May 2020 04:55:38 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:bdb298e230dde60bfce8a476ae8ea8988828f7ec9f5452f38f46102a609f57c1`  
		Last Modified: Thu, 14 May 2020 23:11:24 GMT  
		Size: 25.7 MB (25712933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cece491188eb2d303ebdf2c5c605c4188f88621e2c52ead69279f8a4d3dd01`  
		Last Modified: Fri, 15 May 2020 04:57:15 GMT  
		Size: 37.1 MB (37080704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbd1f950482d273b5ee7196619d3e99df11ed109a5740f3b09c8e2f4ad67ca9`  
		Last Modified: Fri, 15 May 2020 04:57:08 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e163a09d636f5f77c944dc57a7d0c624cc67ce11821882fac80ae48c280d47d6`  
		Last Modified: Fri, 15 May 2020 04:57:08 GMT  
		Size: 636.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
