<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.10`](#arangodb310)
-	[`arangodb:3.10.9`](#arangodb3109)
-	[`arangodb:3.11`](#arangodb311)
-	[`arangodb:3.11.1`](#arangodb3111)
-	[`arangodb:3.9`](#arangodb39)
-	[`arangodb:3.9.11`](#arangodb3911)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.10`

```console
$ docker pull arangodb@sha256:91e2fe09b8a52eafb9d3e74b062e64429549fdb8dbeb47926e645947f5291eea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10` - linux; amd64

```console
$ docker pull arangodb@sha256:62339d4c292d87affe420f3c61a1a9a7af8488ff07e4f900bae4cf88834c43bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.3 MB (222258499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29910f7d2868c41f097d71cf6f3711d312dec605f00368991be61a6a7bb05e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:31:43 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 20 Jun 2023 20:19:32 GMT
ENV ARANGO_VERSION=3.10.7
# Tue, 20 Jun 2023 20:20:01 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 20 Jun 2023 20:20:03 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 20 Jun 2023 20:20:03 GMT
RUN echo "UTC" > /etc/timezone
# Tue, 20 Jun 2023 20:20:03 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 20 Jun 2023 20:20:04 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 20 Jun 2023 20:20:04 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 20 Jun 2023 20:20:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 20:20:04 GMT
EXPOSE 8529
# Tue, 20 Jun 2023 20:20:04 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b859690d59ed1a82441902fd56ccc1acca20f99c139d6cfdf7caeca801a3ba`  
		Last Modified: Tue, 20 Jun 2023 20:21:21 GMT  
		Size: 219.4 MB (219448354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19620aaa2ac72b632d9241f2b2393fb932becbd4af1563545a1f7bc72cd84b21`  
		Last Modified: Tue, 20 Jun 2023 20:20:59 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1d8418cfb3b862f699198544eb624631e802523e2a13fe473b6ffffe8da7c8`  
		Last Modified: Tue, 20 Jun 2023 20:20:59 GMT  
		Size: 2.1 KB (2082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d54c66cf50948c66443542c7165e33068aba27dc8d47154573325df44acc51e`  
		Last Modified: Tue, 20 Jun 2023 20:21:00 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:62eb04ada711ea920fc2246d1de2e02243bb7848911c381780b8a52eb096c619
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217473136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c463184dddd7aac25b52521ba7ea492abae2a794d9c45bc4748b74a57d51b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:45:26 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 20 Jun 2023 20:39:15 GMT
ENV ARANGO_VERSION=3.10.7
# Tue, 20 Jun 2023 20:39:40 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 20 Jun 2023 20:39:44 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 20 Jun 2023 20:39:44 GMT
RUN echo "UTC" > /etc/timezone
# Tue, 20 Jun 2023 20:39:44 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 20 Jun 2023 20:39:44 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 20 Jun 2023 20:39:44 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 20 Jun 2023 20:39:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 20:39:45 GMT
EXPOSE 8529
# Tue, 20 Jun 2023 20:39:45 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a776ab6c922197fd1b49a5cb7acc08acda3cc4099ed65b0cf7e47d43478fe3a`  
		Last Modified: Tue, 20 Jun 2023 20:40:44 GMT  
		Size: 214.8 MB (214762752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d67aae28297e59c2c14f613ef66557704142b6700f098fa8ed26050ed3156fd`  
		Last Modified: Tue, 20 Jun 2023 20:40:28 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99caf32f87e93353d8a6da87b3820081c67d4dd3f065aa6fbd17be9cbc70001c`  
		Last Modified: Tue, 20 Jun 2023 20:40:28 GMT  
		Size: 2.1 KB (2082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40305d32477e15ef980c757119f9f21a279fdf611b2a8d40ca6c575e6b41ada9`  
		Last Modified: Tue, 20 Jun 2023 20:40:28 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.10.9`

**does not exist** (yet?)

## `arangodb:3.11`

```console
$ docker pull arangodb@sha256:6faebdaf924ae13c4ae0c03213b05cc01255b167d1c1178788d4312d08cf65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.11` - linux; amd64

```console
$ docker pull arangodb@sha256:92e63a7fd0ef923d0a0cbecbd540f02919283e68e946724ee344c9d148b43c47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244507280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2d22af6f68892edd104247abfbefc8a913b842e87e2a9a49ad88019cbf56865`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:31:43 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 20 Jun 2023 20:20:13 GMT
ENV ARANGO_VERSION=3.11.1
# Tue, 20 Jun 2023 20:20:39 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 20 Jun 2023 20:20:40 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 20 Jun 2023 20:20:41 GMT
RUN echo "UTC" > /etc/timezone
# Tue, 20 Jun 2023 20:20:41 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 20 Jun 2023 20:20:41 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 20 Jun 2023 20:20:41 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 20 Jun 2023 20:20:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 20:20:41 GMT
EXPOSE 8529
# Tue, 20 Jun 2023 20:20:41 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd2e41c3757a3897f87d2bc7628a7bb3925949c57a45a1b4cf324d9393e9071`  
		Last Modified: Tue, 20 Jun 2023 20:21:53 GMT  
		Size: 241.7 MB (241697137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9515d503e1f0dc62c65df0af3ff423005022a8d381f22f80e9dfe7d41267604c`  
		Last Modified: Tue, 20 Jun 2023 20:21:30 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd77e2f0e79bdbcb05d12713faf463692382208e9ac35480429a8ab39b16f08`  
		Last Modified: Tue, 20 Jun 2023 20:21:30 GMT  
		Size: 2.1 KB (2079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8876046ac800cf70b43667ed9d0403dd660b523d93c7b4a410282fdff86e57f`  
		Last Modified: Tue, 20 Jun 2023 20:21:30 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.11` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:db213e4a254a620968a91a572c485b21af41baabdd0fc38644caf7a4e9f72138
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238930320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa0e6f73b91831fcafe50afb7d2183b840468243e1a0824dae04468ae57f026a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:45:26 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 20 Jun 2023 20:39:48 GMT
ENV ARANGO_VERSION=3.11.1
# Tue, 20 Jun 2023 20:40:12 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 20 Jun 2023 20:40:16 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 20 Jun 2023 20:40:17 GMT
RUN echo "UTC" > /etc/timezone
# Tue, 20 Jun 2023 20:40:17 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 20 Jun 2023 20:40:17 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 20 Jun 2023 20:40:17 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 20 Jun 2023 20:40:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 20:40:17 GMT
EXPOSE 8529
# Tue, 20 Jun 2023 20:40:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e645bfc23fce653d0ae9c85504192cdd5c5750a026359d5ee3cb957f1b25140`  
		Last Modified: Tue, 20 Jun 2023 20:41:10 GMT  
		Size: 236.2 MB (236219935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f18a1abe64decc301219a0d3e20f65b090984b0793ad7db5cf493d68b784a6`  
		Last Modified: Tue, 20 Jun 2023 20:40:54 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604bb6f22400d5760c77f868120ba8cd2083ce7b90f0f20bda20907c82db4dc6`  
		Last Modified: Tue, 20 Jun 2023 20:40:54 GMT  
		Size: 2.1 KB (2083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a940a72288c4d57c949200c09230817370ea559b3ec25b7bd55d591f1257f0e`  
		Last Modified: Tue, 20 Jun 2023 20:40:54 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.11.1`

```console
$ docker pull arangodb@sha256:6faebdaf924ae13c4ae0c03213b05cc01255b167d1c1178788d4312d08cf65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.11.1` - linux; amd64

```console
$ docker pull arangodb@sha256:92e63a7fd0ef923d0a0cbecbd540f02919283e68e946724ee344c9d148b43c47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244507280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2d22af6f68892edd104247abfbefc8a913b842e87e2a9a49ad88019cbf56865`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:31:43 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 20 Jun 2023 20:20:13 GMT
ENV ARANGO_VERSION=3.11.1
# Tue, 20 Jun 2023 20:20:39 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 20 Jun 2023 20:20:40 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 20 Jun 2023 20:20:41 GMT
RUN echo "UTC" > /etc/timezone
# Tue, 20 Jun 2023 20:20:41 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 20 Jun 2023 20:20:41 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 20 Jun 2023 20:20:41 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 20 Jun 2023 20:20:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 20:20:41 GMT
EXPOSE 8529
# Tue, 20 Jun 2023 20:20:41 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd2e41c3757a3897f87d2bc7628a7bb3925949c57a45a1b4cf324d9393e9071`  
		Last Modified: Tue, 20 Jun 2023 20:21:53 GMT  
		Size: 241.7 MB (241697137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9515d503e1f0dc62c65df0af3ff423005022a8d381f22f80e9dfe7d41267604c`  
		Last Modified: Tue, 20 Jun 2023 20:21:30 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd77e2f0e79bdbcb05d12713faf463692382208e9ac35480429a8ab39b16f08`  
		Last Modified: Tue, 20 Jun 2023 20:21:30 GMT  
		Size: 2.1 KB (2079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8876046ac800cf70b43667ed9d0403dd660b523d93c7b4a410282fdff86e57f`  
		Last Modified: Tue, 20 Jun 2023 20:21:30 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.11.1` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:db213e4a254a620968a91a572c485b21af41baabdd0fc38644caf7a4e9f72138
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238930320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa0e6f73b91831fcafe50afb7d2183b840468243e1a0824dae04468ae57f026a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:45:26 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 20 Jun 2023 20:39:48 GMT
ENV ARANGO_VERSION=3.11.1
# Tue, 20 Jun 2023 20:40:12 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 20 Jun 2023 20:40:16 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 20 Jun 2023 20:40:17 GMT
RUN echo "UTC" > /etc/timezone
# Tue, 20 Jun 2023 20:40:17 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 20 Jun 2023 20:40:17 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 20 Jun 2023 20:40:17 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 20 Jun 2023 20:40:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 20:40:17 GMT
EXPOSE 8529
# Tue, 20 Jun 2023 20:40:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e645bfc23fce653d0ae9c85504192cdd5c5750a026359d5ee3cb957f1b25140`  
		Last Modified: Tue, 20 Jun 2023 20:41:10 GMT  
		Size: 236.2 MB (236219935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f18a1abe64decc301219a0d3e20f65b090984b0793ad7db5cf493d68b784a6`  
		Last Modified: Tue, 20 Jun 2023 20:40:54 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604bb6f22400d5760c77f868120ba8cd2083ce7b90f0f20bda20907c82db4dc6`  
		Last Modified: Tue, 20 Jun 2023 20:40:54 GMT  
		Size: 2.1 KB (2083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a940a72288c4d57c949200c09230817370ea559b3ec25b7bd55d591f1257f0e`  
		Last Modified: Tue, 20 Jun 2023 20:40:54 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9`

```console
$ docker pull arangodb@sha256:ccf0b7efd9fdec9bee4d9be7146a5de6ac31f9f81fc6af3f117c69f3fae8a6fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9` - linux; amd64

```console
$ docker pull arangodb@sha256:ab0472c6a34396b6ee935ff2d20e728e7cee47c1185aa4c2e87ad5e5e5be7071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204918983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b57af32609c3ba32aed5579df23b0bcdd83cc24cf847e6e8e9ce09087203469e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:31:09 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 15 Jun 2023 04:31:09 GMT
ENV ARANGO_VERSION=3.9.11
# Thu, 15 Jun 2023 04:31:09 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Thu, 15 Jun 2023 04:31:09 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.11-1_amd64.deb
# Thu, 15 Jun 2023 04:31:09 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.11-1_amd64.deb
# Thu, 15 Jun 2023 04:31:09 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.11-1_amd64.deb.asc
# Thu, 15 Jun 2023 04:31:33 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 15 Jun 2023 04:31:35 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 15 Jun 2023 04:31:35 GMT
RUN echo "UTC" > /etc/timezone
# Thu, 15 Jun 2023 04:31:36 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 15 Jun 2023 04:31:36 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 15 Jun 2023 04:31:36 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 15 Jun 2023 04:31:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:31:36 GMT
EXPOSE 8529
# Thu, 15 Jun 2023 04:31:36 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c16a1d2ea9ec99f711bc1f059e3453f6aef7ed8a715c89fc6641bbfeaae75a`  
		Last Modified: Thu, 15 Jun 2023 04:33:20 GMT  
		Size: 202.1 MB (202090582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51cd75103f25338f7755dd747750cdfce1fc4ce93f6574938d8a09eb5038ace`  
		Last Modified: Thu, 15 Jun 2023 04:32:59 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d618805dae2b46f80669fc843875aee0478255cb03b54b1900549877120ea31e`  
		Last Modified: Thu, 15 Jun 2023 04:32:59 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fabe4d9a822ca5fd9154a10fc60698da3125d474633150cd5010745963b7ce2`  
		Last Modified: Thu, 15 Jun 2023 04:33:00 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9.11`

```console
$ docker pull arangodb@sha256:ccf0b7efd9fdec9bee4d9be7146a5de6ac31f9f81fc6af3f117c69f3fae8a6fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9.11` - linux; amd64

```console
$ docker pull arangodb@sha256:ab0472c6a34396b6ee935ff2d20e728e7cee47c1185aa4c2e87ad5e5e5be7071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204918983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b57af32609c3ba32aed5579df23b0bcdd83cc24cf847e6e8e9ce09087203469e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:31:09 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 15 Jun 2023 04:31:09 GMT
ENV ARANGO_VERSION=3.9.11
# Thu, 15 Jun 2023 04:31:09 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Thu, 15 Jun 2023 04:31:09 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.11-1_amd64.deb
# Thu, 15 Jun 2023 04:31:09 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.11-1_amd64.deb
# Thu, 15 Jun 2023 04:31:09 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.11-1_amd64.deb.asc
# Thu, 15 Jun 2023 04:31:33 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 15 Jun 2023 04:31:35 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 15 Jun 2023 04:31:35 GMT
RUN echo "UTC" > /etc/timezone
# Thu, 15 Jun 2023 04:31:36 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 15 Jun 2023 04:31:36 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 15 Jun 2023 04:31:36 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 15 Jun 2023 04:31:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:31:36 GMT
EXPOSE 8529
# Thu, 15 Jun 2023 04:31:36 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c16a1d2ea9ec99f711bc1f059e3453f6aef7ed8a715c89fc6641bbfeaae75a`  
		Last Modified: Thu, 15 Jun 2023 04:33:20 GMT  
		Size: 202.1 MB (202090582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51cd75103f25338f7755dd747750cdfce1fc4ce93f6574938d8a09eb5038ace`  
		Last Modified: Thu, 15 Jun 2023 04:32:59 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d618805dae2b46f80669fc843875aee0478255cb03b54b1900549877120ea31e`  
		Last Modified: Thu, 15 Jun 2023 04:32:59 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fabe4d9a822ca5fd9154a10fc60698da3125d474633150cd5010745963b7ce2`  
		Last Modified: Thu, 15 Jun 2023 04:33:00 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:6faebdaf924ae13c4ae0c03213b05cc01255b167d1c1178788d4312d08cf65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:92e63a7fd0ef923d0a0cbecbd540f02919283e68e946724ee344c9d148b43c47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244507280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2d22af6f68892edd104247abfbefc8a913b842e87e2a9a49ad88019cbf56865`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:31:43 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 20 Jun 2023 20:20:13 GMT
ENV ARANGO_VERSION=3.11.1
# Tue, 20 Jun 2023 20:20:39 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 20 Jun 2023 20:20:40 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 20 Jun 2023 20:20:41 GMT
RUN echo "UTC" > /etc/timezone
# Tue, 20 Jun 2023 20:20:41 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 20 Jun 2023 20:20:41 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 20 Jun 2023 20:20:41 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 20 Jun 2023 20:20:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 20:20:41 GMT
EXPOSE 8529
# Tue, 20 Jun 2023 20:20:41 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd2e41c3757a3897f87d2bc7628a7bb3925949c57a45a1b4cf324d9393e9071`  
		Last Modified: Tue, 20 Jun 2023 20:21:53 GMT  
		Size: 241.7 MB (241697137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9515d503e1f0dc62c65df0af3ff423005022a8d381f22f80e9dfe7d41267604c`  
		Last Modified: Tue, 20 Jun 2023 20:21:30 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd77e2f0e79bdbcb05d12713faf463692382208e9ac35480429a8ab39b16f08`  
		Last Modified: Tue, 20 Jun 2023 20:21:30 GMT  
		Size: 2.1 KB (2079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8876046ac800cf70b43667ed9d0403dd660b523d93c7b4a410282fdff86e57f`  
		Last Modified: Tue, 20 Jun 2023 20:21:30 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:latest` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:db213e4a254a620968a91a572c485b21af41baabdd0fc38644caf7a4e9f72138
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.9 MB (238930320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa0e6f73b91831fcafe50afb7d2183b840468243e1a0824dae04468ae57f026a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:45:26 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 20 Jun 2023 20:39:48 GMT
ENV ARANGO_VERSION=3.11.1
# Tue, 20 Jun 2023 20:40:12 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 20 Jun 2023 20:40:16 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 20 Jun 2023 20:40:17 GMT
RUN echo "UTC" > /etc/timezone
# Tue, 20 Jun 2023 20:40:17 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 20 Jun 2023 20:40:17 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 20 Jun 2023 20:40:17 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 20 Jun 2023 20:40:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jun 2023 20:40:17 GMT
EXPOSE 8529
# Tue, 20 Jun 2023 20:40:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e645bfc23fce653d0ae9c85504192cdd5c5750a026359d5ee3cb957f1b25140`  
		Last Modified: Tue, 20 Jun 2023 20:41:10 GMT  
		Size: 236.2 MB (236219935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f18a1abe64decc301219a0d3e20f65b090984b0793ad7db5cf493d68b784a6`  
		Last Modified: Tue, 20 Jun 2023 20:40:54 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604bb6f22400d5760c77f868120ba8cd2083ce7b90f0f20bda20907c82db4dc6`  
		Last Modified: Tue, 20 Jun 2023 20:40:54 GMT  
		Size: 2.1 KB (2083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a940a72288c4d57c949200c09230817370ea559b3ec25b7bd55d591f1257f0e`  
		Last Modified: Tue, 20 Jun 2023 20:40:54 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
