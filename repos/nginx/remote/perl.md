## `nginx:perl`

```console
$ docker pull nginx@sha256:2473d836bd6b0adbca73dfffbf66e6aac9864dd9f1fc41c403701a7e3002fbeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `nginx:perl` - linux; amd64

```console
$ docker pull nginx@sha256:81a8931d346812c913b06aac33e4ef68b03c1603b3f0aeb51984666bd958e553
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67914262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:942a2f7928176bb09831500eacee4e71ecbfd025acff4c8fee428327a6967bc5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:17:00 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 02 Aug 2022 05:17:00 GMT
ENV NGINX_VERSION=1.23.1
# Tue, 02 Aug 2022 05:17:00 GMT
ENV NJS_VERSION=0.7.6
# Tue, 02 Aug 2022 05:17:00 GMT
ENV PKG_RELEASE=1~bullseye
# Tue, 02 Aug 2022 05:17:43 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 02 Aug 2022 05:17:43 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 02 Aug 2022 05:17:43 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 02 Aug 2022 05:17:43 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 02 Aug 2022 05:17:43 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 02 Aug 2022 05:17:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 05:17:43 GMT
EXPOSE 80
# Tue, 02 Aug 2022 05:17:44 GMT
STOPSIGNAL SIGQUIT
# Tue, 02 Aug 2022 05:17:44 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefeb3d229238e49e78fd8bf9b5c6b4262a5b869ba1e58550a53d29ebc995752`  
		Last Modified: Tue, 02 Aug 2022 05:19:40 GMT  
		Size: 36.5 MB (36543949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb222bdf1dc531b28bc73ddf2a43728d284a22e1f534a38bab1ca22a0c6bf181`  
		Last Modified: Tue, 02 Aug 2022 05:19:34 GMT  
		Size: 601.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b2e6ad20eea13b8b3caaa56b00a096ed762adeca6258befa5d067e92405653`  
		Last Modified: Tue, 02 Aug 2022 05:19:34 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea8baab01d6e231664ea64b63e391c42829854d879b5abe0a81f023490ace26`  
		Last Modified: Tue, 02 Aug 2022 05:19:34 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a13b84b2f0d86e15a300733280cd58e3b867bd1faa4fe85965da03319ca3921`  
		Last Modified: Tue, 02 Aug 2022 05:19:34 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; arm variant v5

```console
$ docker pull nginx@sha256:075fcb732c06a2e1d91cd00afd0df4d57e93b9590f5b24650c4489c0938026ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63849298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3120870f9034652d3b0c843382216ead11b69c594b333ae027721baebd4b1c0d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 02 Aug 2022 00:49:10 GMT
ADD file:4cd2f95737fd3007912428eeac56036c9e67e989e66cec08a8be99da47f88494 in / 
# Tue, 02 Aug 2022 00:49:10 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:13:51 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 02 Aug 2022 02:13:51 GMT
ENV NGINX_VERSION=1.23.1
# Tue, 02 Aug 2022 02:13:51 GMT
ENV NJS_VERSION=0.7.6
# Tue, 02 Aug 2022 02:13:52 GMT
ENV PKG_RELEASE=1~bullseye
# Tue, 02 Aug 2022 02:24:29 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 02 Aug 2022 02:24:29 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 02 Aug 2022 02:24:29 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 02 Aug 2022 02:24:29 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 02 Aug 2022 02:24:29 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 02 Aug 2022 02:24:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 02:24:29 GMT
EXPOSE 80
# Tue, 02 Aug 2022 02:24:30 GMT
STOPSIGNAL SIGQUIT
# Tue, 02 Aug 2022 02:24:30 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:5890b0ca6af5e8467a488e68716691950496a8f247d0495c2d595ddcb1893aff`  
		Last Modified: Tue, 02 Aug 2022 00:56:06 GMT  
		Size: 28.9 MB (28905515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e2e3da4979850487c31c688885fc47bee99c73979031804ebb32b6621034fe`  
		Last Modified: Tue, 02 Aug 2022 02:34:01 GMT  
		Size: 34.9 MB (34940222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e9dcb0b07c995167c023679653280b8b7a84769a27798c7e6bbb64d1739c5f`  
		Last Modified: Tue, 02 Aug 2022 02:33:51 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47384addcba595697bca68bbc875e46f57b0f18176457c2c18399adc88d0861c`  
		Last Modified: Tue, 02 Aug 2022 02:33:51 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47e0228aea4c341b5044d1ca8e11adc8f0bcdefbd83d7e94299c640ffda8e1c`  
		Last Modified: Tue, 02 Aug 2022 02:33:51 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb84ce5381a2edd42c4b2aae7255b748cd27d1ecf7c7c7f7b2c8aa964e2e5bc1`  
		Last Modified: Tue, 02 Aug 2022 02:33:51 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; arm variant v7

```console
$ docker pull nginx@sha256:68f22ac74df854b4eb131c2d8a0b15692f359214bc61df6a486b418ea0ba346c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60476199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4be8fe03abf4edb8679c628280ddb5acb3a0d87e8cd77b7a41e1da33a0da0848`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:13:05 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 19 Jul 2022 18:58:12 GMT
ENV NGINX_VERSION=1.23.1
# Tue, 19 Jul 2022 18:58:13 GMT
ENV NJS_VERSION=0.7.6
# Tue, 19 Jul 2022 18:58:13 GMT
ENV PKG_RELEASE=1~bullseye
# Tue, 19 Jul 2022 19:17:02 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 19 Jul 2022 19:17:03 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 19 Jul 2022 19:17:04 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 19 Jul 2022 19:17:04 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 19 Jul 2022 19:17:05 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 19 Jul 2022 19:17:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 19 Jul 2022 19:17:06 GMT
EXPOSE 80
# Tue, 19 Jul 2022 19:17:06 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Jul 2022 19:17:06 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d1ea7ecdfcb68d939d4bcb674c8266ba81b5ab240429503c2e13bae66dfcc`  
		Last Modified: Tue, 19 Jul 2022 20:10:24 GMT  
		Size: 33.9 MB (33912078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7f7f5c6f76e7ef4a89f5cee1fc9d2575fc304485df168cea7005e0f4b2ff5f`  
		Last Modified: Tue, 19 Jul 2022 20:10:01 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169a1822377921866985cdf23357a2d7eb5f1db0559edd0b60484b9d050830a6`  
		Last Modified: Tue, 19 Jul 2022 20:10:01 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa77c2fd04edf1a89c9f76dfb4baa74b91981d8a49c9a7ac31614c3e56dac368`  
		Last Modified: Tue, 19 Jul 2022 20:10:01 GMT  
		Size: 668.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ebe36daf04528409cd4d2b4ced3bccbc9c4d9f4bc5cd09a86e4f00ab2e1534`  
		Last Modified: Tue, 19 Jul 2022 20:10:01 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:8310242cbdde2f398cc1e151c94c26275aec0ba388ffc00a4040bafb3586596a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66434272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4ad6a2ac74967c1d2f368602d5339fb566a24df68ce183fb05df666cdded8be`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:14:23 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 02 Aug 2022 04:14:24 GMT
ENV NGINX_VERSION=1.23.1
# Tue, 02 Aug 2022 04:14:25 GMT
ENV NJS_VERSION=0.7.6
# Tue, 02 Aug 2022 04:14:26 GMT
ENV PKG_RELEASE=1~bullseye
# Tue, 02 Aug 2022 04:15:19 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 02 Aug 2022 04:15:20 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 02 Aug 2022 04:15:21 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 02 Aug 2022 04:15:22 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 02 Aug 2022 04:15:23 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 02 Aug 2022 04:15:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 04:15:24 GMT
EXPOSE 80
# Tue, 02 Aug 2022 04:15:25 GMT
STOPSIGNAL SIGQUIT
# Tue, 02 Aug 2022 04:15:26 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcff169f006c018710eaefa4c0d4709eebcb31bc348ab0a35a7e7ddeb38ff27c`  
		Last Modified: Tue, 02 Aug 2022 04:18:20 GMT  
		Size: 36.4 MB (36376414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c1e2e9e365c180c0aa1fd33b8c3730b127d4c4f60d0a5e5e7f988d488e9f46`  
		Last Modified: Tue, 02 Aug 2022 04:18:14 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff81e8786693b9fd9f3ce30ba65bba312f97e2a28817e743a246ad0711e9e99`  
		Last Modified: Tue, 02 Aug 2022 04:18:14 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf1a12e3cf15f3df21b278a7aa4f4c2ea38c9de5c7ef9b8332b2a90f1b9511d`  
		Last Modified: Tue, 02 Aug 2022 04:18:15 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b03f5c82f6d4b186672e43a2795750f40f22fb8c313bc5551c303b23009e48`  
		Last Modified: Tue, 02 Aug 2022 04:18:15 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; 386

```console
$ docker pull nginx@sha256:08e8ecb7e1d2894fc986732c855f0df42f510e5e96a88616e0390dcf95216828
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69324467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d0efcd56b4bf1d75faf7087f4ed637df3a45a6c9694ab8269fcce6ba7c3fc3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 16:00:03 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 02 Aug 2022 16:00:04 GMT
ENV NGINX_VERSION=1.23.1
# Tue, 02 Aug 2022 16:00:05 GMT
ENV NJS_VERSION=0.7.6
# Tue, 02 Aug 2022 16:00:06 GMT
ENV PKG_RELEASE=1~bullseye
# Tue, 02 Aug 2022 16:07:07 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 02 Aug 2022 16:07:08 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 02 Aug 2022 16:07:09 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 02 Aug 2022 16:07:10 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 02 Aug 2022 16:07:11 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 02 Aug 2022 16:07:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 16:07:12 GMT
EXPOSE 80
# Tue, 02 Aug 2022 16:07:13 GMT
STOPSIGNAL SIGQUIT
# Tue, 02 Aug 2022 16:07:14 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3326d89a8492297a0d109eba906f408ab6372377bad9da7b7dda6442de743fbb`  
		Last Modified: Tue, 02 Aug 2022 16:17:17 GMT  
		Size: 36.9 MB (36946853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485c460c8c6dce037849d1109a202ce48526468d4a82eb0976d21ec36ed3da9a`  
		Last Modified: Tue, 02 Aug 2022 16:17:10 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fd8835a19adc6f196305994191b2135641db1588b42c630f3f682572322cc8`  
		Last Modified: Tue, 02 Aug 2022 16:17:10 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e23f4c4424b84b8cf7ce59cbc3e51cef9efd5011d10468ce2ff5bfb3cdc2691`  
		Last Modified: Tue, 02 Aug 2022 16:17:10 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3529666ebf637d30703ab91703af06ccb0286a1847a49b4fcb00f62db9e1018`  
		Last Modified: Tue, 02 Aug 2022 16:17:10 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; mips64le

```console
$ docker pull nginx@sha256:e9aa8b134246b9c4d6df00357e28bafcaabd3eab48285f88e4a31c22ce4335c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65335253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c82058a2d19e4304a0db6f6f9d1b6649baa8f08a2a1fbd2021465a3cb5f15348`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 02 Aug 2022 01:10:34 GMT
ADD file:6dc22a1e5b5fcf23f2549406ddcc45c4e244f46e21eafa881de81fa87438e5d8 in / 
# Tue, 02 Aug 2022 01:10:38 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 14:36:55 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 03 Aug 2022 14:36:58 GMT
ENV NGINX_VERSION=1.23.1
# Wed, 03 Aug 2022 14:37:00 GMT
ENV NJS_VERSION=0.7.6
# Wed, 03 Aug 2022 14:37:03 GMT
ENV PKG_RELEASE=1~bullseye
# Wed, 03 Aug 2022 15:10:43 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 03 Aug 2022 15:10:46 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Wed, 03 Aug 2022 15:10:48 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Wed, 03 Aug 2022 15:10:50 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Wed, 03 Aug 2022 15:10:53 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Wed, 03 Aug 2022 15:10:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 03 Aug 2022 15:10:59 GMT
EXPOSE 80
# Wed, 03 Aug 2022 15:11:02 GMT
STOPSIGNAL SIGQUIT
# Wed, 03 Aug 2022 15:11:05 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:88350749a27614c791450c256b051f023d81cdd256211274b1efac493779d2be`  
		Last Modified: Tue, 02 Aug 2022 01:21:02 GMT  
		Size: 29.6 MB (29628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29cbd68db6a6c85f8477354e3d30eaaaa8e204ececf39829720a32ebb8e4e58`  
		Last Modified: Wed, 03 Aug 2022 15:46:52 GMT  
		Size: 35.7 MB (35702730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb4aa492395f8fcc3800b2b644c03915722487deeaf92ac5e57ec81f1dd8685`  
		Last Modified: Wed, 03 Aug 2022 15:46:28 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa566d938e99ec46855666618dbed249804df4643c24ce37c5bd387ee5ef6bc`  
		Last Modified: Wed, 03 Aug 2022 15:46:28 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c29ba7e111981c90b5266288af15e3bc1d4dfa467fe7e6da011bbfb8e67c67`  
		Last Modified: Wed, 03 Aug 2022 15:46:28 GMT  
		Size: 665.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30127287ce51460eba0b30a1ca79cf9eadb45c1c98796f3acb6412c388adc6ad`  
		Last Modified: Wed, 03 Aug 2022 15:46:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; ppc64le

```console
$ docker pull nginx@sha256:c7f8954778d56e89f0c45d0950e7dc31ef4b9c18b59d3d603d277b074dc80e70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73885813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d5e5363b114779aeb4c378a85baccf15082ad07e736e67caa7dfec4c66c9b0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Jul 2022 01:25:28 GMT
ADD file:9e1afe48f40d94f879aefb12a7e68da2f0772d701e95b8219bd1f79a83e1933a in / 
# Tue, 12 Jul 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 16:21:37 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 19 Jul 2022 19:27:30 GMT
ENV NGINX_VERSION=1.23.1
# Tue, 19 Jul 2022 19:27:34 GMT
ENV NJS_VERSION=0.7.6
# Tue, 19 Jul 2022 19:27:36 GMT
ENV PKG_RELEASE=1~bullseye
# Tue, 19 Jul 2022 20:49:39 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 19 Jul 2022 20:49:45 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 19 Jul 2022 20:49:51 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 19 Jul 2022 20:49:58 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 19 Jul 2022 20:50:00 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 19 Jul 2022 20:50:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 19 Jul 2022 20:50:08 GMT
EXPOSE 80
# Tue, 19 Jul 2022 20:50:12 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Jul 2022 20:50:16 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:bd3d68d1ce583727f6378a16916795b955cc0ad39e0ebe754a26007ef54744fa`  
		Last Modified: Tue, 12 Jul 2022 01:36:03 GMT  
		Size: 35.3 MB (35272500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2778be2a67bc7f4b03bd478c3de08eca35c82d43d15b954a7e0ec847c05586e1`  
		Last Modified: Tue, 19 Jul 2022 21:01:38 GMT  
		Size: 38.6 MB (38609750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34841cfbacec0af7ba30bdfbbb0d51389a2acd598c953255de0122aefb361cfc`  
		Last Modified: Tue, 19 Jul 2022 21:01:30 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc29070371cd55904a19e1582a8904b8434bf5b6da5570e091ac1d3945aa9b1d`  
		Last Modified: Tue, 19 Jul 2022 21:01:30 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d3cbd0d92d3c3d670ee5b9690b8156902961c0282096d218c27ffc030bb5cb`  
		Last Modified: Tue, 19 Jul 2022 21:01:30 GMT  
		Size: 668.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4335b345548e5506131b34557270413243aa0878d89e26e0def206bfc3ec946c`  
		Last Modified: Tue, 19 Jul 2022 21:01:30 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; s390x

```console
$ docker pull nginx@sha256:5de3c115ebd79629be02f22a11f89c42d00d7e3799f35d7eb564544e3af5ce33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66308227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed51e492b2a3583bd22b92cfbf0d7f3cd7823cd7ee5da29fb75b592c09f58496`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:41:56 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 02 Aug 2022 02:41:56 GMT
ENV NGINX_VERSION=1.23.1
# Tue, 02 Aug 2022 02:41:56 GMT
ENV NJS_VERSION=0.7.6
# Tue, 02 Aug 2022 02:41:56 GMT
ENV PKG_RELEASE=1~bullseye
# Tue, 02 Aug 2022 02:45:37 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 02 Aug 2022 02:45:40 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 02 Aug 2022 02:45:40 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 02 Aug 2022 02:45:40 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 02 Aug 2022 02:45:40 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 02 Aug 2022 02:45:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 02:45:40 GMT
EXPOSE 80
# Tue, 02 Aug 2022 02:45:40 GMT
STOPSIGNAL SIGQUIT
# Tue, 02 Aug 2022 02:45:41 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642f35fdd1c85c6198a747da3cd668220c22f6d45c06946208dc9e514e1920a4`  
		Last Modified: Tue, 02 Aug 2022 02:50:55 GMT  
		Size: 36.7 MB (36664413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40152670d43f8ba9d94e9db1393e3553cfe27552a4bba5805cc1a89b1c059eeb`  
		Last Modified: Tue, 02 Aug 2022 02:50:50 GMT  
		Size: 601.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0df6092da81691330bf4dc1abfe81a9e80bff3936e458af60793320748ab2e`  
		Last Modified: Tue, 02 Aug 2022 02:50:50 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da456ea8f8bab1fb7569298fb925787c6fffbb46cc066b126194411b4a55689`  
		Last Modified: Tue, 02 Aug 2022 02:50:50 GMT  
		Size: 665.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca4b3f6d7b59030479deda415264325c9ee068773b41bf3b583b7ffb59cc108`  
		Last Modified: Tue, 02 Aug 2022 02:50:50 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
