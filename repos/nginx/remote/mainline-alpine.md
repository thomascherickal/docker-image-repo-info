## `nginx:mainline-alpine`

```console
$ docker pull nginx@sha256:a97eb9ecc708c8aa715ccfb5e9338f5456e4b65575daf304f108301f3b497314
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `nginx:mainline-alpine` - linux; amd64

```console
$ docker pull nginx@sha256:4635b632d2aaf8c37c8a1cf76a1f96d11b899f74caa2c6946ea56d0a5af02c0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9609786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f715d38cfe0eb66b672219f3466f471dda7395b7b7e80e79394508d0dccb5ef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 14 Aug 2020 00:37:22 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 14 Aug 2020 00:37:22 GMT
ENV NGINX_VERSION=1.19.2
# Fri, 14 Aug 2020 00:37:22 GMT
ENV NJS_VERSION=0.4.3
# Fri, 14 Aug 2020 00:37:22 GMT
ENV PKG_RELEASE=1
# Fri, 14 Aug 2020 00:37:27 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-r${PKG_RELEASE}     "     && case "$apkArch" in         x86_64)             set -x             && KEY_SHA512="e7fa8303923d9b95db37a77ad46c68fd4755ff935d0a534d26eba83de193c76166c68bfe7f65471bf8881004ef4aa6df3e34689c305662750c0172fca5d8552a *stdin"             && apk add --no-cache --virtual .cert-deps                 openssl             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if [ "$(openssl rsa -pubin -in /tmp/nginx_signing.rsa.pub -text -noout | openssl sha512 -r)" = "$KEY_SHA512" ]; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk del .cert-deps             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre-dev                 zlib-dev                 linux-headers                 libxslt-dev                 gd-dev                 geoip-dev                 perl-dev                 libedit-dev                 mercurial                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && hg clone https://hg.nginx.org/pkg-oss                 && cd pkg-oss                 && hg up ${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make all                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && apk add --no-cache curl ca-certificates     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Fri, 14 Aug 2020 00:37:27 GMT
COPY file:e7e183879c35719c18aa7f733651029fbcc55f5d8c22a877ae199b389425789e in / 
# Fri, 14 Aug 2020 00:37:27 GMT
COPY file:1d0a4127e78a26c11640bbedaeaa28ecafb5c40effef923390c04428192d665a in /docker-entrypoint.d 
# Fri, 14 Aug 2020 00:37:27 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Fri, 14 Aug 2020 00:37:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Aug 2020 00:37:28 GMT
EXPOSE 80
# Fri, 14 Aug 2020 00:37:28 GMT
STOPSIGNAL SIGTERM
# Fri, 14 Aug 2020 00:37:28 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db268b1fe8f743c7430c9fb160d06dfd359f81b2df63f753a6de45c0ef88b7e`  
		Last Modified: Fri, 14 Aug 2020 00:38:47 GMT  
		Size: 6.8 MB (6810082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f682f0660e7a979bdcbfd71e1076e5579e60cf7c744d70ef98fbfc5c9fa8860e`  
		Last Modified: Fri, 14 Aug 2020 00:38:45 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb0e8838bc0b40e740a27488d750217660b860d87187dad2b3bc41b3ff7b3ef`  
		Last Modified: Fri, 14 Aug 2020 00:38:46 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bf1226cc170609d873015a51ec618b5282a156acd8b2442b10f0405d1b14dc`  
		Last Modified: Fri, 14 Aug 2020 00:38:45 GMT  
		Size: 665.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline-alpine` - linux; arm variant v6

```console
$ docker pull nginx@sha256:5995af2a5938bf540d32f21a611a564a46d16f10725e947d8ed845bb43cdad68
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9489628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca8e6d9e71c0699a52ce8d74a2554c5189ba2a33516fb35106a2c6cb8c15820`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 14 Aug 2020 00:51:07 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 14 Aug 2020 00:51:08 GMT
ENV NGINX_VERSION=1.19.2
# Fri, 14 Aug 2020 00:51:09 GMT
ENV NJS_VERSION=0.4.3
# Fri, 14 Aug 2020 00:51:10 GMT
ENV PKG_RELEASE=1
# Fri, 14 Aug 2020 00:54:59 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-r${PKG_RELEASE}     "     && case "$apkArch" in         x86_64)             set -x             && KEY_SHA512="e7fa8303923d9b95db37a77ad46c68fd4755ff935d0a534d26eba83de193c76166c68bfe7f65471bf8881004ef4aa6df3e34689c305662750c0172fca5d8552a *stdin"             && apk add --no-cache --virtual .cert-deps                 openssl             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if [ "$(openssl rsa -pubin -in /tmp/nginx_signing.rsa.pub -text -noout | openssl sha512 -r)" = "$KEY_SHA512" ]; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk del .cert-deps             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre-dev                 zlib-dev                 linux-headers                 libxslt-dev                 gd-dev                 geoip-dev                 perl-dev                 libedit-dev                 mercurial                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && hg clone https://hg.nginx.org/pkg-oss                 && cd pkg-oss                 && hg up ${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make all                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && apk add --no-cache curl ca-certificates     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Fri, 14 Aug 2020 00:55:00 GMT
COPY file:e7e183879c35719c18aa7f733651029fbcc55f5d8c22a877ae199b389425789e in / 
# Fri, 14 Aug 2020 00:55:01 GMT
COPY file:1d0a4127e78a26c11640bbedaeaa28ecafb5c40effef923390c04428192d665a in /docker-entrypoint.d 
# Fri, 14 Aug 2020 00:55:02 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Fri, 14 Aug 2020 00:55:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Aug 2020 00:55:04 GMT
EXPOSE 80
# Fri, 14 Aug 2020 00:55:05 GMT
STOPSIGNAL SIGTERM
# Fri, 14 Aug 2020 00:55:06 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e8d99b3c2493d4197a039cdbc737125ccae9d5324add0b7822e3e86bb1231c`  
		Last Modified: Fri, 14 Aug 2020 01:00:12 GMT  
		Size: 6.9 MB (6884172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53c08009e5356e422ce8f007192f7625314cc12c36ffc865f513a0f2f2f0e69`  
		Last Modified: Fri, 14 Aug 2020 01:00:10 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ccb53075093a9feccefeabd5cc10fcfad896c3e93a380052ca9127cbdaff49`  
		Last Modified: Fri, 14 Aug 2020 01:00:10 GMT  
		Size: 901.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5417798c6a134fefe5d45d452ce8500db43ca685735f7aac5d38f5101a18df4`  
		Last Modified: Fri, 14 Aug 2020 01:00:10 GMT  
		Size: 669.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline-alpine` - linux; arm variant v7

```console
$ docker pull nginx@sha256:b78b19a1af2eaac8185215c08183a8f71f17d028bcb5e03a86be2051dddc6271
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8732215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb9ec6bcda2481a64fa32b961f8a6cfb4e4e2e4b286d4ef8b06c7a0547b9d299`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Fri, 14 Aug 2020 01:12:15 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 14 Aug 2020 01:12:16 GMT
ENV NGINX_VERSION=1.19.2
# Fri, 14 Aug 2020 01:12:16 GMT
ENV NJS_VERSION=0.4.3
# Fri, 14 Aug 2020 01:12:17 GMT
ENV PKG_RELEASE=1
# Fri, 14 Aug 2020 01:15:35 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-r${PKG_RELEASE}     "     && case "$apkArch" in         x86_64)             set -x             && KEY_SHA512="e7fa8303923d9b95db37a77ad46c68fd4755ff935d0a534d26eba83de193c76166c68bfe7f65471bf8881004ef4aa6df3e34689c305662750c0172fca5d8552a *stdin"             && apk add --no-cache --virtual .cert-deps                 openssl             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if [ "$(openssl rsa -pubin -in /tmp/nginx_signing.rsa.pub -text -noout | openssl sha512 -r)" = "$KEY_SHA512" ]; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk del .cert-deps             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre-dev                 zlib-dev                 linux-headers                 libxslt-dev                 gd-dev                 geoip-dev                 perl-dev                 libedit-dev                 mercurial                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && hg clone https://hg.nginx.org/pkg-oss                 && cd pkg-oss                 && hg up ${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make all                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && apk add --no-cache curl ca-certificates     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Fri, 14 Aug 2020 01:15:36 GMT
COPY file:e7e183879c35719c18aa7f733651029fbcc55f5d8c22a877ae199b389425789e in / 
# Fri, 14 Aug 2020 01:15:36 GMT
COPY file:1d0a4127e78a26c11640bbedaeaa28ecafb5c40effef923390c04428192d665a in /docker-entrypoint.d 
# Fri, 14 Aug 2020 01:15:37 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Fri, 14 Aug 2020 01:15:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Aug 2020 01:15:39 GMT
EXPOSE 80
# Fri, 14 Aug 2020 01:15:39 GMT
STOPSIGNAL SIGTERM
# Fri, 14 Aug 2020 01:15:40 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1db2de826a699777802decb44e122da9cad052f158fb896e75c929b20960785`  
		Last Modified: Fri, 14 Aug 2020 01:20:42 GMT  
		Size: 6.3 MB (6323286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637301d0198dd8b1a4b52ca36eae3544cb91dc6be5fe35c1aca282c350e486bd`  
		Last Modified: Fri, 14 Aug 2020 01:20:40 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e062a33c3800f0eb61891c89894907c7e44567fe342546838532c3690d1e0104`  
		Last Modified: Fri, 14 Aug 2020 01:20:40 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e76287358eb40d1e8724b6a377fb6bd6d7842816b4927f08bfa83b1e50535c7`  
		Last Modified: Fri, 14 Aug 2020 01:20:40 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline-alpine` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:8d99a3e08d0f07ca0fdf1db5c56b1f30d9cc97af5458ecfac604b8887cba289a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9857297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068614b905e936c8385dfe78226faa7329858b327edb0236eadd1f1c7d0903f8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 14 Aug 2020 00:59:11 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 14 Aug 2020 00:59:12 GMT
ENV NGINX_VERSION=1.19.2
# Fri, 14 Aug 2020 00:59:13 GMT
ENV NJS_VERSION=0.4.3
# Fri, 14 Aug 2020 00:59:15 GMT
ENV PKG_RELEASE=1
# Fri, 14 Aug 2020 01:02:57 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-r${PKG_RELEASE}     "     && case "$apkArch" in         x86_64)             set -x             && KEY_SHA512="e7fa8303923d9b95db37a77ad46c68fd4755ff935d0a534d26eba83de193c76166c68bfe7f65471bf8881004ef4aa6df3e34689c305662750c0172fca5d8552a *stdin"             && apk add --no-cache --virtual .cert-deps                 openssl             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if [ "$(openssl rsa -pubin -in /tmp/nginx_signing.rsa.pub -text -noout | openssl sha512 -r)" = "$KEY_SHA512" ]; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk del .cert-deps             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre-dev                 zlib-dev                 linux-headers                 libxslt-dev                 gd-dev                 geoip-dev                 perl-dev                 libedit-dev                 mercurial                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && hg clone https://hg.nginx.org/pkg-oss                 && cd pkg-oss                 && hg up ${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make all                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && apk add --no-cache curl ca-certificates     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Fri, 14 Aug 2020 01:02:58 GMT
COPY file:e7e183879c35719c18aa7f733651029fbcc55f5d8c22a877ae199b389425789e in / 
# Fri, 14 Aug 2020 01:02:59 GMT
COPY file:1d0a4127e78a26c11640bbedaeaa28ecafb5c40effef923390c04428192d665a in /docker-entrypoint.d 
# Fri, 14 Aug 2020 01:03:00 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Fri, 14 Aug 2020 01:03:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Aug 2020 01:03:01 GMT
EXPOSE 80
# Fri, 14 Aug 2020 01:03:02 GMT
STOPSIGNAL SIGTERM
# Fri, 14 Aug 2020 01:03:03 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66942047c7b3b1e4cfa170855e791fffb10e70e4061f5d20cdf3d712b1d9ba79`  
		Last Modified: Fri, 14 Aug 2020 01:08:39 GMT  
		Size: 7.1 MB (7147164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03513b8933dacfb95cb1d00fc4846b0c28686aba484b00ef5409ae368e83c922`  
		Last Modified: Fri, 14 Aug 2020 01:08:39 GMT  
		Size: 602.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81823b5c9b536108c620f3c7b371517e997a25caa8495ef8cb040a17a1eb8be`  
		Last Modified: Fri, 14 Aug 2020 01:08:38 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ade662cda571f878ef3c7f9a69bb8649b60974fa25680948cad5ab16cac36b`  
		Last Modified: Fri, 14 Aug 2020 01:08:38 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline-alpine` - linux; 386

```console
$ docker pull nginx@sha256:3d4c3485cf8af9c0e38718409918ed6255caa32d6867cf667a7339b0c5a5641e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10428409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aa40102050829f287e665efff7b43cbee41db765121ba63ccd762b1575a49ef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 14 Aug 2020 00:39:47 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 14 Aug 2020 00:39:47 GMT
ENV NGINX_VERSION=1.19.2
# Fri, 14 Aug 2020 00:39:47 GMT
ENV NJS_VERSION=0.4.3
# Fri, 14 Aug 2020 00:39:47 GMT
ENV PKG_RELEASE=1
# Fri, 14 Aug 2020 00:42:53 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-r${PKG_RELEASE}     "     && case "$apkArch" in         x86_64)             set -x             && KEY_SHA512="e7fa8303923d9b95db37a77ad46c68fd4755ff935d0a534d26eba83de193c76166c68bfe7f65471bf8881004ef4aa6df3e34689c305662750c0172fca5d8552a *stdin"             && apk add --no-cache --virtual .cert-deps                 openssl             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if [ "$(openssl rsa -pubin -in /tmp/nginx_signing.rsa.pub -text -noout | openssl sha512 -r)" = "$KEY_SHA512" ]; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk del .cert-deps             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre-dev                 zlib-dev                 linux-headers                 libxslt-dev                 gd-dev                 geoip-dev                 perl-dev                 libedit-dev                 mercurial                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && hg clone https://hg.nginx.org/pkg-oss                 && cd pkg-oss                 && hg up ${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make all                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && apk add --no-cache curl ca-certificates     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Fri, 14 Aug 2020 00:42:54 GMT
COPY file:e7e183879c35719c18aa7f733651029fbcc55f5d8c22a877ae199b389425789e in / 
# Fri, 14 Aug 2020 00:42:54 GMT
COPY file:1d0a4127e78a26c11640bbedaeaa28ecafb5c40effef923390c04428192d665a in /docker-entrypoint.d 
# Fri, 14 Aug 2020 00:42:54 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Fri, 14 Aug 2020 00:42:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Aug 2020 00:42:54 GMT
EXPOSE 80
# Fri, 14 Aug 2020 00:42:55 GMT
STOPSIGNAL SIGTERM
# Fri, 14 Aug 2020 00:42:55 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43a9c2ec9efc8299f946b9ffd592f00320591f6c0572ed8fe809654b18c6bef`  
		Last Modified: Fri, 14 Aug 2020 00:47:19 GMT  
		Size: 7.6 MB (7633943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aac9309b1dd9a008fbb05ca3bf678d3aa040d38bdedecff9be9a40c178d8540`  
		Last Modified: Fri, 14 Aug 2020 00:47:17 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b43a30e9e524c7f0765279dfb92b68fd6d9b013a542f91c119567c6334247b`  
		Last Modified: Fri, 14 Aug 2020 00:47:17 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70dfd730b7de6600a5cc681528e98ce08f9f3016353c8b154695b12f299f1218`  
		Last Modified: Fri, 14 Aug 2020 00:47:17 GMT  
		Size: 668.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline-alpine` - linux; ppc64le

```console
$ docker pull nginx@sha256:10bdb5cdba74478710feeb55a38b74fd57b5ea3f69072e1f8250af6c40b0fcb8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10231624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2faa4d94b239dc8a6d0a03a0df60c492eb5cf2a8efd9592dbdd773c997c4f71f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Fri, 14 Aug 2020 00:50:35 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 14 Aug 2020 00:50:42 GMT
ENV NGINX_VERSION=1.19.2
# Fri, 14 Aug 2020 00:50:52 GMT
ENV NJS_VERSION=0.4.3
# Fri, 14 Aug 2020 00:50:55 GMT
ENV PKG_RELEASE=1
# Fri, 14 Aug 2020 00:55:33 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-r${PKG_RELEASE}     "     && case "$apkArch" in         x86_64)             set -x             && KEY_SHA512="e7fa8303923d9b95db37a77ad46c68fd4755ff935d0a534d26eba83de193c76166c68bfe7f65471bf8881004ef4aa6df3e34689c305662750c0172fca5d8552a *stdin"             && apk add --no-cache --virtual .cert-deps                 openssl             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if [ "$(openssl rsa -pubin -in /tmp/nginx_signing.rsa.pub -text -noout | openssl sha512 -r)" = "$KEY_SHA512" ]; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk del .cert-deps             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre-dev                 zlib-dev                 linux-headers                 libxslt-dev                 gd-dev                 geoip-dev                 perl-dev                 libedit-dev                 mercurial                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && hg clone https://hg.nginx.org/pkg-oss                 && cd pkg-oss                 && hg up ${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make all                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && apk add --no-cache curl ca-certificates     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Fri, 14 Aug 2020 00:55:37 GMT
COPY file:e7e183879c35719c18aa7f733651029fbcc55f5d8c22a877ae199b389425789e in / 
# Fri, 14 Aug 2020 00:55:39 GMT
COPY file:1d0a4127e78a26c11640bbedaeaa28ecafb5c40effef923390c04428192d665a in /docker-entrypoint.d 
# Fri, 14 Aug 2020 00:55:42 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Fri, 14 Aug 2020 00:55:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Aug 2020 00:55:54 GMT
EXPOSE 80
# Fri, 14 Aug 2020 00:56:02 GMT
STOPSIGNAL SIGTERM
# Fri, 14 Aug 2020 00:56:16 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f956f8ab07af20453f09944555026f4b7a9982dcb6cb4d90135c0a73fd16ee`  
		Last Modified: Fri, 14 Aug 2020 01:02:20 GMT  
		Size: 7.4 MB (7424255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c1fc6c05cab5a8fbba89116fbe22b24ed3e89f4862eef43c611ac5d4297a87`  
		Last Modified: Fri, 14 Aug 2020 01:02:18 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d512d517cfc150833ff4a72f6a2b1c971dd92fc9d2bdfcb8ff2b54fe731a8aa`  
		Last Modified: Fri, 14 Aug 2020 01:02:18 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b831a5d94aa19e3d5d5048eeeb69992402effd2e5557404ae596c9ebaf504919`  
		Last Modified: Fri, 14 Aug 2020 01:02:18 GMT  
		Size: 670.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:mainline-alpine` - linux; s390x

```console
$ docker pull nginx@sha256:2a873cb3287184911dd525ef2abbc1e69df5f24902d653e3c0c28849f8020cc7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9713935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40fa7afd2c5aa5cec14db6359411afe456b632b6868c1dc7d50a82341ceeef34`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Fri, 14 Aug 2020 00:46:44 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Fri, 14 Aug 2020 00:46:44 GMT
ENV NGINX_VERSION=1.19.2
# Fri, 14 Aug 2020 00:46:44 GMT
ENV NJS_VERSION=0.4.3
# Fri, 14 Aug 2020 00:46:44 GMT
ENV PKG_RELEASE=1
# Fri, 14 Aug 2020 00:48:17 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-xslt=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-geoip=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-image-filter=${NGINX_VERSION}-r${PKG_RELEASE}         nginx-module-njs=${NGINX_VERSION}.${NJS_VERSION}-r${PKG_RELEASE}     "     && case "$apkArch" in         x86_64)             set -x             && KEY_SHA512="e7fa8303923d9b95db37a77ad46c68fd4755ff935d0a534d26eba83de193c76166c68bfe7f65471bf8881004ef4aa6df3e34689c305662750c0172fca5d8552a *stdin"             && apk add --no-cache --virtual .cert-deps                 openssl             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if [ "$(openssl rsa -pubin -in /tmp/nginx_signing.rsa.pub -text -noout | openssl sha512 -r)" = "$KEY_SHA512" ]; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk del .cert-deps             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre-dev                 zlib-dev                 linux-headers                 libxslt-dev                 gd-dev                 geoip-dev                 perl-dev                 libedit-dev                 mercurial                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && hg clone https://hg.nginx.org/pkg-oss                 && cd pkg-oss                 && hg up ${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make all                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && apk add --no-cache curl ca-certificates     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Fri, 14 Aug 2020 00:48:17 GMT
COPY file:e7e183879c35719c18aa7f733651029fbcc55f5d8c22a877ae199b389425789e in / 
# Fri, 14 Aug 2020 00:48:17 GMT
COPY file:1d0a4127e78a26c11640bbedaeaa28ecafb5c40effef923390c04428192d665a in /docker-entrypoint.d 
# Fri, 14 Aug 2020 00:48:18 GMT
COPY file:0fd5fca330dcd6a7de297435e32af634f29f7132ed0550d342cad9fd20158258 in /docker-entrypoint.d 
# Fri, 14 Aug 2020 00:48:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 14 Aug 2020 00:48:18 GMT
EXPOSE 80
# Fri, 14 Aug 2020 00:48:18 GMT
STOPSIGNAL SIGTERM
# Fri, 14 Aug 2020 00:48:18 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bdfd6cdb9bc4e15cdad688b6fcdadef514977f68933372e1534961a057d831c`  
		Last Modified: Fri, 14 Aug 2020 00:51:15 GMT  
		Size: 7.1 MB (7145579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278ec6f8ab4e79388325a0e42a03528a62348908932a569c7ad0f01529b4af8a`  
		Last Modified: Fri, 14 Aug 2020 00:51:15 GMT  
		Size: 600.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbafec86d54db7f5ee2cecdc4f2b269706a79af0dc8fda7d6f0d057081f2634`  
		Last Modified: Fri, 14 Aug 2020 00:51:14 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c210841728949bec746f1b87c9f3a0b559f1cea5f25b8d6f48c0109263831b4`  
		Last Modified: Fri, 14 Aug 2020 00:51:14 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
