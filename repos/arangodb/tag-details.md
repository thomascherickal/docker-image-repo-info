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
-	[`arangodb:3.6.3`](#arangodb363)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:2.8`

```console
$ docker pull arangodb@sha256:1b07bb2f780d4fde796dd81ae323b56dd85ed0036b04c85a5e3858da5f60d9b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:2.8` - linux; amd64

```console
$ docker pull arangodb@sha256:18fa4100125b4dd18699b2cecc29b1db422625540925a6d59ca1d47afdeeb573
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115105919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eca24c1577763aa9c9f6176336960e9303f975a7b46036262c31c1d5cec59da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 16 Apr 2020 03:23:07 GMT
ADD file:06c434cd627b8970a4f3d8d76b36955fbf53b74db3f0ce29f1fc3b269c81f2eb in / 
# Thu, 16 Apr 2020 03:23:08 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:24:10 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 16 Apr 2020 04:24:11 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Thu, 16 Apr 2020 04:24:11 GMT
ENV ARCHITECTURE=amd64
# Thu, 16 Apr 2020 04:24:11 GMT
ENV ARANGO_VERSION=2.8.11
# Thu, 16 Apr 2020 04:24:11 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb2/Debian_8.0
# Thu, 16 Apr 2020 04:24:11 GMT
ENV ARANGO_PACKAGE=arangodb_2.8.11_amd64.deb
# Thu, 16 Apr 2020 04:24:12 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb
# Thu, 16 Apr 2020 04:24:12 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb.asc
# Thu, 16 Apr 2020 04:26:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libgoogle-perftools4         ca-certificates         pwgen         wget     &&     rm -rf /var/lib/apt/lists/* &&     wget ${ARANGO_SIGNATURE_URL} &&           wget ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     dpkg -i ${ARANGO_PACKAGE} &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^#\s*uid\s*=.*!uid = arangodb!'         -e 's!^#\s*gid\s*=.*!gid = arangodb!'         /etc/arangodb/arangod.conf     &&     apt-get purge -y --auto-remove ca-certificates wget &&     rm -f ${ARANGO_PACKAGE}*
# Thu, 16 Apr 2020 04:26:50 GMT
RUN chown arangodb:arangodb /var/lib/arangodb &&   chown arangodb:arangodb /var/lib/arangodb-apps
# Thu, 16 Apr 2020 04:26:50 GMT
VOLUME [/var/lib/arangodb /var/lib/arangodb-apps]
# Thu, 16 Apr 2020 04:26:50 GMT
COPY file:9a5bd6b5ab4e3a7842ac5f3e59bb9907920e9e2dc31d297c3676110b569a9d7e in /entrypoint.sh 
# Thu, 16 Apr 2020 04:26:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Apr 2020 04:26:51 GMT
EXPOSE 8529
# Thu, 16 Apr 2020 04:26:51 GMT
USER arangodb
# Thu, 16 Apr 2020 04:26:52 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:3707da5d661028328ae23959ded4ecbb1e5ddbe2a4e8551cd5b6f90e90e6cbd5`  
		Last Modified: Thu, 16 Apr 2020 03:32:06 GMT  
		Size: 54.4 MB (54390842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa14ea9f5b557a4ba54f5b37f8994f35203434bb8089899a5cd4be410216c22`  
		Last Modified: Thu, 16 Apr 2020 04:29:26 GMT  
		Size: 8.6 KB (8594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14613a0552f3711f3fa539e79ea8bc4cee558fc313250d90620e851bd19457c`  
		Last Modified: Thu, 16 Apr 2020 04:29:44 GMT  
		Size: 60.7 MB (60705223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471b87a8c1b02234315d75cfe84c96f97d2df31c3cd4a5606fd33e4d6b92e0b5`  
		Last Modified: Thu, 16 Apr 2020 04:29:26 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7347a6ccaa908a1824921a7af9492b24e1a97ce8d74194a79adf9ea84aeb435b`  
		Last Modified: Thu, 16 Apr 2020 04:29:26 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:2.8.11`

```console
$ docker pull arangodb@sha256:1b07bb2f780d4fde796dd81ae323b56dd85ed0036b04c85a5e3858da5f60d9b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:2.8.11` - linux; amd64

```console
$ docker pull arangodb@sha256:18fa4100125b4dd18699b2cecc29b1db422625540925a6d59ca1d47afdeeb573
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115105919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eca24c1577763aa9c9f6176336960e9303f975a7b46036262c31c1d5cec59da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 16 Apr 2020 03:23:07 GMT
ADD file:06c434cd627b8970a4f3d8d76b36955fbf53b74db3f0ce29f1fc3b269c81f2eb in / 
# Thu, 16 Apr 2020 03:23:08 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:24:10 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 16 Apr 2020 04:24:11 GMT
RUN gpg --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Thu, 16 Apr 2020 04:24:11 GMT
ENV ARCHITECTURE=amd64
# Thu, 16 Apr 2020 04:24:11 GMT
ENV ARANGO_VERSION=2.8.11
# Thu, 16 Apr 2020 04:24:11 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb2/Debian_8.0
# Thu, 16 Apr 2020 04:24:11 GMT
ENV ARANGO_PACKAGE=arangodb_2.8.11_amd64.deb
# Thu, 16 Apr 2020 04:24:12 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb
# Thu, 16 Apr 2020 04:24:12 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb2/Debian_8.0/amd64/arangodb_2.8.11_amd64.deb.asc
# Thu, 16 Apr 2020 04:26:48 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libgoogle-perftools4         ca-certificates         pwgen         wget     &&     rm -rf /var/lib/apt/lists/* &&     wget ${ARANGO_SIGNATURE_URL} &&           wget ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     dpkg -i ${ARANGO_PACKAGE} &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^#\s*uid\s*=.*!uid = arangodb!'         -e 's!^#\s*gid\s*=.*!gid = arangodb!'         /etc/arangodb/arangod.conf     &&     apt-get purge -y --auto-remove ca-certificates wget &&     rm -f ${ARANGO_PACKAGE}*
# Thu, 16 Apr 2020 04:26:50 GMT
RUN chown arangodb:arangodb /var/lib/arangodb &&   chown arangodb:arangodb /var/lib/arangodb-apps
# Thu, 16 Apr 2020 04:26:50 GMT
VOLUME [/var/lib/arangodb /var/lib/arangodb-apps]
# Thu, 16 Apr 2020 04:26:50 GMT
COPY file:9a5bd6b5ab4e3a7842ac5f3e59bb9907920e9e2dc31d297c3676110b569a9d7e in /entrypoint.sh 
# Thu, 16 Apr 2020 04:26:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Apr 2020 04:26:51 GMT
EXPOSE 8529
# Thu, 16 Apr 2020 04:26:51 GMT
USER arangodb
# Thu, 16 Apr 2020 04:26:52 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:3707da5d661028328ae23959ded4ecbb1e5ddbe2a4e8551cd5b6f90e90e6cbd5`  
		Last Modified: Thu, 16 Apr 2020 03:32:06 GMT  
		Size: 54.4 MB (54390842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa14ea9f5b557a4ba54f5b37f8994f35203434bb8089899a5cd4be410216c22`  
		Last Modified: Thu, 16 Apr 2020 04:29:26 GMT  
		Size: 8.6 KB (8594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14613a0552f3711f3fa539e79ea8bc4cee558fc313250d90620e851bd19457c`  
		Last Modified: Thu, 16 Apr 2020 04:29:44 GMT  
		Size: 60.7 MB (60705223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471b87a8c1b02234315d75cfe84c96f97d2df31c3cd4a5606fd33e4d6b92e0b5`  
		Last Modified: Thu, 16 Apr 2020 04:29:26 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7347a6ccaa908a1824921a7af9492b24e1a97ce8d74194a79adf9ea84aeb435b`  
		Last Modified: Thu, 16 Apr 2020 04:29:26 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.2`

```console
$ docker pull arangodb@sha256:b4ea39a77ebc5d98d8a318ccf84f55b999fd9aca607d003397c411c9257ff509
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.2` - linux; amd64

```console
$ docker pull arangodb@sha256:a79ec9256026fdfa9bd4da1f6fb17e54e2bc31496521b9ad29b9427f7a57c024
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113546194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2984e750df6e511cbe88951072745077cd9beb2263e9611226233d2070cd75e5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:22 GMT
ADD file:9f6f0c8b90de3204ad5db95d10d8aa76b42454def6ac811c888ad4e274292c9c in / 
# Thu, 16 Apr 2020 03:27:22 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:26:57 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 16 Apr 2020 04:26:57 GMT
ENV ARCHITECTURE=amd64
# Thu, 16 Apr 2020 04:26:58 GMT
ENV DEB_PACKAGE_VERSION=1
# Thu, 16 Apr 2020 04:26:58 GMT
ENV ARANGO_VERSION=3.2.17
# Thu, 16 Apr 2020 04:26:58 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb32/Debian_9.0
# Thu, 16 Apr 2020 04:26:59 GMT
ENV ARANGO_PACKAGE=arangodb3-3.2.17-1_amd64.deb
# Thu, 16 Apr 2020 04:26:59 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb
# Thu, 16 Apr 2020 04:26:59 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb.asc
# Thu, 16 Apr 2020 04:27:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gpg dirmngr     &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:27:18 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Thu, 16 Apr 2020 04:27:31 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libjemalloc1         ca-certificates         pwgen         curl         numactl     &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:27:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 04:27:52 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Thu, 16 Apr 2020 04:27:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 16 Apr 2020 04:27:53 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Thu, 16 Apr 2020 04:27:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Apr 2020 04:27:54 GMT
EXPOSE 8529
# Thu, 16 Apr 2020 04:27:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:7568c21980bd8003ca9d23a218302c6386aac91e069cc0c0be6bedf45476f056`  
		Last Modified: Thu, 16 Apr 2020 03:34:47 GMT  
		Size: 45.4 MB (45375910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d34063570b60fba19709c5c910d54c2a21088421a178a298e4f11a24c76899`  
		Last Modified: Thu, 16 Apr 2020 04:29:52 GMT  
		Size: 6.6 MB (6566510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519e674146a7cf7f2b1b0426080ecd6e92ce51141d514afebb6b2439976d1df7`  
		Last Modified: Thu, 16 Apr 2020 04:29:48 GMT  
		Size: 4.4 KB (4446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5a2f778a4b91fd069c238e2e277c692ab58e03c40782d8c188c766757c20ce`  
		Last Modified: Thu, 16 Apr 2020 04:29:51 GMT  
		Size: 7.5 MB (7461570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5dbf315bcdc33bcc34a72e71e2be1f45a64a528b98c70d138e3710ebccd7e6b`  
		Last Modified: Thu, 16 Apr 2020 04:29:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2350746e6a7636ffdd49af7ab5b230cc2c4bd23ffcc03f0b0cb031e4d389826`  
		Last Modified: Thu, 16 Apr 2020 04:30:21 GMT  
		Size: 54.1 MB (54135605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0119297c7b651a7fd691c60914f621e89cd30370a18bdf85532342514626ed5d`  
		Last Modified: Thu, 16 Apr 2020 04:29:48 GMT  
		Size: 2.0 KB (2038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.2.17`

```console
$ docker pull arangodb@sha256:b4ea39a77ebc5d98d8a318ccf84f55b999fd9aca607d003397c411c9257ff509
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.2.17` - linux; amd64

```console
$ docker pull arangodb@sha256:a79ec9256026fdfa9bd4da1f6fb17e54e2bc31496521b9ad29b9427f7a57c024
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113546194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2984e750df6e511cbe88951072745077cd9beb2263e9611226233d2070cd75e5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:22 GMT
ADD file:9f6f0c8b90de3204ad5db95d10d8aa76b42454def6ac811c888ad4e274292c9c in / 
# Thu, 16 Apr 2020 03:27:22 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:26:57 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 16 Apr 2020 04:26:57 GMT
ENV ARCHITECTURE=amd64
# Thu, 16 Apr 2020 04:26:58 GMT
ENV DEB_PACKAGE_VERSION=1
# Thu, 16 Apr 2020 04:26:58 GMT
ENV ARANGO_VERSION=3.2.17
# Thu, 16 Apr 2020 04:26:58 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb32/Debian_9.0
# Thu, 16 Apr 2020 04:26:59 GMT
ENV ARANGO_PACKAGE=arangodb3-3.2.17-1_amd64.deb
# Thu, 16 Apr 2020 04:26:59 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb
# Thu, 16 Apr 2020 04:26:59 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb32/Debian_9.0/amd64/arangodb3-3.2.17-1_amd64.deb.asc
# Thu, 16 Apr 2020 04:27:08 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends gpg dirmngr     &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:27:18 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Thu, 16 Apr 2020 04:27:31 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         libjemalloc1         ca-certificates         pwgen         curl         numactl     &&     rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:27:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 04:27:52 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Thu, 16 Apr 2020 04:27:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 16 Apr 2020 04:27:53 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Thu, 16 Apr 2020 04:27:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Apr 2020 04:27:54 GMT
EXPOSE 8529
# Thu, 16 Apr 2020 04:27:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:7568c21980bd8003ca9d23a218302c6386aac91e069cc0c0be6bedf45476f056`  
		Last Modified: Thu, 16 Apr 2020 03:34:47 GMT  
		Size: 45.4 MB (45375910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d34063570b60fba19709c5c910d54c2a21088421a178a298e4f11a24c76899`  
		Last Modified: Thu, 16 Apr 2020 04:29:52 GMT  
		Size: 6.6 MB (6566510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519e674146a7cf7f2b1b0426080ecd6e92ce51141d514afebb6b2439976d1df7`  
		Last Modified: Thu, 16 Apr 2020 04:29:48 GMT  
		Size: 4.4 KB (4446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5a2f778a4b91fd069c238e2e277c692ab58e03c40782d8c188c766757c20ce`  
		Last Modified: Thu, 16 Apr 2020 04:29:51 GMT  
		Size: 7.5 MB (7461570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5dbf315bcdc33bcc34a72e71e2be1f45a64a528b98c70d138e3710ebccd7e6b`  
		Last Modified: Thu, 16 Apr 2020 04:29:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2350746e6a7636ffdd49af7ab5b230cc2c4bd23ffcc03f0b0cb031e4d389826`  
		Last Modified: Thu, 16 Apr 2020 04:30:21 GMT  
		Size: 54.1 MB (54135605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0119297c7b651a7fd691c60914f621e89cd30370a18bdf85532342514626ed5d`  
		Last Modified: Thu, 16 Apr 2020 04:29:48 GMT  
		Size: 2.0 KB (2038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.3`

```console
$ docker pull arangodb@sha256:9df1daa528f11b32d00c0a9b61b3a2bb7e087e51c45b2719c4bd58370117615d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.3` - linux; amd64

```console
$ docker pull arangodb@sha256:6118b838612c8b4d861aa65294460bc47be8e5ea3d5ccca985ed3adef85b4898
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117196057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0c1990f4a7678299de06638b51a54fdcb23f59492b106019b8e36320f1a3901`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:22 GMT
ADD file:9f6f0c8b90de3204ad5db95d10d8aa76b42454def6ac811c888ad4e274292c9c in / 
# Thu, 16 Apr 2020 03:27:22 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:26:57 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 16 Apr 2020 04:26:57 GMT
ENV ARCHITECTURE=amd64
# Thu, 16 Apr 2020 04:26:58 GMT
ENV DEB_PACKAGE_VERSION=1
# Thu, 16 Apr 2020 04:28:01 GMT
ENV ARANGO_VERSION=3.3.25
# Thu, 16 Apr 2020 04:28:01 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb33/Debian_9.0
# Thu, 16 Apr 2020 04:28:01 GMT
ENV ARANGO_PACKAGE=arangodb3-3.3.25-1_amd64.deb
# Thu, 16 Apr 2020 04:28:02 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.25-1_amd64.deb
# Thu, 16 Apr 2020 04:28:02 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.25-1_amd64.deb.asc
# Thu, 16 Apr 2020 04:28:10 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         dirmngr         gpg     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:28:17 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Thu, 16 Apr 2020 04:28:31 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         curl         libjemalloc1         libtasn1-6         numactl         openssl         pwgen         sensible-utils     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:28:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 04:28:51 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Thu, 16 Apr 2020 04:28:52 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 16 Apr 2020 04:28:52 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Thu, 16 Apr 2020 04:28:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Apr 2020 04:28:53 GMT
EXPOSE 8529
# Thu, 16 Apr 2020 04:28:53 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:7568c21980bd8003ca9d23a218302c6386aac91e069cc0c0be6bedf45476f056`  
		Last Modified: Thu, 16 Apr 2020 03:34:47 GMT  
		Size: 45.4 MB (45375910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3eeea74a93292f4bf0df5834350b4f135d1a7b9ee1e4efbe8c2e67388cfdbc`  
		Last Modified: Thu, 16 Apr 2020 04:30:30 GMT  
		Size: 6.6 MB (6566515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bd5588dd7cdd3c0b90578a07acbd21f38ca9daae03f0dcc3defcc5e7789e90`  
		Last Modified: Thu, 16 Apr 2020 04:30:27 GMT  
		Size: 4.4 KB (4444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d1ac25f0e1180d3655a6114cdfe87b4dd23e8042d171d31cc4a25fdddb84e8`  
		Last Modified: Thu, 16 Apr 2020 04:30:30 GMT  
		Size: 7.5 MB (7461683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9642d49cd090df6535744ee4c4c3ab97b399ff8ba5814218a39041019e336e05`  
		Last Modified: Thu, 16 Apr 2020 04:30:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e534efe29baabc838b3b6c0b57d4245aa0febb37000187b4ef4c936afcbe159`  
		Last Modified: Thu, 16 Apr 2020 04:30:43 GMT  
		Size: 57.8 MB (57785352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb95207c5610ed980c1def2f0e37be8b6342edfa7787c9996d7ec48672e1852`  
		Last Modified: Thu, 16 Apr 2020 04:30:27 GMT  
		Size: 2.0 KB (2038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.3.25`

```console
$ docker pull arangodb@sha256:9df1daa528f11b32d00c0a9b61b3a2bb7e087e51c45b2719c4bd58370117615d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.3.25` - linux; amd64

```console
$ docker pull arangodb@sha256:6118b838612c8b4d861aa65294460bc47be8e5ea3d5ccca985ed3adef85b4898
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117196057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0c1990f4a7678299de06638b51a54fdcb23f59492b106019b8e36320f1a3901`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 16 Apr 2020 03:27:22 GMT
ADD file:9f6f0c8b90de3204ad5db95d10d8aa76b42454def6ac811c888ad4e274292c9c in / 
# Thu, 16 Apr 2020 03:27:22 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:26:57 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 16 Apr 2020 04:26:57 GMT
ENV ARCHITECTURE=amd64
# Thu, 16 Apr 2020 04:26:58 GMT
ENV DEB_PACKAGE_VERSION=1
# Thu, 16 Apr 2020 04:28:01 GMT
ENV ARANGO_VERSION=3.3.25
# Thu, 16 Apr 2020 04:28:01 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb33/Debian_9.0
# Thu, 16 Apr 2020 04:28:01 GMT
ENV ARANGO_PACKAGE=arangodb3-3.3.25-1_amd64.deb
# Thu, 16 Apr 2020 04:28:02 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.25-1_amd64.deb
# Thu, 16 Apr 2020 04:28:02 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb33/Debian_9.0/amd64/arangodb3-3.3.25-1_amd64.deb.asc
# Thu, 16 Apr 2020 04:28:10 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         dirmngr         gpg     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:28:17 GMT
RUN gpg --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B
# Thu, 16 Apr 2020 04:28:31 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends         ca-certificates         curl         curl         libjemalloc1         libtasn1-6         numactl         openssl         pwgen         sensible-utils     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:28:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 04:28:51 GMT
RUN curl --fail -O ${ARANGO_SIGNATURE_URL} &&           curl --fail -O ${ARANGO_PACKAGE_URL} &&             gpg --verify ${ARANGO_PACKAGE}.asc &&     (echo arangodb3 arangodb3/password password test | debconf-set-selections) &&     (echo arangodb3 arangodb3/password_again password test | debconf-set-selections) &&     DEBIAN_FRONTEND="noninteractive" dpkg -i ${ARANGO_PACKAGE} &&     rm -rf /var/lib/arangodb3/* &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf     && chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps     && chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps     &&     rm -f ${ARANGO_PACKAGE}*
# Thu, 16 Apr 2020 04:28:52 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 16 Apr 2020 04:28:52 GMT
COPY file:01bdd453b032c9d383e66c7e6332049490bb7877724d3bb90d185f11336934d2 in /entrypoint.sh 
# Thu, 16 Apr 2020 04:28:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Apr 2020 04:28:53 GMT
EXPOSE 8529
# Thu, 16 Apr 2020 04:28:53 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:7568c21980bd8003ca9d23a218302c6386aac91e069cc0c0be6bedf45476f056`  
		Last Modified: Thu, 16 Apr 2020 03:34:47 GMT  
		Size: 45.4 MB (45375910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3eeea74a93292f4bf0df5834350b4f135d1a7b9ee1e4efbe8c2e67388cfdbc`  
		Last Modified: Thu, 16 Apr 2020 04:30:30 GMT  
		Size: 6.6 MB (6566515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bd5588dd7cdd3c0b90578a07acbd21f38ca9daae03f0dcc3defcc5e7789e90`  
		Last Modified: Thu, 16 Apr 2020 04:30:27 GMT  
		Size: 4.4 KB (4444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d1ac25f0e1180d3655a6114cdfe87b4dd23e8042d171d31cc4a25fdddb84e8`  
		Last Modified: Thu, 16 Apr 2020 04:30:30 GMT  
		Size: 7.5 MB (7461683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9642d49cd090df6535744ee4c4c3ab97b399ff8ba5814218a39041019e336e05`  
		Last Modified: Thu, 16 Apr 2020 04:30:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e534efe29baabc838b3b6c0b57d4245aa0febb37000187b4ef4c936afcbe159`  
		Last Modified: Thu, 16 Apr 2020 04:30:43 GMT  
		Size: 57.8 MB (57785352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb95207c5610ed980c1def2f0e37be8b6342edfa7787c9996d7ec48672e1852`  
		Last Modified: Thu, 16 Apr 2020 04:30:27 GMT  
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
$ docker pull arangodb@sha256:cfa7fa806d66aa2677034100b42ec87d479dc9c6600d83aa1e4a12310c3fb3b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:d10f34e0f53e9d1a1f5fd79856253a632269791fc03f38eea5eac4ed0e4ddc33
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110717994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4178648ffd4bbe76b16899ad5a0bdc735963d7658e3c47a610de29c28c9ef7e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 22 Apr 2020 23:20:49 GMT
ENV ARANGO_VERSION=3.6.3
# Wed, 22 Apr 2020 23:20:49 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Wed, 22 Apr 2020 23:20:50 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.3-1_amd64.deb
# Wed, 22 Apr 2020 23:20:50 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb
# Wed, 22 Apr 2020 23:20:50 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb.asc
# Wed, 22 Apr 2020 23:21:14 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 22 Apr 2020 23:21:14 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 22 Apr 2020 23:21:15 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Wed, 22 Apr 2020 23:21:15 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Wed, 22 Apr 2020 23:21:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Apr 2020 23:21:15 GMT
EXPOSE 8529
# Wed, 22 Apr 2020 23:21:15 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad5ab8ff5bda63b2d74cddeca87157dc16158cabe1ae0042e7389a4bf90ec77`  
		Last Modified: Wed, 22 Apr 2020 23:21:48 GMT  
		Size: 107.9 MB (107928588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7437ce257aeecca0baec1488aecef796f734a25a972cf2eae7d586766d0c6854`  
		Last Modified: Wed, 22 Apr 2020 23:21:30 GMT  
		Size: 2.2 KB (2202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ff9411eaece6ebcf7b7fb929cbee662ddd493b9cf2c10427a4b602c9ba32c3`  
		Last Modified: Wed, 22 Apr 2020 23:21:29 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.3`

```console
$ docker pull arangodb@sha256:cfa7fa806d66aa2677034100b42ec87d479dc9c6600d83aa1e4a12310c3fb3b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6.3` - linux; amd64

```console
$ docker pull arangodb@sha256:d10f34e0f53e9d1a1f5fd79856253a632269791fc03f38eea5eac4ed0e4ddc33
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110717994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4178648ffd4bbe76b16899ad5a0bdc735963d7658e3c47a610de29c28c9ef7e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 22 Apr 2020 23:20:49 GMT
ENV ARANGO_VERSION=3.6.3
# Wed, 22 Apr 2020 23:20:49 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Wed, 22 Apr 2020 23:20:50 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.3-1_amd64.deb
# Wed, 22 Apr 2020 23:20:50 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb
# Wed, 22 Apr 2020 23:20:50 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb.asc
# Wed, 22 Apr 2020 23:21:14 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 22 Apr 2020 23:21:14 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 22 Apr 2020 23:21:15 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Wed, 22 Apr 2020 23:21:15 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Wed, 22 Apr 2020 23:21:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Apr 2020 23:21:15 GMT
EXPOSE 8529
# Wed, 22 Apr 2020 23:21:15 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad5ab8ff5bda63b2d74cddeca87157dc16158cabe1ae0042e7389a4bf90ec77`  
		Last Modified: Wed, 22 Apr 2020 23:21:48 GMT  
		Size: 107.9 MB (107928588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7437ce257aeecca0baec1488aecef796f734a25a972cf2eae7d586766d0c6854`  
		Last Modified: Wed, 22 Apr 2020 23:21:30 GMT  
		Size: 2.2 KB (2202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ff9411eaece6ebcf7b7fb929cbee662ddd493b9cf2c10427a4b602c9ba32c3`  
		Last Modified: Wed, 22 Apr 2020 23:21:29 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:cfa7fa806d66aa2677034100b42ec87d479dc9c6600d83aa1e4a12310c3fb3b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:d10f34e0f53e9d1a1f5fd79856253a632269791fc03f38eea5eac4ed0e4ddc33
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110717994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4178648ffd4bbe76b16899ad5a0bdc735963d7658e3c47a610de29c28c9ef7e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:09:20 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 22 Apr 2020 23:20:49 GMT
ENV ARANGO_VERSION=3.6.3
# Wed, 22 Apr 2020 23:20:49 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Wed, 22 Apr 2020 23:20:50 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.3-1_amd64.deb
# Wed, 22 Apr 2020 23:20:50 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb
# Wed, 22 Apr 2020 23:20:50 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb.asc
# Wed, 22 Apr 2020 23:21:14 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 22 Apr 2020 23:21:14 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 22 Apr 2020 23:21:15 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Wed, 22 Apr 2020 23:21:15 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Wed, 22 Apr 2020 23:21:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Apr 2020 23:21:15 GMT
EXPOSE 8529
# Wed, 22 Apr 2020 23:21:15 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad5ab8ff5bda63b2d74cddeca87157dc16158cabe1ae0042e7389a4bf90ec77`  
		Last Modified: Wed, 22 Apr 2020 23:21:48 GMT  
		Size: 107.9 MB (107928588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7437ce257aeecca0baec1488aecef796f734a25a972cf2eae7d586766d0c6854`  
		Last Modified: Wed, 22 Apr 2020 23:21:30 GMT  
		Size: 2.2 KB (2202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ff9411eaece6ebcf7b7fb929cbee662ddd493b9cf2c10427a4b602c9ba32c3`  
		Last Modified: Wed, 22 Apr 2020 23:21:29 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
