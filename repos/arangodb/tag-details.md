<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.15`](#arangodb3615)
-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.14`](#arangodb3714)
-	[`arangodb:3.8`](#arangodb38)
-	[`arangodb:3.8.0`](#arangodb380)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.6`

```console
$ docker pull arangodb@sha256:9c691498b18102e3f5bf5997df612e7612c6bf58b9fef99462611730f9a6bac3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:e106eec9ed7521a9323b929181d375db2c30eae8968034d3ceb3f6ccc5623ba2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (121045304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e2408ee0800f8e983baa05a5765e5427bd5f258deee78c9da226b9e457f0ade`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 20 Jul 2021 18:19:23 GMT
ENV ARANGO_VERSION=3.6.15
# Tue, 20 Jul 2021 18:19:23 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Tue, 20 Jul 2021 18:19:23 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.15-1_amd64.deb
# Tue, 20 Jul 2021 18:19:24 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.15-1_amd64.deb
# Tue, 20 Jul 2021 18:19:24 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.15-1_amd64.deb.asc
# Tue, 20 Jul 2021 18:19:46 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 20 Jul 2021 18:19:48 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 20 Jul 2021 18:19:48 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 20 Jul 2021 18:19:48 GMT
COPY file:0906ed6b024317ae8adc7caf5905c27c8ed6d7c227bbbfd131411e3fb9a6beaa in /entrypoint.sh 
# Tue, 20 Jul 2021 18:19:48 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 20 Jul 2021 18:19:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jul 2021 18:19:49 GMT
EXPOSE 8529
# Tue, 20 Jul 2021 18:19:49 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384b8e58b765f337f3d734494d7ea3e7d40e521dc5787c986fd3affa3817c908`  
		Last Modified: Tue, 20 Jul 2021 18:20:23 GMT  
		Size: 118.2 MB (118226620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eeaded918f209cedad301b30d932c00465bcb371d0a790ffb2ce9fad033408`  
		Last Modified: Tue, 20 Jul 2021 18:20:06 GMT  
		Size: 2.2 KB (2177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d07fe17f901bae079b959a2eed15f430822c3b4e391496eca5abceee136b5bf`  
		Last Modified: Tue, 20 Jul 2021 18:20:06 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.15`

```console
$ docker pull arangodb@sha256:9c691498b18102e3f5bf5997df612e7612c6bf58b9fef99462611730f9a6bac3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.6.15` - linux; amd64

```console
$ docker pull arangodb@sha256:e106eec9ed7521a9323b929181d375db2c30eae8968034d3ceb3f6ccc5623ba2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (121045304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e2408ee0800f8e983baa05a5765e5427bd5f258deee78c9da226b9e457f0ade`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 20 Jul 2021 18:19:23 GMT
ENV ARANGO_VERSION=3.6.15
# Tue, 20 Jul 2021 18:19:23 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Tue, 20 Jul 2021 18:19:23 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.15-1_amd64.deb
# Tue, 20 Jul 2021 18:19:24 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.15-1_amd64.deb
# Tue, 20 Jul 2021 18:19:24 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.15-1_amd64.deb.asc
# Tue, 20 Jul 2021 18:19:46 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 20 Jul 2021 18:19:48 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 20 Jul 2021 18:19:48 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 20 Jul 2021 18:19:48 GMT
COPY file:0906ed6b024317ae8adc7caf5905c27c8ed6d7c227bbbfd131411e3fb9a6beaa in /entrypoint.sh 
# Tue, 20 Jul 2021 18:19:48 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 20 Jul 2021 18:19:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 20 Jul 2021 18:19:49 GMT
EXPOSE 8529
# Tue, 20 Jul 2021 18:19:49 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384b8e58b765f337f3d734494d7ea3e7d40e521dc5787c986fd3affa3817c908`  
		Last Modified: Tue, 20 Jul 2021 18:20:23 GMT  
		Size: 118.2 MB (118226620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eeaded918f209cedad301b30d932c00465bcb371d0a790ffb2ce9fad033408`  
		Last Modified: Tue, 20 Jul 2021 18:20:06 GMT  
		Size: 2.2 KB (2177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d07fe17f901bae079b959a2eed15f430822c3b4e391496eca5abceee136b5bf`  
		Last Modified: Tue, 20 Jul 2021 18:20:06 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7`

```console
$ docker pull arangodb@sha256:9e30b37b2130ab06eec43e7c0cdbd63d640dd1c140703ea1493c8ec617996787
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.7` - linux; amd64

```console
$ docker pull arangodb@sha256:e6d9762166dd4356a31e8f075bb5183061bd698ef65b466d61c53be2e24a36c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129566516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:840975495c66b640a00fae5c33c935a1aaf18c6cc4ee87d822879b999bedd682`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 20 Aug 2021 18:19:25 GMT
ENV ARANGO_VERSION=3.7.14
# Fri, 20 Aug 2021 18:19:25 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Fri, 20 Aug 2021 18:19:25 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.14-1_amd64.deb
# Fri, 20 Aug 2021 18:19:25 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.14-1_amd64.deb
# Fri, 20 Aug 2021 18:19:26 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.14-1_amd64.deb.asc
# Fri, 20 Aug 2021 18:19:51 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 20 Aug 2021 18:19:52 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 20 Aug 2021 18:19:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 20 Aug 2021 18:19:53 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 20 Aug 2021 18:19:53 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 20 Aug 2021 18:19:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Aug 2021 18:19:53 GMT
EXPOSE 8529
# Fri, 20 Aug 2021 18:19:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09f977108a029ff3a9bb4461b40961e2abe741a869c72d3bbc39413fc164fd6`  
		Last Modified: Fri, 20 Aug 2021 18:20:35 GMT  
		Size: 126.7 MB (126747925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566be8092c752d68fa53c5aaf5987f3a8eb4fb2fdcdf38751625bff75b8edcd4`  
		Last Modified: Fri, 20 Aug 2021 18:20:16 GMT  
		Size: 2.1 KB (2084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1f8ea665065343e0eb10f9d0a98afe226cb6e258ec48806c98a6010ef6bda1`  
		Last Modified: Fri, 20 Aug 2021 18:20:16 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7.14`

```console
$ docker pull arangodb@sha256:9e30b37b2130ab06eec43e7c0cdbd63d640dd1c140703ea1493c8ec617996787
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.7.14` - linux; amd64

```console
$ docker pull arangodb@sha256:e6d9762166dd4356a31e8f075bb5183061bd698ef65b466d61c53be2e24a36c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129566516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:840975495c66b640a00fae5c33c935a1aaf18c6cc4ee87d822879b999bedd682`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 20 Aug 2021 18:19:25 GMT
ENV ARANGO_VERSION=3.7.14
# Fri, 20 Aug 2021 18:19:25 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Fri, 20 Aug 2021 18:19:25 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.14-1_amd64.deb
# Fri, 20 Aug 2021 18:19:25 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.14-1_amd64.deb
# Fri, 20 Aug 2021 18:19:26 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.14-1_amd64.deb.asc
# Fri, 20 Aug 2021 18:19:51 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 20 Aug 2021 18:19:52 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 20 Aug 2021 18:19:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 20 Aug 2021 18:19:53 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 20 Aug 2021 18:19:53 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 20 Aug 2021 18:19:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 20 Aug 2021 18:19:53 GMT
EXPOSE 8529
# Fri, 20 Aug 2021 18:19:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09f977108a029ff3a9bb4461b40961e2abe741a869c72d3bbc39413fc164fd6`  
		Last Modified: Fri, 20 Aug 2021 18:20:35 GMT  
		Size: 126.7 MB (126747925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566be8092c752d68fa53c5aaf5987f3a8eb4fb2fdcdf38751625bff75b8edcd4`  
		Last Modified: Fri, 20 Aug 2021 18:20:16 GMT  
		Size: 2.1 KB (2084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1f8ea665065343e0eb10f9d0a98afe226cb6e258ec48806c98a6010ef6bda1`  
		Last Modified: Fri, 20 Aug 2021 18:20:16 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8`

```console
$ docker pull arangodb@sha256:16ab007ac5754142a66190ecafd863cbaafb4b051a41baae2eb0b48cfdcd2d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8` - linux; amd64

```console
$ docker pull arangodb@sha256:62bb282708ba0510a72e50d719de1beb20bd7855bbdcf7f7ead4f9286745a769
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.6 MB (187621388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccf72ccc5db8e8a4c735d6960058ef45cbc095992ab32a2239885389ae3b4d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 27 Jul 2021 22:19:26 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_VERSION=3.8.0
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.0-1_amd64.deb
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.0-1_amd64.deb
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.0-1_amd64.deb.asc
# Tue, 27 Jul 2021 22:19:54 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 27 Jul 2021 22:19:56 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 27 Jul 2021 22:19:56 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 27 Jul 2021 22:19:56 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 27 Jul 2021 22:19:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 27 Jul 2021 22:19:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Jul 2021 22:19:57 GMT
EXPOSE 8529
# Tue, 27 Jul 2021 22:19:57 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f13a1126730804187e7d4fa639e4a3658c0560373e36f0d79bb8919ebd20d6`  
		Last Modified: Tue, 27 Jul 2021 22:20:38 GMT  
		Size: 184.8 MB (184818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34458411efbdaef33dfdfa98a9e71892aaa4df092b944400058954187dd10722`  
		Last Modified: Tue, 27 Jul 2021 22:20:17 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b498c1b7a4ef83dd37b290cec6de264b185db17fff4d2ac9fdc859607ffe67f`  
		Last Modified: Tue, 27 Jul 2021 22:20:17 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8.0`

```console
$ docker pull arangodb@sha256:16ab007ac5754142a66190ecafd863cbaafb4b051a41baae2eb0b48cfdcd2d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8.0` - linux; amd64

```console
$ docker pull arangodb@sha256:62bb282708ba0510a72e50d719de1beb20bd7855bbdcf7f7ead4f9286745a769
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.6 MB (187621388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccf72ccc5db8e8a4c735d6960058ef45cbc095992ab32a2239885389ae3b4d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 27 Jul 2021 22:19:26 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_VERSION=3.8.0
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.0-1_amd64.deb
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.0-1_amd64.deb
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.0-1_amd64.deb.asc
# Tue, 27 Jul 2021 22:19:54 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 27 Jul 2021 22:19:56 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 27 Jul 2021 22:19:56 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 27 Jul 2021 22:19:56 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 27 Jul 2021 22:19:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 27 Jul 2021 22:19:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Jul 2021 22:19:57 GMT
EXPOSE 8529
# Tue, 27 Jul 2021 22:19:57 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f13a1126730804187e7d4fa639e4a3658c0560373e36f0d79bb8919ebd20d6`  
		Last Modified: Tue, 27 Jul 2021 22:20:38 GMT  
		Size: 184.8 MB (184818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34458411efbdaef33dfdfa98a9e71892aaa4df092b944400058954187dd10722`  
		Last Modified: Tue, 27 Jul 2021 22:20:17 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b498c1b7a4ef83dd37b290cec6de264b185db17fff4d2ac9fdc859607ffe67f`  
		Last Modified: Tue, 27 Jul 2021 22:20:17 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:16ab007ac5754142a66190ecafd863cbaafb4b051a41baae2eb0b48cfdcd2d87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:62bb282708ba0510a72e50d719de1beb20bd7855bbdcf7f7ead4f9286745a769
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.6 MB (187621388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bccf72ccc5db8e8a4c735d6960058ef45cbc095992ab32a2239885389ae3b4d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Tue, 27 Jul 2021 22:19:26 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_VERSION=3.8.0
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.0-1_amd64.deb
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.0-1_amd64.deb
# Tue, 27 Jul 2021 22:19:27 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.0-1_amd64.deb.asc
# Tue, 27 Jul 2021 22:19:54 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 27 Jul 2021 22:19:56 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 27 Jul 2021 22:19:56 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 27 Jul 2021 22:19:56 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 27 Jul 2021 22:19:56 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 27 Jul 2021 22:19:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 27 Jul 2021 22:19:57 GMT
EXPOSE 8529
# Tue, 27 Jul 2021 22:19:57 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f13a1126730804187e7d4fa639e4a3658c0560373e36f0d79bb8919ebd20d6`  
		Last Modified: Tue, 27 Jul 2021 22:20:38 GMT  
		Size: 184.8 MB (184818474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34458411efbdaef33dfdfa98a9e71892aaa4df092b944400058954187dd10722`  
		Last Modified: Tue, 27 Jul 2021 22:20:17 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b498c1b7a4ef83dd37b290cec6de264b185db17fff4d2ac9fdc859607ffe67f`  
		Last Modified: Tue, 27 Jul 2021 22:20:17 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
