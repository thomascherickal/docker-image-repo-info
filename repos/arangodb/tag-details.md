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
$ docker pull arangodb@sha256:2cdfb192429df2653f8d0ea248953f1b08c44ece81c55bd3cc85e5576635ad8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.4` - linux; amd64

```console
$ docker pull arangodb@sha256:91375e062dc5b848001dce93fa34950fe94af4ce7376b15185b5365c6afa1d2b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101933871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12dcca406953d0ddcd827a7efe598ba75589129f6d862a1e25ff86b38d8e9c5c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Apr 2020 14:25:39 GMT
ENV ARANGO_VERSION=3.4.9
# Fri, 24 Apr 2020 14:25:39 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64
# Fri, 24 Apr 2020 14:25:39 GMT
ENV ARANGO_PACKAGE=arangodb3_3.4.9-1_amd64.deb
# Fri, 24 Apr 2020 14:25:39 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.9-1_amd64.deb
# Fri, 24 Apr 2020 14:25:40 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb34/DEBIAN/amd64/arangodb3_3.4.9-1_amd64.deb.asc
# Fri, 24 Apr 2020 14:26:07 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Apr 2020 14:26:08 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Apr 2020 14:26:08 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Fri, 24 Apr 2020 14:26:08 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Fri, 24 Apr 2020 14:26:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:26:08 GMT
EXPOSE 8529
# Fri, 24 Apr 2020 14:26:09 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33aa0366b67d947812ac41beb620067819fc5af0e12b86e43e488d8c8112cff6`  
		Last Modified: Fri, 24 Apr 2020 14:27:47 GMT  
		Size: 99.1 MB (99135843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de56e10f9429e456d1190600352abf06db0de599113cdbb67cb5e836a5216cd`  
		Last Modified: Fri, 24 Apr 2020 14:27:30 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185cc885eff3f22e78c71f173b1ed283541dd8072234497d82b7b08e751c99cc`  
		Last Modified: Fri, 24 Apr 2020 14:27:30 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.4.10`

**does not exist** (yet?)

## `arangodb:3.5`

```console
$ docker pull arangodb@sha256:63eaf16f773e1344b24a9692331afb0ca9643445b91cd9a44aeeaa26ccd62735
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5` - linux; amd64

```console
$ docker pull arangodb@sha256:8034723e31871ceb7220f6ad6c3233aa9d53e8d43eecf4f1ee1bc91e3dcd3c65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110461196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3918952d46e959abbae78db4079110fcd689abed2aaffa59922bbdc1e1b82c50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Apr 2020 14:26:12 GMT
ENV ARANGO_VERSION=3.5.4
# Fri, 24 Apr 2020 14:26:13 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Fri, 24 Apr 2020 14:26:13 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.4-1_amd64.deb
# Fri, 24 Apr 2020 14:26:13 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.4-1_amd64.deb
# Fri, 24 Apr 2020 14:26:13 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.4-1_amd64.deb.asc
# Fri, 24 Apr 2020 14:26:39 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Apr 2020 14:26:40 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Apr 2020 14:26:40 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Fri, 24 Apr 2020 14:26:40 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Fri, 24 Apr 2020 14:26:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:26:40 GMT
EXPOSE 8529
# Fri, 24 Apr 2020 14:26:41 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0f9b3aa9b8d5b21d4e5155fc3c5427a525f7132cf794e1ce6f9561b4d6f4a3`  
		Last Modified: Fri, 24 Apr 2020 14:28:11 GMT  
		Size: 107.7 MB (107663169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a714953d713aa30eab33a9d30bef914e41d0d4cabbfabab6a7ed8bf950a6f0e`  
		Last Modified: Fri, 24 Apr 2020 14:27:52 GMT  
		Size: 2.2 KB (2205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0516f133014847f7d8a643f408fdd2d190a2687c71fe0dcdf63cfa9f617ef85`  
		Last Modified: Fri, 24 Apr 2020 14:27:52 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.5.5`

**does not exist** (yet?)

## `arangodb:3.6`

```console
$ docker pull arangodb@sha256:0567c5148055aa1636d30833532822e8df2714a54ec64289020bc9986b445270
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:ec0070c150a79e3b089e4c2ccd3a727a874c2c20405e64fcd634923f5d3e696d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110726676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaa194fbe2d2481f197a58bb019542bd905938e7c4b34110774fd2d4d6e9e599`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Apr 2020 14:26:46 GMT
ENV ARANGO_VERSION=3.6.3
# Fri, 24 Apr 2020 14:26:46 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Fri, 24 Apr 2020 14:26:47 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.3-1_amd64.deb
# Fri, 24 Apr 2020 14:26:47 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb
# Fri, 24 Apr 2020 14:26:47 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb.asc
# Fri, 24 Apr 2020 14:27:11 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Apr 2020 14:27:12 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Apr 2020 14:27:13 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Fri, 24 Apr 2020 14:27:13 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Fri, 24 Apr 2020 14:27:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:27:13 GMT
EXPOSE 8529
# Fri, 24 Apr 2020 14:27:13 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92795292e9bd4a6e7952a64071bc05b4381920ce7578f57fffd2634e36f79b`  
		Last Modified: Fri, 24 Apr 2020 14:28:34 GMT  
		Size: 107.9 MB (107928650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93234b5acb0cc0b74774f8cbbd0e101fcba5b49cb2fcba0d40b157e48a86e858`  
		Last Modified: Fri, 24 Apr 2020 14:28:15 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c91f4b630f7a8e9d7cc720b3da3bbd32c001fdba81d240c9339bc60c0c06be`  
		Last Modified: Fri, 24 Apr 2020 14:28:16 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.3`

```console
$ docker pull arangodb@sha256:0567c5148055aa1636d30833532822e8df2714a54ec64289020bc9986b445270
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6.3` - linux; amd64

```console
$ docker pull arangodb@sha256:ec0070c150a79e3b089e4c2ccd3a727a874c2c20405e64fcd634923f5d3e696d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110726676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaa194fbe2d2481f197a58bb019542bd905938e7c4b34110774fd2d4d6e9e599`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Apr 2020 14:26:46 GMT
ENV ARANGO_VERSION=3.6.3
# Fri, 24 Apr 2020 14:26:46 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Fri, 24 Apr 2020 14:26:47 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.3-1_amd64.deb
# Fri, 24 Apr 2020 14:26:47 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb
# Fri, 24 Apr 2020 14:26:47 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb.asc
# Fri, 24 Apr 2020 14:27:11 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Apr 2020 14:27:12 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Apr 2020 14:27:13 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Fri, 24 Apr 2020 14:27:13 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Fri, 24 Apr 2020 14:27:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:27:13 GMT
EXPOSE 8529
# Fri, 24 Apr 2020 14:27:13 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92795292e9bd4a6e7952a64071bc05b4381920ce7578f57fffd2634e36f79b`  
		Last Modified: Fri, 24 Apr 2020 14:28:34 GMT  
		Size: 107.9 MB (107928650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93234b5acb0cc0b74774f8cbbd0e101fcba5b49cb2fcba0d40b157e48a86e858`  
		Last Modified: Fri, 24 Apr 2020 14:28:15 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c91f4b630f7a8e9d7cc720b3da3bbd32c001fdba81d240c9339bc60c0c06be`  
		Last Modified: Fri, 24 Apr 2020 14:28:16 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:0567c5148055aa1636d30833532822e8df2714a54ec64289020bc9986b445270
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:ec0070c150a79e3b089e4c2ccd3a727a874c2c20405e64fcd634923f5d3e696d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110726676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaa194fbe2d2481f197a58bb019542bd905938e7c4b34110774fd2d4d6e9e599`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:25:39 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Apr 2020 14:26:46 GMT
ENV ARANGO_VERSION=3.6.3
# Fri, 24 Apr 2020 14:26:46 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Fri, 24 Apr 2020 14:26:47 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.3-1_amd64.deb
# Fri, 24 Apr 2020 14:26:47 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb
# Fri, 24 Apr 2020 14:26:47 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.3-1_amd64.deb.asc
# Fri, 24 Apr 2020 14:27:11 GMT
RUN apk add --no-cache gnupg pwgen nodejs npm binutils numactl numactl-tools &&     npm install -g foxx-cli &&     rm -rf /root/.npm &&     gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Apr 2020 14:27:12 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Apr 2020 14:27:13 GMT
COPY file:912d8c5e20cd837dbed0bf2608b1376ffffdd2d6de3e5b0af4cc869508443235 in /entrypoint.sh 
# Fri, 24 Apr 2020 14:27:13 GMT
COPY file:62d691f3a389929940df44ad84590c9019bdc0c8ce47667d5eb5dab0b2e66954 in /usr/bin/foxx 
# Fri, 24 Apr 2020 14:27:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:27:13 GMT
EXPOSE 8529
# Fri, 24 Apr 2020 14:27:13 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92795292e9bd4a6e7952a64071bc05b4381920ce7578f57fffd2634e36f79b`  
		Last Modified: Fri, 24 Apr 2020 14:28:34 GMT  
		Size: 107.9 MB (107928650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93234b5acb0cc0b74774f8cbbd0e101fcba5b49cb2fcba0d40b157e48a86e858`  
		Last Modified: Fri, 24 Apr 2020 14:28:15 GMT  
		Size: 2.2 KB (2204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c91f4b630f7a8e9d7cc720b3da3bbd32c001fdba81d240c9339bc60c0c06be`  
		Last Modified: Fri, 24 Apr 2020 14:28:16 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
