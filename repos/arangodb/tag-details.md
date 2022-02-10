<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.17`](#arangodb3717)
-	[`arangodb:3.8`](#arangodb38)
-	[`arangodb:3.8.5`](#arangodb385)
-	[`arangodb:3.9`](#arangodb39)
-	[`arangodb:3.9.0`](#arangodb390)
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
$ docker pull arangodb@sha256:7e73e745ffc4957caca5dd91053d5b9fbd09c57b0212bfc86d43c6e239772568
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8` - linux; amd64

```console
$ docker pull arangodb@sha256:406a79b4a2e94b1310e06e5ff82235c518cac5696f33e0ff29c7a4637fb1f780
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191106191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:581ad62f9ac36fbd74034ea78718a2bceea17d0d62b8f9bbd08643befac43751`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 24 Jan 2022 23:19:42 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 04 Feb 2022 23:42:35 GMT
ENV ARANGO_VERSION=3.8.5.1
# Fri, 04 Feb 2022 23:42:35 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Fri, 04 Feb 2022 23:42:35 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.5.1-1_amd64.deb
# Fri, 04 Feb 2022 23:42:36 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.5.1-1_amd64.deb
# Fri, 04 Feb 2022 23:42:36 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.5.1-1_amd64.deb.asc
# Fri, 04 Feb 2022 23:43:24 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 04 Feb 2022 23:43:26 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 04 Feb 2022 23:43:26 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 04 Feb 2022 23:43:26 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 04 Feb 2022 23:43:26 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 04 Feb 2022 23:43:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 04 Feb 2022 23:43:27 GMT
EXPOSE 8529
# Fri, 04 Feb 2022 23:43:27 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca1012f3510f76e81858e9f187b2875f52dd86d131b0c1c9f82a484b134f321`  
		Last Modified: Fri, 04 Feb 2022 23:44:06 GMT  
		Size: 188.3 MB (188280861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce8f8b945733459ff736c5e687f03b7364f2d79cea7518a32eeef75c22d9c41`  
		Last Modified: Fri, 04 Feb 2022 23:43:42 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c520e72aa8977b32e3dc267e482acf44e843f8222a4873bd8f78674674668ae`  
		Last Modified: Fri, 04 Feb 2022 23:43:42 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8.5`

```console
$ docker pull arangodb@sha256:7e73e745ffc4957caca5dd91053d5b9fbd09c57b0212bfc86d43c6e239772568
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8.5` - linux; amd64

```console
$ docker pull arangodb@sha256:406a79b4a2e94b1310e06e5ff82235c518cac5696f33e0ff29c7a4637fb1f780
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191106191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:581ad62f9ac36fbd74034ea78718a2bceea17d0d62b8f9bbd08643befac43751`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 24 Jan 2022 23:19:42 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 04 Feb 2022 23:42:35 GMT
ENV ARANGO_VERSION=3.8.5.1
# Fri, 04 Feb 2022 23:42:35 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Fri, 04 Feb 2022 23:42:35 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.5.1-1_amd64.deb
# Fri, 04 Feb 2022 23:42:36 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.5.1-1_amd64.deb
# Fri, 04 Feb 2022 23:42:36 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.5.1-1_amd64.deb.asc
# Fri, 04 Feb 2022 23:43:24 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 04 Feb 2022 23:43:26 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 04 Feb 2022 23:43:26 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 04 Feb 2022 23:43:26 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 04 Feb 2022 23:43:26 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 04 Feb 2022 23:43:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 04 Feb 2022 23:43:27 GMT
EXPOSE 8529
# Fri, 04 Feb 2022 23:43:27 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca1012f3510f76e81858e9f187b2875f52dd86d131b0c1c9f82a484b134f321`  
		Last Modified: Fri, 04 Feb 2022 23:44:06 GMT  
		Size: 188.3 MB (188280861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce8f8b945733459ff736c5e687f03b7364f2d79cea7518a32eeef75c22d9c41`  
		Last Modified: Fri, 04 Feb 2022 23:43:42 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c520e72aa8977b32e3dc267e482acf44e843f8222a4873bd8f78674674668ae`  
		Last Modified: Fri, 04 Feb 2022 23:43:42 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9`

```console
$ docker pull arangodb@sha256:9fba4f596cefc32f8886c6a15de699185ec486b8b7e24b60b76db6170133f59d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9` - linux; amd64

```console
$ docker pull arangodb@sha256:0f469bbcb43f0c21f0d18580334444e0220225d687d8e4ec8e4e7288db58abad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.9 MB (197863337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e501430d3240ce0de619698fd06175826e5f5a7716f065e5872cc2c24cf79c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 24 Jan 2022 23:19:42 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 09 Feb 2022 20:19:17 GMT
ENV ARANGO_VERSION=3.9.0
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.0-1_amd64.deb
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.0-1_amd64.deb
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.0-1_amd64.deb.asc
# Wed, 09 Feb 2022 20:19:44 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 09 Feb 2022 20:19:46 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 09 Feb 2022 20:19:46 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 09 Feb 2022 20:19:46 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 09 Feb 2022 20:19:46 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 09 Feb 2022 20:19:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Feb 2022 20:19:47 GMT
EXPOSE 8529
# Wed, 09 Feb 2022 20:19:47 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02a853c7927a577dfc0ac95ac85249d61600035e0f5cbaaa06c6c4eb946582c`  
		Last Modified: Wed, 09 Feb 2022 20:20:25 GMT  
		Size: 195.0 MB (195038012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d34c0c7faf0c8c16dbf6629b3a2202f3dc4c43008811d594b86833a729ed65`  
		Last Modified: Wed, 09 Feb 2022 20:20:03 GMT  
		Size: 2.1 KB (2084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706c235208c4c929f663f80c4edaf478530749a2c26e2b1d4290d68fe4e2e36a`  
		Last Modified: Wed, 09 Feb 2022 20:20:03 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9.0`

```console
$ docker pull arangodb@sha256:9fba4f596cefc32f8886c6a15de699185ec486b8b7e24b60b76db6170133f59d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9.0` - linux; amd64

```console
$ docker pull arangodb@sha256:0f469bbcb43f0c21f0d18580334444e0220225d687d8e4ec8e4e7288db58abad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.9 MB (197863337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e501430d3240ce0de619698fd06175826e5f5a7716f065e5872cc2c24cf79c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 24 Jan 2022 23:19:42 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 09 Feb 2022 20:19:17 GMT
ENV ARANGO_VERSION=3.9.0
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.0-1_amd64.deb
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.0-1_amd64.deb
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.0-1_amd64.deb.asc
# Wed, 09 Feb 2022 20:19:44 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 09 Feb 2022 20:19:46 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 09 Feb 2022 20:19:46 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 09 Feb 2022 20:19:46 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 09 Feb 2022 20:19:46 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 09 Feb 2022 20:19:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Feb 2022 20:19:47 GMT
EXPOSE 8529
# Wed, 09 Feb 2022 20:19:47 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02a853c7927a577dfc0ac95ac85249d61600035e0f5cbaaa06c6c4eb946582c`  
		Last Modified: Wed, 09 Feb 2022 20:20:25 GMT  
		Size: 195.0 MB (195038012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d34c0c7faf0c8c16dbf6629b3a2202f3dc4c43008811d594b86833a729ed65`  
		Last Modified: Wed, 09 Feb 2022 20:20:03 GMT  
		Size: 2.1 KB (2084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706c235208c4c929f663f80c4edaf478530749a2c26e2b1d4290d68fe4e2e36a`  
		Last Modified: Wed, 09 Feb 2022 20:20:03 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:9fba4f596cefc32f8886c6a15de699185ec486b8b7e24b60b76db6170133f59d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:0f469bbcb43f0c21f0d18580334444e0220225d687d8e4ec8e4e7288db58abad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.9 MB (197863337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e501430d3240ce0de619698fd06175826e5f5a7716f065e5872cc2c24cf79c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 24 Jan 2022 23:19:42 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 09 Feb 2022 20:19:17 GMT
ENV ARANGO_VERSION=3.9.0
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.0-1_amd64.deb
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.0-1_amd64.deb
# Wed, 09 Feb 2022 20:19:18 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.0-1_amd64.deb.asc
# Wed, 09 Feb 2022 20:19:44 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 09 Feb 2022 20:19:46 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 09 Feb 2022 20:19:46 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 09 Feb 2022 20:19:46 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 09 Feb 2022 20:19:46 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 09 Feb 2022 20:19:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Feb 2022 20:19:47 GMT
EXPOSE 8529
# Wed, 09 Feb 2022 20:19:47 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02a853c7927a577dfc0ac95ac85249d61600035e0f5cbaaa06c6c4eb946582c`  
		Last Modified: Wed, 09 Feb 2022 20:20:25 GMT  
		Size: 195.0 MB (195038012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d34c0c7faf0c8c16dbf6629b3a2202f3dc4c43008811d594b86833a729ed65`  
		Last Modified: Wed, 09 Feb 2022 20:20:03 GMT  
		Size: 2.1 KB (2084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706c235208c4c929f663f80c4edaf478530749a2c26e2b1d4290d68fe4e2e36a`  
		Last Modified: Wed, 09 Feb 2022 20:20:03 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
