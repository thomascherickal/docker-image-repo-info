## `nginx:perl`

```console
$ docker pull nginx@sha256:ebfadccc2ab4e93e72c85aba5c573de428451f39118b2b9e1de1961948fdaa48
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
$ docker pull nginx@sha256:009add6dbcadb068175eddc2dfd83e19ab92e380fb2f090634fcc680fc59e661
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64728247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42057d9974583a079db1acd4c28ea39bf8dbe9f82326f37dac9c74962370c95d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:03:10 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 12 Oct 2021 02:03:10 GMT
ENV NGINX_VERSION=1.21.3
# Tue, 12 Oct 2021 02:03:10 GMT
ENV NJS_VERSION=0.6.2
# Tue, 12 Oct 2021 02:03:10 GMT
ENV PKG_RELEASE=1~buster
# Tue, 12 Oct 2021 02:04:08 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 12 Oct 2021 02:04:08 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 12 Oct 2021 02:04:08 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:04:08 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:04:09 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:04:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 02:04:09 GMT
EXPOSE 80
# Tue, 12 Oct 2021 02:04:09 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Oct 2021 02:04:09 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df33b9180e7e5e6291d012c181e3e18a23ad90bdb17f3808bad7202872b12a73`  
		Last Modified: Tue, 12 Oct 2021 02:06:27 GMT  
		Size: 37.6 MB (37585177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b076340d2482648f4d345a3b30d1f7e5a8fad29c57423bf9b4828b27d69772ca`  
		Last Modified: Tue, 12 Oct 2021 02:06:21 GMT  
		Size: 601.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b316cddbc45999d1793beb7810468c6603552854831598c2427fe6603ba271`  
		Last Modified: Tue, 12 Oct 2021 02:06:21 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e608138570fbfafa9bce00408b74bfc0fb8dfa13c680761a429c2b944985707e`  
		Last Modified: Tue, 12 Oct 2021 02:06:21 GMT  
		Size: 668.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcd06b8383219fc083cf927dc7b3a56f99b02d0279433a4a2d6d2018400505b`  
		Last Modified: Tue, 12 Oct 2021 02:06:21 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; arm variant v5

```console
$ docker pull nginx@sha256:897468df8abfe15afba38ab2ccb90ee1b01559b45b4a52fa198c2efdb6ba90c4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.7 MB (60683658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca882db63fa75e45810759f2a96ce26723f0cb4d8c491071ef4c32adda2ea176`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:42 GMT
ADD file:6524935705c59a0eda67f61fe1005a28b4b388258e2d5636dd5b831333200dc8 in / 
# Tue, 28 Sep 2021 01:51:43 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 03:38:24 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 28 Sep 2021 03:38:24 GMT
ENV NGINX_VERSION=1.21.3
# Tue, 28 Sep 2021 03:38:24 GMT
ENV NJS_VERSION=0.6.2
# Tue, 28 Sep 2021 03:38:25 GMT
ENV PKG_RELEASE=1~buster
# Tue, 28 Sep 2021 03:57:18 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 28 Sep 2021 03:57:19 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 28 Sep 2021 03:57:19 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 28 Sep 2021 03:57:20 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 28 Sep 2021 03:57:20 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 28 Sep 2021 03:57:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 28 Sep 2021 03:57:21 GMT
EXPOSE 80
# Tue, 28 Sep 2021 03:57:22 GMT
STOPSIGNAL SIGQUIT
# Tue, 28 Sep 2021 03:57:22 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:85d14771cf32dc23d1c8e99a9aad844b3db9d67f4781455c81749ffe43b05513`  
		Last Modified: Tue, 28 Sep 2021 02:08:05 GMT  
		Size: 24.9 MB (24879067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc98c9327bd4ba82d1aeb57871321050e662f87113a52d22bba157c54d04b3e`  
		Last Modified: Tue, 28 Sep 2021 04:19:09 GMT  
		Size: 35.8 MB (35801039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42621c2c35c9785e582f6e469213577b36c05bb80a7cb01fdc73cbd997b394a2`  
		Last Modified: Tue, 28 Sep 2021 04:18:45 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62f77f238623385425df1c7c62de9d45ec8abde9a649b4cd8644949e497980e`  
		Last Modified: Tue, 28 Sep 2021 04:18:45 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d245e869abde2ca273c106f7b63605d60a085a29b545c16430d5783f0dbbe4`  
		Last Modified: Tue, 28 Sep 2021 04:18:45 GMT  
		Size: 665.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8007cbe8c5d7eaa08c737b0bcc4ea21a51622bb446f746e49ee2732a2b099dff`  
		Last Modified: Tue, 28 Sep 2021 04:18:45 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; arm variant v7

```console
$ docker pull nginx@sha256:daffcbf7ca4347c5283ce7f6bff729efb810bb526e91bf1f9b17f4d15d6dd43b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57439907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26a6b9932aa80bc7698be8fe6dca114e87185710511982adb2992ae1fb97fa2d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:10:41 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 12 Oct 2021 06:10:41 GMT
ENV NGINX_VERSION=1.21.3
# Tue, 12 Oct 2021 06:10:42 GMT
ENV NJS_VERSION=0.6.2
# Tue, 12 Oct 2021 06:10:42 GMT
ENV PKG_RELEASE=1~buster
# Tue, 12 Oct 2021 06:28:37 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 12 Oct 2021 06:28:38 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 12 Oct 2021 06:28:39 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 12 Oct 2021 06:28:39 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 06:28:40 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 06:28:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 06:28:40 GMT
EXPOSE 80
# Tue, 12 Oct 2021 06:28:41 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Oct 2021 06:28:41 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe51df6627397ca0eba45354de365a6b2ceb0bf2d4a2091ade2a2e13d230a2d1`  
		Last Modified: Tue, 12 Oct 2021 06:50:56 GMT  
		Size: 34.7 MB (34696648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c0b7efbd2b1e891683bdf2ce436de8ac9ef13535381124b2215ff16824e83e`  
		Last Modified: Tue, 12 Oct 2021 06:50:34 GMT  
		Size: 603.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561289795bdbced9e9af4334af215413b45257e41c536332888ff944a593a87`  
		Last Modified: Tue, 12 Oct 2021 06:50:34 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a5244ea381f354c140f4fd518676d1b5fa83be7b70ce9ac0c6fafbee4882fb`  
		Last Modified: Tue, 12 Oct 2021 06:50:34 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b678c094ac22592f8c1d12171da8e4ebf8dafb3c45577a9866f5e0ef8517747e`  
		Last Modified: Tue, 12 Oct 2021 06:50:34 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:fda48984d341a14234bbe016c47558b7c629d6ee30e2243d5323a39ed975891c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.3 MB (63259017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a527700f33e58e63b0ef09e17d7c3c5ae4c0e8bf933dbd160b4b5cd401ba3a9e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:36:40 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 12 Oct 2021 04:36:40 GMT
ENV NGINX_VERSION=1.21.3
# Tue, 12 Oct 2021 04:36:40 GMT
ENV NJS_VERSION=0.6.2
# Tue, 12 Oct 2021 04:36:40 GMT
ENV PKG_RELEASE=1~buster
# Tue, 12 Oct 2021 04:37:38 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 12 Oct 2021 04:37:39 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 12 Oct 2021 04:37:39 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 12 Oct 2021 04:37:39 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 04:37:39 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 04:37:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 04:37:40 GMT
EXPOSE 80
# Tue, 12 Oct 2021 04:37:40 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Oct 2021 04:37:40 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558f7ec0fb277353202df79af9a501b65302ad50111ee191ac6cf11d4821e851`  
		Last Modified: Tue, 12 Oct 2021 04:40:41 GMT  
		Size: 37.3 MB (37346982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf043de54e0696fbb8b2f286dd2b30946c79346126ba561f6e149b788e42832`  
		Last Modified: Tue, 12 Oct 2021 04:40:35 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1759e89501e1d32c0f291285cebbd2f3b35047214b4df88e8d63385fb5eef1b6`  
		Last Modified: Tue, 12 Oct 2021 04:40:35 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc973dc08a1655fdb5e18c39dc983c08b5e4699420259590de87dd5e2bb7389`  
		Last Modified: Tue, 12 Oct 2021 04:40:35 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c152ef6fcde8e5ad43433a7549ab394c07444c922644c19f467e3eaf1a0d5fc3`  
		Last Modified: Tue, 12 Oct 2021 04:40:35 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; 386

```console
$ docker pull nginx@sha256:adccdc859bb993b0d0c36c18d49b5f3fd055f25ca8f3b5c96fd3996946ca8681
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65739421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f1bf998f49c80d6bfdf790d47fda4c2ab91c2dd50e5c1cdc4d15e104e9140f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:36:33 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 12 Oct 2021 02:36:33 GMT
ENV NGINX_VERSION=1.21.3
# Tue, 12 Oct 2021 02:36:33 GMT
ENV NJS_VERSION=0.6.2
# Tue, 12 Oct 2021 02:36:33 GMT
ENV PKG_RELEASE=1~buster
# Tue, 12 Oct 2021 02:38:19 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 12 Oct 2021 02:38:20 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 12 Oct 2021 02:38:20 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:38:20 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:38:21 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:38:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 02:38:21 GMT
EXPOSE 80
# Tue, 12 Oct 2021 02:38:21 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Oct 2021 02:38:22 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf5866456824e529b85efe0b21a679c7f1e2a0e990eb6d45ecb98862b7fcf38`  
		Last Modified: Tue, 12 Oct 2021 02:41:48 GMT  
		Size: 37.9 MB (37944420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a3c696482c03364125392c106b71fac2597c66633c17841ec8a48a09340667`  
		Last Modified: Tue, 12 Oct 2021 02:41:40 GMT  
		Size: 601.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2a68dc60123d6942ee653b431ac586808123effb9660a608dd9bfc739dc924`  
		Last Modified: Tue, 12 Oct 2021 02:41:39 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f269a86964b96f041da4d772d6ed489af662053c4575cf9a9c24452159d90783`  
		Last Modified: Tue, 12 Oct 2021 02:41:39 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fad0b308cc0e4d4c86865b3317039f650eaf5c0ee3e1474b5e17468e7cefbb0`  
		Last Modified: Tue, 12 Oct 2021 02:41:39 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; mips64le

```console
$ docker pull nginx@sha256:a4ca86de99e1af5ef76d1216357d86ebed702487f071ab9187e653b917fb33a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62269775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c68717905a9e568f17b7a30a1290bb0c60d66dd1dee3bb1b8a481a5193939b42`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:49 GMT
ADD file:219b2ce847fd4b227257f60cf40dee2eaf7688371fd76658752f6ccbac9c4353 in / 
# Fri, 03 Sep 2021 01:10:49 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:40:19 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 09 Sep 2021 18:12:42 GMT
ENV NGINX_VERSION=1.21.3
# Thu, 09 Sep 2021 18:12:42 GMT
ENV NJS_VERSION=0.6.2
# Thu, 09 Sep 2021 18:12:43 GMT
ENV PKG_RELEASE=1~buster
# Thu, 09 Sep 2021 18:37:26 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Thu, 09 Sep 2021 18:37:27 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Thu, 09 Sep 2021 18:37:27 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Thu, 09 Sep 2021 18:37:28 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Thu, 09 Sep 2021 18:37:28 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Thu, 09 Sep 2021 18:37:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 09 Sep 2021 18:37:29 GMT
EXPOSE 80
# Thu, 09 Sep 2021 18:37:29 GMT
STOPSIGNAL SIGQUIT
# Thu, 09 Sep 2021 18:37:29 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:c11f388d181c313e7657eea7b1ffa2d20856b4701922412adea724a19acdb79f`  
		Last Modified: Fri, 03 Sep 2021 01:19:51 GMT  
		Size: 25.8 MB (25812853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576c3e01bbedc6387745ebeefbcf659e841d061ed8f6667e963128f2a59e1f69`  
		Last Modified: Thu, 09 Sep 2021 18:39:01 GMT  
		Size: 36.5 MB (36453362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504c5fcc4f754d5eee81568636e4922655f54bb09c1c45d9ae75e6df937280c4`  
		Last Modified: Thu, 09 Sep 2021 18:38:35 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75968412eb46b99e43a9eb78903dd81531b20fb102a40d2a7cd7bb6992c88bcc`  
		Last Modified: Thu, 09 Sep 2021 18:38:35 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370b98dbbaa053391efb8fb553e76bef58625dfc288024026fe99f496ce264a0`  
		Last Modified: Thu, 09 Sep 2021 18:38:35 GMT  
		Size: 668.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92b1ec224a804b5cc205805b5d30ed956b9cabdc6cc0f4dbcffe92c3eb3b33a`  
		Last Modified: Thu, 09 Sep 2021 18:38:35 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; ppc64le

```console
$ docker pull nginx@sha256:5cb4c6c44555443277a18e7e98848a136f463e6c24cf2c038da38cecc6677d78
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70483700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6c6cd0bfd5989cc0641bedb29495338a6aebae952e32622b1ff208253e2194`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Mon, 04 Oct 2021 17:56:14 GMT
ADD file:0b55ec14c2e9aa78512985a5bff3881b6fabf6794ce4406bb874b173d5a60799 in / 
# Mon, 04 Oct 2021 17:56:20 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 16:30:18 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 05 Oct 2021 16:30:21 GMT
ENV NGINX_VERSION=1.21.3
# Tue, 05 Oct 2021 16:30:26 GMT
ENV NJS_VERSION=0.6.2
# Tue, 05 Oct 2021 16:30:31 GMT
ENV PKG_RELEASE=1~buster
# Tue, 05 Oct 2021 17:09:58 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 05 Oct 2021 17:10:03 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 05 Oct 2021 17:10:07 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 05 Oct 2021 17:10:08 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 05 Oct 2021 17:10:10 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 05 Oct 2021 17:10:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:10:16 GMT
EXPOSE 80
# Tue, 05 Oct 2021 17:10:19 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Oct 2021 17:10:21 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:5736db2c6d2424206be3309412da520d7fe1fe4933cc2cc72641b311dd7d9099`  
		Last Modified: Mon, 04 Oct 2021 18:08:33 GMT  
		Size: 30.6 MB (30553728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7c5614d14d353829509b6e180a2c707aa1a2ba441b9e451a58a0b767297175`  
		Last Modified: Tue, 05 Oct 2021 17:43:49 GMT  
		Size: 39.9 MB (39926417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0d9899b91affc24470a6a08e4337b1da8a6d844ff2ee6dd0cf52583497f021`  
		Last Modified: Tue, 05 Oct 2021 17:43:41 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20447a328ad541e9f52110f6a74aec7b958bced23ef7f3a9b968da6fefc00f88`  
		Last Modified: Tue, 05 Oct 2021 17:43:41 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf6e4cc0e10c79c730145284ab7da8874b460c767bd61b9777d8a9e844803ea`  
		Last Modified: Tue, 05 Oct 2021 17:43:41 GMT  
		Size: 665.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2836391f0d7214c00407c695417dd1dc33152a466b95728418500acff0f3ff`  
		Last Modified: Tue, 05 Oct 2021 17:43:41 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:perl` - linux; s390x

```console
$ docker pull nginx@sha256:99bd192d67f3ca249643ee82b1feeb11711e10e756f95068f171c65b4293d95a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63244561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2d93553a1669bbccc97b392b075eae6810a6205a793f58d583a7376d9b1695b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:58:34 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 12 Oct 2021 06:58:34 GMT
ENV NGINX_VERSION=1.21.3
# Tue, 12 Oct 2021 06:58:34 GMT
ENV NJS_VERSION=0.6.2
# Tue, 12 Oct 2021 06:58:35 GMT
ENV PKG_RELEASE=1~buster
# Tue, 12 Oct 2021 07:04:05 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/mainline/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 12 Oct 2021 07:04:06 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 12 Oct 2021 07:04:06 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 12 Oct 2021 07:04:07 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 07:04:07 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 07:04:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 07:04:07 GMT
EXPOSE 80
# Tue, 12 Oct 2021 07:04:07 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Oct 2021 07:04:07 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90362814666c4e3a32325f1a1af17066b03288274c3b0df3a491bd0440a4bc58`  
		Last Modified: Tue, 12 Oct 2021 07:11:31 GMT  
		Size: 37.5 MB (37486758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f289a756c71b4f444808691b93e60c65b016638c7dbe9f520819e5944e8dae`  
		Last Modified: Tue, 12 Oct 2021 07:11:26 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebae1a890854067e3fd2c829b3495b2205bbceb9018e03bcef570fb52d799df3`  
		Last Modified: Tue, 12 Oct 2021 07:11:25 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e3c1f3d5b8205c2849f1f810d54b0600d6b98ca1e84c218dffea6691c44c52`  
		Last Modified: Tue, 12 Oct 2021 07:11:26 GMT  
		Size: 665.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5ff6641021092d71b57d62e470ac5035e19fbf95e1f043d66d4454adb26621`  
		Last Modified: Tue, 12 Oct 2021 07:11:26 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
