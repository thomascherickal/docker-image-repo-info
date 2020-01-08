<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:2.8`](#arangodb28)
-	[`arangodb:2.8.11`](#arangodb2811)
-	[`arangodb:3.2`](#arangodb32)
-	[`arangodb:3.2.17`](#arangodb3217)
-	[`arangodb:3.3`](#arangodb33)
-	[`arangodb:3.3.23`](#arangodb3323)
-	[`arangodb:3.4`](#arangodb34)
-	[`arangodb:3.4.8`](#arangodb348)
-	[`arangodb:3.5`](#arangodb35)
-	[`arangodb:3.5.3`](#arangodb353)
-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.0`](#arangodb360)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:2.8`

```console
$ docker pull arangodb@sha256:e1c88170b700d5d74116956e12b9002147d37bd97eabaa58064504ca021890b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:2.8` - linux; amd64

```console
$ docker pull arangodb@sha256:5fb9b9f4cbfa5fe0120b0f5ff26fe5644a1973ca50392ec34e49ebfe54cefcc7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115104663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc58e81270de0a8f7dccfa580b17435ccdcd54227d5c75ef8d17cc3c81be9dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:35 GMT
ADD file:6bea7fdf1d11cd3f2dfa923395205f70d42d388f597b21e289e7f516a2c687f1 in / 
# Sat, 28 Dec 2019 04:21:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:08:18 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 28 Dec 2019 05:08:20 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Sat, 28 Dec 2019 05:08:20 GMT
ENV ARCHITECTURE=amd64
# Sat, 28 Dec 2019 05:08:21 GMT
ENV ARANGO_VERSION=2.8.11
# Sat, 28 Dec 2019 05:08:21 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb2/Debian_8.0
# Sat, 28 Dec 2019 05:08:21 GMT
ENV ARANGO_PACKAGE=arangodb_2.8.11_amd64.deb
# Sat, 28 Dec 2019 05:08:21 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb
# Sat, 28 Dec 2019 05:08:21 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb.asc
# Sat, 28 Dec 2019 05:10:43 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libgoogle-perftools4         ca-certificates         pwgen         wget     &&     rm -rf /var/lib/apt/lists/* &&     wget ${ARANGO_SIGNATURE_URL} &&           wget ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     dpkg -i ${ARANGO_PACKAGE} &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^#\s*uid\s*=.*!uid = arangodb!'         -e 's!^#\s*gid\s*=.*!gid = arangodb!'         /etc/arangodb/arangod.conf     &&     apt-get purge -y --auto-remove ca-certificates wget &&     rm -f ${ARANGO_PACKAGE}*
# Sat, 28 Dec 2019 05:10:44 GMT
RUN chown arangodb:arangodb /var/lib/arangodb &&   chown arangodb:arangodb /var/lib/arangodb-apps
# Sat, 28 Dec 2019 05:10:44 GMT
VOLUME [/var/lib/arangodb /var/lib/arangodb-apps]
# Sat, 28 Dec 2019 05:10:44 GMT
COPY file:9a5bd6b5ab4e3a7842ac5f3e59bb9907920e9e2dc31d297c3676110b569a9d7e in /entrypoint.sh 
# Sat, 28 Dec 2019 05:10:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 28 Dec 2019 05:10:45 GMT
EXPOSE 8529
# Sat, 28 Dec 2019 05:10:45 GMT
USER arangodb
# Sat, 28 Dec 2019 05:10:45 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:a4888a2f4fb02c1971555f590f5c9ef6369e7fa4599e586fb70cdfe80330370b`  
		Last Modified: Sat, 28 Dec 2019 04:26:07 GMT  
		Size: 54.4 MB (54389662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928c34f3b89f675ed95f3388a5a183daab18a88610ea4441e2c25d1f9cb51e56`  
		Last Modified: Sat, 28 Dec 2019 05:12:48 GMT  
		Size: 8.6 KB (8594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6676c241b82c74278b2c0a5bc5e4b89678559abed3563998307118485c137445`  
		Last Modified: Sat, 28 Dec 2019 05:12:59 GMT  
		Size: 60.7 MB (60705146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a415eef62fb2ed136736f7d27e2f39bc0130651ffcf541db1e80b2c10750f62`  
		Last Modified: Sat, 28 Dec 2019 05:12:48 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df7b501101c91394cfde80a97137dce2fe5ad0275df3e03d5c4478ab6db7c9`  
		Last Modified: Sat, 28 Dec 2019 05:12:48 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:2.8.11`

```console
$ docker pull arangodb@sha256:e1c88170b700d5d74116956e12b9002147d37bd97eabaa58064504ca021890b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:2.8.11` - linux; amd64

```console
$ docker pull arangodb@sha256:5fb9b9f4cbfa5fe0120b0f5ff26fe5644a1973ca50392ec34e49ebfe54cefcc7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115104663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc58e81270de0a8f7dccfa580b17435ccdcd54227d5c75ef8d17cc3c81be9dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:35 GMT
ADD file:6bea7fdf1d11cd3f2dfa923395205f70d42d388f597b21e289e7f516a2c687f1 in / 
# Sat, 28 Dec 2019 04:21:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:08:18 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 28 Dec 2019 05:08:20 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Sat, 28 Dec 2019 05:08:20 GMT
ENV ARCHITECTURE=amd64
# Sat, 28 Dec 2019 05:08:21 GMT
ENV ARANGO_VERSION=2.8.11
# Sat, 28 Dec 2019 05:08:21 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb2/Debian_8.0
# Sat, 28 Dec 2019 05:08:21 GMT
ENV ARANGO_PACKAGE=arangodb_2.8.11_amd64.deb
# Sat, 28 Dec 2019 05:08:21 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb
# Sat, 28 Dec 2019 05:08:21 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb.asc
# Sat, 28 Dec 2019 05:10:43 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libgoogle-perftools4         ca-certificates         pwgen         wget     &&     rm -rf /var/lib/apt/lists/* &&     wget ${ARANGO_SIGNATURE_URL} &&           wget ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     dpkg -i ${ARANGO_PACKAGE} &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^#\s*uid\s*=.*!uid = arangodb!'         -e 's!^#\s*gid\s*=.*!gid = arangodb!'         /etc/arangodb/arangod.conf     &&     apt-get purge -y --auto-remove ca-certificates wget &&     rm -f ${ARANGO_PACKAGE}*
# Sat, 28 Dec 2019 05:10:44 GMT
RUN chown arangodb:arangodb /var/lib/arangodb &&   chown arangodb:arangodb /var/lib/arangodb-apps
# Sat, 28 Dec 2019 05:10:44 GMT
VOLUME [/var/lib/arangodb /var/lib/arangodb-apps]
# Sat, 28 Dec 2019 05:10:44 GMT
COPY file:9a5bd6b5ab4e3a7842ac5f3e59bb9907920e9e2dc31d297c3676110b569a9d7e in /entrypoint.sh 
# Sat, 28 Dec 2019 05:10:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 28 Dec 2019 05:10:45 GMT
EXPOSE 8529
# Sat, 28 Dec 2019 05:10:45 GMT
USER arangodb
# Sat, 28 Dec 2019 05:10:45 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:a4888a2f4fb02c1971555f590f5c9ef6369e7fa4599e586fb70cdfe80330370b`  
		Last Modified: Sat, 28 Dec 2019 04:26:07 GMT  
		Size: 54.4 MB (54389662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928c34f3b89f675ed95f3388a5a183daab18a88610ea4441e2c25d1f9cb51e56`  
		Last Modified: Sat, 28 Dec 2019 05:12:48 GMT  
		Size: 8.6 KB (8594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6676c241b82c74278b2c0a5bc5e4b89678559abed3563998307118485c137445`  
		Last Modified: Sat, 28 Dec 2019 05:12:59 GMT  
		Size: 60.7 MB (60705146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a415eef62fb2ed136736f7d27e2f39bc0130651ffcf541db1e80b2c10750f62`  
		Last Modified: Sat, 28 Dec 2019 05:12:48 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df7b501101c91394cfde80a97137dce2fe5ad0275df3e03d5c4478ab6db7c9`  
		Last Modified: Sat, 28 Dec 2019 05:12:48 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.2`

```console
$ docker pull arangodb@sha256:4032c5cff056be0a89d14db15df69390aa44f3f7599ff4a3bdc37a8d491f4563
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.2` - linux; amd64

```console
$ docker pull arangodb@sha256:057f3b1db2e552e23aba839ac532a5b289adbe19a0f2dc126e420bd329a28054
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113550740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742872477df9195e4c3d0b01bfd9604b309fcb12d61390d8fe72e753ced0e8aa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:11:02 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 28 Dec 2019 05:11:02 GMT
ENV ARCHITECTURE=amd64
# Sat, 28 Dec 2019 05:11:03 GMT
ENV DEB_PACKAGE_VERSION=1
# Sat, 28 Dec 2019 05:11:03 GMT
ENV ARANGO_VERSION=3.2.17
# Sat, 28 Dec 2019 05:11:03 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb32/Debian_9.0
# Sat, 28 Dec 2019 05:11:03 GMT
ENV ARANGO_PACKAGE=arangodb3-3.2.17-1_amd64.deb
# Sat, 28 Dec 2019 05:11:04 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb
# Sat, 28 Dec 2019 05:11:04 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb.asc
# Sat, 28 Dec 2019 05:11:10 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gpg dirmngr     &&     rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:11:17 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Sat, 28 Dec 2019 05:11:27 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libjemalloc1         ca-certificates         pwgen         curl         numactl     &&     rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:11:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 Dec 2019 05:11:42 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Sat, 28 Dec 2019 05:11:42 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 28 Dec 2019 05:11:42 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Sat, 28 Dec 2019 05:11:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 28 Dec 2019 05:11:43 GMT
EXPOSE 8529
# Sat, 28 Dec 2019 05:11:43 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c975fd667743955e2cf2a6cdf27555045ed81db9466082abccc639d52d01a4`  
		Last Modified: Sat, 28 Dec 2019 05:13:05 GMT  
		Size: 6.6 MB (6566470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fa06b212be9787f6dac9d29fffa37aa659bfca8189b640ead7d32756661d28`  
		Last Modified: Sat, 28 Dec 2019 05:13:03 GMT  
		Size: 4.4 KB (4444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d4d8fcd957a7bca81fb95b639b7ed84da276d32f800d47898442399dc41f31`  
		Last Modified: Sat, 28 Dec 2019 05:13:04 GMT  
		Size: 7.5 MB (7461274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd77648f1bb7aa2099b5254f5f67d6b27881fa454d58e0a3ebdfaebcbc369328`  
		Last Modified: Sat, 28 Dec 2019 05:13:03 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7a811039e2f12daab7c2dadf442ed17b7985909b7180b2160955615f4c9dc1`  
		Last Modified: Sat, 28 Dec 2019 05:13:14 GMT  
		Size: 54.1 MB (54135655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaeb8cf29e2af2289e2f3baa7c31eee4e24c2d762d9484b01d45fa1e9424f19f`  
		Last Modified: Sat, 28 Dec 2019 05:13:03 GMT  
		Size: 2.0 KB (2038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.2.17`

```console
$ docker pull arangodb@sha256:4032c5cff056be0a89d14db15df69390aa44f3f7599ff4a3bdc37a8d491f4563
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.2.17` - linux; amd64

```console
$ docker pull arangodb@sha256:057f3b1db2e552e23aba839ac532a5b289adbe19a0f2dc126e420bd329a28054
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113550740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742872477df9195e4c3d0b01bfd9604b309fcb12d61390d8fe72e753ced0e8aa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:11:02 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 28 Dec 2019 05:11:02 GMT
ENV ARCHITECTURE=amd64
# Sat, 28 Dec 2019 05:11:03 GMT
ENV DEB_PACKAGE_VERSION=1
# Sat, 28 Dec 2019 05:11:03 GMT
ENV ARANGO_VERSION=3.2.17
# Sat, 28 Dec 2019 05:11:03 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb32/Debian_9.0
# Sat, 28 Dec 2019 05:11:03 GMT
ENV ARANGO_PACKAGE=arangodb3-3.2.17-1_amd64.deb
# Sat, 28 Dec 2019 05:11:04 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb
# Sat, 28 Dec 2019 05:11:04 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb.asc
# Sat, 28 Dec 2019 05:11:10 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gpg dirmngr     &&     rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:11:17 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Sat, 28 Dec 2019 05:11:27 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libjemalloc1         ca-certificates         pwgen         curl         numactl     &&     rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:11:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 Dec 2019 05:11:42 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Sat, 28 Dec 2019 05:11:42 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 28 Dec 2019 05:11:42 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Sat, 28 Dec 2019 05:11:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 28 Dec 2019 05:11:43 GMT
EXPOSE 8529
# Sat, 28 Dec 2019 05:11:43 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c975fd667743955e2cf2a6cdf27555045ed81db9466082abccc639d52d01a4`  
		Last Modified: Sat, 28 Dec 2019 05:13:05 GMT  
		Size: 6.6 MB (6566470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fa06b212be9787f6dac9d29fffa37aa659bfca8189b640ead7d32756661d28`  
		Last Modified: Sat, 28 Dec 2019 05:13:03 GMT  
		Size: 4.4 KB (4444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d4d8fcd957a7bca81fb95b639b7ed84da276d32f800d47898442399dc41f31`  
		Last Modified: Sat, 28 Dec 2019 05:13:04 GMT  
		Size: 7.5 MB (7461274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd77648f1bb7aa2099b5254f5f67d6b27881fa454d58e0a3ebdfaebcbc369328`  
		Last Modified: Sat, 28 Dec 2019 05:13:03 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7a811039e2f12daab7c2dadf442ed17b7985909b7180b2160955615f4c9dc1`  
		Last Modified: Sat, 28 Dec 2019 05:13:14 GMT  
		Size: 54.1 MB (54135655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaeb8cf29e2af2289e2f3baa7c31eee4e24c2d762d9484b01d45fa1e9424f19f`  
		Last Modified: Sat, 28 Dec 2019 05:13:03 GMT  
		Size: 2.0 KB (2038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.3`

```console
$ docker pull arangodb@sha256:9943cea089b59eea4fd25b6468824c657d1d2e6a567a327fd1c37a77ff45fe41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.3` - linux; amd64

```console
$ docker pull arangodb@sha256:0653d271817c083d5310b00eb33d46f47ba63cfd4ad9e58a81a9eb0e736f72fe
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114315392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a5b7663fcacb51e134c516012ed86cd5a41f714123d7d3a9376b72587e8dc9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:11:02 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 28 Dec 2019 05:11:02 GMT
ENV ARCHITECTURE=amd64
# Sat, 28 Dec 2019 05:11:03 GMT
ENV DEB_PACKAGE_VERSION=1
# Sat, 28 Dec 2019 05:11:48 GMT
ENV ARANGO_VERSION=3.3.23
# Sat, 28 Dec 2019 05:11:48 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb33/Debian_9.0
# Sat, 28 Dec 2019 05:11:48 GMT
ENV ARANGO_PACKAGE=arangodb3-3.3.23-1_amd64.deb
# Sat, 28 Dec 2019 05:11:48 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.23-1_amd64.deb
# Sat, 28 Dec 2019 05:11:48 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.23-1_amd64.deb.asc
# Sat, 28 Dec 2019 05:11:54 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         dirmngr         gpg     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:12:04 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Sat, 28 Dec 2019 05:12:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         curl         libjemalloc1         libtasn1-6         numactl         openssl         pwgen         sensible-utils     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:12:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 Dec 2019 05:12:29 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Sat, 28 Dec 2019 05:12:30 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 28 Dec 2019 05:12:30 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Sat, 28 Dec 2019 05:12:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 28 Dec 2019 05:12:30 GMT
EXPOSE 8529
# Sat, 28 Dec 2019 05:12:31 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ea704adb0c2623badb769235d3c24a33f07f4a9c99b2eba7b08272fce5b256`  
		Last Modified: Sat, 28 Dec 2019 05:13:20 GMT  
		Size: 6.6 MB (6566465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047359938697d5b99465183296707f060b17b7dd9dd35c56eccd3a66e4e5dc6`  
		Last Modified: Sat, 28 Dec 2019 05:13:18 GMT  
		Size: 4.4 KB (4447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1985023342f778a18e2e6c21d9be04973132a2454b836d663843c6d48b64c05`  
		Last Modified: Sat, 28 Dec 2019 05:13:20 GMT  
		Size: 7.5 MB (7461262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037c893674219bbc3ef69f2432cf7acf4014846a92559b8a748404ce707c45fb`  
		Last Modified: Sat, 28 Dec 2019 05:13:18 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43053ced8451c90b285d6ef70c22baa44d51f896cadf7bbaf4053fd51e6d4141`  
		Last Modified: Sat, 28 Dec 2019 05:13:28 GMT  
		Size: 54.9 MB (54900322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef3847cdb5216470b8883637519e95180ea65f0d9cc56ebd110d32856ce1d33`  
		Last Modified: Sat, 28 Dec 2019 05:13:18 GMT  
		Size: 2.0 KB (2037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.3.23`

```console
$ docker pull arangodb@sha256:9943cea089b59eea4fd25b6468824c657d1d2e6a567a327fd1c37a77ff45fe41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.3.23` - linux; amd64

```console
$ docker pull arangodb@sha256:0653d271817c083d5310b00eb33d46f47ba63cfd4ad9e58a81a9eb0e736f72fe
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114315392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a5b7663fcacb51e134c516012ed86cd5a41f714123d7d3a9376b72587e8dc9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:11:02 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 28 Dec 2019 05:11:02 GMT
ENV ARCHITECTURE=amd64
# Sat, 28 Dec 2019 05:11:03 GMT
ENV DEB_PACKAGE_VERSION=1
# Sat, 28 Dec 2019 05:11:48 GMT
ENV ARANGO_VERSION=3.3.23
# Sat, 28 Dec 2019 05:11:48 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb33/Debian_9.0
# Sat, 28 Dec 2019 05:11:48 GMT
ENV ARANGO_PACKAGE=arangodb3-3.3.23-1_amd64.deb
# Sat, 28 Dec 2019 05:11:48 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.23-1_amd64.deb
# Sat, 28 Dec 2019 05:11:48 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.23-1_amd64.deb.asc
# Sat, 28 Dec 2019 05:11:54 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         dirmngr         gpg     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:12:04 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Sat, 28 Dec 2019 05:12:14 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         curl         libjemalloc1         libtasn1-6         numactl         openssl         pwgen         sensible-utils     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:12:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 Dec 2019 05:12:29 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Sat, 28 Dec 2019 05:12:30 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 28 Dec 2019 05:12:30 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Sat, 28 Dec 2019 05:12:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 28 Dec 2019 05:12:30 GMT
EXPOSE 8529
# Sat, 28 Dec 2019 05:12:31 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ea704adb0c2623badb769235d3c24a33f07f4a9c99b2eba7b08272fce5b256`  
		Last Modified: Sat, 28 Dec 2019 05:13:20 GMT  
		Size: 6.6 MB (6566465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047359938697d5b99465183296707f060b17b7dd9dd35c56eccd3a66e4e5dc6`  
		Last Modified: Sat, 28 Dec 2019 05:13:18 GMT  
		Size: 4.4 KB (4447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1985023342f778a18e2e6c21d9be04973132a2454b836d663843c6d48b64c05`  
		Last Modified: Sat, 28 Dec 2019 05:13:20 GMT  
		Size: 7.5 MB (7461262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037c893674219bbc3ef69f2432cf7acf4014846a92559b8a748404ce707c45fb`  
		Last Modified: Sat, 28 Dec 2019 05:13:18 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43053ced8451c90b285d6ef70c22baa44d51f896cadf7bbaf4053fd51e6d4141`  
		Last Modified: Sat, 28 Dec 2019 05:13:28 GMT  
		Size: 54.9 MB (54900322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef3847cdb5216470b8883637519e95180ea65f0d9cc56ebd110d32856ce1d33`  
		Last Modified: Sat, 28 Dec 2019 05:13:18 GMT  
		Size: 2.0 KB (2037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.4`

```console
$ docker pull arangodb@sha256:17d89ad3423e070844191fb0f0388c5833c5147aa6a80bc52f0fc7b34e8e2bac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.4` - linux; amd64

```console
$ docker pull arangodb@sha256:30259be84302e401cf3ebd1ad66df79c05f706ea10e298735c5c195f95201fb9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101733479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b74e41eea3641fe4082736c5a059463672c286649055b706f74df8f810183060`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:01:24 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 21 Oct 2019 18:01:24 GMT
ENV ARANGO_VERSION=3.4.8
# Mon, 21 Oct 2019 18:01:25 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64
# Mon, 21 Oct 2019 18:01:25 GMT
ENV ARANGO_PACKAGE=arangodb3_3.4.8-1_amd64.deb
# Mon, 21 Oct 2019 18:01:25 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.8-1_amd64.deb
# Mon, 21 Oct 2019 18:01:25 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.8-1_amd64.deb.asc
# Mon, 21 Oct 2019 18:01:52 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 21 Oct 2019 18:01:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 21 Oct 2019 18:01:53 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Mon, 21 Oct 2019 18:01:54 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Mon, 21 Oct 2019 18:01:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 21 Oct 2019 18:01:54 GMT
EXPOSE 8529
# Mon, 21 Oct 2019 18:01:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048fad2f7dae6974f6ed8ca4ef47dd03f53266826d3afa526e188d7b53048a20`  
		Last Modified: Mon, 21 Oct 2019 18:03:27 GMT  
		Size: 98.9 MB (98943896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc32380755ab2a7146be142874b4e38039f5f15de25d046b4711eab65bb0b2e2`  
		Last Modified: Mon, 21 Oct 2019 18:03:09 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c173abd82ad56e2e7b790e77de6cf02b5f93c4fb6c34345711756c876c760b`  
		Last Modified: Mon, 21 Oct 2019 18:03:08 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.4.8`

```console
$ docker pull arangodb@sha256:17d89ad3423e070844191fb0f0388c5833c5147aa6a80bc52f0fc7b34e8e2bac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.4.8` - linux; amd64

```console
$ docker pull arangodb@sha256:30259be84302e401cf3ebd1ad66df79c05f706ea10e298735c5c195f95201fb9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101733479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b74e41eea3641fe4082736c5a059463672c286649055b706f74df8f810183060`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:01:24 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 21 Oct 2019 18:01:24 GMT
ENV ARANGO_VERSION=3.4.8
# Mon, 21 Oct 2019 18:01:25 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64
# Mon, 21 Oct 2019 18:01:25 GMT
ENV ARANGO_PACKAGE=arangodb3_3.4.8-1_amd64.deb
# Mon, 21 Oct 2019 18:01:25 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.8-1_amd64.deb
# Mon, 21 Oct 2019 18:01:25 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.8-1_amd64.deb.asc
# Mon, 21 Oct 2019 18:01:52 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 21 Oct 2019 18:01:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 21 Oct 2019 18:01:53 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Mon, 21 Oct 2019 18:01:54 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Mon, 21 Oct 2019 18:01:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 21 Oct 2019 18:01:54 GMT
EXPOSE 8529
# Mon, 21 Oct 2019 18:01:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048fad2f7dae6974f6ed8ca4ef47dd03f53266826d3afa526e188d7b53048a20`  
		Last Modified: Mon, 21 Oct 2019 18:03:27 GMT  
		Size: 98.9 MB (98943896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc32380755ab2a7146be142874b4e38039f5f15de25d046b4711eab65bb0b2e2`  
		Last Modified: Mon, 21 Oct 2019 18:03:09 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c173abd82ad56e2e7b790e77de6cf02b5f93c4fb6c34345711756c876c760b`  
		Last Modified: Mon, 21 Oct 2019 18:03:08 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.5`

```console
$ docker pull arangodb@sha256:a0f91d8c6c19ba53b4c9975086fd6a94dadc76f048c070d79014b41981af57dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5` - linux; amd64

```console
$ docker pull arangodb@sha256:f2edf003e179b9b347364e3dc17fe6d1b67fac0878cabd2356a5416d80eeff80
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110386860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c5d2a85e2c1a2e508caca44dec9eef2e56659141df0ae7a2e88871bb6a7b82e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:01:24 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_VERSION=3.5.3
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.3-1_amd64.deb
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.3-1_amd64.deb
# Mon, 02 Dec 2019 21:22:48 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.3-1_amd64.deb.asc
# Mon, 02 Dec 2019 21:23:15 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 02 Dec 2019 21:23:15 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 02 Dec 2019 21:23:15 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Mon, 02 Dec 2019 21:23:15 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Mon, 02 Dec 2019 21:23:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 02 Dec 2019 21:23:16 GMT
EXPOSE 8529
# Mon, 02 Dec 2019 21:23:16 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772932e707dd283f507304182f6e0e096cb3eab33adac426e7071167ec313bdd`  
		Last Modified: Mon, 02 Dec 2019 21:23:58 GMT  
		Size: 107.6 MB (107597278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e295ecba915b8ea4e8e1927790578ed2ad9001680d9c9fb9f876b207c072d`  
		Last Modified: Mon, 02 Dec 2019 21:23:39 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248fa831e65eda3a54cd43b947df9844ff5e949ad99063233ab159d56c12d14a`  
		Last Modified: Mon, 02 Dec 2019 21:23:39 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.5.3`

```console
$ docker pull arangodb@sha256:a0f91d8c6c19ba53b4c9975086fd6a94dadc76f048c070d79014b41981af57dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5.3` - linux; amd64

```console
$ docker pull arangodb@sha256:f2edf003e179b9b347364e3dc17fe6d1b67fac0878cabd2356a5416d80eeff80
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110386860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c5d2a85e2c1a2e508caca44dec9eef2e56659141df0ae7a2e88871bb6a7b82e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:01:24 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_VERSION=3.5.3
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.3-1_amd64.deb
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.3-1_amd64.deb
# Mon, 02 Dec 2019 21:22:48 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.3-1_amd64.deb.asc
# Mon, 02 Dec 2019 21:23:15 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 02 Dec 2019 21:23:15 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 02 Dec 2019 21:23:15 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Mon, 02 Dec 2019 21:23:15 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Mon, 02 Dec 2019 21:23:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 02 Dec 2019 21:23:16 GMT
EXPOSE 8529
# Mon, 02 Dec 2019 21:23:16 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772932e707dd283f507304182f6e0e096cb3eab33adac426e7071167ec313bdd`  
		Last Modified: Mon, 02 Dec 2019 21:23:58 GMT  
		Size: 107.6 MB (107597278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e295ecba915b8ea4e8e1927790578ed2ad9001680d9c9fb9f876b207c072d`  
		Last Modified: Mon, 02 Dec 2019 21:23:39 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248fa831e65eda3a54cd43b947df9844ff5e949ad99063233ab159d56c12d14a`  
		Last Modified: Mon, 02 Dec 2019 21:23:39 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6`

**does not exist** (yet?)

## `arangodb:3.6.0`

**does not exist** (yet?)

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:a0f91d8c6c19ba53b4c9975086fd6a94dadc76f048c070d79014b41981af57dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:f2edf003e179b9b347364e3dc17fe6d1b67fac0878cabd2356a5416d80eeff80
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110386860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c5d2a85e2c1a2e508caca44dec9eef2e56659141df0ae7a2e88871bb6a7b82e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:01:24 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_VERSION=3.5.3
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.3-1_amd64.deb
# Mon, 02 Dec 2019 21:22:47 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.3-1_amd64.deb
# Mon, 02 Dec 2019 21:22:48 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.3-1_amd64.deb.asc
# Mon, 02 Dec 2019 21:23:15 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 02 Dec 2019 21:23:15 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 02 Dec 2019 21:23:15 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Mon, 02 Dec 2019 21:23:15 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Mon, 02 Dec 2019 21:23:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 02 Dec 2019 21:23:16 GMT
EXPOSE 8529
# Mon, 02 Dec 2019 21:23:16 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772932e707dd283f507304182f6e0e096cb3eab33adac426e7071167ec313bdd`  
		Last Modified: Mon, 02 Dec 2019 21:23:58 GMT  
		Size: 107.6 MB (107597278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e295ecba915b8ea4e8e1927790578ed2ad9001680d9c9fb9f876b207c072d`  
		Last Modified: Mon, 02 Dec 2019 21:23:39 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248fa831e65eda3a54cd43b947df9844ff5e949ad99063233ab159d56c12d14a`  
		Last Modified: Mon, 02 Dec 2019 21:23:39 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
