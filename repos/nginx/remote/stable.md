## `nginx:stable`

```console
$ docker pull nginx@sha256:032bee3fd159cf340314739866268042291b9563e1dc563931a5e9144c699232
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
$ docker pull nginx@sha256:d7573e9b475c64dbf09dac0808517e8d5a919918aa772ceca381091365a970aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56812126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c9eabeac475449c72ad457ccbc014788a02dbbc64f24158b0a40fdc5def2dc9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 18:42:53 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Mar 2023 18:43:33 GMT
ENV NGINX_VERSION=1.22.1
# Wed, 01 Mar 2023 18:43:33 GMT
ENV NJS_VERSION=0.7.7
# Wed, 01 Mar 2023 18:43:33 GMT
ENV PKG_RELEASE=1~bullseye
# Wed, 01 Mar 2023 18:43:51 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 18:43:51 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 18:43:51 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 18:43:51 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 18:43:51 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 18:43:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 18:43:51 GMT
EXPOSE 80
# Wed, 01 Mar 2023 18:43:51 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 18:43:52 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3cdc1adeef9cbd6fd04801bf2b50e410555a227dd942052fd10e00e273cd5a`  
		Last Modified: Wed, 01 Mar 2023 18:45:42 GMT  
		Size: 25.4 MB (25396961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d20c7b11e51f844cd1df7d0c39d52308612c7868e50eb59b14271b92c8824a5`  
		Last Modified: Wed, 01 Mar 2023 18:45:38 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f98bdf28b77e45d609499eba86cb3c2cc17e1b07b93f39c10ec3f4fadd2086d`  
		Last Modified: Wed, 01 Mar 2023 18:45:38 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f8f705fe4d993a83d7ca82d173d09ab016755072999eb83e94bb0fee195545`  
		Last Modified: Wed, 01 Mar 2023 18:45:38 GMT  
		Size: 773.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66350be01a8b3b6ae3a0d6d47b65c3d0c13eff97421f3ec420741a03f03f911d`  
		Last Modified: Wed, 01 Mar 2023 18:45:38 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; arm variant v5

```console
$ docker pull nginx@sha256:373bc0416c9403dbba8ecda2579ccb50b856a3f19d52ea0587fd04ceb8c18d14
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53493030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1faad1a8d46b98b12c2d866cb1d2f57e6d221ae11626354a9acfad8bfc8f4996`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 10:06:00 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Mar 2023 10:11:05 GMT
ENV NGINX_VERSION=1.22.1
# Wed, 01 Mar 2023 10:11:05 GMT
ENV NJS_VERSION=0.7.7
# Wed, 01 Mar 2023 10:11:06 GMT
ENV PKG_RELEASE=1~bullseye
# Wed, 01 Mar 2023 10:14:24 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 10:14:24 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 10:14:24 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 10:14:24 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 10:14:24 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 10:14:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 10:14:24 GMT
EXPOSE 80
# Wed, 01 Mar 2023 10:14:24 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 10:14:24 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88af123d2fb8d709bf23a020b2ee7a8a90e08033c9096bc1f25219d9229d5a9d`  
		Last Modified: Wed, 01 Mar 2023 10:19:49 GMT  
		Size: 24.6 MB (24573498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20444a7080183109db57eaccb27d87ae63f5d573624986c4ff66a904b8860fd6`  
		Last Modified: Wed, 01 Mar 2023 10:19:45 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a2eb6f53eff13c9123d04f769616b17e0de883206eac88e1e8cad127278518`  
		Last Modified: Wed, 01 Mar 2023 10:19:45 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92adf6b95dee1ef8fd2eedc8dfe1fac1c5180fba334fe8735ae38e2e90e610e4`  
		Last Modified: Wed, 01 Mar 2023 10:19:45 GMT  
		Size: 772.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c4eadb9c0b2f11f8e9cf7dcf6de56975f2518a4d5e2b453955236af26ba875`  
		Last Modified: Wed, 01 Mar 2023 10:19:45 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; arm variant v7

```console
$ docker pull nginx@sha256:f516ab7631865ee3c3ca66482ef74a00cd7dec5b2a6d4af0da445d00223349f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50294482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64bbe3d719a80d40916a146fcdd70f0b473815cd51fe5d3a170fe1eca061f70`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:55 GMT
ADD file:182fe91b8976a8871aba0d2ff9d4400a60317c8dec282261ba94247500c8d3dc in / 
# Wed, 01 Mar 2023 01:57:55 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:54:50 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Mar 2023 06:00:04 GMT
ENV NGINX_VERSION=1.22.1
# Wed, 01 Mar 2023 06:00:04 GMT
ENV NJS_VERSION=0.7.7
# Wed, 01 Mar 2023 06:00:04 GMT
ENV PKG_RELEASE=1~bullseye
# Wed, 01 Mar 2023 06:03:00 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 06:03:00 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 06:03:00 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 06:03:00 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 06:03:00 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 06:03:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 06:03:00 GMT
EXPOSE 80
# Wed, 01 Mar 2023 06:03:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 06:03:00 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:b4770fcf2ef78c1e46693da734476bfaf03cbe1d0b6e0a0f22c2c2e53419e803`  
		Last Modified: Wed, 01 Mar 2023 02:03:02 GMT  
		Size: 26.6 MB (26577290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6345b1e53b4ac1dd89f1fcee511976552aad1e9466dc281f14c7e9079ed3eabb`  
		Last Modified: Wed, 01 Mar 2023 06:17:23 GMT  
		Size: 23.7 MB (23713427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95df4c8daf7722f40f17481b72b5a38f5a6f6fc3ecaef1371ce52f317740735`  
		Last Modified: Wed, 01 Mar 2023 06:17:20 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffdc342da41b1e3466843c6fa89eb9ee2244064324d3451e0154297bf237d4`  
		Last Modified: Wed, 01 Mar 2023 06:17:20 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99780a0dbc4cd62cff848bfcbb4b0c1fb157cfde8aee9eaa15c9a7a47226fe2e`  
		Last Modified: Wed, 01 Mar 2023 06:17:20 GMT  
		Size: 774.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6456a376057e3650ae13b12b9cf92f866742082f266b5df705b533587d7f6985`  
		Last Modified: Wed, 01 Mar 2023 06:17:20 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:8138170eed7e5e6cbf670729e955418df64a1193dde199185c942e95872b55ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.4 MB (55390369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa87272e39e04fff1a198672eb46bb4df78409cd4e7cd50bf61fb51923e49daf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 05:50:26 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Thu, 23 Mar 2023 05:50:57 GMT
ENV NGINX_VERSION=1.22.1
# Thu, 23 Mar 2023 05:50:57 GMT
ENV NJS_VERSION=0.7.7
# Thu, 23 Mar 2023 05:50:57 GMT
ENV PKG_RELEASE=1~bullseye
# Thu, 23 Mar 2023 05:51:12 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Thu, 23 Mar 2023 05:51:12 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Thu, 23 Mar 2023 05:51:12 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Thu, 23 Mar 2023 05:51:13 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Thu, 23 Mar 2023 05:51:13 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Thu, 23 Mar 2023 05:51:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 05:51:13 GMT
EXPOSE 80
# Thu, 23 Mar 2023 05:51:13 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Mar 2023 05:51:13 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc7b6799e96b05e3e02a27db3cbdf5c2a80fbbd261ff287e1ad411ee81b59da`  
		Last Modified: Thu, 23 Mar 2023 05:52:31 GMT  
		Size: 25.3 MB (25323910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bd528d94a7e1b9f2f32551885704b5dfa3f9716676bb15607de655d9600cfd`  
		Last Modified: Thu, 23 Mar 2023 05:52:28 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de23ca89dc04c4b38c40ba40a170e2b4ace1fdff3c7fc9c3378008560e44ca2`  
		Last Modified: Thu, 23 Mar 2023 05:52:28 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea51009af177c2a6ceefa86cf4c7b927b5213aee8b69940196e86f4184257dd`  
		Last Modified: Thu, 23 Mar 2023 05:52:28 GMT  
		Size: 772.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e86cbceee09ab6c900ccce5836a8d33dd3b616bdfb0a5ac548197e56bd29eb7`  
		Last Modified: Thu, 23 Mar 2023 05:52:28 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; 386

```console
$ docker pull nginx@sha256:c21d45d6975382a186c033fb531f994a8feec85a7661a81da9d3eead4f785945
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.7 MB (58715374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2236ce4e3b7dc5e08637cc3d8476e420639938128d043355125e57bb6f638a6c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:14 GMT
ADD file:7ff48f7b36d13400120a726cd394769a4c39e8424877f5b080aeb9da07eacebe in / 
# Wed, 01 Mar 2023 01:39:15 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:29:58 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Mar 2023 13:37:12 GMT
ENV NGINX_VERSION=1.22.1
# Wed, 01 Mar 2023 13:37:12 GMT
ENV NJS_VERSION=0.7.7
# Wed, 01 Mar 2023 13:37:12 GMT
ENV PKG_RELEASE=1~bullseye
# Wed, 01 Mar 2023 13:41:01 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 13:41:02 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 13:41:02 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 13:41:02 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 13:41:02 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 13:41:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 13:41:02 GMT
EXPOSE 80
# Wed, 01 Mar 2023 13:41:02 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 13:41:02 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:2b884ef8a2d2b7c2016a8d2926b5b284f2130128ee049cae31a2da609cda7257`  
		Last Modified: Wed, 01 Mar 2023 01:44:44 GMT  
		Size: 32.4 MB (32396138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63381a202f792465b73f3c72b70cc02ba35213aa4bdf80f7232d46d43ba28307`  
		Last Modified: Wed, 01 Mar 2023 13:59:40 GMT  
		Size: 26.3 MB (26315474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e7f4d6047bc20378c92c9ec9e38b3ffdecfb9c828fb985bc6f2cc23822ea52`  
		Last Modified: Wed, 01 Mar 2023 13:59:36 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5847cdf4ce4e3bf79f74736140c25957daf7925337c3bdb53cf9bb91bc4a831`  
		Last Modified: Wed, 01 Mar 2023 13:59:36 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274a60bb8ab09c43d42ff52e3429a157c43cfbbe6d71a3d308a974baeee15f47`  
		Last Modified: Wed, 01 Mar 2023 13:59:36 GMT  
		Size: 773.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77def705c5c62fe9313a929180152804af77a984e7b32e44fea8b38372b70c1`  
		Last Modified: Wed, 01 Mar 2023 13:59:36 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; mips64le

```console
$ docker pull nginx@sha256:ce0fae69e50a49f4917427c9364231b0c1ad4e29280ba0a92942bac7d30ff030
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54926351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f98f9689b4e762711f1652a7fc2d9c5e64bffb095a137f3d324941b76af655`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:54 GMT
ADD file:0bcd66a6a099cdb6e018ddc0f00270be93dccd3be6167ce36e9efc99c31549d9 in / 
# Wed, 01 Mar 2023 02:10:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 10:32:23 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Mar 2023 10:53:42 GMT
ENV NGINX_VERSION=1.22.1
# Wed, 01 Mar 2023 10:53:44 GMT
ENV NJS_VERSION=0.7.7
# Wed, 01 Mar 2023 10:53:47 GMT
ENV PKG_RELEASE=1~bullseye
# Wed, 01 Mar 2023 11:09:02 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 11:09:04 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 11:09:06 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 11:09:08 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 11:09:10 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 11:09:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 11:09:15 GMT
EXPOSE 80
# Wed, 01 Mar 2023 11:09:17 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 11:09:20 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:89f6b45a7afd174bf0d443156831cacd9e6a26c834ad62610b6db53c731d257f`  
		Last Modified: Wed, 01 Mar 2023 02:18:50 GMT  
		Size: 29.6 MB (29634488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea08fcbbcb05bc5797088e433f883351832481a9d3063b09e95cdf741116532b`  
		Last Modified: Wed, 01 Mar 2023 11:27:43 GMT  
		Size: 25.3 MB (25288095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ea30fd5d80183eede825521408b1cdecf55b13b8136514c56a6c06e1db9c95`  
		Last Modified: Wed, 01 Mar 2023 11:27:29 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f754cf21322fb5c02eee363a48cf315a3ac7421f9cc7525b93ae350d780a1c8f`  
		Last Modified: Wed, 01 Mar 2023 11:27:29 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68099b11bb7f09763557dfadb26e4a1e1c1a0813a80a71ad3161ac90b4dc313e`  
		Last Modified: Wed, 01 Mar 2023 11:27:29 GMT  
		Size: 775.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6185b8073b067b846a831b62803977c4e8822bac59332325978298906f69df85`  
		Last Modified: Wed, 01 Mar 2023 11:27:29 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; ppc64le

```console
$ docker pull nginx@sha256:e5c3776fc958baac6014cb9c448c22eeca4ad58d2781129e56530c1c239e6196
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.5 MB (62532925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efd52da1211d68f6cc97a568cdc161d5228260b16b0e9022c2e1776cbf13c6b1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:42:35 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Mar 2023 07:53:46 GMT
ENV NGINX_VERSION=1.22.1
# Wed, 01 Mar 2023 07:53:46 GMT
ENV NJS_VERSION=0.7.7
# Wed, 01 Mar 2023 07:53:47 GMT
ENV PKG_RELEASE=1~bullseye
# Wed, 01 Mar 2023 08:01:54 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 08:01:56 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 08:01:56 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 08:01:56 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 08:01:57 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 08:01:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 08:01:57 GMT
EXPOSE 80
# Wed, 01 Mar 2023 08:01:58 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 08:01:59 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf07410949b5c425dc65d6feffa5b94829e51d9d6261464c9985e456cfc884aa`  
		Last Modified: Wed, 01 Mar 2023 08:12:26 GMT  
		Size: 27.2 MB (27241058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51beeacc35b0306ccdedc835ae84cddcfb6c122849bf331620169d8c0279b8b1`  
		Last Modified: Wed, 01 Mar 2023 08:12:20 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2bfbcf6f5a4aeaeb5281379a1d010fcb6f9374ba67f3e57a8b6f609cac08e4`  
		Last Modified: Wed, 01 Mar 2023 08:12:20 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dee03f7b55e7cd972114cbb3e1d32ca8d986ff227cbcc03851c07f84b8ca8b9`  
		Last Modified: Wed, 01 Mar 2023 08:12:20 GMT  
		Size: 774.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7535fb7f05a3cdec0bbe1ddc9959db90c9dbc3986e5c302d06d044e4b29c0498`  
		Last Modified: Wed, 01 Mar 2023 08:12:20 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable` - linux; s390x

```console
$ docker pull nginx@sha256:6b70c15747c34e9dfa632ba74e5e08bf44e767c7692a7e36783b96172222c3b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54864321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92561d3a6025d209a5ef71171e33ff5f1da5acf31d1f59c8bc53eb14e0553635`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:30 GMT
ADD file:01aa3de7444f0716938e0d85522be065193be4ffb6788b3190a0f4fefdbb8d65 in / 
# Wed, 01 Mar 2023 02:50:31 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:18:48 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 01 Mar 2023 04:22:17 GMT
ENV NGINX_VERSION=1.22.1
# Wed, 01 Mar 2023 04:22:17 GMT
ENV NJS_VERSION=0.7.7
# Wed, 01 Mar 2023 04:22:17 GMT
ENV PKG_RELEASE=1~bullseye
# Wed, 01 Mar 2023 04:24:31 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 04:24:32 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 04:24:32 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 04:24:32 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 04:24:33 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 04:24:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:24:33 GMT
EXPOSE 80
# Wed, 01 Mar 2023 04:24:33 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 04:24:33 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:7b8d78f42e32e7fa234bcf890ae6603acab2881bca68a9d8c429981c7f42b1d6`  
		Last Modified: Wed, 01 Mar 2023 02:54:48 GMT  
		Size: 29.6 MB (29646854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1ce7451fb69d09dbeccf2bca9c9a63e72cc2bab6ffaa00642198c6e4e47c66`  
		Last Modified: Wed, 01 Mar 2023 04:29:28 GMT  
		Size: 25.2 MB (25213714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5a59b2f3a72c80f3559f52120beecbb9a356f0140c40d9faaae582c8c112dc`  
		Last Modified: Wed, 01 Mar 2023 04:29:25 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695576f00585083cb0f3b212f1f2d50e86f5899cfa713974e16fb77fd20ef0d`  
		Last Modified: Wed, 01 Mar 2023 04:29:24 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a261431bf5c80e542dab3aa9f8f116662a3fec8f277b47a58b9dceebe7ac93ba`  
		Last Modified: Wed, 01 Mar 2023 04:29:24 GMT  
		Size: 770.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7a4129aa08940103d998062d8196535076ddb1347f404c11defc824206d1d8`  
		Last Modified: Wed, 01 Mar 2023 04:29:24 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
