## `arangodb:latest`

```console
$ docker pull arangodb@sha256:9ca3899df8eb7afb7218648590dffa3d2076a29739265d8d656ac00459b7331d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:e83a0a0406868693a19630ef3cb24c747c5c471bcc3c43f14126371ef5375e24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.9 MB (245930699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385586e3b62e68239354f76125957ee2e746c067bd4e34b4ae2d065007d7ef47`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:01:27 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 10 Oct 2023 20:19:32 GMT
ENV ARANGO_VERSION=3.11.4
# Tue, 10 Oct 2023 20:20:01 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 10 Oct 2023 20:20:03 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 10 Oct 2023 20:20:03 GMT
RUN echo "UTC" > /etc/timezone
# Tue, 10 Oct 2023 20:20:03 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 10 Oct 2023 20:20:03 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 10 Oct 2023 20:20:03 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 10 Oct 2023 20:20:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Oct 2023 20:20:04 GMT
EXPOSE 8529
# Tue, 10 Oct 2023 20:20:04 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40c17929e744643ef209039bc401f6e3c88a3f44eb084c98ec49073c2327741`  
		Last Modified: Tue, 10 Oct 2023 20:20:45 GMT  
		Size: 243.1 MB (243120531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac333a05474e1096e4cdfb126d2abb2398ed93f0ff3c7f217c790110436ac59`  
		Last Modified: Tue, 10 Oct 2023 20:20:21 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b253bab378dc981cf86e45de55905957bf580489c4a20eea732e516eac96e594`  
		Last Modified: Tue, 10 Oct 2023 20:20:21 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961952e25751a1b192fd2188b5d65f9818c95ebf651df878e56103bd45fca46c`  
		Last Modified: Tue, 10 Oct 2023 20:20:21 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:latest` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:518df6695d129f07a52a203f8ed9ae9756565dffabae6bf63fc1ebe0641eca9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240165815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:588f47bc717b6967e3b561fb7d180c09cdf69d700aefb2fd94b0872fd4596c82`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:49:17 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 10 Oct 2023 20:39:20 GMT
ENV ARANGO_VERSION=3.11.4
# Tue, 10 Oct 2023 20:39:48 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 10 Oct 2023 20:39:52 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 10 Oct 2023 20:39:52 GMT
RUN echo "UTC" > /etc/timezone
# Tue, 10 Oct 2023 20:39:52 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 10 Oct 2023 20:39:52 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 10 Oct 2023 20:39:52 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 10 Oct 2023 20:39:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 10 Oct 2023 20:39:52 GMT
EXPOSE 8529
# Tue, 10 Oct 2023 20:39:53 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7fadc53ead1472e73f79e577cb71e373306f5844ac1391b35f18b829761497`  
		Last Modified: Tue, 10 Oct 2023 20:40:27 GMT  
		Size: 237.5 MB (237455306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ac4baa6cc31c8fc351e7c4778ad5e83362ff6894f7baeefba934ce1abd216a`  
		Last Modified: Tue, 10 Oct 2023 20:40:07 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e76a37e4541bf1a90443e53a878631b439040e69c39b88247c9fd6d62d00247`  
		Last Modified: Tue, 10 Oct 2023 20:40:07 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3404921af646e64f82a2c18a8bdd2c01d0f6af594529469df16c29d18c033231`  
		Last Modified: Tue, 10 Oct 2023 20:40:08 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
