<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.12`](#arangodb3612)
-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.9`](#arangodb379)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.6`

```console
$ docker pull arangodb@sha256:53454c2527923ba5ca9d7861455d48599ec26a34d4933b152dbee94ed9eadcc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:860138949f4c55dbc83f39f703d65de22353af4fae57fce47ed84d920470bf4b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119355383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:346a758cf6ae2ea64f453f7e070afac5271736cc8e5d6770b0d1e607da30616a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 20:36:06 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 26 Feb 2021 01:19:35 GMT
ENV ARANGO_VERSION=3.6.12
# Fri, 26 Feb 2021 01:19:35 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Fri, 26 Feb 2021 01:19:35 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.12-1_amd64.deb
# Fri, 26 Feb 2021 01:19:35 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.12-1_amd64.deb
# Fri, 26 Feb 2021 01:19:35 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.12-1_amd64.deb.asc
# Fri, 26 Feb 2021 01:20:01 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 26 Feb 2021 01:20:02 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 26 Feb 2021 01:20:02 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 26 Feb 2021 01:20:03 GMT
COPY file:0906ed6b024317ae8adc7caf5905c27c8ed6d7c227bbbfd131411e3fb9a6beaa in /entrypoint.sh 
# Fri, 26 Feb 2021 01:20:03 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 26 Feb 2021 01:20:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Feb 2021 01:20:03 GMT
EXPOSE 8529
# Fri, 26 Feb 2021 01:20:03 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74e90f9e13acb623f875268f359c73d035df0eea870eda4b52c279b5b9e304d`  
		Last Modified: Fri, 26 Feb 2021 01:20:40 GMT  
		Size: 116.5 MB (116537632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622728f67fe9d20e2c4fb29903330fadb5eed8ef3f91ce1dff5d830358f8281c`  
		Last Modified: Fri, 26 Feb 2021 01:20:21 GMT  
		Size: 2.2 KB (2176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3cea913d9ca137322903ffde8a404c0e811f7e01febf274181bcc8474fabec`  
		Last Modified: Fri, 26 Feb 2021 01:20:22 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.12`

```console
$ docker pull arangodb@sha256:53454c2527923ba5ca9d7861455d48599ec26a34d4933b152dbee94ed9eadcc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6.12` - linux; amd64

```console
$ docker pull arangodb@sha256:860138949f4c55dbc83f39f703d65de22353af4fae57fce47ed84d920470bf4b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119355383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:346a758cf6ae2ea64f453f7e070afac5271736cc8e5d6770b0d1e607da30616a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 20:36:06 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 26 Feb 2021 01:19:35 GMT
ENV ARANGO_VERSION=3.6.12
# Fri, 26 Feb 2021 01:19:35 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Fri, 26 Feb 2021 01:19:35 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.12-1_amd64.deb
# Fri, 26 Feb 2021 01:19:35 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.12-1_amd64.deb
# Fri, 26 Feb 2021 01:19:35 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.12-1_amd64.deb.asc
# Fri, 26 Feb 2021 01:20:01 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 26 Feb 2021 01:20:02 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 26 Feb 2021 01:20:02 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 26 Feb 2021 01:20:03 GMT
COPY file:0906ed6b024317ae8adc7caf5905c27c8ed6d7c227bbbfd131411e3fb9a6beaa in /entrypoint.sh 
# Fri, 26 Feb 2021 01:20:03 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 26 Feb 2021 01:20:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Feb 2021 01:20:03 GMT
EXPOSE 8529
# Fri, 26 Feb 2021 01:20:03 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74e90f9e13acb623f875268f359c73d035df0eea870eda4b52c279b5b9e304d`  
		Last Modified: Fri, 26 Feb 2021 01:20:40 GMT  
		Size: 116.5 MB (116537632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622728f67fe9d20e2c4fb29903330fadb5eed8ef3f91ce1dff5d830358f8281c`  
		Last Modified: Fri, 26 Feb 2021 01:20:21 GMT  
		Size: 2.2 KB (2176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3cea913d9ca137322903ffde8a404c0e811f7e01febf274181bcc8474fabec`  
		Last Modified: Fri, 26 Feb 2021 01:20:22 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7`

```console
$ docker pull arangodb@sha256:0c723b690261d331ef9aa307be4c046f35ec671c5f63a6d101acb30734f54463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.7` - linux; amd64

```console
$ docker pull arangodb@sha256:43f86488880c5df118545a262cb0174b2bd06ee1abb78e8e76b7be75b721af29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128152418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a2c07a33395c180d500c2dee5629bcff8bfe35736d7daf69e18a54c3deca2a8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 20:36:06 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 24 Feb 2021 20:36:41 GMT
ENV ARANGO_VERSION=3.7.8
# Wed, 24 Feb 2021 20:36:41 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Wed, 24 Feb 2021 20:36:41 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.8-1_amd64.deb
# Wed, 24 Feb 2021 20:36:41 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.8-1_amd64.deb
# Wed, 24 Feb 2021 20:36:42 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.8-1_amd64.deb.asc
# Wed, 24 Feb 2021 20:37:09 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 24 Feb 2021 20:37:09 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 24 Feb 2021 20:37:10 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 24 Feb 2021 20:37:10 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 24 Feb 2021 20:37:10 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 24 Feb 2021 20:37:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 20:37:10 GMT
EXPOSE 8529
# Wed, 24 Feb 2021 20:37:11 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af0a15c1eae3074fca33dce943301ba04f649d8b938794ac946f3bf18f9048e`  
		Last Modified: Wed, 24 Feb 2021 20:38:10 GMT  
		Size: 125.3 MB (125334758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49236682e8db8727d481a5f618f351b0e3eb979620284f047b1b85fb19090c5`  
		Last Modified: Wed, 24 Feb 2021 20:37:49 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3b8a72fc08b3b6d9af5ef040a77deb3d43d1bdba6a8e8ec90630796adb6fd1`  
		Last Modified: Wed, 24 Feb 2021 20:37:49 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7.9`

```console
$ docker pull arangodb@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:0c723b690261d331ef9aa307be4c046f35ec671c5f63a6d101acb30734f54463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:43f86488880c5df118545a262cb0174b2bd06ee1abb78e8e76b7be75b721af29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128152418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a2c07a33395c180d500c2dee5629bcff8bfe35736d7daf69e18a54c3deca2a8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 20:36:06 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 24 Feb 2021 20:36:41 GMT
ENV ARANGO_VERSION=3.7.8
# Wed, 24 Feb 2021 20:36:41 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Wed, 24 Feb 2021 20:36:41 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.8-1_amd64.deb
# Wed, 24 Feb 2021 20:36:41 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.8-1_amd64.deb
# Wed, 24 Feb 2021 20:36:42 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.8-1_amd64.deb.asc
# Wed, 24 Feb 2021 20:37:09 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 24 Feb 2021 20:37:09 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 24 Feb 2021 20:37:10 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 24 Feb 2021 20:37:10 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 24 Feb 2021 20:37:10 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 24 Feb 2021 20:37:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Feb 2021 20:37:10 GMT
EXPOSE 8529
# Wed, 24 Feb 2021 20:37:11 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af0a15c1eae3074fca33dce943301ba04f649d8b938794ac946f3bf18f9048e`  
		Last Modified: Wed, 24 Feb 2021 20:38:10 GMT  
		Size: 125.3 MB (125334758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49236682e8db8727d481a5f618f351b0e3eb979620284f047b1b85fb19090c5`  
		Last Modified: Wed, 24 Feb 2021 20:37:49 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3b8a72fc08b3b6d9af5ef040a77deb3d43d1bdba6a8e8ec90630796adb6fd1`  
		Last Modified: Wed, 24 Feb 2021 20:37:49 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
