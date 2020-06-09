## `nginx:latest`

```console
$ docker pull nginx@sha256:429818e435feb8d5d056c5bc70abe1f9ae8053f5ca433c5b14b98e2bad7e791d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `nginx:latest` - linux; amd64

```console
$ docker pull nginx@sha256:d9002da0297bcd0909b394c26bd0fc9d8c466caf2b7396f58948cac5318d0d0b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53311441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4392e5dad77dbaf6a573650b0fe1e282b57c5fba6e6cea00a27c7d4b68539b81`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:15:17 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 02 Jun 2020 00:35:23 GMT
ENV NGINX_VERSION=1.19.0
# Tue, 02 Jun 2020 00:35:23 GMT
ENV NJS_VERSION=0.4.1
# Tue, 02 Jun 2020 00:35:23 GMT
ENV PKG_RELEASE=1~buster
# Tue, 02 Jun 2020 00:35:44 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 02 Jun 2020 00:35:44 GMT
COPY file:d68fadb480cbc781c3424ce3e42e1b5be80133bdcce2569655e90411a4045da2 in / 
# Tue, 02 Jun 2020 16:23:39 GMT
COPY file:b96f664d94ca7bbe69241468d85ee421e9d310ffa36f3b04c762dcce9a42c7f1 in /docker-entrypoint.d 
# Tue, 02 Jun 2020 16:23:39 GMT
COPY file:cc7d4f1d03426ebd11e960d6a487961e0540059dcfad14b33762f008eed03788 in /docker-entrypoint.d 
# Tue, 02 Jun 2020 16:23:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 02 Jun 2020 16:23:40 GMT
EXPOSE 80
# Tue, 02 Jun 2020 16:23:40 GMT
STOPSIGNAL SIGTERM
# Tue, 02 Jun 2020 16:23:40 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3ac8106a0bbe43a6e55d2b719fc00a2f8f694e90c7903403e8fdecd2ccc57f`  
		Last Modified: Tue, 02 Jun 2020 00:37:12 GMT  
		Size: 26.2 MB (26210578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de28bdda69b66a8e07b14f03a9762f508bc4caac35cef9543bad53503ce5f53`  
		Last Modified: Tue, 02 Jun 2020 00:37:05 GMT  
		Size: 538.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c431ac2669038db7a758a597c7d1d53cdfb2dd9bf6de2ad3418973569b3fc7`  
		Last Modified: Tue, 02 Jun 2020 16:24:23 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e070d03fd1b5a05aafc7c16830d80b4ed622d546061fabac8163d3082098a849`  
		Last Modified: Tue, 02 Jun 2020 16:24:23 GMT  
		Size: 669.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:latest` - linux; arm variant v5

```console
$ docker pull nginx@sha256:1fbcb4fdaf707a94fb561e6d6ff8c46f0f7f29ef26094876edb9c91a859cf71d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (50030538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5aaab8be5c427d60dfb0d92872c1b90797259235c7a98b7e399e9c889b320da`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 09 Jun 2020 00:51:58 GMT
ADD file:7fde417d1c70a9ef2b4e468f6e2ee4cbd3f340fb2d5b67ede087c81520c95f4a in / 
# Tue, 09 Jun 2020 00:51:59 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:53:44 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 09 Jun 2020 02:53:45 GMT
ENV NGINX_VERSION=1.19.0
# Tue, 09 Jun 2020 02:53:45 GMT
ENV NJS_VERSION=0.4.1
# Tue, 09 Jun 2020 02:53:46 GMT
ENV PKG_RELEASE=1~buster
# Tue, 09 Jun 2020 03:01:08 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 09 Jun 2020 03:01:10 GMT
COPY file:d68fadb480cbc781c3424ce3e42e1b5be80133bdcce2569655e90411a4045da2 in / 
# Tue, 09 Jun 2020 03:01:11 GMT
COPY file:b96f664d94ca7bbe69241468d85ee421e9d310ffa36f3b04c762dcce9a42c7f1 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 03:01:12 GMT
COPY file:cc7d4f1d03426ebd11e960d6a487961e0540059dcfad14b33762f008eed03788 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 03:01:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jun 2020 03:01:13 GMT
EXPOSE 80
# Tue, 09 Jun 2020 03:01:14 GMT
STOPSIGNAL SIGTERM
# Tue, 09 Jun 2020 03:01:14 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:5b11fc09c1a26b11a7df7d593adf43baff53c5cdba71cf8a87ae4a6dd17eb52c`  
		Last Modified: Tue, 09 Jun 2020 00:59:24 GMT  
		Size: 24.8 MB (24837249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11db0758d67c846b2502b38845dd02e41f056aa7117cb9f8cbe72675c1a7416c`  
		Last Modified: Tue, 09 Jun 2020 03:09:10 GMT  
		Size: 25.2 MB (25191176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac677faec7093762814edc50b95f1b33267a5ff09f7a9fee82f42536d5ad5d61`  
		Last Modified: Tue, 09 Jun 2020 03:09:03 GMT  
		Size: 538.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f13969f6bd974488d742aae51f511517e9e07431608ecd11f4ce287b9bca9c3`  
		Last Modified: Tue, 09 Jun 2020 03:09:03 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92bf9633e93fa3df727711c61ae2cf639416a5a6be5af52858dcaa8d0ad62a2`  
		Last Modified: Tue, 09 Jun 2020 03:09:03 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:latest` - linux; arm variant v7

```console
$ docker pull nginx@sha256:f50820bdc7060dd598dc1125e8b307ec155f8224f5f72848c0f29c0ba82b06ce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47019946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afdbea96cc018661510a79b4aa6b2400472eb588b91fa6a42b579c896f5ddc30`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:24 GMT
ADD file:a35ca31d2a743d6a1738b1652f4f06c789abbca314d120f0e7e748311ac09ed2 in / 
# Tue, 09 Jun 2020 01:01:30 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 05:06:10 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 09 Jun 2020 05:06:10 GMT
ENV NGINX_VERSION=1.19.0
# Tue, 09 Jun 2020 05:06:11 GMT
ENV NJS_VERSION=0.4.1
# Tue, 09 Jun 2020 05:06:12 GMT
ENV PKG_RELEASE=1~buster
# Tue, 09 Jun 2020 05:11:57 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 09 Jun 2020 05:11:58 GMT
COPY file:d68fadb480cbc781c3424ce3e42e1b5be80133bdcce2569655e90411a4045da2 in / 
# Tue, 09 Jun 2020 05:11:59 GMT
COPY file:b96f664d94ca7bbe69241468d85ee421e9d310ffa36f3b04c762dcce9a42c7f1 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 05:12:00 GMT
COPY file:cc7d4f1d03426ebd11e960d6a487961e0540059dcfad14b33762f008eed03788 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 05:12:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jun 2020 05:12:03 GMT
EXPOSE 80
# Tue, 09 Jun 2020 05:12:04 GMT
STOPSIGNAL SIGTERM
# Tue, 09 Jun 2020 05:12:05 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:2dd003996c9ab82cac8112be0a4c04068e666e7a5d0cce3c65fb8f064de284e7`  
		Last Modified: Tue, 09 Jun 2020 01:10:25 GMT  
		Size: 22.7 MB (22705913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c8ecc5a54e755a16d8eee25663698006ac2d68889c8442cba00e7a09a03ab0`  
		Last Modified: Tue, 09 Jun 2020 05:32:36 GMT  
		Size: 24.3 MB (24311919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f4618322b8707dab36d3dd18c7780d966997fa63be475eedc5dafbc3a7e7e8`  
		Last Modified: Tue, 09 Jun 2020 05:32:30 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9582d2ded4d43436a287e1fe788c5e208ef1de591bbde6cdebfe7704ec96afbf`  
		Last Modified: Tue, 09 Jun 2020 05:32:30 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def5636789fe51b3070426a92327637eeb0146a849c5f63f6ea7e84e9a3c8eef`  
		Last Modified: Tue, 09 Jun 2020 05:32:30 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:latest` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:b84fef817adb07964c630b574e6eee45bd156dd1cbb2f257ff570d7339cd1417
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52050780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:274c632b9f1369646d70354ea132c3da870027f99d53efcc3cd0b5377c9af086`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 09 Jun 2020 01:52:01 GMT
ADD file:98823648634dfc3af50862b1e2da1028b23996a37adf43b1b0c3c5b29e94b9c7 in / 
# Tue, 09 Jun 2020 01:52:04 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:41:05 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 09 Jun 2020 03:41:05 GMT
ENV NGINX_VERSION=1.19.0
# Tue, 09 Jun 2020 03:41:06 GMT
ENV NJS_VERSION=0.4.1
# Tue, 09 Jun 2020 03:41:07 GMT
ENV PKG_RELEASE=1~buster
# Tue, 09 Jun 2020 03:47:43 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 09 Jun 2020 03:47:45 GMT
COPY file:d68fadb480cbc781c3424ce3e42e1b5be80133bdcce2569655e90411a4045da2 in / 
# Tue, 09 Jun 2020 03:47:45 GMT
COPY file:b96f664d94ca7bbe69241468d85ee421e9d310ffa36f3b04c762dcce9a42c7f1 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 03:47:46 GMT
COPY file:cc7d4f1d03426ebd11e960d6a487961e0540059dcfad14b33762f008eed03788 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 03:47:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jun 2020 03:47:48 GMT
EXPOSE 80
# Tue, 09 Jun 2020 03:47:49 GMT
STOPSIGNAL SIGTERM
# Tue, 09 Jun 2020 03:47:50 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:33cc09c9b190539635d7c971301f623d94fda5b4b5647966c6c240902119009f`  
		Last Modified: Tue, 09 Jun 2020 01:58:14 GMT  
		Size: 25.9 MB (25857704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6db46e5e452143e36eb9e331cf02b1aea52256d1ed5b4255ab1b095e0e0c741`  
		Last Modified: Tue, 09 Jun 2020 04:09:56 GMT  
		Size: 26.2 MB (26190961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e6b96caf5032d43265249f4943ec16002128646075d8bc7912f30028ec84`  
		Last Modified: Tue, 09 Jun 2020 04:09:49 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79409b429d69a5eea1e362d5f1a7cf8fd057e1d311b88698aedc8f3b02887133`  
		Last Modified: Tue, 09 Jun 2020 04:09:49 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb76351c1fc020f34b1160d8922078d33e2c5b12a3fbb079d5117b601dd20782`  
		Last Modified: Tue, 09 Jun 2020 04:09:49 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:latest` - linux; 386

```console
$ docker pull nginx@sha256:4662d289082e30f7745fe7c59c3c24a04857081658aa9a983876fcf4d3457172
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54782222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ee507228744dedc584f72d9aed574fcb5068e709f011c4290bbde139024a303`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 09 Jun 2020 01:39:49 GMT
ADD file:9fb8fd8bf970c4134f555964fe485a3baa84f1d4c91c5aa35276c24404de9d5d in / 
# Tue, 09 Jun 2020 01:39:49 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:05:05 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 09 Jun 2020 02:05:05 GMT
ENV NGINX_VERSION=1.19.0
# Tue, 09 Jun 2020 02:05:05 GMT
ENV NJS_VERSION=0.4.1
# Tue, 09 Jun 2020 02:05:06 GMT
ENV PKG_RELEASE=1~buster
# Tue, 09 Jun 2020 02:05:32 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 09 Jun 2020 02:05:32 GMT
COPY file:d68fadb480cbc781c3424ce3e42e1b5be80133bdcce2569655e90411a4045da2 in / 
# Tue, 09 Jun 2020 02:05:32 GMT
COPY file:b96f664d94ca7bbe69241468d85ee421e9d310ffa36f3b04c762dcce9a42c7f1 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 02:05:33 GMT
COPY file:cc7d4f1d03426ebd11e960d6a487961e0540059dcfad14b33762f008eed03788 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 02:05:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jun 2020 02:05:33 GMT
EXPOSE 80
# Tue, 09 Jun 2020 02:05:33 GMT
STOPSIGNAL SIGTERM
# Tue, 09 Jun 2020 02:05:33 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:860f8957d8be856e2235a28e49fc4dca17254951e0eb67d760769755656f5cad`  
		Last Modified: Tue, 09 Jun 2020 01:45:01 GMT  
		Size: 27.8 MB (27754909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570d9b2830b5113cd9b1de06ecbe0618fed498993637b36609d2b4733e641c9a`  
		Last Modified: Tue, 09 Jun 2020 02:08:08 GMT  
		Size: 27.0 MB (27025204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325fa6842ba0e2888708f4e3bd1638f8556133abe050f047381dbd79c7fd89f5`  
		Last Modified: Tue, 09 Jun 2020 02:08:02 GMT  
		Size: 538.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7257433c5bf561035b93e1a1e994060cce191e59d802e21ec9a38948a0213ee6`  
		Last Modified: Tue, 09 Jun 2020 02:08:03 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89379a5d8bc7d1a71c6443bad9eb23bbbc4c288359fb5b3110c8307c96f8fc9`  
		Last Modified: Tue, 09 Jun 2020 02:08:02 GMT  
		Size: 668.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:latest` - linux; mips64le

```console
$ docker pull nginx@sha256:6d73b8284d351c649a33827d46c9835d73aca9f8df4903607319880e0d4b7194
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51589231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3304d2e610f312ad5c657763ddb02a5fb3d96d618ac1598c1e318e1a51cee2d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 09 Jun 2020 01:10:06 GMT
ADD file:faf18b832680e98050b98c329add242425904e64c6a5a491c22d33e9417ef323 in / 
# Tue, 09 Jun 2020 01:10:06 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 03:01:01 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 09 Jun 2020 03:01:02 GMT
ENV NGINX_VERSION=1.19.0
# Tue, 09 Jun 2020 03:01:02 GMT
ENV NJS_VERSION=0.4.1
# Tue, 09 Jun 2020 03:01:02 GMT
ENV PKG_RELEASE=1~buster
# Tue, 09 Jun 2020 03:13:00 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 09 Jun 2020 03:13:01 GMT
COPY file:d68fadb480cbc781c3424ce3e42e1b5be80133bdcce2569655e90411a4045da2 in / 
# Tue, 09 Jun 2020 03:13:01 GMT
COPY file:b96f664d94ca7bbe69241468d85ee421e9d310ffa36f3b04c762dcce9a42c7f1 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 03:13:02 GMT
COPY file:cc7d4f1d03426ebd11e960d6a487961e0540059dcfad14b33762f008eed03788 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 03:13:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jun 2020 03:13:02 GMT
EXPOSE 80
# Tue, 09 Jun 2020 03:13:03 GMT
STOPSIGNAL SIGTERM
# Tue, 09 Jun 2020 03:13:03 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:76f2a0c8ea98ebd699a77ced9c677e97cd54b038a8c5e89670af78f38b047b33`  
		Last Modified: Tue, 09 Jun 2020 01:18:14 GMT  
		Size: 25.8 MB (25764040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4274d1b4d0e247410e206d3ccf485daa43e1fa388225be3a7c9f5004c135a409`  
		Last Modified: Tue, 09 Jun 2020 03:27:05 GMT  
		Size: 25.8 MB (25823080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046b55484cb3212540e904d04e48423cbc01cdcb1613e2e69178d2196c228b6f`  
		Last Modified: Tue, 09 Jun 2020 03:26:44 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8770f1667f910c496a2ff60404f1d23005615cc24f997a52ef89e053a55e13c9`  
		Last Modified: Tue, 09 Jun 2020 03:26:43 GMT  
		Size: 903.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e6b3c607e2658a0ba2b4f8d4a0b8efa5dad806c7574de9a2aa4c5a02e04d35`  
		Last Modified: Tue, 09 Jun 2020 03:26:43 GMT  
		Size: 669.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:latest` - linux; ppc64le

```console
$ docker pull nginx@sha256:05799da84dd225a188c63e07c3451abd26e54de82c2241004b49488c57ef76fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.7 MB (58732946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95eb6204041395da1b7d097e79982685129ce7344a8f47e79c0fa441b20429db`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 09 Jun 2020 01:22:34 GMT
ADD file:796aad1a35ba276b8cccc19987c152a713db101b2b65e30923db753f5b7f4b0f in / 
# Tue, 09 Jun 2020 01:22:38 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 09:06:40 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 09 Jun 2020 09:06:48 GMT
ENV NGINX_VERSION=1.19.0
# Tue, 09 Jun 2020 09:06:54 GMT
ENV NJS_VERSION=0.4.1
# Tue, 09 Jun 2020 09:07:02 GMT
ENV PKG_RELEASE=1~buster
# Tue, 09 Jun 2020 09:30:07 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 09 Jun 2020 09:30:11 GMT
COPY file:d68fadb480cbc781c3424ce3e42e1b5be80133bdcce2569655e90411a4045da2 in / 
# Tue, 09 Jun 2020 09:30:13 GMT
COPY file:b96f664d94ca7bbe69241468d85ee421e9d310ffa36f3b04c762dcce9a42c7f1 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 09:30:15 GMT
COPY file:cc7d4f1d03426ebd11e960d6a487961e0540059dcfad14b33762f008eed03788 in /docker-entrypoint.d 
# Tue, 09 Jun 2020 09:30:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jun 2020 09:30:34 GMT
EXPOSE 80
# Tue, 09 Jun 2020 09:30:42 GMT
STOPSIGNAL SIGTERM
# Tue, 09 Jun 2020 09:30:49 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:63dbb66c5119bb5086d9e6fb6b154211afc20b44ed136ab7df808f6044cfc6f1`  
		Last Modified: Tue, 09 Jun 2020 01:31:04 GMT  
		Size: 30.5 MB (30524405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c6436f9affad5d3b5bfe512fed6aed5ba1fdb1756764eae20fcae03969ac0f`  
		Last Modified: Tue, 09 Jun 2020 10:34:48 GMT  
		Size: 28.2 MB (28206426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a682b08bf584e6d6a1934f40cb042e9063624f69f9283458d9841a53dd965d01`  
		Last Modified: Tue, 09 Jun 2020 10:34:42 GMT  
		Size: 538.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455ff3bbd8a1313aee46a586fcf43bf53cf09dc8d6ce1750f8e7fae9c0ea62a6`  
		Last Modified: Tue, 09 Jun 2020 10:34:42 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da845f35b6da970f223c80c6d66882118505f90580a97228d24ebd0f742e86d`  
		Last Modified: Tue, 09 Jun 2020 10:34:42 GMT  
		Size: 673.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:latest` - linux; s390x

```console
$ docker pull nginx@sha256:971a1b5f03103df52a6412c43cd841bdf431d2f000cf43e8aa9f85c90aac2202
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51561996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120f1bf01b9d08eaddac444b4f96fa0a6c5fbe4bf25f481cf1145580bee399e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Thu, 14 May 2020 23:06:40 GMT
ADD file:a29e647b8dccf726d8610d8c599d6727d6145426f9374720b985fc9be9ac906c in / 
# Thu, 14 May 2020 23:06:41 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:45:39 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 02 Jun 2020 00:42:41 GMT
ENV NGINX_VERSION=1.19.0
# Tue, 02 Jun 2020 00:42:41 GMT
ENV NJS_VERSION=0.4.1
# Tue, 02 Jun 2020 00:42:41 GMT
ENV PKG_RELEASE=1~buster
# Tue, 02 Jun 2020 00:45:01 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 02 Jun 2020 00:45:02 GMT
COPY file:d68fadb480cbc781c3424ce3e42e1b5be80133bdcce2569655e90411a4045da2 in / 
# Tue, 02 Jun 2020 16:44:19 GMT
COPY file:b96f664d94ca7bbe69241468d85ee421e9d310ffa36f3b04c762dcce9a42c7f1 in /docker-entrypoint.d 
# Tue, 02 Jun 2020 16:44:19 GMT
COPY file:cc7d4f1d03426ebd11e960d6a487961e0540059dcfad14b33762f008eed03788 in /docker-entrypoint.d 
# Tue, 02 Jun 2020 16:44:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 02 Jun 2020 16:44:19 GMT
EXPOSE 80
# Tue, 02 Jun 2020 16:44:20 GMT
STOPSIGNAL SIGTERM
# Tue, 02 Jun 2020 16:44:20 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:bdb298e230dde60bfce8a476ae8ea8988828f7ec9f5452f38f46102a609f57c1`  
		Last Modified: Thu, 14 May 2020 23:11:24 GMT  
		Size: 25.7 MB (25712933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb34024551c8d5b5d5cb3a0ae114d73e1ccc870a5b7476ae3f30a5dda6801e4`  
		Last Modified: Tue, 02 Jun 2020 00:51:38 GMT  
		Size: 25.8 MB (25846961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff57510e6e0e811c118d42fd8a320ec310705c4d6c9b3845749ba6d496a901f`  
		Last Modified: Tue, 02 Jun 2020 00:51:39 GMT  
		Size: 536.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cef171c6128d9c99cac81ddbdce683c5ec191e9d154786ce318df84d2d121b3`  
		Last Modified: Tue, 02 Jun 2020 16:45:06 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7b9a8a1f8e9046a1d316d4c043c0fbafde79e69c40a370d5a57592422cdd46`  
		Last Modified: Tue, 02 Jun 2020 16:45:11 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
