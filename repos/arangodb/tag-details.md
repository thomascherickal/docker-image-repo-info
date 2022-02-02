<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.17`](#arangodb3717)
-	[`arangodb:3.8`](#arangodb38)
-	[`arangodb:3.8.5`](#arangodb385)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.7`

```console
$ docker pull arangodb@sha256:d9f434f9b2beded54b6666bcd69b529ff59d4745706d31ba9d58a17c686a962a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.7` - linux; amd64

```console
$ docker pull arangodb@sha256:a2a42938899b297f04633b9a9085d6f8fcdb09fe793abbf41f75200eca62862b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133138324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8524338ba668cf6d2cdc8e69fe2cf24abff301392a572657b1a88a258f4b1e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 24 Jan 2022 23:19:42 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 01 Feb 2022 22:19:15 GMT
ENV ARANGO_VERSION=3.7.17
# Tue, 01 Feb 2022 22:19:15 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Tue, 01 Feb 2022 22:19:16 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.17-1_amd64.deb
# Tue, 01 Feb 2022 22:19:16 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.17-1_amd64.deb
# Tue, 01 Feb 2022 22:19:16 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.17-1_amd64.deb.asc
# Tue, 01 Feb 2022 22:19:44 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 01 Feb 2022 22:19:46 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 01 Feb 2022 22:19:46 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 01 Feb 2022 22:19:46 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 01 Feb 2022 22:19:46 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 01 Feb 2022 22:19:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Feb 2022 22:19:47 GMT
EXPOSE 8529
# Tue, 01 Feb 2022 22:19:47 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63502ac4eff1694e8166142355a152fbda17f0313931796b554e21abb1b08016`  
		Last Modified: Tue, 01 Feb 2022 22:20:26 GMT  
		Size: 130.3 MB (130312996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46aa055d725b997c61d353d85d90cbef2a3503e20aaa6bcb793e40f855ab604`  
		Last Modified: Tue, 01 Feb 2022 22:20:07 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5388e2c8efed23f36ea92a659a624b99199d9d433c6da21193c20bf01b0ed7f8`  
		Last Modified: Tue, 01 Feb 2022 22:20:07 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7.17`

```console
$ docker pull arangodb@sha256:d9f434f9b2beded54b6666bcd69b529ff59d4745706d31ba9d58a17c686a962a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.7.17` - linux; amd64

```console
$ docker pull arangodb@sha256:a2a42938899b297f04633b9a9085d6f8fcdb09fe793abbf41f75200eca62862b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133138324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8524338ba668cf6d2cdc8e69fe2cf24abff301392a572657b1a88a258f4b1e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 24 Jan 2022 23:19:42 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 01 Feb 2022 22:19:15 GMT
ENV ARANGO_VERSION=3.7.17
# Tue, 01 Feb 2022 22:19:15 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Tue, 01 Feb 2022 22:19:16 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.17-1_amd64.deb
# Tue, 01 Feb 2022 22:19:16 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.17-1_amd64.deb
# Tue, 01 Feb 2022 22:19:16 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.17-1_amd64.deb.asc
# Tue, 01 Feb 2022 22:19:44 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 01 Feb 2022 22:19:46 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 01 Feb 2022 22:19:46 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 01 Feb 2022 22:19:46 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 01 Feb 2022 22:19:46 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 01 Feb 2022 22:19:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 01 Feb 2022 22:19:47 GMT
EXPOSE 8529
# Tue, 01 Feb 2022 22:19:47 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63502ac4eff1694e8166142355a152fbda17f0313931796b554e21abb1b08016`  
		Last Modified: Tue, 01 Feb 2022 22:20:26 GMT  
		Size: 130.3 MB (130312996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46aa055d725b997c61d353d85d90cbef2a3503e20aaa6bcb793e40f855ab604`  
		Last Modified: Tue, 01 Feb 2022 22:20:07 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5388e2c8efed23f36ea92a659a624b99199d9d433c6da21193c20bf01b0ed7f8`  
		Last Modified: Tue, 01 Feb 2022 22:20:07 GMT  
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
