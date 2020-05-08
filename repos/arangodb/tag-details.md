<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.4`](#arangodb34)
-	[`arangodb:3.4.10`](#arangodb3410)
-	[`arangodb:3.5`](#arangodb35)
-	[`arangodb:3.5.5`](#arangodb355)
-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.3`](#arangodb363)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.4`

```console
$ docker pull arangodb@sha256:9855f6023492e8429c9caefbc9896a4d4e99d2dbde8b2785f09c254970401bd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.4` - linux; amd64

```console
$ docker pull arangodb@sha256:0515dc5b6662e554412311fd76b707e8c9f6decbdb107c9c5f4f97e75d11cf16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101984822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a06eac4d03db5e47aa9f9a4774a2a2f5bf2fa1a93a69d9485a08ff3f9636c3d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 07 May 2020 23:19:23 GMT
ENV ARANGO_VERSION=3.4.10
# Thu, 07 May 2020 23:19:24 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64
# Thu, 07 May 2020 23:19:24 GMT
ENV ARANGO_PACKAGE=arangodb3_3.4.10-1_amd64.deb
# Thu, 07 May 2020 23:19:24 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.10-1_amd64.deb
# Thu, 07 May 2020 23:19:24 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.10-1_amd64.deb.asc
# Thu, 07 May 2020 23:19:47 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 07 May 2020 23:19:48 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 07 May 2020 23:19:48 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 07 May 2020 23:19:48 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 07 May 2020 23:19:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 23:19:48 GMT
EXPOSE 8529
# Thu, 07 May 2020 23:19:49 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3eba28f44c50d59fa2761db8b35d9975b38192f9d18b5f4cde4bb4999eb493`  
		Last Modified: Thu, 07 May 2020 23:21:18 GMT  
		Size: 99.2 MB (99186795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92322f8d70e37609e7ebba8260f8ae970c1da6a53389ab2f365cfe82cb157316`  
		Last Modified: Thu, 07 May 2020 23:21:00 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984ad122196ad0447bfc9d236b7e5dbf7ee7ac4b576e0c43d4b7c1f0f677d002`  
		Last Modified: Thu, 07 May 2020 23:21:00 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.4.10`

```console
$ docker pull arangodb@sha256:9855f6023492e8429c9caefbc9896a4d4e99d2dbde8b2785f09c254970401bd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.4.10` - linux; amd64

```console
$ docker pull arangodb@sha256:0515dc5b6662e554412311fd76b707e8c9f6decbdb107c9c5f4f97e75d11cf16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101984822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a06eac4d03db5e47aa9f9a4774a2a2f5bf2fa1a93a69d9485a08ff3f9636c3d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 07 May 2020 23:19:23 GMT
ENV ARANGO_VERSION=3.4.10
# Thu, 07 May 2020 23:19:24 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64
# Thu, 07 May 2020 23:19:24 GMT
ENV ARANGO_PACKAGE=arangodb3_3.4.10-1_amd64.deb
# Thu, 07 May 2020 23:19:24 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.10-1_amd64.deb
# Thu, 07 May 2020 23:19:24 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.10-1_amd64.deb.asc
# Thu, 07 May 2020 23:19:47 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 07 May 2020 23:19:48 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 07 May 2020 23:19:48 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 07 May 2020 23:19:48 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 07 May 2020 23:19:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 23:19:48 GMT
EXPOSE 8529
# Thu, 07 May 2020 23:19:49 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3eba28f44c50d59fa2761db8b35d9975b38192f9d18b5f4cde4bb4999eb493`  
		Last Modified: Thu, 07 May 2020 23:21:18 GMT  
		Size: 99.2 MB (99186795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92322f8d70e37609e7ebba8260f8ae970c1da6a53389ab2f365cfe82cb157316`  
		Last Modified: Thu, 07 May 2020 23:21:00 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984ad122196ad0447bfc9d236b7e5dbf7ee7ac4b576e0c43d4b7c1f0f677d002`  
		Last Modified: Thu, 07 May 2020 23:21:00 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.5`

```console
$ docker pull arangodb@sha256:a0978381765c0e54bc66c93e7ba95b71f2ab752dd8d930eaf147378eda23516f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5` - linux; amd64

```console
$ docker pull arangodb@sha256:9c0006b18e4c9936fc9a89b90478d49b3a258f679fe9ea3ae0f94c862f968107
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110853466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fa3eb67d57cc48eb91d8dd57e10f30cb3a90a77db3d9e7b3d59ef291f0bd78b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 07 May 2020 23:19:53 GMT
ENV ARANGO_VERSION=3.5.5
# Thu, 07 May 2020 23:19:53 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Thu, 07 May 2020 23:19:53 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.5-1_amd64.deb
# Thu, 07 May 2020 23:19:53 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5-1_amd64.deb
# Thu, 07 May 2020 23:19:53 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5-1_amd64.deb.asc
# Thu, 07 May 2020 23:20:16 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 07 May 2020 23:20:16 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 07 May 2020 23:20:17 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 07 May 2020 23:20:17 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 07 May 2020 23:20:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 23:20:17 GMT
EXPOSE 8529
# Thu, 07 May 2020 23:20:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb2099fe2f15ad1b078637a254692057abced031bbaee2746aabd3981869606`  
		Last Modified: Thu, 07 May 2020 23:21:41 GMT  
		Size: 108.1 MB (108055442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416e03c4774379dbfb0e24b4cbde8d454d4f7ccbee92c64a0f78dc4829f95090`  
		Last Modified: Thu, 07 May 2020 23:21:23 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8aea6d547fc6a587ee7c408b65f1742268b0e0409bd7541e423511e244029a0`  
		Last Modified: Thu, 07 May 2020 23:21:22 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.5.5`

```console
$ docker pull arangodb@sha256:a0978381765c0e54bc66c93e7ba95b71f2ab752dd8d930eaf147378eda23516f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5.5` - linux; amd64

```console
$ docker pull arangodb@sha256:9c0006b18e4c9936fc9a89b90478d49b3a258f679fe9ea3ae0f94c862f968107
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110853466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fa3eb67d57cc48eb91d8dd57e10f30cb3a90a77db3d9e7b3d59ef291f0bd78b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 07 May 2020 23:19:53 GMT
ENV ARANGO_VERSION=3.5.5
# Thu, 07 May 2020 23:19:53 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Thu, 07 May 2020 23:19:53 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.5-1_amd64.deb
# Thu, 07 May 2020 23:19:53 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5-1_amd64.deb
# Thu, 07 May 2020 23:19:53 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5-1_amd64.deb.asc
# Thu, 07 May 2020 23:20:16 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 07 May 2020 23:20:16 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 07 May 2020 23:20:17 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 07 May 2020 23:20:17 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 07 May 2020 23:20:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 23:20:17 GMT
EXPOSE 8529
# Thu, 07 May 2020 23:20:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb2099fe2f15ad1b078637a254692057abced031bbaee2746aabd3981869606`  
		Last Modified: Thu, 07 May 2020 23:21:41 GMT  
		Size: 108.1 MB (108055442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416e03c4774379dbfb0e24b4cbde8d454d4f7ccbee92c64a0f78dc4829f95090`  
		Last Modified: Thu, 07 May 2020 23:21:23 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8aea6d547fc6a587ee7c408b65f1742268b0e0409bd7541e423511e244029a0`  
		Last Modified: Thu, 07 May 2020 23:21:22 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6`

```console
$ docker pull arangodb@sha256:074e722951bdaa03890bc01ddbfdcd8adfaad57b8f23f5d0dbb3b7f8f8690e31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:9fe18fa61fdd5b2c9e9cb9dd68dc620fdd8a20db15dbe9b9369d2a75ef8b4d7f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110724534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2c693ce470b5326eb739244bc35e690b562eb22270269ad074e6e4ce4cbd00`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_VERSION=3.6.3.1
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.3.1-1_amd64.deb
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3.1-1_amd64.deb
# Thu, 07 May 2020 23:20:23 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3.1-1_amd64.deb.asc
# Thu, 07 May 2020 23:20:45 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 07 May 2020 23:20:45 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 07 May 2020 23:20:46 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 07 May 2020 23:20:46 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 07 May 2020 23:20:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 23:20:48 GMT
EXPOSE 8529
# Thu, 07 May 2020 23:20:49 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d59356e6003347ec80566fc117a8c56f25687097c892e3dcd1b06315559d87`  
		Last Modified: Thu, 07 May 2020 23:22:06 GMT  
		Size: 107.9 MB (107926506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deebaef2906d896ed5f292cfa3357dd2604d912f4dc40d8f73ca4928909c795e`  
		Last Modified: Thu, 07 May 2020 23:21:45 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db206e046b399f49a32b193021d752c35aa5697da51578ed9918a408069570ac`  
		Last Modified: Thu, 07 May 2020 23:21:45 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.3`

```console
$ docker pull arangodb@sha256:074e722951bdaa03890bc01ddbfdcd8adfaad57b8f23f5d0dbb3b7f8f8690e31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6.3` - linux; amd64

```console
$ docker pull arangodb@sha256:9fe18fa61fdd5b2c9e9cb9dd68dc620fdd8a20db15dbe9b9369d2a75ef8b4d7f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110724534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2c693ce470b5326eb739244bc35e690b562eb22270269ad074e6e4ce4cbd00`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_VERSION=3.6.3.1
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.3.1-1_amd64.deb
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3.1-1_amd64.deb
# Thu, 07 May 2020 23:20:23 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3.1-1_amd64.deb.asc
# Thu, 07 May 2020 23:20:45 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 07 May 2020 23:20:45 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 07 May 2020 23:20:46 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 07 May 2020 23:20:46 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 07 May 2020 23:20:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 23:20:48 GMT
EXPOSE 8529
# Thu, 07 May 2020 23:20:49 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d59356e6003347ec80566fc117a8c56f25687097c892e3dcd1b06315559d87`  
		Last Modified: Thu, 07 May 2020 23:22:06 GMT  
		Size: 107.9 MB (107926506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deebaef2906d896ed5f292cfa3357dd2604d912f4dc40d8f73ca4928909c795e`  
		Last Modified: Thu, 07 May 2020 23:21:45 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db206e046b399f49a32b193021d752c35aa5697da51578ed9918a408069570ac`  
		Last Modified: Thu, 07 May 2020 23:21:45 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:074e722951bdaa03890bc01ddbfdcd8adfaad57b8f23f5d0dbb3b7f8f8690e31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:9fe18fa61fdd5b2c9e9cb9dd68dc620fdd8a20db15dbe9b9369d2a75ef8b4d7f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110724534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2c693ce470b5326eb739244bc35e690b562eb22270269ad074e6e4ce4cbd00`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_VERSION=3.6.3.1
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.3.1-1_amd64.deb
# Thu, 07 May 2020 23:20:22 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3.1-1_amd64.deb
# Thu, 07 May 2020 23:20:23 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3.1-1_amd64.deb.asc
# Thu, 07 May 2020 23:20:45 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 07 May 2020 23:20:45 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 07 May 2020 23:20:46 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Thu, 07 May 2020 23:20:46 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Thu, 07 May 2020 23:20:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 May 2020 23:20:48 GMT
EXPOSE 8529
# Thu, 07 May 2020 23:20:49 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d59356e6003347ec80566fc117a8c56f25687097c892e3dcd1b06315559d87`  
		Last Modified: Thu, 07 May 2020 23:22:06 GMT  
		Size: 107.9 MB (107926506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deebaef2906d896ed5f292cfa3357dd2604d912f4dc40d8f73ca4928909c795e`  
		Last Modified: Thu, 07 May 2020 23:21:45 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db206e046b399f49a32b193021d752c35aa5697da51578ed9918a408069570ac`  
		Last Modified: Thu, 07 May 2020 23:21:45 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
