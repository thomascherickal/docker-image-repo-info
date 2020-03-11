<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:2.8`](#arangodb28)
-	[`arangodb:2.8.11`](#arangodb2811)
-	[`arangodb:3.2`](#arangodb32)
-	[`arangodb:3.2.17`](#arangodb3217)
-	[`arangodb:3.3`](#arangodb33)
-	[`arangodb:3.3.25`](#arangodb3325)
-	[`arangodb:3.4`](#arangodb34)
-	[`arangodb:3.4.9`](#arangodb349)
-	[`arangodb:3.5`](#arangodb35)
-	[`arangodb:3.5.4`](#arangodb354)
-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.2`](#arangodb362)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:2.8`

```console
$ docker pull arangodb@sha256:39f5c107c8bf1d9d24aa6df4e6513ab9a7587c816f7858b6f9f3b2bb4210e711
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:2.8` - linux; amd64

```console
$ docker pull arangodb@sha256:951180dc87b347264abbabe4220fdde287383f9bf6c086fa756ca9b124824b95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115103797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7cdecb0ad4ff5c1a76076826307a146e2dbba18bda41c1ebd6a2945986959f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:57 GMT
ADD file:607350db53d30cfbdaaa75b7a47bd59de2bfa83fe4a50be9e7cccddcbfa7c61a in / 
# Wed, 26 Feb 2020 00:37:58 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 17:52:11 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 26 Feb 2020 17:52:12 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Wed, 26 Feb 2020 17:52:12 GMT
ENV ARCHITECTURE=amd64
# Wed, 26 Feb 2020 17:52:13 GMT
ENV ARANGO_VERSION=2.8.11
# Wed, 26 Feb 2020 17:52:13 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb2/Debian_8.0
# Wed, 26 Feb 2020 17:52:13 GMT
ENV ARANGO_PACKAGE=arangodb_2.8.11_amd64.deb
# Wed, 26 Feb 2020 17:52:13 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb
# Wed, 26 Feb 2020 17:52:14 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb.asc
# Wed, 26 Feb 2020 17:54:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libgoogle-perftools4         ca-certificates         pwgen         wget     &&     rm -rf /var/lib/apt/lists/* &&     wget ${ARANGO_SIGNATURE_URL} &&           wget ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     dpkg -i ${ARANGO_PACKAGE} &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^#\s*uid\s*=.*!uid = arangodb!'         -e 's!^#\s*gid\s*=.*!gid = arangodb!'         /etc/arangodb/arangod.conf     &&     apt-get purge -y --auto-remove ca-certificates wget &&     rm -f ${ARANGO_PACKAGE}*
# Wed, 26 Feb 2020 17:54:45 GMT
RUN chown arangodb:arangodb /var/lib/arangodb &&   chown arangodb:arangodb /var/lib/arangodb-apps
# Wed, 26 Feb 2020 17:54:45 GMT
VOLUME [/var/lib/arangodb /var/lib/arangodb-apps]
# Wed, 26 Feb 2020 17:54:45 GMT
COPY file:9a5bd6b5ab4e3a7842ac5f3e59bb9907920e9e2dc31d297c3676110b569a9d7e in /entrypoint.sh 
# Wed, 26 Feb 2020 17:54:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 17:54:45 GMT
EXPOSE 8529
# Wed, 26 Feb 2020 17:54:46 GMT
USER arangodb
# Wed, 26 Feb 2020 17:54:46 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:92d14a6520e1a734155afb0c5b456614718259f56397290ed22fab220c2b96f4`  
		Last Modified: Wed, 26 Feb 2020 00:44:41 GMT  
		Size: 54.4 MB (54388885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65947afe089639006f59139973a28d478f5be23a4ef5d7132d85cf691bcb5ddb`  
		Last Modified: Wed, 26 Feb 2020 17:57:15 GMT  
		Size: 8.6 KB (8594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43a8907d751754f9e47c5a70ddf30ad0d7d9760de77dfd2df5dadbf072c5bbd`  
		Last Modified: Wed, 26 Feb 2020 17:57:29 GMT  
		Size: 60.7 MB (60705058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244b988f0fe43709dd423ad5fdfb8f90c43b951fff9e48aa8123084d454acd91`  
		Last Modified: Wed, 26 Feb 2020 17:57:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f040f19b7ebcef7bc332bb503a138962590ebedc9d8868822225fdc31355e0`  
		Last Modified: Wed, 26 Feb 2020 17:57:15 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:2.8.11`

```console
$ docker pull arangodb@sha256:39f5c107c8bf1d9d24aa6df4e6513ab9a7587c816f7858b6f9f3b2bb4210e711
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:2.8.11` - linux; amd64

```console
$ docker pull arangodb@sha256:951180dc87b347264abbabe4220fdde287383f9bf6c086fa756ca9b124824b95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115103797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7cdecb0ad4ff5c1a76076826307a146e2dbba18bda41c1ebd6a2945986959f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:57 GMT
ADD file:607350db53d30cfbdaaa75b7a47bd59de2bfa83fe4a50be9e7cccddcbfa7c61a in / 
# Wed, 26 Feb 2020 00:37:58 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 17:52:11 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 26 Feb 2020 17:52:12 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Wed, 26 Feb 2020 17:52:12 GMT
ENV ARCHITECTURE=amd64
# Wed, 26 Feb 2020 17:52:13 GMT
ENV ARANGO_VERSION=2.8.11
# Wed, 26 Feb 2020 17:52:13 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb2/Debian_8.0
# Wed, 26 Feb 2020 17:52:13 GMT
ENV ARANGO_PACKAGE=arangodb_2.8.11_amd64.deb
# Wed, 26 Feb 2020 17:52:13 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb
# Wed, 26 Feb 2020 17:52:14 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb.asc
# Wed, 26 Feb 2020 17:54:44 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libgoogle-perftools4         ca-certificates         pwgen         wget     &&     rm -rf /var/lib/apt/lists/* &&     wget ${ARANGO_SIGNATURE_URL} &&           wget ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     dpkg -i ${ARANGO_PACKAGE} &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^#\s*uid\s*=.*!uid = arangodb!'         -e 's!^#\s*gid\s*=.*!gid = arangodb!'         /etc/arangodb/arangod.conf     &&     apt-get purge -y --auto-remove ca-certificates wget &&     rm -f ${ARANGO_PACKAGE}*
# Wed, 26 Feb 2020 17:54:45 GMT
RUN chown arangodb:arangodb /var/lib/arangodb &&   chown arangodb:arangodb /var/lib/arangodb-apps
# Wed, 26 Feb 2020 17:54:45 GMT
VOLUME [/var/lib/arangodb /var/lib/arangodb-apps]
# Wed, 26 Feb 2020 17:54:45 GMT
COPY file:9a5bd6b5ab4e3a7842ac5f3e59bb9907920e9e2dc31d297c3676110b569a9d7e in /entrypoint.sh 
# Wed, 26 Feb 2020 17:54:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 17:54:45 GMT
EXPOSE 8529
# Wed, 26 Feb 2020 17:54:46 GMT
USER arangodb
# Wed, 26 Feb 2020 17:54:46 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:92d14a6520e1a734155afb0c5b456614718259f56397290ed22fab220c2b96f4`  
		Last Modified: Wed, 26 Feb 2020 00:44:41 GMT  
		Size: 54.4 MB (54388885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65947afe089639006f59139973a28d478f5be23a4ef5d7132d85cf691bcb5ddb`  
		Last Modified: Wed, 26 Feb 2020 17:57:15 GMT  
		Size: 8.6 KB (8594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43a8907d751754f9e47c5a70ddf30ad0d7d9760de77dfd2df5dadbf072c5bbd`  
		Last Modified: Wed, 26 Feb 2020 17:57:29 GMT  
		Size: 60.7 MB (60705058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244b988f0fe43709dd423ad5fdfb8f90c43b951fff9e48aa8123084d454acd91`  
		Last Modified: Wed, 26 Feb 2020 17:57:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f040f19b7ebcef7bc332bb503a138962590ebedc9d8868822225fdc31355e0`  
		Last Modified: Wed, 26 Feb 2020 17:57:15 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.2`

```console
$ docker pull arangodb@sha256:6b4a99844dd39b7f73667a39b0ea5838df62759b22a04475d60fe551edadcfc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.2` - linux; amd64

```console
$ docker pull arangodb@sha256:f10c5995afff4103f50199780344b5d234b268475cff76613c1390222f65e7d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113546207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9754122f0f6673923638eb19b5e43543ab474c830c2c876931b2c2a7c93fd1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 17:54:55 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 26 Feb 2020 17:54:55 GMT
ENV ARCHITECTURE=amd64
# Wed, 26 Feb 2020 17:54:55 GMT
ENV DEB_PACKAGE_VERSION=1
# Wed, 26 Feb 2020 17:54:55 GMT
ENV ARANGO_VERSION=3.2.17
# Wed, 26 Feb 2020 17:54:56 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb32/Debian_9.0
# Wed, 26 Feb 2020 17:54:56 GMT
ENV ARANGO_PACKAGE=arangodb3-3.2.17-1_amd64.deb
# Wed, 26 Feb 2020 17:54:56 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb
# Wed, 26 Feb 2020 17:54:56 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb.asc
# Wed, 26 Feb 2020 17:55:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gpg dirmngr     &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 17:55:07 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Wed, 26 Feb 2020 17:55:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libjemalloc1         ca-certificates         pwgen         curl         numactl     &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 17:55:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Feb 2020 17:55:31 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Wed, 26 Feb 2020 17:55:31 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 26 Feb 2020 17:55:31 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Wed, 26 Feb 2020 17:55:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 17:55:32 GMT
EXPOSE 8529
# Wed, 26 Feb 2020 17:55:32 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dced73f9de62e77cdf83c54c6b375a4d3389f0a07d50de08dfa5fa8507aee2f4`  
		Last Modified: Wed, 26 Feb 2020 17:57:37 GMT  
		Size: 6.6 MB (6566493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbe47048ae4d91412e3baaadd0f7070da8961d8e37f1d5039eec9cc48f330c0`  
		Last Modified: Wed, 26 Feb 2020 17:57:34 GMT  
		Size: 4.4 KB (4447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2b0c133413a2fc839f536dc23bd02297422eb0465e83aacd787d68696170c`  
		Last Modified: Wed, 26 Feb 2020 17:57:36 GMT  
		Size: 7.5 MB (7461563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1487e62ba334415c6648895a87afed02ff57d6872d0c45f4357bbe459a7fc642`  
		Last Modified: Wed, 26 Feb 2020 17:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9901cdd6710cc412abe4fbcc960fd6293da5060c1874e8b9069c250e27fc6140`  
		Last Modified: Wed, 26 Feb 2020 17:57:49 GMT  
		Size: 54.1 MB (54135620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840b8a12dba4481645cf3aedd5ea79e95814e87f704167082a44b535ed6f35f`  
		Last Modified: Wed, 26 Feb 2020 17:57:33 GMT  
		Size: 2.0 KB (2037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.2.17`

```console
$ docker pull arangodb@sha256:6b4a99844dd39b7f73667a39b0ea5838df62759b22a04475d60fe551edadcfc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.2.17` - linux; amd64

```console
$ docker pull arangodb@sha256:f10c5995afff4103f50199780344b5d234b268475cff76613c1390222f65e7d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113546207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9754122f0f6673923638eb19b5e43543ab474c830c2c876931b2c2a7c93fd1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 17:54:55 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 26 Feb 2020 17:54:55 GMT
ENV ARCHITECTURE=amd64
# Wed, 26 Feb 2020 17:54:55 GMT
ENV DEB_PACKAGE_VERSION=1
# Wed, 26 Feb 2020 17:54:55 GMT
ENV ARANGO_VERSION=3.2.17
# Wed, 26 Feb 2020 17:54:56 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb32/Debian_9.0
# Wed, 26 Feb 2020 17:54:56 GMT
ENV ARANGO_PACKAGE=arangodb3-3.2.17-1_amd64.deb
# Wed, 26 Feb 2020 17:54:56 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb
# Wed, 26 Feb 2020 17:54:56 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb.asc
# Wed, 26 Feb 2020 17:55:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gpg dirmngr     &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 17:55:07 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Wed, 26 Feb 2020 17:55:17 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libjemalloc1         ca-certificates         pwgen         curl         numactl     &&     rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 17:55:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Feb 2020 17:55:31 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Wed, 26 Feb 2020 17:55:31 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 26 Feb 2020 17:55:31 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Wed, 26 Feb 2020 17:55:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 17:55:32 GMT
EXPOSE 8529
# Wed, 26 Feb 2020 17:55:32 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dced73f9de62e77cdf83c54c6b375a4d3389f0a07d50de08dfa5fa8507aee2f4`  
		Last Modified: Wed, 26 Feb 2020 17:57:37 GMT  
		Size: 6.6 MB (6566493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbe47048ae4d91412e3baaadd0f7070da8961d8e37f1d5039eec9cc48f330c0`  
		Last Modified: Wed, 26 Feb 2020 17:57:34 GMT  
		Size: 4.4 KB (4447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2b0c133413a2fc839f536dc23bd02297422eb0465e83aacd787d68696170c`  
		Last Modified: Wed, 26 Feb 2020 17:57:36 GMT  
		Size: 7.5 MB (7461563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1487e62ba334415c6648895a87afed02ff57d6872d0c45f4357bbe459a7fc642`  
		Last Modified: Wed, 26 Feb 2020 17:57:33 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9901cdd6710cc412abe4fbcc960fd6293da5060c1874e8b9069c250e27fc6140`  
		Last Modified: Wed, 26 Feb 2020 17:57:49 GMT  
		Size: 54.1 MB (54135620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840b8a12dba4481645cf3aedd5ea79e95814e87f704167082a44b535ed6f35f`  
		Last Modified: Wed, 26 Feb 2020 17:57:33 GMT  
		Size: 2.0 KB (2037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.3`

```console
$ docker pull arangodb@sha256:d3113b3091834861cdfbde5b8b072506bff45afcb64ece1591948ee38aaf5631
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.3` - linux; amd64

```console
$ docker pull arangodb@sha256:0e8ea50a96309f7885ea851ddb7f8d8f5141b0f9737e6c4f655c2fa908c7fc3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117195891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd99e471d21b7ca66d3df6a8a8a6525e0ea748dcdc79ad3e2c7fd5340dbce477`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 17:54:55 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 26 Feb 2020 17:54:55 GMT
ENV ARCHITECTURE=amd64
# Wed, 26 Feb 2020 17:54:55 GMT
ENV DEB_PACKAGE_VERSION=1
# Fri, 28 Feb 2020 22:19:31 GMT
ENV ARANGO_VERSION=3.3.25
# Fri, 28 Feb 2020 22:19:31 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb33/Debian_9.0
# Fri, 28 Feb 2020 22:19:32 GMT
ENV ARANGO_PACKAGE=arangodb3-3.3.25-1_amd64.deb
# Fri, 28 Feb 2020 22:19:32 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.25-1_amd64.deb
# Fri, 28 Feb 2020 22:19:32 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.25-1_amd64.deb.asc
# Fri, 28 Feb 2020 22:19:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         dirmngr         gpg     && rm -rf /var/lib/apt/lists/*
# Fri, 28 Feb 2020 22:19:41 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Fri, 28 Feb 2020 22:19:49 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         curl         libjemalloc1         libtasn1-6         numactl         openssl         pwgen         sensible-utils     && rm -rf /var/lib/apt/lists/*
# Fri, 28 Feb 2020 22:19:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 28 Feb 2020 22:20:02 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Fri, 28 Feb 2020 22:20:03 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 28 Feb 2020 22:20:03 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Fri, 28 Feb 2020 22:20:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:20:03 GMT
EXPOSE 8529
# Fri, 28 Feb 2020 22:20:03 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091bce0528b81f095a20ed060198f0143294edba7b823e0d54b16c3587c11d73`  
		Last Modified: Fri, 28 Feb 2020 22:20:27 GMT  
		Size: 6.6 MB (6566487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11fe49f215315444f1af2bee44bcf210493dc2126ee3f043e9967bad86bf3787`  
		Last Modified: Fri, 28 Feb 2020 22:20:25 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158d27be03c1f27d6767277f04f57a775af8a724f51350e0f255a12dcbb4ee82`  
		Last Modified: Fri, 28 Feb 2020 22:20:26 GMT  
		Size: 7.5 MB (7461625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9662d768e8cd06e8317727e405622b30ee610765808da57a32d4f6d9ca827177`  
		Last Modified: Fri, 28 Feb 2020 22:20:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b4f86f780b2e36c4db597b9d369aa75465930c288b854c721aaa8ed9a67850`  
		Last Modified: Fri, 28 Feb 2020 22:20:35 GMT  
		Size: 57.8 MB (57785249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a5558b3d8300a2ccf27c58cb798083bef03c9ad18cde516b6f4ed865c40b01`  
		Last Modified: Fri, 28 Feb 2020 22:20:25 GMT  
		Size: 2.0 KB (2038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.3.25`

```console
$ docker pull arangodb@sha256:d3113b3091834861cdfbde5b8b072506bff45afcb64ece1591948ee38aaf5631
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.3.25` - linux; amd64

```console
$ docker pull arangodb@sha256:0e8ea50a96309f7885ea851ddb7f8d8f5141b0f9737e6c4f655c2fa908c7fc3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117195891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd99e471d21b7ca66d3df6a8a8a6525e0ea748dcdc79ad3e2c7fd5340dbce477`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 17:54:55 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 26 Feb 2020 17:54:55 GMT
ENV ARCHITECTURE=amd64
# Wed, 26 Feb 2020 17:54:55 GMT
ENV DEB_PACKAGE_VERSION=1
# Fri, 28 Feb 2020 22:19:31 GMT
ENV ARANGO_VERSION=3.3.25
# Fri, 28 Feb 2020 22:19:31 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb33/Debian_9.0
# Fri, 28 Feb 2020 22:19:32 GMT
ENV ARANGO_PACKAGE=arangodb3-3.3.25-1_amd64.deb
# Fri, 28 Feb 2020 22:19:32 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.25-1_amd64.deb
# Fri, 28 Feb 2020 22:19:32 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.25-1_amd64.deb.asc
# Fri, 28 Feb 2020 22:19:38 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         dirmngr         gpg     && rm -rf /var/lib/apt/lists/*
# Fri, 28 Feb 2020 22:19:41 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Fri, 28 Feb 2020 22:19:49 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         curl         libjemalloc1         libtasn1-6         numactl         openssl         pwgen         sensible-utils     && rm -rf /var/lib/apt/lists/*
# Fri, 28 Feb 2020 22:19:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 28 Feb 2020 22:20:02 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Fri, 28 Feb 2020 22:20:03 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 28 Feb 2020 22:20:03 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Fri, 28 Feb 2020 22:20:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 28 Feb 2020 22:20:03 GMT
EXPOSE 8529
# Fri, 28 Feb 2020 22:20:03 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091bce0528b81f095a20ed060198f0143294edba7b823e0d54b16c3587c11d73`  
		Last Modified: Fri, 28 Feb 2020 22:20:27 GMT  
		Size: 6.6 MB (6566487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11fe49f215315444f1af2bee44bcf210493dc2126ee3f043e9967bad86bf3787`  
		Last Modified: Fri, 28 Feb 2020 22:20:25 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158d27be03c1f27d6767277f04f57a775af8a724f51350e0f255a12dcbb4ee82`  
		Last Modified: Fri, 28 Feb 2020 22:20:26 GMT  
		Size: 7.5 MB (7461625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9662d768e8cd06e8317727e405622b30ee610765808da57a32d4f6d9ca827177`  
		Last Modified: Fri, 28 Feb 2020 22:20:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b4f86f780b2e36c4db597b9d369aa75465930c288b854c721aaa8ed9a67850`  
		Last Modified: Fri, 28 Feb 2020 22:20:35 GMT  
		Size: 57.8 MB (57785249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a5558b3d8300a2ccf27c58cb798083bef03c9ad18cde516b6f4ed865c40b01`  
		Last Modified: Fri, 28 Feb 2020 22:20:25 GMT  
		Size: 2.0 KB (2038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.4`

```console
$ docker pull arangodb@sha256:c32bcd08a60c1da2e96b02fa8db1ac2bde22b899245a4699c6449d16fe736e49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.4` - linux; amd64

```console
$ docker pull arangodb@sha256:f354f9650ae0c94def2826c2aa13b289f6007fec9d4cd575d66e2a13a591456b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101990383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8bbe8672ebba1abbf2225666e1dfc2e153874340c4fa52b0b08755e5d85ad7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 25 Jan 2020 01:19:37 GMT
ENV ARANGO_VERSION=3.4.9
# Sat, 25 Jan 2020 01:19:38 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64
# Sat, 25 Jan 2020 01:19:38 GMT
ENV ARANGO_PACKAGE=arangodb3_3.4.9-1_amd64.deb
# Sat, 25 Jan 2020 01:19:38 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.9-1_amd64.deb
# Sat, 25 Jan 2020 01:19:38 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.9-1_amd64.deb.asc
# Sat, 25 Jan 2020 01:20:01 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 25 Jan 2020 01:20:02 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 25 Jan 2020 01:20:02 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Sat, 25 Jan 2020 01:20:02 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Sat, 25 Jan 2020 01:20:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 25 Jan 2020 01:20:03 GMT
EXPOSE 8529
# Sat, 25 Jan 2020 01:20:03 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd71998e0104b799cecf1dc84120cc5f654bcf1b1a01fec4714dd1b9e417ca52`  
		Last Modified: Sat, 25 Jan 2020 01:20:42 GMT  
		Size: 99.2 MB (99200973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccb3bc7bf0a313e2619890c9ae7742e6e557d431b852716e5dd195d3808f442`  
		Last Modified: Sat, 25 Jan 2020 01:20:24 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1993e49cf3e237fbc357190ae1df3b0b9b49ec93e21d2e4fb7f92d762443632`  
		Last Modified: Sat, 25 Jan 2020 01:20:24 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.4.9`

```console
$ docker pull arangodb@sha256:c32bcd08a60c1da2e96b02fa8db1ac2bde22b899245a4699c6449d16fe736e49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.4.9` - linux; amd64

```console
$ docker pull arangodb@sha256:f354f9650ae0c94def2826c2aa13b289f6007fec9d4cd575d66e2a13a591456b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101990383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8bbe8672ebba1abbf2225666e1dfc2e153874340c4fa52b0b08755e5d85ad7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 25 Jan 2020 01:19:37 GMT
ENV ARANGO_VERSION=3.4.9
# Sat, 25 Jan 2020 01:19:38 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64
# Sat, 25 Jan 2020 01:19:38 GMT
ENV ARANGO_PACKAGE=arangodb3_3.4.9-1_amd64.deb
# Sat, 25 Jan 2020 01:19:38 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.9-1_amd64.deb
# Sat, 25 Jan 2020 01:19:38 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.9-1_amd64.deb.asc
# Sat, 25 Jan 2020 01:20:01 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 25 Jan 2020 01:20:02 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 25 Jan 2020 01:20:02 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Sat, 25 Jan 2020 01:20:02 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Sat, 25 Jan 2020 01:20:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 25 Jan 2020 01:20:03 GMT
EXPOSE 8529
# Sat, 25 Jan 2020 01:20:03 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd71998e0104b799cecf1dc84120cc5f654bcf1b1a01fec4714dd1b9e417ca52`  
		Last Modified: Sat, 25 Jan 2020 01:20:42 GMT  
		Size: 99.2 MB (99200973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccb3bc7bf0a313e2619890c9ae7742e6e557d431b852716e5dd195d3808f442`  
		Last Modified: Sat, 25 Jan 2020 01:20:24 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1993e49cf3e237fbc357190ae1df3b0b9b49ec93e21d2e4fb7f92d762443632`  
		Last Modified: Sat, 25 Jan 2020 01:20:24 GMT  
		Size: 244.0 B  
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
$ docker pull arangodb@sha256:4bb3878ecd81707d4bf143322158be458b2e5bf4b1afa704effe483fb1dad6a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:b605bcfff5618a390bf29e102c0ee91c0216195cd725fd7b90bf9b73bd2e04ff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110398482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49c471eee813987c4c0ce4d57c878122f88e26aba7b2407661243394e129b0d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 30 Jan 2020 23:19:44 GMT
ENV ARANGO_VERSION=3.6.1
# Thu, 30 Jan 2020 23:19:44 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Thu, 30 Jan 2020 23:19:44 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.1-1_amd64.deb
# Thu, 30 Jan 2020 23:19:44 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.1-1_amd64.deb
# Thu, 30 Jan 2020 23:19:44 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.1-1_amd64.deb.asc
# Thu, 30 Jan 2020 23:20:07 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 30 Jan 2020 23:20:07 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 30 Jan 2020 23:20:08 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 30 Jan 2020 23:20:08 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 30 Jan 2020 23:20:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Jan 2020 23:20:08 GMT
EXPOSE 8529
# Thu, 30 Jan 2020 23:20:08 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3580c6d05ad3793c5d37991d7e15df84c4d088ad89bd15d86163bfc6043851b5`  
		Last Modified: Thu, 30 Jan 2020 23:20:48 GMT  
		Size: 107.6 MB (107609071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737c6cb81dee9412594ace6ca5bd2ff89e15c98440e5c6443d17e691e34dcd62`  
		Last Modified: Thu, 30 Jan 2020 23:20:22 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af15ccb07504c19dee0ee0610fe117883b8172a499a9426b87635e06311e9665`  
		Last Modified: Thu, 30 Jan 2020 23:20:22 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.2`

**does not exist** (yet?)

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:4bb3878ecd81707d4bf143322158be458b2e5bf4b1afa704effe483fb1dad6a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:b605bcfff5618a390bf29e102c0ee91c0216195cd725fd7b90bf9b73bd2e04ff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110398482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49c471eee813987c4c0ce4d57c878122f88e26aba7b2407661243394e129b0d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 30 Jan 2020 23:19:44 GMT
ENV ARANGO_VERSION=3.6.1
# Thu, 30 Jan 2020 23:19:44 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Thu, 30 Jan 2020 23:19:44 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.1-1_amd64.deb
# Thu, 30 Jan 2020 23:19:44 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.1-1_amd64.deb
# Thu, 30 Jan 2020 23:19:44 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.1-1_amd64.deb.asc
# Thu, 30 Jan 2020 23:20:07 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 30 Jan 2020 23:20:07 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 30 Jan 2020 23:20:08 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 30 Jan 2020 23:20:08 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 30 Jan 2020 23:20:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Jan 2020 23:20:08 GMT
EXPOSE 8529
# Thu, 30 Jan 2020 23:20:08 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3580c6d05ad3793c5d37991d7e15df84c4d088ad89bd15d86163bfc6043851b5`  
		Last Modified: Thu, 30 Jan 2020 23:20:48 GMT  
		Size: 107.6 MB (107609071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737c6cb81dee9412594ace6ca5bd2ff89e15c98440e5c6443d17e691e34dcd62`  
		Last Modified: Thu, 30 Jan 2020 23:20:22 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af15ccb07504c19dee0ee0610fe117883b8172a499a9426b87635e06311e9665`  
		Last Modified: Thu, 30 Jan 2020 23:20:22 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
