## `nginx:stable`

```console
$ docker pull nginx@sha256:e1f9e922aba026954bc78b788f3f2b916051a7d7b30f1bcffb45ae6152c66d9c
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

### `nginx:stable` - linux; amd64

```console
$ docker pull nginx@sha256:ee2970c234800c5b5841d20d04b7ddc2a08f8653ce6d3376782c8a48eb61428b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53721649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d03f6b8b915209c54fc8ead682f7a5709d11226f6b81185850199f18b277a2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:03:10 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 12 Oct 2021 02:04:21 GMT
ENV NGINX_VERSION=1.20.1
# Tue, 12 Oct 2021 02:04:21 GMT
ENV NJS_VERSION=0.5.3
# Tue, 12 Oct 2021 02:04:21 GMT
ENV PKG_RELEASE=1~buster
# Tue, 12 Oct 2021 02:04:43 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 12 Oct 2021 02:04:43 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 12 Oct 2021 02:04:43 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:04:44 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:04:44 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:04:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 02:04:44 GMT
EXPOSE 80
# Tue, 12 Oct 2021 02:04:44 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Oct 2021 02:04:45 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83acae5e2daa7de1558d14970fed734716c0067ca4dee30ece2e9f9a99571a2c`  
		Last Modified: Tue, 12 Oct 2021 02:06:53 GMT  
		Size: 26.6 MB (26578583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33715b419f9b2252d30ae8392aaccb066e9213beaa33652d180c33631b28800f`  
		Last Modified: Tue, 12 Oct 2021 02:06:49 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb08b4d557d89c8c6b9463d700312167e1c8f727bbc146675f0c343de619210f`  
		Last Modified: Tue, 12 Oct 2021 02:06:49 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d5bdecd9556e517c9b902afd3c406bd9b5ab264f2a52a33f0fd1febaff48a1`  
		Last Modified: Tue, 12 Oct 2021 02:06:49 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0820d7f251418edaeef6662a2bba5842bcb7621b786160d3977856e225271972`  
		Last Modified: Tue, 12 Oct 2021 02:06:49 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; arm variant v5

```console
$ docker pull nginx@sha256:72964983233fcf69a2136dc0eab38034213d8df2de1888ed6c8328c278ae7a37
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50393506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73e317f24153c99675018f820b4e07b6935096220bc212936df8472b9ec02273`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 28 Sep 2021 01:51:42 GMT
ADD file:6524935705c59a0eda67f61fe1005a28b4b388258e2d5636dd5b831333200dc8 in / 
# Tue, 28 Sep 2021 01:51:43 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 03:38:24 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 28 Sep 2021 03:57:40 GMT
ENV NGINX_VERSION=1.20.1
# Tue, 28 Sep 2021 03:57:40 GMT
ENV NJS_VERSION=0.5.3
# Tue, 28 Sep 2021 03:57:41 GMT
ENV PKG_RELEASE=1~buster
# Tue, 28 Sep 2021 04:06:23 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 28 Sep 2021 04:06:23 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 28 Sep 2021 04:06:24 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 28 Sep 2021 04:06:24 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 28 Sep 2021 04:06:25 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 28 Sep 2021 04:06:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 28 Sep 2021 04:06:26 GMT
EXPOSE 80
# Tue, 28 Sep 2021 04:06:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 28 Sep 2021 04:06:26 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:85d14771cf32dc23d1c8e99a9aad844b3db9d67f4781455c81749ffe43b05513`  
		Last Modified: Tue, 28 Sep 2021 02:08:05 GMT  
		Size: 24.9 MB (24879067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df89695f9d8119fd1ca0b3bd172c9dd5b563387438ec0e232a4e92881a107be1`  
		Last Modified: Tue, 28 Sep 2021 04:19:48 GMT  
		Size: 25.5 MB (25510886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca26de6ce523b065e093befb73773c4fc634318fcf130df6a833bc395474c4b0`  
		Last Modified: Tue, 28 Sep 2021 04:19:33 GMT  
		Size: 601.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d510db78f718ecc89d11e74bab8003b641a55d5978ee496298a29cbe3b7c47`  
		Last Modified: Tue, 28 Sep 2021 04:19:33 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0a7a21069b26d51d77be9585daebc53ddaae931fcb8a63dd94c0f6e97791e0`  
		Last Modified: Tue, 28 Sep 2021 04:19:33 GMT  
		Size: 664.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6385b370b79c065149049ba1cbcc9b1442eac7ff2819d40a2acb26ba1d951a`  
		Last Modified: Tue, 28 Sep 2021 04:19:33 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; arm variant v7

```console
$ docker pull nginx@sha256:d78659dabc793be40781b8dce576d885b9d08ffe6cca67f2534ed8cf1338bf51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47349720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaddafe6f0b55450a73a24bb5a0cf35f01b4e00f7f03a612486d1c74375f084a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:10:41 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 12 Oct 2021 06:29:29 GMT
ENV NGINX_VERSION=1.20.1
# Tue, 12 Oct 2021 06:29:29 GMT
ENV NJS_VERSION=0.5.3
# Tue, 12 Oct 2021 06:29:30 GMT
ENV PKG_RELEASE=1~buster
# Tue, 12 Oct 2021 06:37:36 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 12 Oct 2021 06:37:37 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 12 Oct 2021 06:37:37 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 12 Oct 2021 06:37:38 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 06:37:38 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 06:37:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 06:37:39 GMT
EXPOSE 80
# Tue, 12 Oct 2021 06:37:40 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Oct 2021 06:37:40 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8cf508b501b1f3b56fe4973c2fc83a6933a2d2487df556c7857241e82435c1`  
		Last Modified: Tue, 12 Oct 2021 06:51:50 GMT  
		Size: 24.6 MB (24606460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd36ee3255dda12f062f682a4365eedc257ba730af72d51043692f05d3225636`  
		Last Modified: Tue, 12 Oct 2021 06:51:37 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040fc83e4bc1981097ae60474da12c22c3ed33da5873bad39034d2c1e6808611`  
		Last Modified: Tue, 12 Oct 2021 06:51:36 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82315649b72ec4ca86b5b40c3f4134c1e478ae4c0c04c9e79f7c600edd361cf1`  
		Last Modified: Tue, 12 Oct 2021 06:51:37 GMT  
		Size: 668.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c191a01bba870eda73caf58e3f5158d1f618e6132d343b2595f1fe7e7a5c98a`  
		Last Modified: Tue, 12 Oct 2021 06:51:37 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:5765338321f69694c74c7b42c492aeaa85b2157d678e0ef08e7765ae06216466
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52303313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eb25865d142e6ce0e0a0e181b2cef34f8e8876c9ef1f2fa7ac9d7ccd219cb8b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:36:40 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 12 Oct 2021 04:37:57 GMT
ENV NGINX_VERSION=1.20.1
# Tue, 12 Oct 2021 04:37:57 GMT
ENV NJS_VERSION=0.5.3
# Tue, 12 Oct 2021 04:37:58 GMT
ENV PKG_RELEASE=1~buster
# Tue, 12 Oct 2021 04:38:18 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 12 Oct 2021 04:38:19 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 12 Oct 2021 04:38:19 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 12 Oct 2021 04:38:19 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 04:38:19 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 04:38:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 04:38:20 GMT
EXPOSE 80
# Tue, 12 Oct 2021 04:38:20 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Oct 2021 04:38:20 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79aa200e2b940e8f72798ef25e708131dfcb221e228b923163f122f8be80feb6`  
		Last Modified: Tue, 12 Oct 2021 04:41:14 GMT  
		Size: 26.4 MB (26391280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb61bd238884a6110e3b1d2cdd199aaa320bc6a0086ad06cc48a15d09fbab46e`  
		Last Modified: Tue, 12 Oct 2021 04:41:10 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df5875af5c98f27959499f64065512076d42f0af94c6a59bc3ef90b3459d84`  
		Last Modified: Tue, 12 Oct 2021 04:41:10 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56da0358117f3f1db772796763fbdbb17b7cdfccf6701c1ebe86e873f7ee28a5`  
		Last Modified: Tue, 12 Oct 2021 04:41:10 GMT  
		Size: 665.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8428267bf00ed2a94abe29ae07e0ef1ec016a9c5b8e24a7fc9c5d49a86545f`  
		Last Modified: Tue, 12 Oct 2021 04:41:10 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; 386

```console
$ docker pull nginx@sha256:7004e2d0c172e1348aaa410fce8f075c98a05b96873743f68ba34b78ba66a8bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.2 MB (55221932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da69df42b0403f5f65babf9b4ae1f2c760e961d2017232b8125681c86de9df64`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:36:33 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 12 Oct 2021 02:38:57 GMT
ENV NGINX_VERSION=1.20.1
# Tue, 12 Oct 2021 02:38:57 GMT
ENV NJS_VERSION=0.5.3
# Tue, 12 Oct 2021 02:38:57 GMT
ENV PKG_RELEASE=1~buster
# Tue, 12 Oct 2021 02:39:24 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 12 Oct 2021 02:39:25 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 12 Oct 2021 02:39:25 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:39:25 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:39:26 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 02:39:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 02:39:26 GMT
EXPOSE 80
# Tue, 12 Oct 2021 02:39:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Oct 2021 02:39:27 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53be18e15e4d44209f4d3a684442dbad47e037902258b820b30a92d27678b95`  
		Last Modified: Tue, 12 Oct 2021 02:42:15 GMT  
		Size: 27.4 MB (27426942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf379e6050e2586a0814af79098f3ce8d18dcfa041806afdd8b2675bbe712e4`  
		Last Modified: Tue, 12 Oct 2021 02:42:10 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d595ad9fb25e6e5984846490bfd3c5d1a5a07b4ad05810bfe37d6f3791312db8`  
		Last Modified: Tue, 12 Oct 2021 02:42:10 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d406c6198af545a862ae040518417b51cef2dac40e20d164fb6584b0615d980`  
		Last Modified: Tue, 12 Oct 2021 02:42:10 GMT  
		Size: 664.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4477172ece020bdfe4a0858b119caf40de47c5e48a76b2c63c0d8c0124ac872e`  
		Last Modified: Tue, 12 Oct 2021 02:42:10 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; mips64le

```console
$ docker pull nginx@sha256:c2b1173a4c9806ea9fc05c0146dcca47721bf8a97e0aa40df4ba9360cfa723a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (51951580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4222fb63533933bf5d2a82726931b6bc364c03fdfa399dc048e5899a022fdfa1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:49 GMT
ADD file:219b2ce847fd4b227257f60cf40dee2eaf7688371fd76658752f6ccbac9c4353 in / 
# Fri, 03 Sep 2021 01:10:49 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:40:19 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 03 Sep 2021 03:05:18 GMT
ENV NGINX_VERSION=1.20.1
# Fri, 03 Sep 2021 03:05:19 GMT
ENV NJS_VERSION=0.5.3
# Fri, 03 Sep 2021 03:05:19 GMT
ENV PKG_RELEASE=1~buster
# Fri, 03 Sep 2021 03:16:46 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Fri, 03 Sep 2021 03:16:47 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Fri, 03 Sep 2021 03:16:47 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Fri, 03 Sep 2021 03:16:47 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Fri, 03 Sep 2021 03:16:48 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Fri, 03 Sep 2021 03:16:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 03:16:48 GMT
EXPOSE 80
# Fri, 03 Sep 2021 03:16:49 GMT
STOPSIGNAL SIGQUIT
# Fri, 03 Sep 2021 03:16:49 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:c11f388d181c313e7657eea7b1ffa2d20856b4701922412adea724a19acdb79f`  
		Last Modified: Fri, 03 Sep 2021 01:19:51 GMT  
		Size: 25.8 MB (25812853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781e3d2196d3ddcdb21bf59f188bac28dde670e3152ab22cfde3ef1fb7b89e9a`  
		Last Modified: Fri, 03 Sep 2021 03:31:39 GMT  
		Size: 26.1 MB (26135168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f683b7c5c657f78ea06486f1f323c3f2154d87eb2727b87262d25cf582680d3`  
		Last Modified: Fri, 03 Sep 2021 03:31:22 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e823c599f124163e10a5630ac7fdba86b14a3e85bdd709b67010acb1a9d71ea8`  
		Last Modified: Fri, 03 Sep 2021 03:31:22 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ca5bcd080c04f39baaddb10b266a88d25736b18c25b4e603bf5fafa6b2c0d9`  
		Last Modified: Fri, 03 Sep 2021 03:31:22 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68906a3d1cc9c573cf94de7d9f15ba292ab2608da5d68c91559fa0ddc5ae5d9d`  
		Last Modified: Fri, 03 Sep 2021 03:31:22 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; ppc64le

```console
$ docker pull nginx@sha256:442a86df321ec53358b3972b9538150505e6456144c5f11aca33260b07dc8e01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.2 MB (59223814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3250606252f86bca4fce98747c070f820293c5806822f5038d24d4cb698e09a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Mon, 04 Oct 2021 17:56:14 GMT
ADD file:0b55ec14c2e9aa78512985a5bff3881b6fabf6794ce4406bb874b173d5a60799 in / 
# Mon, 04 Oct 2021 17:56:20 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 16:30:18 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 05 Oct 2021 17:10:47 GMT
ENV NGINX_VERSION=1.20.1
# Tue, 05 Oct 2021 17:10:51 GMT
ENV NJS_VERSION=0.5.3
# Tue, 05 Oct 2021 17:10:54 GMT
ENV PKG_RELEASE=1~buster
# Tue, 05 Oct 2021 17:25:15 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 05 Oct 2021 17:25:18 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 05 Oct 2021 17:25:20 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 05 Oct 2021 17:25:21 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 05 Oct 2021 17:25:23 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 05 Oct 2021 17:25:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:25:28 GMT
EXPOSE 80
# Tue, 05 Oct 2021 17:25:31 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Oct 2021 17:25:33 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:5736db2c6d2424206be3309412da520d7fe1fe4933cc2cc72641b311dd7d9099`  
		Last Modified: Mon, 04 Oct 2021 18:08:33 GMT  
		Size: 30.6 MB (30553728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a201c4c34381cdc1d18b37cf0c34c8b5bd9d3513aa78559336cac07ad0758e5`  
		Last Modified: Tue, 05 Oct 2021 17:44:21 GMT  
		Size: 28.7 MB (28666527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84016c8c7bf1b979acd85a89bf7727d5a8f2ce5794347ba8e050dbdb7258bd63`  
		Last Modified: Tue, 05 Oct 2021 17:44:16 GMT  
		Size: 603.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203239a54090ea3c75c659b01ef28aac090bbf30532c3d0a30b68da3178b3a32`  
		Last Modified: Tue, 05 Oct 2021 17:44:16 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa10ff05f879eb7f7a04df81852f8bcda0821c763ae7a980156ea72f8e7795b`  
		Last Modified: Tue, 05 Oct 2021 17:44:16 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7066103780c53fd906f5bcf404fa83ab1410f61418c1a4bf972abe31bd088ff0`  
		Last Modified: Tue, 05 Oct 2021 17:44:16 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; s390x

```console
$ docker pull nginx@sha256:d220f0351114b00427c794904d45205415fe5a2326ff8fbe66cb048d196eceed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51904591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5da38c214d077a98959b05d325360edd2c2f65f3de251acd7011b0072e5b1b80`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:58:34 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 12 Oct 2021 07:04:38 GMT
ENV NGINX_VERSION=1.20.1
# Tue, 12 Oct 2021 07:04:38 GMT
ENV NJS_VERSION=0.5.3
# Tue, 12 Oct 2021 07:04:38 GMT
ENV PKG_RELEASE=1~buster
# Tue, 12 Oct 2021 07:06:54 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|i386|arm64)             echo "deb https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ buster nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 12 Oct 2021 07:06:55 GMT
COPY file:65504f71f5855ca017fb64d502ce873a31b2e0decd75297a8fb0a287f97acf92 in / 
# Tue, 12 Oct 2021 07:06:55 GMT
COPY file:0b866ff3fc1ef5b03c4e6c8c513ae014f691fb05d530257dfffd07035c1b75da in /docker-entrypoint.d 
# Tue, 12 Oct 2021 07:06:55 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 07:06:55 GMT
COPY file:09a214a3e07c919af2fb2d7c749ccbc446b8c10eb217366e5a65640ee9edcc25 in /docker-entrypoint.d 
# Tue, 12 Oct 2021 07:06:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 07:06:55 GMT
EXPOSE 80
# Tue, 12 Oct 2021 07:06:56 GMT
STOPSIGNAL SIGQUIT
# Tue, 12 Oct 2021 07:06:56 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6707671c0b2e6ee777b053d284a4179684410a4bb0ad476924a7cd27065a799`  
		Last Modified: Tue, 12 Oct 2021 07:11:54 GMT  
		Size: 26.1 MB (26146779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5b45ee349dc6e70d9d5c2a4a1329cef9c4bf72c397391b9b878548c388e7bf`  
		Last Modified: Tue, 12 Oct 2021 07:11:51 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5246fa638b0bf580fa953abf592e9c2a61a2ed8a8ed4b90d226f2477eba59fd0`  
		Last Modified: Tue, 12 Oct 2021 07:11:51 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e409ae9614c34fe47035c8162232a22683299d3a18f12090cf9e66b32057cedb`  
		Last Modified: Tue, 12 Oct 2021 07:11:51 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b0bc18f0c86d75e1449f58a98e421114f26ce2b2a9e4c5a4263ef87f8de14d`  
		Last Modified: Tue, 12 Oct 2021 07:11:51 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
