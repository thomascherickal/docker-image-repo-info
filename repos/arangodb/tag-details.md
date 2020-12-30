<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.5`](#arangodb35)
-	[`arangodb:3.5.7`](#arangodb357)
-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.10`](#arangodb3610)
-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.5`](#arangodb375)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.5`

```console
$ docker pull arangodb@sha256:76c7ce92b8c81e2be67cff45e5a9529d6814ed723e66d3a11474b29904973ac4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5` - linux; amd64

```console
$ docker pull arangodb@sha256:5b323777db79258d52a29d6d2523b26301b8b9ac96cc7931ce1bae94c76cf1e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118731129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5cdaf303d9f7d876389ef96b70e1968426efdf4f3d6cc4c6a5f0970542752f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:53:15 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 30 Dec 2020 19:19:28 GMT
ENV ARANGO_VERSION=3.5.7
# Wed, 30 Dec 2020 19:19:28 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Wed, 30 Dec 2020 19:19:28 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.7-1_amd64.deb
# Wed, 30 Dec 2020 19:19:29 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.7-1_amd64.deb
# Wed, 30 Dec 2020 19:19:29 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.7-1_amd64.deb.asc
# Wed, 30 Dec 2020 19:19:54 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 30 Dec 2020 19:19:55 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 30 Dec 2020 19:19:55 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 30 Dec 2020 19:19:55 GMT
COPY file:3a0ad717437ce87e5e260280982f3288fcfff74b46a1f17e5cd07f64d64ee5fa in /entrypoint.sh 
# Wed, 30 Dec 2020 19:19:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 30 Dec 2020 19:19:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Dec 2020 19:19:56 GMT
EXPOSE 8529
# Wed, 30 Dec 2020 19:19:56 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f95ba22862cd0ee3e96b284a3e745ef9b947d639f9eaa4515b7475370c82b3d`  
		Last Modified: Wed, 30 Dec 2020 19:20:38 GMT  
		Size: 115.9 MB (115913828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38084f48f1375be6ddc30e4106c4414df98cd0adf78fcbe30b34fb9c1fcaa53f`  
		Last Modified: Wed, 30 Dec 2020 19:20:18 GMT  
		Size: 2.2 KB (2177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e44b50a63325230f8b77b3cb36c9c9091bc003b2869ab8a4efcf13c6900e637`  
		Last Modified: Wed, 30 Dec 2020 19:20:18 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.5.7`

```console
$ docker pull arangodb@sha256:76c7ce92b8c81e2be67cff45e5a9529d6814ed723e66d3a11474b29904973ac4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.5.7` - linux; amd64

```console
$ docker pull arangodb@sha256:5b323777db79258d52a29d6d2523b26301b8b9ac96cc7931ce1bae94c76cf1e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118731129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5cdaf303d9f7d876389ef96b70e1968426efdf4f3d6cc4c6a5f0970542752f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:53:15 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 30 Dec 2020 19:19:28 GMT
ENV ARANGO_VERSION=3.5.7
# Wed, 30 Dec 2020 19:19:28 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64
# Wed, 30 Dec 2020 19:19:28 GMT
ENV ARANGO_PACKAGE=arangodb3_3.5.7-1_amd64.deb
# Wed, 30 Dec 2020 19:19:29 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.7-1_amd64.deb
# Wed, 30 Dec 2020 19:19:29 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb35/DEBIAN/amd64/arangodb3_3.5.7-1_amd64.deb.asc
# Wed, 30 Dec 2020 19:19:54 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 30 Dec 2020 19:19:55 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 30 Dec 2020 19:19:55 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 30 Dec 2020 19:19:55 GMT
COPY file:3a0ad717437ce87e5e260280982f3288fcfff74b46a1f17e5cd07f64d64ee5fa in /entrypoint.sh 
# Wed, 30 Dec 2020 19:19:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 30 Dec 2020 19:19:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Dec 2020 19:19:56 GMT
EXPOSE 8529
# Wed, 30 Dec 2020 19:19:56 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f95ba22862cd0ee3e96b284a3e745ef9b947d639f9eaa4515b7475370c82b3d`  
		Last Modified: Wed, 30 Dec 2020 19:20:38 GMT  
		Size: 115.9 MB (115913828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38084f48f1375be6ddc30e4106c4414df98cd0adf78fcbe30b34fb9c1fcaa53f`  
		Last Modified: Wed, 30 Dec 2020 19:20:18 GMT  
		Size: 2.2 KB (2177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e44b50a63325230f8b77b3cb36c9c9091bc003b2869ab8a4efcf13c6900e637`  
		Last Modified: Wed, 30 Dec 2020 19:20:18 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6`

```console
$ docker pull arangodb@sha256:b6e80bf55f9a1abed0468d34b8049ff17729dea4405f24a30bc95673637f8af4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:3f9c26b20c78227fe6303bdf057e0ecd36d5974a10ecad726d00fd7aaf24f44e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119247048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:beee5392196d1bb53ae2fa0435f59efe08ee4a8b382a0430fcc39f4860a197dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:53:15 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 19 Dec 2020 00:22:04 GMT
ENV ARANGO_VERSION=3.6.10
# Sat, 19 Dec 2020 00:22:04 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Sat, 19 Dec 2020 00:22:05 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.10-1_amd64.deb
# Sat, 19 Dec 2020 00:22:05 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.10-1_amd64.deb
# Sat, 19 Dec 2020 00:22:05 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.10-1_amd64.deb.asc
# Sat, 19 Dec 2020 00:22:30 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 19 Dec 2020 00:22:31 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 19 Dec 2020 00:22:31 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 19 Dec 2020 00:22:32 GMT
COPY file:3a0ad717437ce87e5e260280982f3288fcfff74b46a1f17e5cd07f64d64ee5fa in /entrypoint.sh 
# Sat, 19 Dec 2020 00:22:32 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 19 Dec 2020 00:22:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Dec 2020 00:22:32 GMT
EXPOSE 8529
# Sat, 19 Dec 2020 00:22:32 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cceae571931e17b60c8b1e1a0bffda8e6b2d8eb435bad226e5dabce1450334`  
		Last Modified: Sat, 19 Dec 2020 00:23:11 GMT  
		Size: 116.4 MB (116429742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55272ae18861a7f5abf537861ed40c879186071121da46b4e25ec4f16a7aa074`  
		Last Modified: Sat, 19 Dec 2020 00:22:52 GMT  
		Size: 2.2 KB (2181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b447fc4821672085c5c6586036861852a52a902b183bb145e9a53702278b44`  
		Last Modified: Sat, 19 Dec 2020 00:22:52 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.10`

```console
$ docker pull arangodb@sha256:b6e80bf55f9a1abed0468d34b8049ff17729dea4405f24a30bc95673637f8af4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6.10` - linux; amd64

```console
$ docker pull arangodb@sha256:3f9c26b20c78227fe6303bdf057e0ecd36d5974a10ecad726d00fd7aaf24f44e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119247048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:beee5392196d1bb53ae2fa0435f59efe08ee4a8b382a0430fcc39f4860a197dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:53:15 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 19 Dec 2020 00:22:04 GMT
ENV ARANGO_VERSION=3.6.10
# Sat, 19 Dec 2020 00:22:04 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Sat, 19 Dec 2020 00:22:05 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.10-1_amd64.deb
# Sat, 19 Dec 2020 00:22:05 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.10-1_amd64.deb
# Sat, 19 Dec 2020 00:22:05 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.10-1_amd64.deb.asc
# Sat, 19 Dec 2020 00:22:30 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 19 Dec 2020 00:22:31 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 19 Dec 2020 00:22:31 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 19 Dec 2020 00:22:32 GMT
COPY file:3a0ad717437ce87e5e260280982f3288fcfff74b46a1f17e5cd07f64d64ee5fa in /entrypoint.sh 
# Sat, 19 Dec 2020 00:22:32 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 19 Dec 2020 00:22:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 19 Dec 2020 00:22:32 GMT
EXPOSE 8529
# Sat, 19 Dec 2020 00:22:32 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cceae571931e17b60c8b1e1a0bffda8e6b2d8eb435bad226e5dabce1450334`  
		Last Modified: Sat, 19 Dec 2020 00:23:11 GMT  
		Size: 116.4 MB (116429742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55272ae18861a7f5abf537861ed40c879186071121da46b4e25ec4f16a7aa074`  
		Last Modified: Sat, 19 Dec 2020 00:22:52 GMT  
		Size: 2.2 KB (2181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b447fc4821672085c5c6586036861852a52a902b183bb145e9a53702278b44`  
		Last Modified: Sat, 19 Dec 2020 00:22:52 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7`

```console
$ docker pull arangodb@sha256:b6b87197cf8780ff6b48ffc0320ff277c2bdea94cdba1044bd6a11a0190bec63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.7` - linux; amd64

```console
$ docker pull arangodb@sha256:7c672cfcfa934557eca7e2c7d2aeda2bf17aa53e484d63bbea27fa2886b0f859
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127871737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:658e449d84a02b9ef5381d991bc4896d6240329fae6ba54d7872bcfd7e23a7f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:53:15 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_VERSION=3.7.5
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.5-1_amd64.deb
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.5-1_amd64.deb
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.5-1_amd64.deb.asc
# Thu, 17 Dec 2020 00:54:52 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 17 Dec 2020 00:54:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 17 Dec 2020 00:54:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 17 Dec 2020 00:54:54 GMT
COPY file:3a0ad717437ce87e5e260280982f3288fcfff74b46a1f17e5cd07f64d64ee5fa in /entrypoint.sh 
# Thu, 17 Dec 2020 00:54:54 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 17 Dec 2020 00:54:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:54:54 GMT
EXPOSE 8529
# Thu, 17 Dec 2020 00:54:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65967002b80f430ae8596954d75fd93a36098009e8b34c6be9a4c0090ebcf5bf`  
		Last Modified: Thu, 17 Dec 2020 00:56:47 GMT  
		Size: 125.1 MB (125054433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5813d1695f2fb37735869e8765cc6c1569e1e13e2103a2ef1f7eb1a01fa57a`  
		Last Modified: Thu, 17 Dec 2020 00:56:22 GMT  
		Size: 2.2 KB (2180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e6d1a8ef864d22d7102ba531ed18b49429e7c17e106826a894580e8ef2281`  
		Last Modified: Thu, 17 Dec 2020 00:56:23 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7.5`

```console
$ docker pull arangodb@sha256:b6b87197cf8780ff6b48ffc0320ff277c2bdea94cdba1044bd6a11a0190bec63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.7.5` - linux; amd64

```console
$ docker pull arangodb@sha256:7c672cfcfa934557eca7e2c7d2aeda2bf17aa53e484d63bbea27fa2886b0f859
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127871737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:658e449d84a02b9ef5381d991bc4896d6240329fae6ba54d7872bcfd7e23a7f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:53:15 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_VERSION=3.7.5
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.5-1_amd64.deb
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.5-1_amd64.deb
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.5-1_amd64.deb.asc
# Thu, 17 Dec 2020 00:54:52 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 17 Dec 2020 00:54:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 17 Dec 2020 00:54:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 17 Dec 2020 00:54:54 GMT
COPY file:3a0ad717437ce87e5e260280982f3288fcfff74b46a1f17e5cd07f64d64ee5fa in /entrypoint.sh 
# Thu, 17 Dec 2020 00:54:54 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 17 Dec 2020 00:54:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:54:54 GMT
EXPOSE 8529
# Thu, 17 Dec 2020 00:54:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65967002b80f430ae8596954d75fd93a36098009e8b34c6be9a4c0090ebcf5bf`  
		Last Modified: Thu, 17 Dec 2020 00:56:47 GMT  
		Size: 125.1 MB (125054433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5813d1695f2fb37735869e8765cc6c1569e1e13e2103a2ef1f7eb1a01fa57a`  
		Last Modified: Thu, 17 Dec 2020 00:56:22 GMT  
		Size: 2.2 KB (2180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e6d1a8ef864d22d7102ba531ed18b49429e7c17e106826a894580e8ef2281`  
		Last Modified: Thu, 17 Dec 2020 00:56:23 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:b6b87197cf8780ff6b48ffc0320ff277c2bdea94cdba1044bd6a11a0190bec63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:7c672cfcfa934557eca7e2c7d2aeda2bf17aa53e484d63bbea27fa2886b0f859
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127871737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:658e449d84a02b9ef5381d991bc4896d6240329fae6ba54d7872bcfd7e23a7f6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:53:15 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_VERSION=3.7.5
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.5-1_amd64.deb
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.5-1_amd64.deb
# Thu, 17 Dec 2020 00:54:24 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.5-1_amd64.deb.asc
# Thu, 17 Dec 2020 00:54:52 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 17 Dec 2020 00:54:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 17 Dec 2020 00:54:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 17 Dec 2020 00:54:54 GMT
COPY file:3a0ad717437ce87e5e260280982f3288fcfff74b46a1f17e5cd07f64d64ee5fa in /entrypoint.sh 
# Thu, 17 Dec 2020 00:54:54 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 17 Dec 2020 00:54:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 00:54:54 GMT
EXPOSE 8529
# Thu, 17 Dec 2020 00:54:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65967002b80f430ae8596954d75fd93a36098009e8b34c6be9a4c0090ebcf5bf`  
		Last Modified: Thu, 17 Dec 2020 00:56:47 GMT  
		Size: 125.1 MB (125054433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5813d1695f2fb37735869e8765cc6c1569e1e13e2103a2ef1f7eb1a01fa57a`  
		Last Modified: Thu, 17 Dec 2020 00:56:22 GMT  
		Size: 2.2 KB (2180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e6d1a8ef864d22d7102ba531ed18b49429e7c17e106826a894580e8ef2281`  
		Last Modified: Thu, 17 Dec 2020 00:56:23 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
