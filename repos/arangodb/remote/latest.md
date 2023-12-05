## `arangodb:latest`

```console
$ docker pull arangodb@sha256:d2c8723c0f339a9a1d0270430718db3ba8a128deaf43f524322cae039a0fe063
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:e867565a4cabc6ed6f6bafdc4e2fc46502b57db65a76e9d7b0797c0133618e2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.4 MB (245398102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcbbbbaf309496fe5fc6a52e237a5f0da1f36f8e39df6578f42720267bcb66b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 30 Nov 2023 23:23:05 GMT
ADD file:282274bb02b29182f35c732f021f3dab6de9f16a1ae24460061ad1abdca6444a in / 
# Thu, 30 Nov 2023 23:23:05 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:33:14 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 01 Dec 2023 06:33:48 GMT
ENV ARANGO_VERSION=3.11.5
# Fri, 01 Dec 2023 06:34:15 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 01 Dec 2023 06:34:17 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 01 Dec 2023 06:34:17 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 01 Dec 2023 06:34:17 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 01 Dec 2023 06:34:17 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 01 Dec 2023 06:34:17 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 01 Dec 2023 06:34:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:34:18 GMT
EXPOSE 8529
# Fri, 01 Dec 2023 06:34:18 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:070eb51debd997eca763a31532c01e2579afe94e43b110d84282a81cb576e342`  
		Last Modified: Thu, 30 Nov 2023 23:23:49 GMT  
		Size: 2.8 MB (2807782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72020d0deb9c722d6f55813d38d0a5c5bff5466b05002f546cf06e8793dbf41`  
		Last Modified: Fri, 01 Dec 2023 06:35:21 GMT  
		Size: 242.6 MB (242587836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0307d8ebad4cbf6f100b6dac5a2dd1d80ac75de77c4721bc820498caa05cf354`  
		Last Modified: Fri, 01 Dec 2023 06:34:59 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0d22aded06793f77eec3afac7718f1f1d5b552332096b06c6fbe01a4a258a8`  
		Last Modified: Fri, 01 Dec 2023 06:34:59 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fefab97d31a60f08f5330a8a4cb7ea4918744db046cb7abe10e7ade98f3a535`  
		Last Modified: Fri, 01 Dec 2023 06:35:00 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:latest` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:b0627b11790bca396bab25097c2d0940c09f19749bed6f12081951e0f411d908
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.8 MB (243831370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b8daadef97aa3b1fd2967d9e4654758ed0a6e5bdf655bbdad78e7b6a3ce9797`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:11 GMT
ADD file:1efd26ad638f3c262f37eb81a32e3f026121dcd60479e91c42097bfc8329ed3b in / 
# Thu, 30 Nov 2023 23:11:11 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:53:16 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 05 Dec 2023 17:39:16 GMT
ENV ARANGO_VERSION=3.11.6
# Tue, 05 Dec 2023 17:39:45 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 05 Dec 2023 17:39:49 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 05 Dec 2023 17:39:50 GMT
RUN echo "UTC" > /etc/timezone
# Tue, 05 Dec 2023 17:39:50 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 05 Dec 2023 17:39:50 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 05 Dec 2023 17:39:50 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 05 Dec 2023 17:39:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Dec 2023 17:39:50 GMT
EXPOSE 8529
# Tue, 05 Dec 2023 17:39:50 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:5362b5901f8a9898f2bcc8eb6c3e6990364aa058617afaae388bdb9f437d3d7e`  
		Last Modified: Thu, 30 Nov 2023 23:11:54 GMT  
		Size: 2.7 MB (2708293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae8476c0054a82176b0a29098e04ecdbb1ea7324e40849f5014235afd50d629`  
		Last Modified: Tue, 05 Dec 2023 17:40:20 GMT  
		Size: 241.1 MB (241120590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad84b93e255d7c8a928830635cb49067f5e65c484ca0f7df1807e6d22812f0e`  
		Last Modified: Tue, 05 Dec 2023 17:40:03 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ceb9fb0ef3ff1db3775d9c17fa6c334b8ebf39a308d8fa5824343bde7ab8bc3`  
		Last Modified: Tue, 05 Dec 2023 17:40:03 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737b8448bc16570f1e609e627abfb0f8a45a0b2dfb559a242688528707d9a42e`  
		Last Modified: Tue, 05 Dec 2023 17:40:03 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
