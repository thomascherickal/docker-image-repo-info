<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.15`](#arangodb3615)
-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.12`](#arangodb3712)
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
$ docker pull arangodb@sha256:975d21be96c8bdf1e5d118562ef1464588d01bceab6146e17c4d13372fba31a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.7` - linux; amd64

```console
$ docker pull arangodb@sha256:1c15453fba3cd543430d01dbafadddc7f6eacce48e81b491df90433be738a72d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129878274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:635481221a47d5a9d9345e29002787db3c2a9dda4b343f2fcef426ffc1fad464`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 18 Jun 2021 22:19:27 GMT
ENV ARANGO_VERSION=3.7.12
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.12-1_amd64.deb
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.12-1_amd64.deb
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.12-1_amd64.deb.asc
# Fri, 18 Jun 2021 22:19:52 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 18 Jun 2021 22:19:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 18 Jun 2021 22:19:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 18 Jun 2021 22:19:54 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 18 Jun 2021 22:19:54 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 18 Jun 2021 22:19:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Jun 2021 22:19:54 GMT
EXPOSE 8529
# Fri, 18 Jun 2021 22:19:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975daedb7a1e98792949426b7fe3af9ed7c8c87d56ecb7ecaf57c9c96cc08cb6`  
		Last Modified: Fri, 18 Jun 2021 22:20:27 GMT  
		Size: 127.1 MB (127059680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766859f2894ed8cb4e3b43d152b8845416de89672466b8dfe1ef303a4c6a34b`  
		Last Modified: Fri, 18 Jun 2021 22:20:08 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a453d96ffa0ea811441602393c544a2754a84b320d0d649e267a31ba7e4ae`  
		Last Modified: Fri, 18 Jun 2021 22:20:08 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7.12`

```console
$ docker pull arangodb@sha256:975d21be96c8bdf1e5d118562ef1464588d01bceab6146e17c4d13372fba31a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.7.12` - linux; amd64

```console
$ docker pull arangodb@sha256:1c15453fba3cd543430d01dbafadddc7f6eacce48e81b491df90433be738a72d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129878274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:635481221a47d5a9d9345e29002787db3c2a9dda4b343f2fcef426ffc1fad464`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 18 Jun 2021 22:19:27 GMT
ENV ARANGO_VERSION=3.7.12
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.12-1_amd64.deb
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.12-1_amd64.deb
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.12-1_amd64.deb.asc
# Fri, 18 Jun 2021 22:19:52 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 18 Jun 2021 22:19:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 18 Jun 2021 22:19:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 18 Jun 2021 22:19:54 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 18 Jun 2021 22:19:54 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 18 Jun 2021 22:19:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Jun 2021 22:19:54 GMT
EXPOSE 8529
# Fri, 18 Jun 2021 22:19:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975daedb7a1e98792949426b7fe3af9ed7c8c87d56ecb7ecaf57c9c96cc08cb6`  
		Last Modified: Fri, 18 Jun 2021 22:20:27 GMT  
		Size: 127.1 MB (127059680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766859f2894ed8cb4e3b43d152b8845416de89672466b8dfe1ef303a4c6a34b`  
		Last Modified: Fri, 18 Jun 2021 22:20:08 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a453d96ffa0ea811441602393c544a2754a84b320d0d649e267a31ba7e4ae`  
		Last Modified: Fri, 18 Jun 2021 22:20:08 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:975d21be96c8bdf1e5d118562ef1464588d01bceab6146e17c4d13372fba31a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:1c15453fba3cd543430d01dbafadddc7f6eacce48e81b491df90433be738a72d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129878274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:635481221a47d5a9d9345e29002787db3c2a9dda4b343f2fcef426ffc1fad464`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 18 Jun 2021 22:19:27 GMT
ENV ARANGO_VERSION=3.7.12
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.12-1_amd64.deb
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.12-1_amd64.deb
# Fri, 18 Jun 2021 22:19:28 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.12-1_amd64.deb.asc
# Fri, 18 Jun 2021 22:19:52 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 18 Jun 2021 22:19:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 18 Jun 2021 22:19:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 18 Jun 2021 22:19:54 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 18 Jun 2021 22:19:54 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 18 Jun 2021 22:19:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 18 Jun 2021 22:19:54 GMT
EXPOSE 8529
# Fri, 18 Jun 2021 22:19:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975daedb7a1e98792949426b7fe3af9ed7c8c87d56ecb7ecaf57c9c96cc08cb6`  
		Last Modified: Fri, 18 Jun 2021 22:20:27 GMT  
		Size: 127.1 MB (127059680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766859f2894ed8cb4e3b43d152b8845416de89672466b8dfe1ef303a4c6a34b`  
		Last Modified: Fri, 18 Jun 2021 22:20:08 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a453d96ffa0ea811441602393c544a2754a84b320d0d649e267a31ba7e4ae`  
		Last Modified: Fri, 18 Jun 2021 22:20:08 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
