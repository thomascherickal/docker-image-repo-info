## `nginx:mainline`

```console
$ docker pull nginx@sha256:725cd8bd9fe9bb36a661b87b718e5d4ca41c579d1d30560ad1799829dbbefaaf
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

### `nginx:mainline` - linux; amd64

```console
$ docker pull nginx@sha256:3c4c1f42a89e343c7b050c5e5d6f670a0e0b82e70e0e7d023f10092a04bbb5a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70532847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6bd71f48f6839d9faae1f29d3babef831e76bc213107682c5cc80f0cbb30866`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:05:08 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 21 Nov 2023 09:05:08 GMT
ENV NGINX_VERSION=1.25.3
# Tue, 21 Nov 2023 09:05:09 GMT
ENV NJS_VERSION=0.8.2
# Tue, 21 Nov 2023 09:05:09 GMT
ENV PKG_RELEASE=1~bookworm
# Tue, 21 Nov 2023 09:05:31 GMT
RUN set -x     && groupadd --system --gid 101 nginx     && useradd --system --gid nginx --no-create-home --home /nonexistent --comment "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     NGINX_GPGKEY_PATH=/usr/share/keyrings/nginx-archive-keyring.gpg;     export GNUPGHOME="$(mktemp -d)";     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         gpg1 --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     gpg1 --export "$NGINX_GPGKEY" > "$NGINX_GPGKEY_PATH" ;     rm -rf "$GNUPGHOME";     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 21 Nov 2023 09:05:31 GMT
COPY file:01e75c6dd0ce317d516928a17584d111cd082840c01e58be0afc851b33adb916 in / 
# Tue, 21 Nov 2023 09:05:31 GMT
COPY file:caec368f5a54f70a844a13005eb2255bed778809b3672d516e719ce2f4bce123 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 09:05:31 GMT
COPY file:3b1b9915b7dd898a0e32f7eb9715a35c9feab914022efff68ba990bc1ec7d169 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 09:05:32 GMT
COPY file:57846632accc89753f45cbc00cb9e6223d991e1d31297eec3395a7ca58eed6a6 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 09:05:32 GMT
COPY file:9e3b2b63db9f8fc702e2dc2bdd0943be0d990c028cddcf1c159f5556a8ba3030 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 09:05:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 09:05:32 GMT
EXPOSE 80
# Tue, 21 Nov 2023 09:05:32 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Nov 2023 09:05:32 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b16c94bb68628753a94b89ddf26abc0974cd35a96f785895ab011d9b5042ee5`  
		Last Modified: Tue, 21 Nov 2023 09:07:18 GMT  
		Size: 41.4 MB (41378367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a59d19f9c5bb1ebdfef2255496b1bb5d658fdccc300c4c1f0d18c73f1bb14b5`  
		Last Modified: Tue, 21 Nov 2023 09:07:11 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea27b074f71d5766a59cdbfaa15f4cd3d17bffb83fed066373eb287326abbd3`  
		Last Modified: Tue, 21 Nov 2023 09:07:11 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6edf33e2524b241a0b191d0a0d2ca3d8d4ae7470333b059dd97ba30e663a1a3`  
		Last Modified: Tue, 21 Nov 2023 09:07:11 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b1ff10387b26e2952f006c0a4fe4c6f3c0743cb08ee448bb7157220ad2fc8f`  
		Last Modified: Tue, 21 Nov 2023 09:07:11 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51735783196785d1f604dc7711ea70fb3fab3cd9d99eaeff991c5afbfa0f20e8`  
		Last Modified: Tue, 21 Nov 2023 09:07:11 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; arm variant v5

```console
$ docker pull nginx@sha256:7cd79f42b8d3fae7ac4215060a081251316682d180ae08a4d1826bb68c93d1d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63117297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c957ac106af6606a836b79c38d2415a2d39f8d63399b4ca2c70bb4c91439769`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:31 GMT
ADD file:c00ddcb556a3791b020308012fd4d7749535c34d372bac47f6ff687a7652b25f in / 
# Wed, 01 Nov 2023 00:48:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 03:11:24 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Nov 2023 03:11:24 GMT
ENV NGINX_VERSION=1.25.3
# Wed, 01 Nov 2023 03:11:24 GMT
ENV NJS_VERSION=0.8.2
# Wed, 01 Nov 2023 03:11:24 GMT
ENV PKG_RELEASE=1~bookworm
# Wed, 01 Nov 2023 03:15:40 GMT
RUN set -x     && groupadd --system --gid 101 nginx     && useradd --system --gid nginx --no-create-home --home /nonexistent --comment "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     NGINX_GPGKEY_PATH=/usr/share/keyrings/nginx-archive-keyring.gpg;     export GNUPGHOME="$(mktemp -d)";     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         gpg1 --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     gpg1 --export "$NGINX_GPGKEY" > "$NGINX_GPGKEY_PATH" ;     rm -rf "$GNUPGHOME";     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Nov 2023 03:15:40 GMT
COPY file:01e75c6dd0ce317d516928a17584d111cd082840c01e58be0afc851b33adb916 in / 
# Wed, 01 Nov 2023 03:15:40 GMT
COPY file:caec368f5a54f70a844a13005eb2255bed778809b3672d516e719ce2f4bce123 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 03:15:40 GMT
COPY file:3b1b9915b7dd898a0e32f7eb9715a35c9feab914022efff68ba990bc1ec7d169 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 03:15:40 GMT
COPY file:57846632accc89753f45cbc00cb9e6223d991e1d31297eec3395a7ca58eed6a6 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 03:15:40 GMT
COPY file:9e3b2b63db9f8fc702e2dc2bdd0943be0d990c028cddcf1c159f5556a8ba3030 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 03:15:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 03:15:41 GMT
EXPOSE 80
# Wed, 01 Nov 2023 03:15:41 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Nov 2023 03:15:41 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:8d7feeb74478e4770869563dfee6adf560c449e1ac037f4250fde21517f75323`  
		Last Modified: Wed, 01 Nov 2023 00:51:29 GMT  
		Size: 26.9 MB (26921998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e8a468f2b53e4b2ad1223bca713b51b11b883292a71a8aee6dd6fb5fb5df9d`  
		Last Modified: Wed, 01 Nov 2023 03:22:38 GMT  
		Size: 36.2 MB (36190717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437cb5155760c3eb1ef9d5da1eef27afd5b4fa773f96a95d04bf6a891338a9e1`  
		Last Modified: Wed, 01 Nov 2023 03:22:31 GMT  
		Size: 628.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1625530c9fd27a7809464c339bd6617507abd3c4667f12fcb6717ec76ce1565c`  
		Last Modified: Wed, 01 Nov 2023 03:22:31 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3362052a494baad50acfe70617e2240bc05e101c89211f99173906787583af43`  
		Last Modified: Wed, 01 Nov 2023 03:22:31 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4265fa56e45abc2f9fb70fbafc65357af0a538e48ed6d6ffa31cbd9ac156b60f`  
		Last Modified: Wed, 01 Nov 2023 03:22:31 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e731dd49112ce49bca18f2a1b1eb0c1b834de2bc5597b9e382aab6ef6dedb5`  
		Last Modified: Wed, 01 Nov 2023 03:22:31 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; arm variant v7

```console
$ docker pull nginx@sha256:ace2c553858adea7dd7603797a58221fd8040552f433dd2307469b7cf3a2119b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59498203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82d38d64dd2cc862b73e1e29b301be6956796150b7e725a7f296a472c4f5dcd2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 11:07:50 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 21 Nov 2023 11:07:50 GMT
ENV NGINX_VERSION=1.25.3
# Tue, 21 Nov 2023 11:07:50 GMT
ENV NJS_VERSION=0.8.2
# Tue, 21 Nov 2023 11:07:50 GMT
ENV PKG_RELEASE=1~bookworm
# Tue, 21 Nov 2023 11:11:42 GMT
RUN set -x     && groupadd --system --gid 101 nginx     && useradd --system --gid nginx --no-create-home --home /nonexistent --comment "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     NGINX_GPGKEY_PATH=/usr/share/keyrings/nginx-archive-keyring.gpg;     export GNUPGHOME="$(mktemp -d)";     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         gpg1 --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     gpg1 --export "$NGINX_GPGKEY" > "$NGINX_GPGKEY_PATH" ;     rm -rf "$GNUPGHOME";     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 21 Nov 2023 11:11:42 GMT
COPY file:01e75c6dd0ce317d516928a17584d111cd082840c01e58be0afc851b33adb916 in / 
# Tue, 21 Nov 2023 11:11:42 GMT
COPY file:caec368f5a54f70a844a13005eb2255bed778809b3672d516e719ce2f4bce123 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 11:11:42 GMT
COPY file:3b1b9915b7dd898a0e32f7eb9715a35c9feab914022efff68ba990bc1ec7d169 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 11:11:42 GMT
COPY file:57846632accc89753f45cbc00cb9e6223d991e1d31297eec3395a7ca58eed6a6 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 11:11:42 GMT
COPY file:9e3b2b63db9f8fc702e2dc2bdd0943be0d990c028cddcf1c159f5556a8ba3030 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 11:11:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 11:11:43 GMT
EXPOSE 80
# Tue, 21 Nov 2023 11:11:43 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Nov 2023 11:11:43 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4b8a65a42c79502f4416e01bfa41ab419f5d095369b6a425c0f32f1b3839fd`  
		Last Modified: Tue, 21 Nov 2023 11:18:39 GMT  
		Size: 34.7 MB (34744696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cde0c8e09ffcec0ebe8aeb9b108bf17840d149611a33da7e032a1e3a166047`  
		Last Modified: Tue, 21 Nov 2023 11:18:32 GMT  
		Size: 628.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba111f8d5e5afe12051556d8062063d580263b9c2bd4fc0aefe86b80c0eef024`  
		Last Modified: Tue, 21 Nov 2023 11:18:36 GMT  
		Size: 961.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f4f8013f5879f8ac3d07bb02e7d8a880f66afb4f7d6d766b391bf19dae977e`  
		Last Modified: Tue, 21 Nov 2023 11:18:31 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80afb86381788f45b1a77bda5d411e4e0165454bad72a3eb9be0de2ce12c316`  
		Last Modified: Tue, 21 Nov 2023 11:18:31 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d38017a334a2178d906d0229b5e265d8c9eac71f8be0a7c0be422c355241aef`  
		Last Modified: Tue, 21 Nov 2023 11:18:31 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:736342e81e97220f954b8c33846ba80d2d95f59b30225a5c63d063c8b250b0ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67229776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5628e5ea3c17fa1cbf49692edf41d5a1cdf198922898e6ffb29c19768dca8fd3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:16:36 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 21 Nov 2023 10:16:36 GMT
ENV NGINX_VERSION=1.25.3
# Tue, 21 Nov 2023 10:16:36 GMT
ENV NJS_VERSION=0.8.2
# Tue, 21 Nov 2023 10:16:36 GMT
ENV PKG_RELEASE=1~bookworm
# Tue, 21 Nov 2023 10:16:57 GMT
RUN set -x     && groupadd --system --gid 101 nginx     && useradd --system --gid nginx --no-create-home --home /nonexistent --comment "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     NGINX_GPGKEY_PATH=/usr/share/keyrings/nginx-archive-keyring.gpg;     export GNUPGHOME="$(mktemp -d)";     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         gpg1 --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     gpg1 --export "$NGINX_GPGKEY" > "$NGINX_GPGKEY_PATH" ;     rm -rf "$GNUPGHOME";     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 21 Nov 2023 10:16:57 GMT
COPY file:01e75c6dd0ce317d516928a17584d111cd082840c01e58be0afc851b33adb916 in / 
# Tue, 21 Nov 2023 10:16:57 GMT
COPY file:caec368f5a54f70a844a13005eb2255bed778809b3672d516e719ce2f4bce123 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 10:16:57 GMT
COPY file:3b1b9915b7dd898a0e32f7eb9715a35c9feab914022efff68ba990bc1ec7d169 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 10:16:57 GMT
COPY file:57846632accc89753f45cbc00cb9e6223d991e1d31297eec3395a7ca58eed6a6 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 10:16:57 GMT
COPY file:9e3b2b63db9f8fc702e2dc2bdd0943be0d990c028cddcf1c159f5556a8ba3030 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 10:16:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 10:16:58 GMT
EXPOSE 80
# Tue, 21 Nov 2023 10:16:58 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Nov 2023 10:16:58 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf6824a0232d7aa50c5587c1bf380ea40cc4b652207456a5deefb30bdef7d4d`  
		Last Modified: Tue, 21 Nov 2023 10:18:32 GMT  
		Size: 38.0 MB (38045928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47d5fcfb558a01e9e6b3e482d4823a35352f536906027afda7f34bbdedb5c5c`  
		Last Modified: Tue, 21 Nov 2023 10:18:26 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecba2628ac35e21c69ee48bbb50460f683b341a5f78f51091da57e689ccb539a`  
		Last Modified: Tue, 21 Nov 2023 10:18:26 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d082d8e4ce10fe6ba51e900cab49b516b0a0d51baa345fd48eb1485e1fb68ef`  
		Last Modified: Tue, 21 Nov 2023 10:18:26 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b90333fd43183032cd31e1779808c0fb5c1386f97b8b4d0331715647d88dfc`  
		Last Modified: Tue, 21 Nov 2023 10:18:26 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef920b5aa7fc69b173b087c1b358f15733a432c1b94d0d5ae51049012c7a32e`  
		Last Modified: Tue, 21 Nov 2023 10:18:26 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; 386

```console
$ docker pull nginx@sha256:610ae6006653195e9b5150f883d72d0e31e25d0234b995069902ed21a4396736
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68696698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb428429f42bb7a53d78c2f3e410f9fa5be2223b17d20fab187b6865fdaebf54`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:56 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Wed, 01 Nov 2023 00:38:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 09:41:00 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Nov 2023 09:41:00 GMT
ENV NGINX_VERSION=1.25.3
# Wed, 01 Nov 2023 09:41:00 GMT
ENV NJS_VERSION=0.8.2
# Wed, 01 Nov 2023 09:41:01 GMT
ENV PKG_RELEASE=1~bookworm
# Wed, 01 Nov 2023 09:46:28 GMT
RUN set -x     && groupadd --system --gid 101 nginx     && useradd --system --gid nginx --no-create-home --home /nonexistent --comment "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     NGINX_GPGKEY_PATH=/usr/share/keyrings/nginx-archive-keyring.gpg;     export GNUPGHOME="$(mktemp -d)";     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         gpg1 --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     gpg1 --export "$NGINX_GPGKEY" > "$NGINX_GPGKEY_PATH" ;     rm -rf "$GNUPGHOME";     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Nov 2023 09:46:29 GMT
COPY file:01e75c6dd0ce317d516928a17584d111cd082840c01e58be0afc851b33adb916 in / 
# Wed, 01 Nov 2023 09:46:29 GMT
COPY file:caec368f5a54f70a844a13005eb2255bed778809b3672d516e719ce2f4bce123 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 09:46:29 GMT
COPY file:3b1b9915b7dd898a0e32f7eb9715a35c9feab914022efff68ba990bc1ec7d169 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 09:46:29 GMT
COPY file:57846632accc89753f45cbc00cb9e6223d991e1d31297eec3395a7ca58eed6a6 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 09:46:29 GMT
COPY file:9e3b2b63db9f8fc702e2dc2bdd0943be0d990c028cddcf1c159f5556a8ba3030 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 09:46:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 09:46:30 GMT
EXPOSE 80
# Wed, 01 Nov 2023 09:46:30 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Nov 2023 09:46:30 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf41f56f631004325011843f5f3b5f87396cfda71fd444a9901faae571f087`  
		Last Modified: Wed, 01 Nov 2023 09:54:44 GMT  
		Size: 38.5 MB (38528075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e233498b51f12ec60b08b490a76e4f7edc0501f84d37377e4ba4e9b531a553ff`  
		Last Modified: Wed, 01 Nov 2023 09:54:34 GMT  
		Size: 628.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f315189a1c530b7ad85b24e501460b988a7f23cc108d2f164e8bcede0055b9`  
		Last Modified: Wed, 01 Nov 2023 09:54:34 GMT  
		Size: 961.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f4a8ea0f64f79c7c6f8c74a128c3010985d58fe047c034edc8b18293625b88`  
		Last Modified: Wed, 01 Nov 2023 09:54:34 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7e0f979564c8eb3d71fedcf1b737fd0eca5a4c25f3bb366e2396c2fd6411de`  
		Last Modified: Wed, 01 Nov 2023 09:54:34 GMT  
		Size: 1.2 KB (1215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d8a6b6e09378c4877453c96e518103c34721519d6f9142d62071e5046f5ca4`  
		Last Modified: Wed, 01 Nov 2023 09:54:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; mips64le

```console
$ docker pull nginx@sha256:26e05ad1e5651db4a3b661130cb5a9a52f5af09b106f7884e6fa331ce3cdc791
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66198094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3a50aa2b286fb5f42c3650c567e46c5a3154e347953816841a58f6ec2b43d07`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:01 GMT
ADD file:902f83a7b431527b044dd807bec38e30f5402c6a655e71f1c8addec0f384768f in / 
# Wed, 01 Nov 2023 01:09:05 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:54:34 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Nov 2023 06:54:36 GMT
ENV NGINX_VERSION=1.25.3
# Wed, 01 Nov 2023 06:54:39 GMT
ENV NJS_VERSION=0.8.2
# Wed, 01 Nov 2023 06:54:41 GMT
ENV PKG_RELEASE=1~bookworm
# Wed, 01 Nov 2023 07:12:51 GMT
RUN set -x     && groupadd --system --gid 101 nginx     && useradd --system --gid nginx --no-create-home --home /nonexistent --comment "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     NGINX_GPGKEY_PATH=/usr/share/keyrings/nginx-archive-keyring.gpg;     export GNUPGHOME="$(mktemp -d)";     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         gpg1 --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     gpg1 --export "$NGINX_GPGKEY" > "$NGINX_GPGKEY_PATH" ;     rm -rf "$GNUPGHOME";     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Nov 2023 07:12:53 GMT
COPY file:01e75c6dd0ce317d516928a17584d111cd082840c01e58be0afc851b33adb916 in / 
# Wed, 01 Nov 2023 07:12:55 GMT
COPY file:caec368f5a54f70a844a13005eb2255bed778809b3672d516e719ce2f4bce123 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 07:12:57 GMT
COPY file:3b1b9915b7dd898a0e32f7eb9715a35c9feab914022efff68ba990bc1ec7d169 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 07:12:59 GMT
COPY file:57846632accc89753f45cbc00cb9e6223d991e1d31297eec3395a7ca58eed6a6 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 07:13:01 GMT
COPY file:9e3b2b63db9f8fc702e2dc2bdd0943be0d990c028cddcf1c159f5556a8ba3030 in /docker-entrypoint.d 
# Wed, 01 Nov 2023 07:13:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 07:13:07 GMT
EXPOSE 80
# Wed, 01 Nov 2023 07:13:09 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Nov 2023 07:13:12 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:0d679670615aaadf144eccb296137109a3362efe18b995cdfda7614231abd659`  
		Last Modified: Wed, 01 Nov 2023 01:19:46 GMT  
		Size: 29.1 MB (29141870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a431147892fcaa92d14c7accc9702e65612ea84d7a1f3e58188aeaddbed868`  
		Last Modified: Wed, 01 Nov 2023 07:40:48 GMT  
		Size: 37.1 MB (37051642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4db06dca9d19baf487748809f517deef9ddb9c0b5e51d1db110069d18b1b68a`  
		Last Modified: Wed, 01 Nov 2023 07:40:24 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d24d37de02dd51c19759dba35d8b64fb470bb13823514713a43e2c09c8a7688`  
		Last Modified: Wed, 01 Nov 2023 07:40:24 GMT  
		Size: 961.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5161006da404561b990d9bdf53398d4a4182c26d2a0b3527f23a3a549d524d`  
		Last Modified: Wed, 01 Nov 2023 07:40:24 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d257833b67781f8c42201c0fac00375b35d2158e1090d258e105c378b77842`  
		Last Modified: Wed, 01 Nov 2023 07:40:24 GMT  
		Size: 1.2 KB (1215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b9608b3866cfc63911937827af51304636dc91dd756a3ac3caa455358e03dd`  
		Last Modified: Wed, 01 Nov 2023 07:40:24 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; ppc64le

```console
$ docker pull nginx@sha256:b6cd7141b3b33ce086013d60e2c7686d95665f516ccd30b618e32c998a4fd334
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74945401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3555b59851f67c7df74c7c3d09fb91eeaa2af165457e8b0ec51b10d5c58be99b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:16:37 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 21 Nov 2023 08:16:37 GMT
ENV NGINX_VERSION=1.25.3
# Tue, 21 Nov 2023 08:16:37 GMT
ENV NJS_VERSION=0.8.2
# Tue, 21 Nov 2023 08:16:37 GMT
ENV PKG_RELEASE=1~bookworm
# Tue, 21 Nov 2023 08:21:44 GMT
RUN set -x     && groupadd --system --gid 101 nginx     && useradd --system --gid nginx --no-create-home --home /nonexistent --comment "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     NGINX_GPGKEY_PATH=/usr/share/keyrings/nginx-archive-keyring.gpg;     export GNUPGHOME="$(mktemp -d)";     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         gpg1 --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     gpg1 --export "$NGINX_GPGKEY" > "$NGINX_GPGKEY_PATH" ;     rm -rf "$GNUPGHOME";     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 21 Nov 2023 08:21:46 GMT
COPY file:01e75c6dd0ce317d516928a17584d111cd082840c01e58be0afc851b33adb916 in / 
# Tue, 21 Nov 2023 08:21:46 GMT
COPY file:caec368f5a54f70a844a13005eb2255bed778809b3672d516e719ce2f4bce123 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 08:21:46 GMT
COPY file:3b1b9915b7dd898a0e32f7eb9715a35c9feab914022efff68ba990bc1ec7d169 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 08:21:47 GMT
COPY file:57846632accc89753f45cbc00cb9e6223d991e1d31297eec3395a7ca58eed6a6 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 08:21:47 GMT
COPY file:9e3b2b63db9f8fc702e2dc2bdd0943be0d990c028cddcf1c159f5556a8ba3030 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 08:21:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 08:21:47 GMT
EXPOSE 80
# Tue, 21 Nov 2023 08:21:48 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Nov 2023 08:21:48 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54db3f037fa0ddd5a42661e6fc934f01792ef3e56dad9486143f84e37db666f`  
		Last Modified: Tue, 21 Nov 2023 08:30:36 GMT  
		Size: 41.8 MB (41799213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c350ebbc66836ecaf5324c8ff7d8265d3da45f4f6c5c251db37a379a701527a`  
		Last Modified: Tue, 21 Nov 2023 08:30:27 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06590c5f207b93522b9e6e8a10c0da2c914d733f07814b8e334faeb076ab8959`  
		Last Modified: Tue, 21 Nov 2023 08:30:27 GMT  
		Size: 961.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1126b368d9cc1dfa29db89dea667caadf1702a6d9d9b72b535bf2e5fd55c31a2`  
		Last Modified: Tue, 21 Nov 2023 08:30:27 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dc414c67b863783d37848463ba9e987d68652492689bc7d26d63b86676d0c8`  
		Last Modified: Tue, 21 Nov 2023 08:30:27 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1049c09dd67d23320fa7c3ceb11005bbd4f5f094d4849c0fe67489f0e9b662b`  
		Last Modified: Tue, 21 Nov 2023 08:30:27 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline` - linux; s390x

```console
$ docker pull nginx@sha256:c3ce3d388b3e488777a69198642a499c74518db8aab88f59b85fa584dc7a1316
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.8 MB (64846595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df79115e2171398b152854ae4137eba7446f529d93f8fb3fc95c2bc92554b89`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:04:36 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 21 Nov 2023 07:04:37 GMT
ENV NGINX_VERSION=1.25.3
# Tue, 21 Nov 2023 07:04:37 GMT
ENV NJS_VERSION=0.8.2
# Tue, 21 Nov 2023 07:04:37 GMT
ENV PKG_RELEASE=1~bookworm
# Tue, 21 Nov 2023 07:07:33 GMT
RUN set -x     && groupadd --system --gid 101 nginx     && useradd --system --gid nginx --no-create-home --home /nonexistent --comment "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     NGINX_GPGKEY_PATH=/usr/share/keyrings/nginx-archive-keyring.gpg;     export GNUPGHOME="$(mktemp -d)";     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         gpg1 --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     gpg1 --export "$NGINX_GPGKEY" > "$NGINX_GPGKEY_PATH" ;     rm -rf "$GNUPGHOME";     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src [signed-by=$NGINX_GPGKEY_PATH] https://nginx.org/packages/mainline/debian/ bookworm nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Tue, 21 Nov 2023 07:07:35 GMT
COPY file:01e75c6dd0ce317d516928a17584d111cd082840c01e58be0afc851b33adb916 in / 
# Tue, 21 Nov 2023 07:07:35 GMT
COPY file:caec368f5a54f70a844a13005eb2255bed778809b3672d516e719ce2f4bce123 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 07:07:35 GMT
COPY file:3b1b9915b7dd898a0e32f7eb9715a35c9feab914022efff68ba990bc1ec7d169 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 07:07:35 GMT
COPY file:57846632accc89753f45cbc00cb9e6223d991e1d31297eec3395a7ca58eed6a6 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 07:07:35 GMT
COPY file:9e3b2b63db9f8fc702e2dc2bdd0943be0d990c028cddcf1c159f5556a8ba3030 in /docker-entrypoint.d 
# Tue, 21 Nov 2023 07:07:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 07:07:36 GMT
EXPOSE 80
# Tue, 21 Nov 2023 07:07:36 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Nov 2023 07:07:36 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6ab77bc599aaa40d036818d2699f77f0cf65a59995eb601bfd1997c5e33a0d`  
		Last Modified: Tue, 21 Nov 2023 07:14:19 GMT  
		Size: 37.3 MB (37329134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7b61a97f737aff097ba06175da51d8a3a8cec8ead80ef6b2a15aeeaeb60bca`  
		Last Modified: Tue, 21 Nov 2023 07:14:13 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa0b40db5619ae9f315372e5b62d2826154cbcd25513e011d9c7254e36402b6`  
		Last Modified: Tue, 21 Nov 2023 07:14:13 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e602139478d3153fcb5ba39b2b242c703550229a67edb7bcd5c173866b897cc3`  
		Last Modified: Tue, 21 Nov 2023 07:14:13 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbb8fdcb91dd6b60d2d7c0733cb6ab63c9b34d604bea650c910f886bf28b7e9`  
		Last Modified: Tue, 21 Nov 2023 07:14:13 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b098410bb35d11572cb33086dcc9fd3b62412746b5f68639d2b7b10f36687929`  
		Last Modified: Tue, 21 Nov 2023 07:14:13 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
