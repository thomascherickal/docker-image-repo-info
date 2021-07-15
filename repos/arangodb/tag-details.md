<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.14`](#arangodb3614)
-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.12`](#arangodb3712)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.6`

```console
$ docker pull arangodb@sha256:aa32cc1ff50a9241960a5cd565db634c32aec67523399534cb72b163c87d9836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:2115dcd2efa68991f93a733ea84e8548fa7e08e8f3c45490b75ddbdb9437f229
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (121032978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e200a1f377932379b9746ba19e4de88905e35f0c16acb04add3b55eb6c71464`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 28 Jun 2021 18:19:20 GMT
ENV ARANGO_VERSION=3.6.14
# Mon, 28 Jun 2021 18:19:21 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Mon, 28 Jun 2021 18:19:21 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.14-1_amd64.deb
# Mon, 28 Jun 2021 18:19:21 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.14-1_amd64.deb
# Mon, 28 Jun 2021 18:19:21 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.14-1_amd64.deb.asc
# Mon, 28 Jun 2021 18:19:48 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 28 Jun 2021 18:19:49 GMT
ENV GLIBCXX_FORCE_NEW=1
# Mon, 28 Jun 2021 18:19:49 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 28 Jun 2021 18:19:50 GMT
COPY file:0906ed6b024317ae8adc7caf5905c27c8ed6d7c227bbbfd131411e3fb9a6beaa in /entrypoint.sh 
# Mon, 28 Jun 2021 18:19:50 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Mon, 28 Jun 2021 18:19:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Jun 2021 18:19:50 GMT
EXPOSE 8529
# Mon, 28 Jun 2021 18:19:51 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c696ffacae1967cfcfa5271df43010fed59dc59348a5200d7ca7a0101eaf910`  
		Last Modified: Mon, 28 Jun 2021 18:20:27 GMT  
		Size: 118.2 MB (118214295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a871261d4855290f6dd8f750add6c3ba55484dd13a9d77abe0700b40769283f`  
		Last Modified: Mon, 28 Jun 2021 18:20:08 GMT  
		Size: 2.2 KB (2176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5bf7104dce94bd9815591cd6e3ffff28fb8a7ba0649be94f22526fce402813`  
		Last Modified: Mon, 28 Jun 2021 18:20:08 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.14`

```console
$ docker pull arangodb@sha256:aa32cc1ff50a9241960a5cd565db634c32aec67523399534cb72b163c87d9836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.6.14` - linux; amd64

```console
$ docker pull arangodb@sha256:2115dcd2efa68991f93a733ea84e8548fa7e08e8f3c45490b75ddbdb9437f229
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (121032978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e200a1f377932379b9746ba19e4de88905e35f0c16acb04add3b55eb6c71464`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:44:03 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 28 Jun 2021 18:19:20 GMT
ENV ARANGO_VERSION=3.6.14
# Mon, 28 Jun 2021 18:19:21 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Mon, 28 Jun 2021 18:19:21 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.14-1_amd64.deb
# Mon, 28 Jun 2021 18:19:21 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.14-1_amd64.deb
# Mon, 28 Jun 2021 18:19:21 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.14-1_amd64.deb.asc
# Mon, 28 Jun 2021 18:19:48 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 28 Jun 2021 18:19:49 GMT
ENV GLIBCXX_FORCE_NEW=1
# Mon, 28 Jun 2021 18:19:49 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 28 Jun 2021 18:19:50 GMT
COPY file:0906ed6b024317ae8adc7caf5905c27c8ed6d7c227bbbfd131411e3fb9a6beaa in /entrypoint.sh 
# Mon, 28 Jun 2021 18:19:50 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Mon, 28 Jun 2021 18:19:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 28 Jun 2021 18:19:50 GMT
EXPOSE 8529
# Mon, 28 Jun 2021 18:19:51 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c696ffacae1967cfcfa5271df43010fed59dc59348a5200d7ca7a0101eaf910`  
		Last Modified: Mon, 28 Jun 2021 18:20:27 GMT  
		Size: 118.2 MB (118214295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a871261d4855290f6dd8f750add6c3ba55484dd13a9d77abe0700b40769283f`  
		Last Modified: Mon, 28 Jun 2021 18:20:08 GMT  
		Size: 2.2 KB (2176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5bf7104dce94bd9815591cd6e3ffff28fb8a7ba0649be94f22526fce402813`  
		Last Modified: Mon, 28 Jun 2021 18:20:08 GMT  
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
