<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.13`](#arangodb3613)
-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.10`](#arangodb3710)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.6`

```console
$ docker pull arangodb@sha256:2e86525171bc8af6ff013471403f3d9817dbb2ca88b837619566dea40b5f4780
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:d92e6b8a211ee61fea0da0eded3d45a51335d4dcf302bd95fc322924d8ba52f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.6 MB (119563708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6598bc0ce89a8e16bfb7d6625b773126eea4e5a3a86de41ea91fc0f3d035d2f4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 15 Apr 2021 09:30:13 GMT
ENV ARANGO_VERSION=3.6.13
# Thu, 15 Apr 2021 09:30:13 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Thu, 15 Apr 2021 09:30:14 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.13-1_amd64.deb
# Thu, 15 Apr 2021 09:30:14 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.13-1_amd64.deb
# Thu, 15 Apr 2021 09:30:14 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.13-1_amd64.deb.asc
# Thu, 15 Apr 2021 09:30:37 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 15 Apr 2021 09:30:39 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 15 Apr 2021 09:30:39 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 15 Apr 2021 09:30:39 GMT
COPY file:0906ed6b024317ae8adc7caf5905c27c8ed6d7c227bbbfd131411e3fb9a6beaa in /entrypoint.sh 
# Thu, 15 Apr 2021 09:30:39 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 15 Apr 2021 09:30:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 09:30:40 GMT
EXPOSE 8529
# Thu, 15 Apr 2021 09:30:40 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eed2fe9f289355b9a77566e86e34a2d8e522dd59b758c2ded308d79a718322`  
		Last Modified: Thu, 15 Apr 2021 09:31:18 GMT  
		Size: 116.7 MB (116745026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa217f79c53f8a438634be05e228d193a51a4629ec9e082238af6092790cc02d`  
		Last Modified: Thu, 15 Apr 2021 09:30:55 GMT  
		Size: 2.2 KB (2176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d8a2d2b6f65ced5f70bf0474148aad1e03031d963f13539f3eabdf847127c0`  
		Last Modified: Thu, 15 Apr 2021 09:30:55 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.13`

```console
$ docker pull arangodb@sha256:2e86525171bc8af6ff013471403f3d9817dbb2ca88b837619566dea40b5f4780
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6.13` - linux; amd64

```console
$ docker pull arangodb@sha256:d92e6b8a211ee61fea0da0eded3d45a51335d4dcf302bd95fc322924d8ba52f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.6 MB (119563708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6598bc0ce89a8e16bfb7d6625b773126eea4e5a3a86de41ea91fc0f3d035d2f4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 15 Apr 2021 09:30:13 GMT
ENV ARANGO_VERSION=3.6.13
# Thu, 15 Apr 2021 09:30:13 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Thu, 15 Apr 2021 09:30:14 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.13-1_amd64.deb
# Thu, 15 Apr 2021 09:30:14 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.13-1_amd64.deb
# Thu, 15 Apr 2021 09:30:14 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.13-1_amd64.deb.asc
# Thu, 15 Apr 2021 09:30:37 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 15 Apr 2021 09:30:39 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 15 Apr 2021 09:30:39 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 15 Apr 2021 09:30:39 GMT
COPY file:0906ed6b024317ae8adc7caf5905c27c8ed6d7c227bbbfd131411e3fb9a6beaa in /entrypoint.sh 
# Thu, 15 Apr 2021 09:30:39 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 15 Apr 2021 09:30:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Apr 2021 09:30:40 GMT
EXPOSE 8529
# Thu, 15 Apr 2021 09:30:40 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eed2fe9f289355b9a77566e86e34a2d8e522dd59b758c2ded308d79a718322`  
		Last Modified: Thu, 15 Apr 2021 09:31:18 GMT  
		Size: 116.7 MB (116745026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa217f79c53f8a438634be05e228d193a51a4629ec9e082238af6092790cc02d`  
		Last Modified: Thu, 15 Apr 2021 09:30:55 GMT  
		Size: 2.2 KB (2176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d8a2d2b6f65ced5f70bf0474148aad1e03031d963f13539f3eabdf847127c0`  
		Last Modified: Thu, 15 Apr 2021 09:30:55 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7`

```console
$ docker pull arangodb@sha256:c519a3f0cdc04b383ab427ad2e769a1ecd39a60adf05dd459554e41de67654d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.7` - linux; amd64

```console
$ docker pull arangodb@sha256:3a2c10697caa3cfaf5831ff771ec8cc1c271fcf81d2a8a353b8b46f0c357da97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128386282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1130753b4a5e75111406446cb6b646b35cf0830e589e86d443ffd0d2a1ad71e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 14 Apr 2021 19:45:02 GMT
ENV ARANGO_VERSION=3.7.10
# Wed, 14 Apr 2021 19:45:02 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Wed, 14 Apr 2021 19:45:02 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.10-1_amd64.deb
# Wed, 14 Apr 2021 19:45:03 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb
# Wed, 14 Apr 2021 19:45:03 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb.asc
# Wed, 14 Apr 2021 19:45:41 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 14 Apr 2021 19:45:42 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 14 Apr 2021 19:45:43 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 14 Apr 2021 19:45:43 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 14 Apr 2021 19:45:43 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 14 Apr 2021 19:45:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 19:45:43 GMT
EXPOSE 8529
# Wed, 14 Apr 2021 19:45:44 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db830100c0602347f966a608b628ae77e0167757cce1d49b800d8c7c6d0e6c3d`  
		Last Modified: Wed, 14 Apr 2021 19:47:03 GMT  
		Size: 125.6 MB (125567688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0feac9b4154be9a863e5c72b916a17ca2760b2ccef40d6d4846e1c0d923582`  
		Last Modified: Wed, 14 Apr 2021 19:46:36 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9493159ae1173b155266563486d5f041617f6c96e4f4ce76ab7e14800d7a6c`  
		Last Modified: Wed, 14 Apr 2021 19:46:36 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7.10`

```console
$ docker pull arangodb@sha256:c519a3f0cdc04b383ab427ad2e769a1ecd39a60adf05dd459554e41de67654d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.7.10` - linux; amd64

```console
$ docker pull arangodb@sha256:3a2c10697caa3cfaf5831ff771ec8cc1c271fcf81d2a8a353b8b46f0c357da97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128386282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1130753b4a5e75111406446cb6b646b35cf0830e589e86d443ffd0d2a1ad71e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 14 Apr 2021 19:45:02 GMT
ENV ARANGO_VERSION=3.7.10
# Wed, 14 Apr 2021 19:45:02 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Wed, 14 Apr 2021 19:45:02 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.10-1_amd64.deb
# Wed, 14 Apr 2021 19:45:03 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb
# Wed, 14 Apr 2021 19:45:03 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb.asc
# Wed, 14 Apr 2021 19:45:41 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 14 Apr 2021 19:45:42 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 14 Apr 2021 19:45:43 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 14 Apr 2021 19:45:43 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 14 Apr 2021 19:45:43 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 14 Apr 2021 19:45:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 19:45:43 GMT
EXPOSE 8529
# Wed, 14 Apr 2021 19:45:44 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db830100c0602347f966a608b628ae77e0167757cce1d49b800d8c7c6d0e6c3d`  
		Last Modified: Wed, 14 Apr 2021 19:47:03 GMT  
		Size: 125.6 MB (125567688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0feac9b4154be9a863e5c72b916a17ca2760b2ccef40d6d4846e1c0d923582`  
		Last Modified: Wed, 14 Apr 2021 19:46:36 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9493159ae1173b155266563486d5f041617f6c96e4f4ce76ab7e14800d7a6c`  
		Last Modified: Wed, 14 Apr 2021 19:46:36 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:c519a3f0cdc04b383ab427ad2e769a1ecd39a60adf05dd459554e41de67654d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:3a2c10697caa3cfaf5831ff771ec8cc1c271fcf81d2a8a353b8b46f0c357da97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128386282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1130753b4a5e75111406446cb6b646b35cf0830e589e86d443ffd0d2a1ad71e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 14 Apr 2021 19:45:02 GMT
ENV ARANGO_VERSION=3.7.10
# Wed, 14 Apr 2021 19:45:02 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Wed, 14 Apr 2021 19:45:02 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.10-1_amd64.deb
# Wed, 14 Apr 2021 19:45:03 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb
# Wed, 14 Apr 2021 19:45:03 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb.asc
# Wed, 14 Apr 2021 19:45:41 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 14 Apr 2021 19:45:42 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 14 Apr 2021 19:45:43 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 14 Apr 2021 19:45:43 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 14 Apr 2021 19:45:43 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 14 Apr 2021 19:45:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 19:45:43 GMT
EXPOSE 8529
# Wed, 14 Apr 2021 19:45:44 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db830100c0602347f966a608b628ae77e0167757cce1d49b800d8c7c6d0e6c3d`  
		Last Modified: Wed, 14 Apr 2021 19:47:03 GMT  
		Size: 125.6 MB (125567688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0feac9b4154be9a863e5c72b916a17ca2760b2ccef40d6d4846e1c0d923582`  
		Last Modified: Wed, 14 Apr 2021 19:46:36 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9493159ae1173b155266563486d5f041617f6c96e4f4ce76ab7e14800d7a6c`  
		Last Modified: Wed, 14 Apr 2021 19:46:36 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
