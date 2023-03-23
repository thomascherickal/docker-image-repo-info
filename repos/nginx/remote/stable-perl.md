## `nginx:stable-perl`

```console
$ docker pull nginx@sha256:df21a34aaf7177301cc3b91e3f07b1b71b6acbb5608ac66789ffbee0067fac99
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

### `nginx:stable-perl` - linux; amd64

```console
$ docker pull nginx@sha256:eafe4c507bffceb0269becc5b202d439f880cf5928816e7e025a068b65dc7db2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67981666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0025d7892946724152e98a0bf2557e01887fa7b8aae31fb5847068fd3cefbb3`
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
# Wed, 01 Mar 2023 18:44:16 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 18:44:17 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 18:44:17 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 18:44:17 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 18:44:17 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 18:44:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 18:44:17 GMT
EXPOSE 80
# Wed, 01 Mar 2023 18:44:17 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 18:44:17 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a09cf258cad7d179f1e0f3d79a0f07edaed8bb679c412f3d1ee071e06f344f9`  
		Last Modified: Wed, 01 Mar 2023 18:45:58 GMT  
		Size: 36.6 MB (36566498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdca5e958a07b19afa4fd67224e4d8dfaa3f31c612c61c06763e7d917416fb64`  
		Last Modified: Wed, 01 Mar 2023 18:45:52 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f968ecf11927f66b6cdfcc01b1267128422fd69d527f96a36c2217c47cf5ae38`  
		Last Modified: Wed, 01 Mar 2023 18:45:52 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1520f40e879ecc4298c0a7ef580130ff78295821b3bfa574854f0f7aac0ecdc7`  
		Last Modified: Wed, 01 Mar 2023 18:45:52 GMT  
		Size: 774.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6ee87b39f4ea3b3f3ad58b1322f22bb2163ba2e8f9c0c0f62ae78aaafc420c`  
		Last Modified: Wed, 01 Mar 2023 18:45:52 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; arm variant v5

```console
$ docker pull nginx@sha256:0f0eb8b9933817a4f12a81db416ced15ffdb150c9d3a9be47c6ea6adf2196f82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63896189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065bb7ab37d0c4ed3b217de8efa8ced35d34dd8b319d39ced269796ec32a6157`
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
# Wed, 01 Mar 2023 10:18:10 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 10:18:10 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 10:18:10 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 10:18:11 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 10:18:11 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 10:18:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 10:18:11 GMT
EXPOSE 80
# Wed, 01 Mar 2023 10:18:11 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 10:18:11 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f99ebf3db3fc03b051713174854ecfb02ae368d84ad72a80387a7270d50d60`  
		Last Modified: Wed, 01 Mar 2023 10:20:09 GMT  
		Size: 35.0 MB (34976647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00e22d1e104bb450191cb09f5ce1e88eef3cf2b318895fc0b3878dc198507c7`  
		Last Modified: Wed, 01 Mar 2023 10:20:03 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4535622286b0b76b0f2998f7cc6f10d83dc9923f85c7f0653448383067cfc3d8`  
		Last Modified: Wed, 01 Mar 2023 10:20:03 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9985f6ad0b63fa7366b96fc8341c355af5457874cb70259125d4314296abedcd`  
		Last Modified: Wed, 01 Mar 2023 10:20:03 GMT  
		Size: 774.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf21e68f30f7ea81d722ada7301e845fa653ce9d33593afeeac4ed0a4d2f67`  
		Last Modified: Wed, 01 Mar 2023 10:20:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; arm variant v7

```console
$ docker pull nginx@sha256:535089a3ae24b0de02743180923b420ed3881afc61424c3bb0a778eb0deb9e8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60509671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10a26ad13921e9848080e56140ead4e78d02965b0cbd2d67e48c904443e2a10f`
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
# Wed, 01 Mar 2023 06:06:24 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 06:06:24 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 06:06:25 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 06:06:25 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 06:06:25 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 06:06:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 06:06:25 GMT
EXPOSE 80
# Wed, 01 Mar 2023 06:06:25 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 06:06:25 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:b4770fcf2ef78c1e46693da734476bfaf03cbe1d0b6e0a0f22c2c2e53419e803`  
		Last Modified: Wed, 01 Mar 2023 02:03:02 GMT  
		Size: 26.6 MB (26577290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4335fe20c196a336046c5736d22d48dbef0d83a9b9a772026b57a136e8a5e5`  
		Last Modified: Wed, 01 Mar 2023 06:17:42 GMT  
		Size: 33.9 MB (33928615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4760626b537ab8bdbbb65a85e18f514479987a8d7f49ba3c3db90dbfb80dce96`  
		Last Modified: Wed, 01 Mar 2023 06:17:36 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57b9788118e303f74decfe0cb9a6cd28170ee0042acbe47e2b3e9bd6ae0ee1b`  
		Last Modified: Wed, 01 Mar 2023 06:17:37 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f6c39c04929a17caf979a29b4232ddd0928a37bbd3a5c686024d361a6becd0`  
		Last Modified: Wed, 01 Mar 2023 06:17:36 GMT  
		Size: 774.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac08285a8d027ef07f3204765a1cb686ebd110182960aceb6748e724c795f920`  
		Last Modified: Wed, 01 Mar 2023 06:17:36 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:79e1649a1b67c14848e3427ba06cfcc8db2a10c32724d078166d892b242874eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66477896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2034cc3d3dd0dd371bf3135306229ad2e53aca49fa2f28038eea831ab295d189`
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
# Thu, 23 Mar 2023 05:51:32 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Thu, 23 Mar 2023 05:51:33 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Thu, 23 Mar 2023 05:51:33 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Thu, 23 Mar 2023 05:51:33 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Thu, 23 Mar 2023 05:51:33 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Thu, 23 Mar 2023 05:51:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 05:51:33 GMT
EXPOSE 80
# Thu, 23 Mar 2023 05:51:33 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Mar 2023 05:51:33 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdea262f4774dfca8b5627e98bc290f8127f8dab21a76d68a51bd065fbb71e68`  
		Last Modified: Thu, 23 Mar 2023 05:52:45 GMT  
		Size: 36.4 MB (36411434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb054bea9d80497ec742b8e94cf5370e91554bbf8a16bd942b6aff8924503a32`  
		Last Modified: Thu, 23 Mar 2023 05:52:41 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c340e7a9553ddef130350da742cd4597113144bec1d8db000737a4f42ccab0a`  
		Last Modified: Thu, 23 Mar 2023 05:52:41 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276abb4f9cf806abac186c270b2dfbbbf30016b604ebe2ad7a27e7bb8a575eb9`  
		Last Modified: Thu, 23 Mar 2023 05:52:41 GMT  
		Size: 773.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf1980d509c86756f25ae700f39cf67c7bad7c8faf0d6961399f3ab8b4e945a`  
		Last Modified: Thu, 23 Mar 2023 05:52:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; 386

```console
$ docker pull nginx@sha256:f764687bf39770f8fee1d1f5824acc858810584d9128cd48a4d9aed83db6bfbd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69379594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8616f83c7860abdd652d599d59345b53ec3bbd29d8609406ba695502f24e90ee`
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
# Wed, 01 Mar 2023 13:45:14 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 13:45:15 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 13:45:15 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 13:45:15 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 13:45:15 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 13:45:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 13:45:15 GMT
EXPOSE 80
# Wed, 01 Mar 2023 13:45:15 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 13:45:16 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:2b884ef8a2d2b7c2016a8d2926b5b284f2130128ee049cae31a2da609cda7257`  
		Last Modified: Wed, 01 Mar 2023 01:44:44 GMT  
		Size: 32.4 MB (32396138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c654d65a00b30126ae1401f24211ce078c7d44302719814ed37d336f9a6b6f`  
		Last Modified: Wed, 01 Mar 2023 14:00:01 GMT  
		Size: 37.0 MB (36979690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d05a034652824383eee1a2fe622e966ecf57717089417acb048fd26d87cd908`  
		Last Modified: Wed, 01 Mar 2023 13:59:53 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2bd71646fd62dee406c8671a6e354ce487a1831bf138be9e777bc0c981eef8`  
		Last Modified: Wed, 01 Mar 2023 13:59:53 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eebd373045481c622f6e3f5f8226217a68012b6f12babf086dbb6bd2d29b503`  
		Last Modified: Wed, 01 Mar 2023 13:59:53 GMT  
		Size: 775.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601485802caedfe38633e5659cac0b9b3bfd4e4a5822bd2bf6eebc8ad916b863`  
		Last Modified: Wed, 01 Mar 2023 13:59:53 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; mips64le

```console
$ docker pull nginx@sha256:c7d13905c2a21f6f1a6dbd678af6b59ec214534d683c16e107c6f14e44c563a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65373059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47252c516689a06a7a15ba89bef011235817363c512da783a648a9640f13cd9c`
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
# Wed, 01 Mar 2023 11:25:52 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 11:25:55 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 11:25:57 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 11:25:59 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 11:26:02 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 11:26:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 11:26:07 GMT
EXPOSE 80
# Wed, 01 Mar 2023 11:26:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 11:26:13 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:89f6b45a7afd174bf0d443156831cacd9e6a26c834ad62610b6db53c731d257f`  
		Last Modified: Wed, 01 Mar 2023 02:18:50 GMT  
		Size: 29.6 MB (29634488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb051cc1d8fddef3eaeb8c94d4e17a830814947b66f011987c9c8f1acfe87942`  
		Last Modified: Wed, 01 Mar 2023 11:28:17 GMT  
		Size: 35.7 MB (35734806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0881e79b56c2f34748a3839e719a6e323433d39791aabd97860e5c13b29d18f7`  
		Last Modified: Wed, 01 Mar 2023 11:27:54 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb95f188be3a0020ebf5ddda528de56a10e876fc1c46fde69ecb20876cb030`  
		Last Modified: Wed, 01 Mar 2023 11:27:54 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124300e65883b62c5b44ae21aa9bb7945f34888e28f91537004882b99638d36f`  
		Last Modified: Wed, 01 Mar 2023 11:27:54 GMT  
		Size: 774.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48ee13cc67de9e150fbfc6c04faa5e7b79cce0793af7a2592c97d7f068ba318`  
		Last Modified: Wed, 01 Mar 2023 11:27:54 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; ppc64le

```console
$ docker pull nginx@sha256:cb07c8cb1f01fe96efa337e027b642fec8aa1549f27189389b9440586a2fb748
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73907295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:585c45e8c58aad7d607c09423e8f1eb7b2171d2e27214e3311cd58305a6da02d`
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
# Wed, 01 Mar 2023 08:09:48 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 08:09:50 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 08:09:50 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 08:09:51 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 08:09:51 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 08:09:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 08:09:51 GMT
EXPOSE 80
# Wed, 01 Mar 2023 08:09:52 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 08:09:52 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8882a7f62b6dbbd6fc16f93bf67bf6b3c9858d30db97f819871189886175cc`  
		Last Modified: Wed, 01 Mar 2023 08:12:50 GMT  
		Size: 38.6 MB (38615430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cd7f99df7488a2dcf235df2c69ce683087d5d622aadb40cb2d08b09c9152c`  
		Last Modified: Wed, 01 Mar 2023 08:12:40 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a32e89f7a4f5f1a29bfac1102d8e0b417e6142deb823df3bc58fac38668255f`  
		Last Modified: Wed, 01 Mar 2023 08:12:40 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bd4f2a33e46f351aebc49c97bda3490138cc4327ebe359b3454e8e0984182d`  
		Last Modified: Wed, 01 Mar 2023 08:12:40 GMT  
		Size: 774.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423cc9694bdd73020b256fbefa3e8326635293d1c87013da2429442da3564a88`  
		Last Modified: Wed, 01 Mar 2023 08:12:40 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:stable-perl` - linux; s390x

```console
$ docker pull nginx@sha256:9dbcf04d211ea401524e9870e8499e3e2c71c73ad0c1964c6154c84501559faf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66350921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa467a2338d7297345bdc23f0369f435ac80e878db36a69c52232b98b4ec0612`
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
# Wed, 01 Mar 2023 04:27:16 GMT
RUN set -x     && addgroup --system --gid 101 nginx     && adduser --system --disabled-login --ingroup nginx --no-create-home --home /nonexistent --gecos "nginx user" --shell /bin/false --uid 101 nginx     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y gnupg1 ca-certificates     &&     NGINX_GPGKEY=573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62;     found='';     for server in         hkp://keyserver.ubuntu.com:80         pgp.mit.edu     ; do         echo "Fetching GPG key $NGINX_GPGKEY from $server";         apt-key adv --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$NGINX_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $NGINX_GPGKEY" && exit 1;     apt-get remove --purge --auto-remove -y gnupg1 && rm -rf /var/lib/apt/lists/*     && dpkgArch="$(dpkg --print-architecture)"     && nginxPackages="         nginx=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-perl=${NGINX_VERSION}-${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}+${NJS_VERSION}-${PKG_RELEASE}     "     && case "$dpkgArch" in         amd64|arm64)             echo "deb https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list             && apt-get update             ;;         *)             echo "deb-src https://nginx.org/packages/debian/ bullseye nginx" >> /etc/apt/sources.list.d/nginx.list                         && tempDir="$(mktemp -d)"             && chmod 777 "$tempDir"                         && savedAptMark="$(apt-mark showmanual)"                         && apt-get update             && apt-get build-dep -y $nginxPackages             && (                 cd "$tempDir"                 && DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)"                     apt-get source --compile $nginxPackages             )                         && apt-mark showmanual | xargs apt-mark auto > /dev/null             && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }                         && ls -lAFh "$tempDir"             && ( cd "$tempDir" && dpkg-scanpackages . > Packages )             && grep '^Package: ' "$tempDir/Packages"             && echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list             && apt-get -o Acquire::GzipIndexes=false update             ;;     esac         && apt-get install --no-install-recommends --no-install-suggests -y                         $nginxPackages                         gettext-base                         curl     && apt-get remove --purge --auto-remove -y && rm -rf /var/lib/apt/lists/* /etc/apt/sources.list.d/nginx.list         && if [ -n "$tempDir" ]; then         apt-get purge -y --auto-remove         && rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list;     fi     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 01 Mar 2023 04:27:18 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 01 Mar 2023 04:27:18 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 01 Mar 2023 04:27:18 GMT
COPY file:abbcbf84dc17ee4454b6b2e3cf914be88e02cf84d344ec45a5b31235379d722a in /docker-entrypoint.d 
# Wed, 01 Mar 2023 04:27:18 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 01 Mar 2023 04:27:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:27:19 GMT
EXPOSE 80
# Wed, 01 Mar 2023 04:27:19 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 04:27:19 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:7b8d78f42e32e7fa234bcf890ae6603acab2881bca68a9d8c429981c7f42b1d6`  
		Last Modified: Wed, 01 Mar 2023 02:54:48 GMT  
		Size: 29.6 MB (29646854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bff44877966effac8b3d58debc25f8f89691e214bfebfe4515770e92885f8c`  
		Last Modified: Wed, 01 Mar 2023 04:29:40 GMT  
		Size: 36.7 MB (36700301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778b4732072b11c80266e79b3c33a49e8345d9d1f7066dc4a0e3994086553413`  
		Last Modified: Wed, 01 Mar 2023 04:29:35 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78ea3c8f6c9e40cf224cdd5dee54f08e26ea3e78284f76150a8151d155233c9`  
		Last Modified: Wed, 01 Mar 2023 04:29:35 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65916fd6e7199c88e7ea70fdaaacfbee6b8394b1edad165e7baf3dc897fd4671`  
		Last Modified: Wed, 01 Mar 2023 04:29:35 GMT  
		Size: 774.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db848d82547d6629c12673eddea08189215ea91b5027d2421653dde0da6ed97`  
		Last Modified: Wed, 01 Mar 2023 04:29:35 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
