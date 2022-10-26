<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.10`](#arangodb310)
-	[`arangodb:3.10.0`](#arangodb3100)
-	[`arangodb:3.8`](#arangodb38)
-	[`arangodb:3.8.8`](#arangodb388)
-	[`arangodb:3.9`](#arangodb39)
-	[`arangodb:3.9.4`](#arangodb394)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.10`

```console
$ docker pull arangodb@sha256:c1089d0fbadad5be3252ec935a561342cf2179d9d3b0aa55e6f27eabaf2d848c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10` - linux; amd64

```console
$ docker pull arangodb@sha256:c0d4e9df6dcd8645c3d84395fe84652b87cf8b07db363d2d5e70274f8cef3dd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.8 MB (218752791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d2f9a9d5c96eecd66cb16c817989e3fabe592fabcd60165237466af2d6e788`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 12 Oct 2022 19:19:28 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 12 Oct 2022 19:19:28 GMT
ENV ARANGO_VERSION=3.10.0
# Wed, 12 Oct 2022 19:19:53 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 12 Oct 2022 19:19:55 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 12 Oct 2022 19:19:55 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 12 Oct 2022 19:19:56 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 12 Oct 2022 19:19:56 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 12 Oct 2022 19:19:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 12 Oct 2022 19:19:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Oct 2022 19:19:56 GMT
EXPOSE 8529
# Wed, 12 Oct 2022 19:19:56 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614c1b15d1f618586750750d537cb77ab74b182930266a4a1f432fd6d556e276`  
		Last Modified: Wed, 12 Oct 2022 19:20:55 GMT  
		Size: 215.9 MB (215944251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be0edb86b44826c4c52b741d7b62ad5a0a50bb46af0e6726d5ad25c6712b43e`  
		Last Modified: Wed, 12 Oct 2022 19:20:14 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c743a53b7ac0379787c5abb5643c79f7ce16f2c646c485c5ac347eb213a4c8`  
		Last Modified: Wed, 12 Oct 2022 19:20:14 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69f3d2d920cde77d2e955d7fae092c587aa8976f94c63e34bd79bc48188ee20`  
		Last Modified: Wed, 12 Oct 2022 19:20:14 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:45cb799bce59eb0347493f7b1dc2e1d1c6f4fb4266447a6efd462ed724a50e6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.3 MB (213305202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d90c8846412a12aea287bcfa464cddb8cd4e41bf61d144eb23a785ed2640391`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 12 Oct 2022 23:39:22 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 12 Oct 2022 23:39:23 GMT
ENV ARANGO_VERSION=3.10.0
# Wed, 12 Oct 2022 23:39:50 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 12 Oct 2022 23:39:51 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 12 Oct 2022 23:39:53 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 12 Oct 2022 23:39:54 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 12 Oct 2022 23:39:55 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 12 Oct 2022 23:39:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 12 Oct 2022 23:39:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Oct 2022 23:39:57 GMT
EXPOSE 8529
# Wed, 12 Oct 2022 23:39:58 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0d28a757c0873e11430af2040601c8b44c8d9d61133328101a0d02bd84b769`  
		Last Modified: Wed, 12 Oct 2022 23:40:40 GMT  
		Size: 210.6 MB (210595052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d74b64274ed2dd7a1eac1e633fca519907067d0fb0582ed2083d8f1cab67914`  
		Last Modified: Wed, 12 Oct 2022 23:40:16 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bc407de99440dc4240bcc39354b27affa1064456447674436a9147b0be6529`  
		Last Modified: Wed, 12 Oct 2022 23:40:16 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2a38770968bbd3053b373f10d13d3cdd8bac9db587e73acd43262270ab440f`  
		Last Modified: Wed, 12 Oct 2022 23:40:16 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.10.0`

```console
$ docker pull arangodb@sha256:c1089d0fbadad5be3252ec935a561342cf2179d9d3b0aa55e6f27eabaf2d848c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10.0` - linux; amd64

```console
$ docker pull arangodb@sha256:c0d4e9df6dcd8645c3d84395fe84652b87cf8b07db363d2d5e70274f8cef3dd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.8 MB (218752791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d2f9a9d5c96eecd66cb16c817989e3fabe592fabcd60165237466af2d6e788`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 12 Oct 2022 19:19:28 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 12 Oct 2022 19:19:28 GMT
ENV ARANGO_VERSION=3.10.0
# Wed, 12 Oct 2022 19:19:53 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 12 Oct 2022 19:19:55 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 12 Oct 2022 19:19:55 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 12 Oct 2022 19:19:56 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 12 Oct 2022 19:19:56 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 12 Oct 2022 19:19:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 12 Oct 2022 19:19:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Oct 2022 19:19:56 GMT
EXPOSE 8529
# Wed, 12 Oct 2022 19:19:56 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614c1b15d1f618586750750d537cb77ab74b182930266a4a1f432fd6d556e276`  
		Last Modified: Wed, 12 Oct 2022 19:20:55 GMT  
		Size: 215.9 MB (215944251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be0edb86b44826c4c52b741d7b62ad5a0a50bb46af0e6726d5ad25c6712b43e`  
		Last Modified: Wed, 12 Oct 2022 19:20:14 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c743a53b7ac0379787c5abb5643c79f7ce16f2c646c485c5ac347eb213a4c8`  
		Last Modified: Wed, 12 Oct 2022 19:20:14 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69f3d2d920cde77d2e955d7fae092c587aa8976f94c63e34bd79bc48188ee20`  
		Last Modified: Wed, 12 Oct 2022 19:20:14 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10.0` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:45cb799bce59eb0347493f7b1dc2e1d1c6f4fb4266447a6efd462ed724a50e6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.3 MB (213305202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d90c8846412a12aea287bcfa464cddb8cd4e41bf61d144eb23a785ed2640391`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 12 Oct 2022 23:39:22 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 12 Oct 2022 23:39:23 GMT
ENV ARANGO_VERSION=3.10.0
# Wed, 12 Oct 2022 23:39:50 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 12 Oct 2022 23:39:51 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 12 Oct 2022 23:39:53 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 12 Oct 2022 23:39:54 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 12 Oct 2022 23:39:55 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 12 Oct 2022 23:39:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 12 Oct 2022 23:39:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Oct 2022 23:39:57 GMT
EXPOSE 8529
# Wed, 12 Oct 2022 23:39:58 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0d28a757c0873e11430af2040601c8b44c8d9d61133328101a0d02bd84b769`  
		Last Modified: Wed, 12 Oct 2022 23:40:40 GMT  
		Size: 210.6 MB (210595052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d74b64274ed2dd7a1eac1e633fca519907067d0fb0582ed2083d8f1cab67914`  
		Last Modified: Wed, 12 Oct 2022 23:40:16 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bc407de99440dc4240bcc39354b27affa1064456447674436a9147b0be6529`  
		Last Modified: Wed, 12 Oct 2022 23:40:16 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2a38770968bbd3053b373f10d13d3cdd8bac9db587e73acd43262270ab440f`  
		Last Modified: Wed, 12 Oct 2022 23:40:16 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8`

```console
$ docker pull arangodb@sha256:cbb2dd0e3d6c33a5a569d94108648423b8462d7fe2ee03ccea067701b9f0a309
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8` - linux; amd64

```console
$ docker pull arangodb@sha256:639d75587d5501c651d4be6c73e317a7998923f638cc942192785b2347b00c60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195462869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb2a216d69e5be1767539cce2f442d3ed688dd241ae3f95c6241abb569a1b96f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:51:41 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 06 Oct 2022 19:51:41 GMT
ENV ARANGO_VERSION=3.8.7
# Thu, 06 Oct 2022 19:51:41 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Thu, 06 Oct 2022 19:51:41 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.7-1_amd64.deb
# Thu, 06 Oct 2022 19:51:41 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.7-1_amd64.deb
# Thu, 06 Oct 2022 19:51:42 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.7-1_amd64.deb.asc
# Thu, 06 Oct 2022 19:52:10 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 06 Oct 2022 19:52:12 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 06 Oct 2022 19:52:12 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 06 Oct 2022 19:52:12 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 06 Oct 2022 19:52:12 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 06 Oct 2022 19:52:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 19:52:12 GMT
EXPOSE 8529
# Thu, 06 Oct 2022 19:52:12 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e9775ec3b5069ed5efe2248239365986d057eb0385ac2fc0c53278584cdfd9`  
		Last Modified: Thu, 06 Oct 2022 19:53:20 GMT  
		Size: 192.6 MB (192633033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f7963295ca7efe2c1523098c42cac3fb49a6e9674b0fac19069ab00e90425d`  
		Last Modified: Thu, 06 Oct 2022 19:52:58 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbed31d889de3075b13bc411f44d3ede2c6b0d306af6ef46167d9c62f8586e6`  
		Last Modified: Thu, 06 Oct 2022 19:52:58 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8.8`

**does not exist** (yet?)

## `arangodb:3.9`

```console
$ docker pull arangodb@sha256:1473513a62b3bc8d5b6bec88dfb3797df99fc5a1c7f637e07c5ebcd075902dde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9` - linux; amd64

```console
$ docker pull arangodb@sha256:5871e58bc4205073ae72f93739d3d3f7c59df1234fb8b997bb19003d8e2267d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.2 MB (201164652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66558e1dbf6bbbf2f653b92e1d4fee19713c7b144f9fe9962ff239c931ea9564`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:51:41 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 06 Oct 2022 19:52:15 GMT
ENV ARANGO_VERSION=3.9.3
# Thu, 06 Oct 2022 19:52:15 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Thu, 06 Oct 2022 19:52:15 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.3-1_amd64.deb
# Thu, 06 Oct 2022 19:52:15 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.3-1_amd64.deb
# Thu, 06 Oct 2022 19:52:15 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.3-1_amd64.deb.asc
# Thu, 06 Oct 2022 19:52:42 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 06 Oct 2022 19:52:43 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 06 Oct 2022 19:52:44 GMT
RUN echo "UTC" > /etc/timezone
# Thu, 06 Oct 2022 19:52:44 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 06 Oct 2022 19:52:44 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 06 Oct 2022 19:52:44 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 06 Oct 2022 19:52:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 06 Oct 2022 19:52:44 GMT
EXPOSE 8529
# Thu, 06 Oct 2022 19:52:44 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d2e28d78a90b0910e64739a3514b58212d33755fdf49b1fd7d1a1691c7620b`  
		Last Modified: Thu, 06 Oct 2022 19:53:52 GMT  
		Size: 198.3 MB (198334675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e24444b684c9850ee9d71c36862c5ea05ed8d03d6d178581d8d921d92443871`  
		Last Modified: Thu, 06 Oct 2022 19:53:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc405a118acd2437261c2391c38b4d3332ca39fbb5eae4d3e0a58895951e6336`  
		Last Modified: Thu, 06 Oct 2022 19:53:29 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca561580ab8f06159eb6a0687bfdee1a25232814c66f89bccd3ce9a879bd098`  
		Last Modified: Thu, 06 Oct 2022 19:53:29 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9.4`

**does not exist** (yet?)

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:c1089d0fbadad5be3252ec935a561342cf2179d9d3b0aa55e6f27eabaf2d848c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:c0d4e9df6dcd8645c3d84395fe84652b87cf8b07db363d2d5e70274f8cef3dd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.8 MB (218752791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d2f9a9d5c96eecd66cb16c817989e3fabe592fabcd60165237466af2d6e788`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 12 Oct 2022 19:19:28 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 12 Oct 2022 19:19:28 GMT
ENV ARANGO_VERSION=3.10.0
# Wed, 12 Oct 2022 19:19:53 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 12 Oct 2022 19:19:55 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 12 Oct 2022 19:19:55 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 12 Oct 2022 19:19:56 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 12 Oct 2022 19:19:56 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 12 Oct 2022 19:19:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 12 Oct 2022 19:19:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Oct 2022 19:19:56 GMT
EXPOSE 8529
# Wed, 12 Oct 2022 19:19:56 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614c1b15d1f618586750750d537cb77ab74b182930266a4a1f432fd6d556e276`  
		Last Modified: Wed, 12 Oct 2022 19:20:55 GMT  
		Size: 215.9 MB (215944251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be0edb86b44826c4c52b741d7b62ad5a0a50bb46af0e6726d5ad25c6712b43e`  
		Last Modified: Wed, 12 Oct 2022 19:20:14 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c743a53b7ac0379787c5abb5643c79f7ce16f2c646c485c5ac347eb213a4c8`  
		Last Modified: Wed, 12 Oct 2022 19:20:14 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69f3d2d920cde77d2e955d7fae092c587aa8976f94c63e34bd79bc48188ee20`  
		Last Modified: Wed, 12 Oct 2022 19:20:14 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:latest` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:45cb799bce59eb0347493f7b1dc2e1d1c6f4fb4266447a6efd462ed724a50e6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.3 MB (213305202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d90c8846412a12aea287bcfa464cddb8cd4e41bf61d144eb23a785ed2640391`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 12 Oct 2022 23:39:22 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 12 Oct 2022 23:39:23 GMT
ENV ARANGO_VERSION=3.10.0
# Wed, 12 Oct 2022 23:39:50 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 12 Oct 2022 23:39:51 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 12 Oct 2022 23:39:53 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 12 Oct 2022 23:39:54 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 12 Oct 2022 23:39:55 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 12 Oct 2022 23:39:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 12 Oct 2022 23:39:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 Oct 2022 23:39:57 GMT
EXPOSE 8529
# Wed, 12 Oct 2022 23:39:58 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0d28a757c0873e11430af2040601c8b44c8d9d61133328101a0d02bd84b769`  
		Last Modified: Wed, 12 Oct 2022 23:40:40 GMT  
		Size: 210.6 MB (210595052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d74b64274ed2dd7a1eac1e633fca519907067d0fb0582ed2083d8f1cab67914`  
		Last Modified: Wed, 12 Oct 2022 23:40:16 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bc407de99440dc4240bcc39354b27affa1064456447674436a9147b0be6529`  
		Last Modified: Wed, 12 Oct 2022 23:40:16 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2a38770968bbd3053b373f10d13d3cdd8bac9db587e73acd43262270ab440f`  
		Last Modified: Wed, 12 Oct 2022 23:40:16 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
