<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.4`](#arangodb34)
-	[`arangodb:3.4.10`](#arangodb3410)
-	[`arangodb:3.5`](#arangodb35)
-	[`arangodb:3.5.5`](#arangodb355)
-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.5`](#arangodb365)
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
$ docker pull arangodb@sha256:1289e1a474419e99a4f535302bf394ff6b63985dfa374b6d7d39d13f06a2a3e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5` - linux; amd64

```console
$ docker pull arangodb@sha256:a9e17825955c640d3c346b8bd92dfefb556a3f5392a942e9d42351bccb0e6835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110854571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef05ad11e4c12f280b1bc175bcbdf36891446d510820052c13c568ad33676924`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 11 May 2020 15:20:31 GMT
ENV ARANGO_VERSION=3.5.5.1
# Mon, 11 May 2020 15:20:31 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Mon, 11 May 2020 15:20:31 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.5.1-1_amd64.deb
# Mon, 11 May 2020 15:20:31 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5.1-1_amd64.deb
# Mon, 11 May 2020 15:20:31 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5.1-1_amd64.deb.asc
# Mon, 11 May 2020 15:20:55 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 11 May 2020 15:20:56 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 11 May 2020 15:20:56 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Mon, 11 May 2020 15:20:56 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Mon, 11 May 2020 15:20:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 May 2020 15:20:56 GMT
EXPOSE 8529
# Mon, 11 May 2020 15:20:57 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbf091d13a7f900dedf5f9a05b4e1652f15cf677a952e0d2c47b025009633b8`  
		Last Modified: Mon, 11 May 2020 15:21:30 GMT  
		Size: 108.1 MB (108056542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae853fbf2cc343f8217a2e959312f8c9e7f51931b4ae1c6be0f929d3909543c`  
		Last Modified: Mon, 11 May 2020 15:21:12 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ea6dad4bc4831c972106771ef21081d63b50cacdde6b5b76b681263df1839a`  
		Last Modified: Mon, 11 May 2020 15:21:13 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.5.5`

```console
$ docker pull arangodb@sha256:1289e1a474419e99a4f535302bf394ff6b63985dfa374b6d7d39d13f06a2a3e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5.5` - linux; amd64

```console
$ docker pull arangodb@sha256:a9e17825955c640d3c346b8bd92dfefb556a3f5392a942e9d42351bccb0e6835
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110854571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef05ad11e4c12f280b1bc175bcbdf36891446d510820052c13c568ad33676924`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 11 May 2020 15:20:31 GMT
ENV ARANGO_VERSION=3.5.5.1
# Mon, 11 May 2020 15:20:31 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Mon, 11 May 2020 15:20:31 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.5.1-1_amd64.deb
# Mon, 11 May 2020 15:20:31 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5.1-1_amd64.deb
# Mon, 11 May 2020 15:20:31 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.5.1-1_amd64.deb.asc
# Mon, 11 May 2020 15:20:55 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 11 May 2020 15:20:56 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 11 May 2020 15:20:56 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Mon, 11 May 2020 15:20:56 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Mon, 11 May 2020 15:20:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 May 2020 15:20:56 GMT
EXPOSE 8529
# Mon, 11 May 2020 15:20:57 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbf091d13a7f900dedf5f9a05b4e1652f15cf677a952e0d2c47b025009633b8`  
		Last Modified: Mon, 11 May 2020 15:21:30 GMT  
		Size: 108.1 MB (108056542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae853fbf2cc343f8217a2e959312f8c9e7f51931b4ae1c6be0f929d3909543c`  
		Last Modified: Mon, 11 May 2020 15:21:12 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ea6dad4bc4831c972106771ef21081d63b50cacdde6b5b76b681263df1839a`  
		Last Modified: Mon, 11 May 2020 15:21:13 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6`

```console
$ docker pull arangodb@sha256:5d5e0e4f116939577031d321354c8aeadbca004f2e2f4c5d0bf617962e327742
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:d615d0ebd872b7b69d16b240ca800bd3709d49d8a29378abb5ca221e256405fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110914435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79c99b3e2810c7d609802b484462244e46352d2475d7ec880cc90c29ac28d71c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 02 Jun 2020 01:27:22 GMT
ENV ARANGO_VERSION=3.6.4
# Tue, 02 Jun 2020 01:27:22 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Tue, 02 Jun 2020 01:27:22 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.4-1_amd64.deb
# Tue, 02 Jun 2020 01:27:22 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.4-1_amd64.deb
# Tue, 02 Jun 2020 01:27:23 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.4-1_amd64.deb.asc
# Tue, 02 Jun 2020 01:27:49 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 02 Jun 2020 01:27:50 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 02 Jun 2020 01:27:50 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Tue, 02 Jun 2020 01:27:50 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Tue, 02 Jun 2020 01:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Jun 2020 01:27:51 GMT
EXPOSE 8529
# Tue, 02 Jun 2020 01:27:51 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb97f40ea79744938abfbf1d169544c60ebb94c91a355e5dbaba81202442d911`  
		Last Modified: Tue, 02 Jun 2020 01:28:19 GMT  
		Size: 108.1 MB (108116408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93ae66f4a8a330afd694ddc160ef4105c7523d043c4e04366d0af73ff51b5e`  
		Last Modified: Tue, 02 Jun 2020 01:28:00 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a66587e4c9741c1664197d5557efd19b1eb9e47074c106dac1acf365168302e`  
		Last Modified: Tue, 02 Jun 2020 01:28:00 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.5`

```console
$ docker pull arangodb@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:5d5e0e4f116939577031d321354c8aeadbca004f2e2f4c5d0bf617962e327742
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:d615d0ebd872b7b69d16b240ca800bd3709d49d8a29378abb5ca221e256405fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110914435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79c99b3e2810c7d609802b484462244e46352d2475d7ec880cc90c29ac28d71c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 02 Jun 2020 01:27:22 GMT
ENV ARANGO_VERSION=3.6.4
# Tue, 02 Jun 2020 01:27:22 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Tue, 02 Jun 2020 01:27:22 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.4-1_amd64.deb
# Tue, 02 Jun 2020 01:27:22 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.4-1_amd64.deb
# Tue, 02 Jun 2020 01:27:23 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.4-1_amd64.deb.asc
# Tue, 02 Jun 2020 01:27:49 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 02 Jun 2020 01:27:50 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 02 Jun 2020 01:27:50 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Tue, 02 Jun 2020 01:27:50 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Tue, 02 Jun 2020 01:27:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Jun 2020 01:27:51 GMT
EXPOSE 8529
# Tue, 02 Jun 2020 01:27:51 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb97f40ea79744938abfbf1d169544c60ebb94c91a355e5dbaba81202442d911`  
		Last Modified: Tue, 02 Jun 2020 01:28:19 GMT  
		Size: 108.1 MB (108116408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d93ae66f4a8a330afd694ddc160ef4105c7523d043c4e04366d0af73ff51b5e`  
		Last Modified: Tue, 02 Jun 2020 01:28:00 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a66587e4c9741c1664197d5557efd19b1eb9e47074c106dac1acf365168302e`  
		Last Modified: Tue, 02 Jun 2020 01:28:00 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
