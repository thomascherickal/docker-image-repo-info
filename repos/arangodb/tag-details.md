<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.16`](#arangodb3716)
-	[`arangodb:3.8`](#arangodb38)
-	[`arangodb:3.8.5`](#arangodb385)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.7`

```console
$ docker pull arangodb@sha256:698d6e77da3e489b90b90e248015971fcbbc8d03b026ecf3f0777b4810d42ff6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.7` - linux; amd64

```console
$ docker pull arangodb@sha256:5f3d7baa1ac1bb1619a0edaf299ab3fe5f6b374822353727a9091d270a4fdc48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129852374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab06ec13d370dc7d8a3bd427355464266ba070c73c43ceeb57cf898b16292a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 23:39:44 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 30 Nov 2021 02:04:38 GMT
ENV ARANGO_VERSION=3.7.16
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.16-1_amd64.deb
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.16-1_amd64.deb
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.16-1_amd64.deb.asc
# Tue, 30 Nov 2021 02:05:08 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 30 Nov 2021 02:05:09 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 30 Nov 2021 02:05:09 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 30 Nov 2021 02:05:10 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 30 Nov 2021 02:05:10 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 30 Nov 2021 02:05:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Nov 2021 02:05:10 GMT
EXPOSE 8529
# Tue, 30 Nov 2021 02:05:10 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326555101505cf4c0cbca4a485745d6347b07afab2743a6613c92206ea93e86a`  
		Last Modified: Tue, 30 Nov 2021 02:05:49 GMT  
		Size: 127.0 MB (127040553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1e8bfc72f79aaecc8c16669712400f2dcd30cd0eb102d53a2ac410d440ad91`  
		Last Modified: Tue, 30 Nov 2021 02:05:28 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d67776f010a857b6e06385539c82f4026a667cd113a26fd360ece160f846e0`  
		Last Modified: Tue, 30 Nov 2021 02:05:28 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7.16`

```console
$ docker pull arangodb@sha256:698d6e77da3e489b90b90e248015971fcbbc8d03b026ecf3f0777b4810d42ff6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.7.16` - linux; amd64

```console
$ docker pull arangodb@sha256:5f3d7baa1ac1bb1619a0edaf299ab3fe5f6b374822353727a9091d270a4fdc48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129852374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab06ec13d370dc7d8a3bd427355464266ba070c73c43ceeb57cf898b16292a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 23:39:44 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 30 Nov 2021 02:04:38 GMT
ENV ARANGO_VERSION=3.7.16
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.16-1_amd64.deb
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.16-1_amd64.deb
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.16-1_amd64.deb.asc
# Tue, 30 Nov 2021 02:05:08 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 30 Nov 2021 02:05:09 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 30 Nov 2021 02:05:09 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 30 Nov 2021 02:05:10 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 30 Nov 2021 02:05:10 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 30 Nov 2021 02:05:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Nov 2021 02:05:10 GMT
EXPOSE 8529
# Tue, 30 Nov 2021 02:05:10 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326555101505cf4c0cbca4a485745d6347b07afab2743a6613c92206ea93e86a`  
		Last Modified: Tue, 30 Nov 2021 02:05:49 GMT  
		Size: 127.0 MB (127040553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1e8bfc72f79aaecc8c16669712400f2dcd30cd0eb102d53a2ac410d440ad91`  
		Last Modified: Tue, 30 Nov 2021 02:05:28 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d67776f010a857b6e06385539c82f4026a667cd113a26fd360ece160f846e0`  
		Last Modified: Tue, 30 Nov 2021 02:05:28 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8`

```console
$ docker pull arangodb@sha256:29961aed4abbd3e59058ab67500113451f12dea6f6ca8f09433adf625c289e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8` - linux; amd64

```console
$ docker pull arangodb@sha256:b740f7c169c3894f7e56e56ac26fb5c79936eaabd03758a33fca4813bdf7d2d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.9 MB (190942252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f122b8e5228cd96ffca98393189ec6c109770f49b78bb9c5b2071a1c67d9bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 24 Jan 2022 23:19:42 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 24 Jan 2022 23:19:42 GMT
ENV ARANGO_VERSION=3.8.5
# Mon, 24 Jan 2022 23:19:42 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Mon, 24 Jan 2022 23:19:43 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.5-1_amd64.deb
# Mon, 24 Jan 2022 23:19:43 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.5-1_amd64.deb
# Mon, 24 Jan 2022 23:19:43 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.5-1_amd64.deb.asc
# Mon, 24 Jan 2022 23:20:14 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 24 Jan 2022 23:20:16 GMT
ENV GLIBCXX_FORCE_NEW=1
# Mon, 24 Jan 2022 23:20:16 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 24 Jan 2022 23:20:16 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Mon, 24 Jan 2022 23:20:16 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Mon, 24 Jan 2022 23:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Jan 2022 23:20:17 GMT
EXPOSE 8529
# Mon, 24 Jan 2022 23:20:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ed1a596e4434531e6c22f3365699ef06a41bd12826223952ed10a50d391c8a`  
		Last Modified: Mon, 24 Jan 2022 23:20:58 GMT  
		Size: 188.1 MB (188116923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd156c42d695e883867b79fd93c87ff5c9b09e71d74b5cff967e396d642cf40`  
		Last Modified: Mon, 24 Jan 2022 23:20:38 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3688f86f7a379ca4f05a1c6ea9791f7fb55d6973a131eddeddf683c2a8bf5714`  
		Last Modified: Mon, 24 Jan 2022 23:20:38 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8.5`

```console
$ docker pull arangodb@sha256:29961aed4abbd3e59058ab67500113451f12dea6f6ca8f09433adf625c289e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8.5` - linux; amd64

```console
$ docker pull arangodb@sha256:b740f7c169c3894f7e56e56ac26fb5c79936eaabd03758a33fca4813bdf7d2d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.9 MB (190942252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f122b8e5228cd96ffca98393189ec6c109770f49b78bb9c5b2071a1c67d9bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 24 Jan 2022 23:19:42 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 24 Jan 2022 23:19:42 GMT
ENV ARANGO_VERSION=3.8.5
# Mon, 24 Jan 2022 23:19:42 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Mon, 24 Jan 2022 23:19:43 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.5-1_amd64.deb
# Mon, 24 Jan 2022 23:19:43 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.5-1_amd64.deb
# Mon, 24 Jan 2022 23:19:43 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.5-1_amd64.deb.asc
# Mon, 24 Jan 2022 23:20:14 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 24 Jan 2022 23:20:16 GMT
ENV GLIBCXX_FORCE_NEW=1
# Mon, 24 Jan 2022 23:20:16 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 24 Jan 2022 23:20:16 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Mon, 24 Jan 2022 23:20:16 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Mon, 24 Jan 2022 23:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Jan 2022 23:20:17 GMT
EXPOSE 8529
# Mon, 24 Jan 2022 23:20:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ed1a596e4434531e6c22f3365699ef06a41bd12826223952ed10a50d391c8a`  
		Last Modified: Mon, 24 Jan 2022 23:20:58 GMT  
		Size: 188.1 MB (188116923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd156c42d695e883867b79fd93c87ff5c9b09e71d74b5cff967e396d642cf40`  
		Last Modified: Mon, 24 Jan 2022 23:20:38 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3688f86f7a379ca4f05a1c6ea9791f7fb55d6973a131eddeddf683c2a8bf5714`  
		Last Modified: Mon, 24 Jan 2022 23:20:38 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:29961aed4abbd3e59058ab67500113451f12dea6f6ca8f09433adf625c289e39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:b740f7c169c3894f7e56e56ac26fb5c79936eaabd03758a33fca4813bdf7d2d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.9 MB (190942252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f122b8e5228cd96ffca98393189ec6c109770f49b78bb9c5b2071a1c67d9bb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 24 Jan 2022 23:19:42 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 24 Jan 2022 23:19:42 GMT
ENV ARANGO_VERSION=3.8.5
# Mon, 24 Jan 2022 23:19:42 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Mon, 24 Jan 2022 23:19:43 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.5-1_amd64.deb
# Mon, 24 Jan 2022 23:19:43 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.5-1_amd64.deb
# Mon, 24 Jan 2022 23:19:43 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.5-1_amd64.deb.asc
# Mon, 24 Jan 2022 23:20:14 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 24 Jan 2022 23:20:16 GMT
ENV GLIBCXX_FORCE_NEW=1
# Mon, 24 Jan 2022 23:20:16 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 24 Jan 2022 23:20:16 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Mon, 24 Jan 2022 23:20:16 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Mon, 24 Jan 2022 23:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Jan 2022 23:20:17 GMT
EXPOSE 8529
# Mon, 24 Jan 2022 23:20:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ed1a596e4434531e6c22f3365699ef06a41bd12826223952ed10a50d391c8a`  
		Last Modified: Mon, 24 Jan 2022 23:20:58 GMT  
		Size: 188.1 MB (188116923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd156c42d695e883867b79fd93c87ff5c9b09e71d74b5cff967e396d642cf40`  
		Last Modified: Mon, 24 Jan 2022 23:20:38 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3688f86f7a379ca4f05a1c6ea9791f7fb55d6973a131eddeddf683c2a8bf5714`  
		Last Modified: Mon, 24 Jan 2022 23:20:38 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
