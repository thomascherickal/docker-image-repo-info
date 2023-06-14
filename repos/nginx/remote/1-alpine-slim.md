## `nginx:1-alpine-slim`

```console
$ docker pull nginx@sha256:43b29fbd7559c586fc868f10aeb02c1930e9bceca79aaeb08f73d7b60d048137
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `nginx:1-alpine-slim` - linux; amd64

```console
$ docker pull nginx@sha256:01364a4c474a270ea5d056f62c01c1c31e6cb368f698b9fb6c662d2c3fb674c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7352078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dafe3ae8e82441c07e86d877bc8b943b804ce5edcf4c06d043336d5db21c2f8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:31:10 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 14 Jun 2023 07:16:53 GMT
ENV NGINX_VERSION=1.25.1
# Wed, 14 Jun 2023 07:16:54 GMT
ENV PKG_RELEASE=1
# Wed, 14 Jun 2023 07:16:59 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}     "     && apk add --no-cache --virtual .checksum-deps         openssl     && case "$apkArch" in         x86_64|aarch64)             set -x             && KEY_SHA512="e09fa32f0a0eab2b879ccbbc4d0e4fb9751486eedda75e35fac65802cc9faa266425edf83e261137a2f4d16281ce2c1a5f4502930fe75154723da014214f0655"             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if echo "$KEY_SHA512 */tmp/nginx_signing.rsa.pub" | sha512sum -c -; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre2-dev                 zlib-dev                 linux-headers                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && curl -f -O https://hg.nginx.org/pkg-oss/archive/${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && PKGOSSCHECKSUM=\"dd08a5c2b441817d58ffc91ade0d927a21bc9854c768391e92a005997a2961bcda64ca6a5cfce98d5394ac2787c8f4839b150f206835a8a7db944625651f9fd8 *${NGINX_VERSION}-${PKG_RELEASE}.tar.gz\"                 && if [ \"\$(openssl sha512 -r ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz)\" = \"\$PKGOSSCHECKSUM\" ]; then                     echo \"pkg-oss tarball checksum verification succeeded!\";                 else                     echo \"pkg-oss tarball checksum verification failed!\";                     exit 1;                 fi                 && tar xzvf ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && cd pkg-oss-${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make base                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del --no-network .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && apk del --no-network .checksum-deps     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del --no-network .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 14 Jun 2023 07:16:59 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 14 Jun 2023 07:16:59 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 14 Jun 2023 07:17:00 GMT
COPY file:d4375883ed5db364232ccf781e8ad28514cd005edb385d43dbfb984f2c63edb9 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 07:17:00 GMT
COPY file:36429cfeeb299f9913b84ea136b004be12fbe4bb4f975a977a3608044e8bfa91 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 07:17:00 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 14 Jun 2023 07:17:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jun 2023 07:17:00 GMT
EXPOSE 80
# Wed, 14 Jun 2023 07:17:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 07:17:00 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d172045870582ea218237514cac9fac7bc0523eac097802e8b40ed8aac184d`  
		Last Modified: Wed, 14 Jun 2023 07:19:03 GMT  
		Size: 4.0 MB (3972952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2fb18bfd235c475c8bf1d27c7a7fe6489edfbcbb2318fec747e37f6609f8ac`  
		Last Modified: Wed, 14 Jun 2023 07:19:01 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa560e1d2511c3554c07737085c62a94479d1263a54d97b1c2af377597ba381e`  
		Last Modified: Wed, 14 Jun 2023 07:19:01 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc4eddbd7a2ebce356e60e2a81d30230e8d4e426187415a625df81b978f7b07`  
		Last Modified: Wed, 14 Jun 2023 07:19:01 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bdf9d00df94d897f3b6a1ce2ae3ff74a1e2377e3165f0e2fd50ed5902b12b76`  
		Last Modified: Wed, 14 Jun 2023 07:19:01 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3357c574c133587e647a296588ea850a6599a73f8c9ac3d9b84ef1966e5e5cc7`  
		Last Modified: Wed, 14 Jun 2023 07:19:01 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:1-alpine-slim` - linux; arm variant v6

```console
$ docker pull nginx@sha256:65081f236f009405c9d001363eeb420376c64e86e1a075a859690892052fcb0e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5145420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:051d22efa4ff3734168552a1d9fde38968bdf4b0adfdc7da182204f664cef2e4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:47:55 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 14 Jun 2023 20:47:56 GMT
ENV NGINX_VERSION=1.25.1
# Wed, 14 Jun 2023 20:47:56 GMT
ENV PKG_RELEASE=1
# Wed, 14 Jun 2023 20:48:48 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}     "     && apk add --no-cache --virtual .checksum-deps         openssl     && case "$apkArch" in         x86_64|aarch64)             set -x             && KEY_SHA512="e09fa32f0a0eab2b879ccbbc4d0e4fb9751486eedda75e35fac65802cc9faa266425edf83e261137a2f4d16281ce2c1a5f4502930fe75154723da014214f0655"             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if echo "$KEY_SHA512 */tmp/nginx_signing.rsa.pub" | sha512sum -c -; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre2-dev                 zlib-dev                 linux-headers                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && curl -f -O https://hg.nginx.org/pkg-oss/archive/${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && PKGOSSCHECKSUM=\"dd08a5c2b441817d58ffc91ade0d927a21bc9854c768391e92a005997a2961bcda64ca6a5cfce98d5394ac2787c8f4839b150f206835a8a7db944625651f9fd8 *${NGINX_VERSION}-${PKG_RELEASE}.tar.gz\"                 && if [ \"\$(openssl sha512 -r ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz)\" = \"\$PKGOSSCHECKSUM\" ]; then                     echo \"pkg-oss tarball checksum verification succeeded!\";                 else                     echo \"pkg-oss tarball checksum verification failed!\";                     exit 1;                 fi                 && tar xzvf ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && cd pkg-oss-${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make base                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del --no-network .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && apk del --no-network .checksum-deps     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del --no-network .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 14 Jun 2023 20:48:48 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 14 Jun 2023 20:48:48 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 14 Jun 2023 20:48:48 GMT
COPY file:d4375883ed5db364232ccf781e8ad28514cd005edb385d43dbfb984f2c63edb9 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 20:48:48 GMT
COPY file:36429cfeeb299f9913b84ea136b004be12fbe4bb4f975a977a3608044e8bfa91 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 20:48:48 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 14 Jun 2023 20:48:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:48:49 GMT
EXPOSE 80
# Wed, 14 Jun 2023 20:48:49 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 20:48:49 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0ce43a953a56062aa8de55f0fc61fa39d3036db2adae6e4b023fc770987830`  
		Last Modified: Wed, 14 Jun 2023 20:56:05 GMT  
		Size: 2.0 MB (2029942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9844c3d3bcdf975f2439c19dc11ece7aec826793aaf413d2c8fd867d11efce`  
		Last Modified: Wed, 14 Jun 2023 20:56:02 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a6977b82ef8c36514ff534b741e16a7c6a0d0bf3dfa4fd32dcebf6ef549dc0`  
		Last Modified: Wed, 14 Jun 2023 20:56:02 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae3f0668fa56317fce563b068ee3bb32574064ba89f0b6aebd87511e77e1f3d`  
		Last Modified: Wed, 14 Jun 2023 20:56:02 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f60d9ab335b4ad38964c51276bcaba5e7666522bfb740ca740ec8f32195ba1`  
		Last Modified: Wed, 14 Jun 2023 20:56:02 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3408fcb6e08000798e05d70c4f16bf7f18181ffdbec94b9d333ab695409d3b`  
		Last Modified: Wed, 14 Jun 2023 20:56:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:1-alpine-slim` - linux; arm variant v7

```console
$ docker pull nginx@sha256:59501480c67ff3a490658d2f7a5afed9e7bcfaea3fa9b29ffed01f01598822d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6712321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43a470b88b10dd1d0f1df9aab8761e6014f277f6fa2df7e7ff1f1a6a6c33c851`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:27:03 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 14 Jun 2023 04:58:41 GMT
ENV NGINX_VERSION=1.25.1
# Wed, 14 Jun 2023 04:58:41 GMT
ENV PKG_RELEASE=1
# Wed, 14 Jun 2023 04:59:31 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}     "     && apk add --no-cache --virtual .checksum-deps         openssl     && case "$apkArch" in         x86_64|aarch64)             set -x             && KEY_SHA512="e09fa32f0a0eab2b879ccbbc4d0e4fb9751486eedda75e35fac65802cc9faa266425edf83e261137a2f4d16281ce2c1a5f4502930fe75154723da014214f0655"             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if echo "$KEY_SHA512 */tmp/nginx_signing.rsa.pub" | sha512sum -c -; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre2-dev                 zlib-dev                 linux-headers                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && curl -f -O https://hg.nginx.org/pkg-oss/archive/${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && PKGOSSCHECKSUM=\"dd08a5c2b441817d58ffc91ade0d927a21bc9854c768391e92a005997a2961bcda64ca6a5cfce98d5394ac2787c8f4839b150f206835a8a7db944625651f9fd8 *${NGINX_VERSION}-${PKG_RELEASE}.tar.gz\"                 && if [ \"\$(openssl sha512 -r ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz)\" = \"\$PKGOSSCHECKSUM\" ]; then                     echo \"pkg-oss tarball checksum verification succeeded!\";                 else                     echo \"pkg-oss tarball checksum verification failed!\";                     exit 1;                 fi                 && tar xzvf ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && cd pkg-oss-${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make base                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del --no-network .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && apk del --no-network .checksum-deps     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del --no-network .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 14 Jun 2023 04:59:31 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 14 Jun 2023 04:59:32 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 14 Jun 2023 04:59:32 GMT
COPY file:d4375883ed5db364232ccf781e8ad28514cd005edb385d43dbfb984f2c63edb9 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 04:59:32 GMT
COPY file:36429cfeeb299f9913b84ea136b004be12fbe4bb4f975a977a3608044e8bfa91 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 04:59:32 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 14 Jun 2023 04:59:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jun 2023 04:59:32 GMT
EXPOSE 80
# Wed, 14 Jun 2023 04:59:32 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 04:59:32 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f5dba7f85f6a949952c7ce25318a3d4526bef6cf58dd74854217a79608cf21`  
		Last Modified: Wed, 14 Jun 2023 05:03:43 GMT  
		Size: 3.8 MB (3839242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6db4f5a10608bdf2bc46259918f153cf2df6f1f241099c6207bdd60e2013976`  
		Last Modified: Wed, 14 Jun 2023 05:03:41 GMT  
		Size: 623.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d0620c5419db4bb77ad2b44a867c10d35dfd56fcff351501cbd08f7c86d801`  
		Last Modified: Wed, 14 Jun 2023 05:03:41 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae35608353551cf824666f5899c07f2634e8e932e1856b16810f4ceb0ca3cdfa`  
		Last Modified: Wed, 14 Jun 2023 05:03:41 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172cb6aca0d945449681bb45da5626d3902113df8e337460deceb8bc88f9004b`  
		Last Modified: Wed, 14 Jun 2023 05:03:41 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef56c562326beb97cdad56d1d6c982454079a148406072e87081add26aa4350`  
		Last Modified: Wed, 14 Jun 2023 05:03:41 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:1-alpine-slim` - linux; arm64 variant v8

```console
$ docker pull nginx@sha256:8b282fd2e709d974b0e88d09ba17e90fc18f0f05f79e162dc76d140f6eb1fb8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7088492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c13acbf9f09ae59393571533f76730bb2412dd153d861dda28be5de65a9b110e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:22:48 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 14 Jun 2023 03:47:18 GMT
ENV NGINX_VERSION=1.25.1
# Wed, 14 Jun 2023 03:47:19 GMT
ENV PKG_RELEASE=1
# Wed, 14 Jun 2023 03:47:24 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}     "     && apk add --no-cache --virtual .checksum-deps         openssl     && case "$apkArch" in         x86_64|aarch64)             set -x             && KEY_SHA512="e09fa32f0a0eab2b879ccbbc4d0e4fb9751486eedda75e35fac65802cc9faa266425edf83e261137a2f4d16281ce2c1a5f4502930fe75154723da014214f0655"             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if echo "$KEY_SHA512 */tmp/nginx_signing.rsa.pub" | sha512sum -c -; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre2-dev                 zlib-dev                 linux-headers                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && curl -f -O https://hg.nginx.org/pkg-oss/archive/${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && PKGOSSCHECKSUM=\"dd08a5c2b441817d58ffc91ade0d927a21bc9854c768391e92a005997a2961bcda64ca6a5cfce98d5394ac2787c8f4839b150f206835a8a7db944625651f9fd8 *${NGINX_VERSION}-${PKG_RELEASE}.tar.gz\"                 && if [ \"\$(openssl sha512 -r ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz)\" = \"\$PKGOSSCHECKSUM\" ]; then                     echo \"pkg-oss tarball checksum verification succeeded!\";                 else                     echo \"pkg-oss tarball checksum verification failed!\";                     exit 1;                 fi                 && tar xzvf ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && cd pkg-oss-${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make base                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del --no-network .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && apk del --no-network .checksum-deps     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del --no-network .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 14 Jun 2023 03:47:24 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 14 Jun 2023 03:47:24 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 14 Jun 2023 03:47:24 GMT
COPY file:d4375883ed5db364232ccf781e8ad28514cd005edb385d43dbfb984f2c63edb9 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 03:47:24 GMT
COPY file:36429cfeeb299f9913b84ea136b004be12fbe4bb4f975a977a3608044e8bfa91 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 03:47:24 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 14 Jun 2023 03:47:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jun 2023 03:47:24 GMT
EXPOSE 80
# Wed, 14 Jun 2023 03:47:24 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 03:47:24 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b9c44cdc0a12e695c8a26ffc475cc7bbd28e816828be3ad77717cb535fccb7`  
		Last Modified: Wed, 14 Jun 2023 03:49:30 GMT  
		Size: 3.8 MB (3822077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6952a44de3c32a4d7421c718994b1fec77999d293ac7190b675a1e9ca2e9a217`  
		Last Modified: Wed, 14 Jun 2023 03:49:28 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d017e32abe9e0794f81740ffe32a9838025e4ccfa1752a8081d7f46c39e837b`  
		Last Modified: Wed, 14 Jun 2023 03:49:28 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37a35334b82568c07e87acb21e654b41790dafc7d6c8b993773a9da06cded68`  
		Last Modified: Wed, 14 Jun 2023 03:49:28 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f7949fe8ad559a1172c78fa311f6ae36c55c195266e98627f8aeb5750bb8c8`  
		Last Modified: Wed, 14 Jun 2023 03:49:28 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4443db816c08ce19446e61e51c961c3b1948011456d1f85d1548b6f96c4cb5ee`  
		Last Modified: Wed, 14 Jun 2023 03:49:28 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:1-alpine-slim` - linux; 386

```console
$ docker pull nginx@sha256:422903ce4b6b08cede2c6da0982f974c8d2e646384c27de6effe76722bf9bc4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8078411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f25853bd947f2588e99f4d3033736f3023d50da02dee1db5fecb3a69d8074298`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:49:29 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 14 Jun 2023 05:26:13 GMT
ENV NGINX_VERSION=1.25.1
# Wed, 14 Jun 2023 05:26:14 GMT
ENV PKG_RELEASE=1
# Wed, 14 Jun 2023 05:28:00 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}     "     && apk add --no-cache --virtual .checksum-deps         openssl     && case "$apkArch" in         x86_64|aarch64)             set -x             && KEY_SHA512="e09fa32f0a0eab2b879ccbbc4d0e4fb9751486eedda75e35fac65802cc9faa266425edf83e261137a2f4d16281ce2c1a5f4502930fe75154723da014214f0655"             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if echo "$KEY_SHA512 */tmp/nginx_signing.rsa.pub" | sha512sum -c -; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre2-dev                 zlib-dev                 linux-headers                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && curl -f -O https://hg.nginx.org/pkg-oss/archive/${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && PKGOSSCHECKSUM=\"dd08a5c2b441817d58ffc91ade0d927a21bc9854c768391e92a005997a2961bcda64ca6a5cfce98d5394ac2787c8f4839b150f206835a8a7db944625651f9fd8 *${NGINX_VERSION}-${PKG_RELEASE}.tar.gz\"                 && if [ \"\$(openssl sha512 -r ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz)\" = \"\$PKGOSSCHECKSUM\" ]; then                     echo \"pkg-oss tarball checksum verification succeeded!\";                 else                     echo \"pkg-oss tarball checksum verification failed!\";                     exit 1;                 fi                 && tar xzvf ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && cd pkg-oss-${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make base                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del --no-network .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && apk del --no-network .checksum-deps     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del --no-network .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 14 Jun 2023 05:28:00 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 14 Jun 2023 05:28:00 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 14 Jun 2023 05:28:00 GMT
COPY file:d4375883ed5db364232ccf781e8ad28514cd005edb385d43dbfb984f2c63edb9 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 05:28:00 GMT
COPY file:36429cfeeb299f9913b84ea136b004be12fbe4bb4f975a977a3608044e8bfa91 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 05:28:00 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 14 Jun 2023 05:28:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jun 2023 05:28:00 GMT
EXPOSE 80
# Wed, 14 Jun 2023 05:28:01 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 05:28:01 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219b8fd2a711fe06df66137280bb4b80501c223a755d7bac78270a75bdbdb7a3`  
		Last Modified: Wed, 14 Jun 2023 05:33:08 GMT  
		Size: 4.7 MB (4661584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f831b778685362a2da144c689e9b37241685dcba21ea8ba997f05d13533fd96`  
		Last Modified: Wed, 14 Jun 2023 05:33:05 GMT  
		Size: 627.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f10ea075525419534a15efc44ece8cb3cf26abf95a5371fc6a02298fb3123d`  
		Last Modified: Wed, 14 Jun 2023 05:33:05 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1cff90566f4a6f79582b98b002827f5f98f899f3594f8c2a82b97a2b65a741`  
		Last Modified: Wed, 14 Jun 2023 05:33:05 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21efd98f342ce62b8e61195d8a5bb3f2ed449bf6f15e00b8d1ecf0b161590982`  
		Last Modified: Wed, 14 Jun 2023 05:33:06 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b96d4202d2ad1a830e378bffe053afcea2e79036a78349322c13e68a636ecb`  
		Last Modified: Wed, 14 Jun 2023 05:33:05 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:1-alpine-slim` - linux; ppc64le

```console
$ docker pull nginx@sha256:9dc6850124f3bd4ced5e56ee78dd9d10883853e2324df3dae3e626e5051d5d37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7925947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d068d1a467cce462af588ca540981b59096f44afc29ed7c794fbb34fdee7e368`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:46:48 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 14 Jun 2023 04:12:19 GMT
ENV NGINX_VERSION=1.25.1
# Wed, 14 Jun 2023 04:12:22 GMT
ENV PKG_RELEASE=1
# Wed, 14 Jun 2023 04:13:29 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}     "     && apk add --no-cache --virtual .checksum-deps         openssl     && case "$apkArch" in         x86_64|aarch64)             set -x             && KEY_SHA512="e09fa32f0a0eab2b879ccbbc4d0e4fb9751486eedda75e35fac65802cc9faa266425edf83e261137a2f4d16281ce2c1a5f4502930fe75154723da014214f0655"             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if echo "$KEY_SHA512 */tmp/nginx_signing.rsa.pub" | sha512sum -c -; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre2-dev                 zlib-dev                 linux-headers                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && curl -f -O https://hg.nginx.org/pkg-oss/archive/${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && PKGOSSCHECKSUM=\"dd08a5c2b441817d58ffc91ade0d927a21bc9854c768391e92a005997a2961bcda64ca6a5cfce98d5394ac2787c8f4839b150f206835a8a7db944625651f9fd8 *${NGINX_VERSION}-${PKG_RELEASE}.tar.gz\"                 && if [ \"\$(openssl sha512 -r ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz)\" = \"\$PKGOSSCHECKSUM\" ]; then                     echo \"pkg-oss tarball checksum verification succeeded!\";                 else                     echo \"pkg-oss tarball checksum verification failed!\";                     exit 1;                 fi                 && tar xzvf ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && cd pkg-oss-${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make base                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del --no-network .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && apk del --no-network .checksum-deps     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del --no-network .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 14 Jun 2023 04:13:30 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 14 Jun 2023 04:13:30 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 14 Jun 2023 04:13:30 GMT
COPY file:d4375883ed5db364232ccf781e8ad28514cd005edb385d43dbfb984f2c63edb9 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 04:13:31 GMT
COPY file:36429cfeeb299f9913b84ea136b004be12fbe4bb4f975a977a3608044e8bfa91 in /docker-entrypoint.d 
# Wed, 14 Jun 2023 04:13:31 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 14 Jun 2023 04:13:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jun 2023 04:13:31 GMT
EXPOSE 80
# Wed, 14 Jun 2023 04:13:32 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Jun 2023 04:13:32 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a2603b408047f5feccbb065e290e9fbc1c8a257da77e95a6237f652c7dc4e1`  
		Last Modified: Wed, 14 Jun 2023 04:20:18 GMT  
		Size: 4.5 MB (4530446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68353f0ed627541ca7d176121f7dc07a373ce35476de71f0a6ea00ad7b466d68`  
		Last Modified: Wed, 14 Jun 2023 04:20:15 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b799a759fcdf2e961f5a387025ba3e502a1352ee69492666d7f53a0e464249`  
		Last Modified: Wed, 14 Jun 2023 04:20:15 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae174967310e30deb20c156d0d866747286a85a7b38625cb05507b001925d72`  
		Last Modified: Wed, 14 Jun 2023 04:20:15 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ab44e91b86ee180f4799a885d4d6ad65746c73230a2ad084689ca177c26977`  
		Last Modified: Wed, 14 Jun 2023 04:20:15 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45e6427104c93d7bb70fcf53f0caade098988e0ea51029d6e5113ce166cee0e`  
		Last Modified: Wed, 14 Jun 2023 04:20:15 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nginx:1-alpine-slim` - linux; s390x

```console
$ docker pull nginx@sha256:6f7e16da84a4fa26308c31c0ff3dad25a50f7b2f79d0dda1cfd6bd260f035797
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7346161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9cc01625d32e5a87219abd3e0c423ba8050db37170ba056c96d4967ffd04936`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["nginx","-g","daemon off;"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 03 May 2023 23:18:27 GMT
LABEL maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>
# Wed, 24 May 2023 21:46:19 GMT
ENV NGINX_VERSION=1.25.0
# Wed, 24 May 2023 21:46:19 GMT
ENV PKG_RELEASE=1
# Wed, 24 May 2023 21:47:16 GMT
RUN set -x     && addgroup -g 101 -S nginx     && adduser -S -D -H -u 101 -h /var/cache/nginx -s /sbin/nologin -G nginx -g nginx nginx     && apkArch="$(cat /etc/apk/arch)"     && nginxPackages="         nginx=${NGINX_VERSION}-r${PKG_RELEASE}     "     && apk add --no-cache --virtual .checksum-deps         openssl     && case "$apkArch" in         x86_64|aarch64)             set -x             && KEY_SHA512="e09fa32f0a0eab2b879ccbbc4d0e4fb9751486eedda75e35fac65802cc9faa266425edf83e261137a2f4d16281ce2c1a5f4502930fe75154723da014214f0655"             && wget -O /tmp/nginx_signing.rsa.pub https://nginx.org/keys/nginx_signing.rsa.pub             && if echo "$KEY_SHA512 */tmp/nginx_signing.rsa.pub" | sha512sum -c -; then                 echo "key verification succeeded!";                 mv /tmp/nginx_signing.rsa.pub /etc/apk/keys/;             else                 echo "key verification failed!";                 exit 1;             fi             && apk add -X "https://nginx.org/packages/mainline/alpine/v$(egrep -o '^[0-9]+\.[0-9]+' /etc/alpine-release)/main" --no-cache $nginxPackages             ;;         *)             set -x             && tempDir="$(mktemp -d)"             && chown nobody:nobody $tempDir             && apk add --no-cache --virtual .build-deps                 gcc                 libc-dev                 make                 openssl-dev                 pcre2-dev                 zlib-dev                 linux-headers                 bash                 alpine-sdk                 findutils             && su nobody -s /bin/sh -c "                 export HOME=${tempDir}                 && cd ${tempDir}                 && curl -f -O https://hg.nginx.org/pkg-oss/archive/${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && PKGOSSCHECKSUM=\"18bee4bd498e0b8da765e8cd2d824e1027d40fd95d55fd59339cdb5d5e0e633795f4196c76045e86027cdfc6ab05a3cc0d39b25bd0a967f1edd47910d813262a *${NGINX_VERSION}-${PKG_RELEASE}.tar.gz\"                 && if [ \"\$(openssl sha512 -r ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz)\" = \"\$PKGOSSCHECKSUM\" ]; then                     echo \"pkg-oss tarball checksum verification succeeded!\";                 else                     echo \"pkg-oss tarball checksum verification failed!\";                     exit 1;                 fi                 && tar xzvf ${NGINX_VERSION}-${PKG_RELEASE}.tar.gz                 && cd pkg-oss-${NGINX_VERSION}-${PKG_RELEASE}                 && cd alpine                 && make base                 && apk index -o ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz ${tempDir}/packages/alpine/${apkArch}/*.apk                 && abuild-sign -k ${tempDir}/.abuild/abuild-key.rsa ${tempDir}/packages/alpine/${apkArch}/APKINDEX.tar.gz                 "             && cp ${tempDir}/.abuild/abuild-key.rsa.pub /etc/apk/keys/             && apk del .build-deps             && apk add -X ${tempDir}/packages/alpine/ --no-cache $nginxPackages             ;;     esac     && apk del .checksum-deps     && if [ -n "$tempDir" ]; then rm -rf "$tempDir"; fi     && if [ -n "/etc/apk/keys/abuild-key.rsa.pub" ]; then rm -f /etc/apk/keys/abuild-key.rsa.pub; fi     && if [ -n "/etc/apk/keys/nginx_signing.rsa.pub" ]; then rm -f /etc/apk/keys/nginx_signing.rsa.pub; fi     && apk add --no-cache --virtual .gettext gettext     && mv /usr/bin/envsubst /tmp/         && runDeps="$(         scanelf --needed --nobanner /tmp/envsubst             | awk '{ gsub(/,/, "\nso:", $2); print "so:" $2 }'             | sort -u             | xargs -r apk info --installed             | sort -u     )"     && apk add --no-cache $runDeps     && apk del .gettext     && mv /tmp/envsubst /usr/local/bin/     && apk add --no-cache tzdata     && ln -sf /dev/stdout /var/log/nginx/access.log     && ln -sf /dev/stderr /var/log/nginx/error.log     && mkdir /docker-entrypoint.d
# Wed, 24 May 2023 21:47:16 GMT
COPY file:7b307b62e82255f040c9812421a30090bf9abf3685f27b02d77fcca99f997911 in / 
# Wed, 24 May 2023 21:47:16 GMT
COPY file:5c18272734349488bd0c94ec8d382c872c1a0a435cca13bd4671353d6021d2cb in /docker-entrypoint.d 
# Wed, 24 May 2023 21:47:16 GMT
COPY file:36429cfeeb299f9913b84ea136b004be12fbe4bb4f975a977a3608044e8bfa91 in /docker-entrypoint.d 
# Wed, 24 May 2023 21:47:16 GMT
COPY file:e57eef017a414ca793499729d80a7b9075790c9a804f930f1417e56d506970cf in /docker-entrypoint.d 
# Wed, 24 May 2023 21:47:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 24 May 2023 21:47:16 GMT
EXPOSE 80
# Wed, 24 May 2023 21:47:17 GMT
STOPSIGNAL SIGQUIT
# Wed, 24 May 2023 21:47:17 GMT
CMD ["nginx" "-g" "daemon off;"]
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b64ecd0df4838aa770c9b8fc95846f73d8a52dd63aa0698b46bb7ff9482ec5`  
		Last Modified: Wed, 24 May 2023 21:50:52 GMT  
		Size: 4.2 MB (4166776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653782be41717db8f1843929eb762ba00e3a65f35a17889a68ddb68da75d53c9`  
		Last Modified: Wed, 24 May 2023 21:50:51 GMT  
		Size: 625.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0efd46ae6e7ee2d44dbb24601fb69ca5465c6ca900b031ed427af142b1d3ac3`  
		Last Modified: Wed, 24 May 2023 21:50:51 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966628688eb7f50f62e759710805dc8818dd3bddfd23d3a95c36757c92196faf`  
		Last Modified: Wed, 24 May 2023 21:50:51 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2887dc3dee087c649e4ee42e38c259d792f938001f72cfc26b54cc793f13bf`  
		Last Modified: Wed, 24 May 2023 21:50:51 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
