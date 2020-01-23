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
-	[`arangodb:3.5.4`](#arangodb354)
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
$ docker pull arangodb@sha256:79384c203248e069d02f18c0a784e2cb5f35dfc562ed88c7ef34bcb1292b98f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.4` - linux; amd64

```console
$ docker pull arangodb@sha256:0160c08cbf8605318d0342484ea27bd76106595583de77e1c633c53e3d25813a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101850160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35744afa825a591becce5e0bb1902cb5a813d0c75b88561822a2d28845646dc7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 23 Jan 2020 17:09:20 GMT
ENV ARANGO_VERSION=3.4.8
# Thu, 23 Jan 2020 17:09:20 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64
# Thu, 23 Jan 2020 17:09:20 GMT
ENV ARANGO_PACKAGE=arangodb3_3.4.8-1_amd64.deb
# Thu, 23 Jan 2020 17:09:21 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.8-1_amd64.deb
# Thu, 23 Jan 2020 17:09:21 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.8-1_amd64.deb.asc
# Thu, 23 Jan 2020 17:09:47 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 23 Jan 2020 17:09:48 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 23 Jan 2020 17:09:48 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 23 Jan 2020 17:09:48 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 23 Jan 2020 17:09:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 17:09:49 GMT
EXPOSE 8529
# Thu, 23 Jan 2020 17:09:49 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c070f9c0a01fb65ce7a7a779d5d2a5630dc1a93fe93d2a8d3a5892c9b2919c82`  
		Last Modified: Thu, 23 Jan 2020 17:11:24 GMT  
		Size: 99.1 MB (99060754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023ecfc5435b9825f17fc58439a14edcba8479de5e536e55616b04e1c783ce47`  
		Last Modified: Thu, 23 Jan 2020 17:11:05 GMT  
		Size: 2.2 KB (2202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f846e9b2d2527d1d6f48b1ed60da16c21af491291ded45b30d12a5a08c87b`  
		Last Modified: Thu, 23 Jan 2020 17:11:05 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.4.8`

```console
$ docker pull arangodb@sha256:79384c203248e069d02f18c0a784e2cb5f35dfc562ed88c7ef34bcb1292b98f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.4.8` - linux; amd64

```console
$ docker pull arangodb@sha256:0160c08cbf8605318d0342484ea27bd76106595583de77e1c633c53e3d25813a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101850160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35744afa825a591becce5e0bb1902cb5a813d0c75b88561822a2d28845646dc7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 23 Jan 2020 17:09:20 GMT
ENV ARANGO_VERSION=3.4.8
# Thu, 23 Jan 2020 17:09:20 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64
# Thu, 23 Jan 2020 17:09:20 GMT
ENV ARANGO_PACKAGE=arangodb3_3.4.8-1_amd64.deb
# Thu, 23 Jan 2020 17:09:21 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.8-1_amd64.deb
# Thu, 23 Jan 2020 17:09:21 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.8-1_amd64.deb.asc
# Thu, 23 Jan 2020 17:09:47 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 23 Jan 2020 17:09:48 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 23 Jan 2020 17:09:48 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 23 Jan 2020 17:09:48 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 23 Jan 2020 17:09:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 17:09:49 GMT
EXPOSE 8529
# Thu, 23 Jan 2020 17:09:49 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c070f9c0a01fb65ce7a7a779d5d2a5630dc1a93fe93d2a8d3a5892c9b2919c82`  
		Last Modified: Thu, 23 Jan 2020 17:11:24 GMT  
		Size: 99.1 MB (99060754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023ecfc5435b9825f17fc58439a14edcba8479de5e536e55616b04e1c783ce47`  
		Last Modified: Thu, 23 Jan 2020 17:11:05 GMT  
		Size: 2.2 KB (2202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113f846e9b2d2527d1d6f48b1ed60da16c21af491291ded45b30d12a5a08c87b`  
		Last Modified: Thu, 23 Jan 2020 17:11:05 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.5`

```console
$ docker pull arangodb@sha256:b935728c194b217f0e7a1cb91fd35d7d638034394d2a683879a2cf0a67c7e68c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5` - linux; amd64

```console
$ docker pull arangodb@sha256:62b5c1907ccfa74533c35e299f4e868f87d2efbf2a0761f8dfc7af99e14520e6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110503803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:044bb2b6b89c3b4d8bfe2a489ed097fcf0c6a5729dc26a2fdc97e435be972cff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 23 Jan 2020 17:09:53 GMT
ENV ARANGO_VERSION=3.5.4
# Thu, 23 Jan 2020 17:09:53 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Thu, 23 Jan 2020 17:09:53 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.4-1_amd64.deb
# Thu, 23 Jan 2020 17:09:53 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.4-1_amd64.deb
# Thu, 23 Jan 2020 17:09:53 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.4-1_amd64.deb.asc
# Thu, 23 Jan 2020 17:10:18 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 23 Jan 2020 17:10:19 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 23 Jan 2020 17:10:19 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 23 Jan 2020 17:10:19 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 23 Jan 2020 17:10:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:19 GMT
EXPOSE 8529
# Thu, 23 Jan 2020 17:10:19 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b894beb4738887c1152b7d7f1549123f4b522147acd9c92006b54013e40134`  
		Last Modified: Thu, 23 Jan 2020 17:11:48 GMT  
		Size: 107.7 MB (107714396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36e3ba3ee3abb406b1eb2d88f2e4f920861b71d868af63b966e113f57b22c5b`  
		Last Modified: Thu, 23 Jan 2020 17:11:29 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded7a88e79982f58478fb0b3dddd36d284712c45855b584ed2a356730b471f91`  
		Last Modified: Thu, 23 Jan 2020 17:11:30 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.5.4`

```console
$ docker pull arangodb@sha256:b935728c194b217f0e7a1cb91fd35d7d638034394d2a683879a2cf0a67c7e68c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5.4` - linux; amd64

```console
$ docker pull arangodb@sha256:62b5c1907ccfa74533c35e299f4e868f87d2efbf2a0761f8dfc7af99e14520e6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110503803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:044bb2b6b89c3b4d8bfe2a489ed097fcf0c6a5729dc26a2fdc97e435be972cff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 23 Jan 2020 17:09:53 GMT
ENV ARANGO_VERSION=3.5.4
# Thu, 23 Jan 2020 17:09:53 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Thu, 23 Jan 2020 17:09:53 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.4-1_amd64.deb
# Thu, 23 Jan 2020 17:09:53 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.4-1_amd64.deb
# Thu, 23 Jan 2020 17:09:53 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.4-1_amd64.deb.asc
# Thu, 23 Jan 2020 17:10:18 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 23 Jan 2020 17:10:19 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 23 Jan 2020 17:10:19 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 23 Jan 2020 17:10:19 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 23 Jan 2020 17:10:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:19 GMT
EXPOSE 8529
# Thu, 23 Jan 2020 17:10:19 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b894beb4738887c1152b7d7f1549123f4b522147acd9c92006b54013e40134`  
		Last Modified: Thu, 23 Jan 2020 17:11:48 GMT  
		Size: 107.7 MB (107714396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36e3ba3ee3abb406b1eb2d88f2e4f920861b71d868af63b966e113f57b22c5b`  
		Last Modified: Thu, 23 Jan 2020 17:11:29 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded7a88e79982f58478fb0b3dddd36d284712c45855b584ed2a356730b471f91`  
		Last Modified: Thu, 23 Jan 2020 17:11:30 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6`

```console
$ docker pull arangodb@sha256:e3d2347035f51108ac2936061c5adb606e36851e7766ab50e2f2a3af5ca385b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:abe5f2131c7ed7da408f6902ce7b78a071b4618dea59838e4ea2635037d13429
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110339990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:421ac5cc2f1194149caaa7c0b8cee65da5ccf6062359df943e17d186d697ec1e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_VERSION=3.6.0
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.0-1_amd64.deb
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.0-1_amd64.deb
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.0-1_amd64.deb.asc
# Thu, 23 Jan 2020 17:10:50 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 23 Jan 2020 17:10:51 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 23 Jan 2020 17:10:51 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 23 Jan 2020 17:10:51 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 23 Jan 2020 17:10:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:52 GMT
EXPOSE 8529
# Thu, 23 Jan 2020 17:10:52 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca8484f7a3f17d860ce5f010964ed46b6013cfb493c34eb7ae483a196a65959`  
		Last Modified: Thu, 23 Jan 2020 17:13:37 GMT  
		Size: 107.6 MB (107550582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe1725aa97b4d35497e7d72b01d698a1ed8a20495067cb17739dbcabb8b7356`  
		Last Modified: Thu, 23 Jan 2020 17:11:53 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93789dbf5792d29eacfd353299490543f678dcd2288008b707a0833d5c9cc1b2`  
		Last Modified: Thu, 23 Jan 2020 17:11:52 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.0`

```console
$ docker pull arangodb@sha256:e3d2347035f51108ac2936061c5adb606e36851e7766ab50e2f2a3af5ca385b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6.0` - linux; amd64

```console
$ docker pull arangodb@sha256:abe5f2131c7ed7da408f6902ce7b78a071b4618dea59838e4ea2635037d13429
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110339990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:421ac5cc2f1194149caaa7c0b8cee65da5ccf6062359df943e17d186d697ec1e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_VERSION=3.6.0
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.0-1_amd64.deb
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.0-1_amd64.deb
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.0-1_amd64.deb.asc
# Thu, 23 Jan 2020 17:10:50 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 23 Jan 2020 17:10:51 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 23 Jan 2020 17:10:51 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 23 Jan 2020 17:10:51 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 23 Jan 2020 17:10:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:52 GMT
EXPOSE 8529
# Thu, 23 Jan 2020 17:10:52 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca8484f7a3f17d860ce5f010964ed46b6013cfb493c34eb7ae483a196a65959`  
		Last Modified: Thu, 23 Jan 2020 17:13:37 GMT  
		Size: 107.6 MB (107550582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe1725aa97b4d35497e7d72b01d698a1ed8a20495067cb17739dbcabb8b7356`  
		Last Modified: Thu, 23 Jan 2020 17:11:53 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93789dbf5792d29eacfd353299490543f678dcd2288008b707a0833d5c9cc1b2`  
		Last Modified: Thu, 23 Jan 2020 17:11:52 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:e3d2347035f51108ac2936061c5adb606e36851e7766ab50e2f2a3af5ca385b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:abe5f2131c7ed7da408f6902ce7b78a071b4618dea59838e4ea2635037d13429
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110339990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:421ac5cc2f1194149caaa7c0b8cee65da5ccf6062359df943e17d186d697ec1e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_VERSION=3.6.0
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.0-1_amd64.deb
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.0-1_amd64.deb
# Thu, 23 Jan 2020 17:10:26 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.0-1_amd64.deb.asc
# Thu, 23 Jan 2020 17:10:50 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 23 Jan 2020 17:10:51 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 23 Jan 2020 17:10:51 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 23 Jan 2020 17:10:51 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 23 Jan 2020 17:10:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jan 2020 17:10:52 GMT
EXPOSE 8529
# Thu, 23 Jan 2020 17:10:52 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca8484f7a3f17d860ce5f010964ed46b6013cfb493c34eb7ae483a196a65959`  
		Last Modified: Thu, 23 Jan 2020 17:13:37 GMT  
		Size: 107.6 MB (107550582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe1725aa97b4d35497e7d72b01d698a1ed8a20495067cb17739dbcabb8b7356`  
		Last Modified: Thu, 23 Jan 2020 17:11:53 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93789dbf5792d29eacfd353299490543f678dcd2288008b707a0833d5c9cc1b2`  
		Last Modified: Thu, 23 Jan 2020 17:11:52 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
