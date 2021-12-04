<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.16`](#arangodb3716)
-	[`arangodb:3.8`](#arangodb38)
-	[`arangodb:3.8.4`](#arangodb384)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.7`

```console
$ docker pull arangodb@sha256:698d6e77da3e489b90b90e248015971fcbbc8d03b026ecf3f0777b4810d42ff6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.7` - linux; amd64

```console
$ docker pull arangodb@sha256:5f3d7baa1ac1bb1619a0edaf299ab3fe5f6b374822353727a9091d270a4fdc48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129852374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab06ec13d370dc7d8a3bd427355464266ba070c73c43ceeb57cf898b16292a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 23:39:44 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 30 Nov 2021 02:04:38 GMT
ENV ARANGO_VERSION=3.7.16
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.16-1_amd64.deb
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.16-1_amd64.deb
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.16-1_amd64.deb.asc
# Tue, 30 Nov 2021 02:05:08 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 30 Nov 2021 02:05:09 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 30 Nov 2021 02:05:09 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 30 Nov 2021 02:05:10 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 30 Nov 2021 02:05:10 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 30 Nov 2021 02:05:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Nov 2021 02:05:10 GMT
EXPOSE 8529
# Tue, 30 Nov 2021 02:05:10 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326555101505cf4c0cbca4a485745d6347b07afab2743a6613c92206ea93e86a`  
		Last Modified: Tue, 30 Nov 2021 02:05:49 GMT  
		Size: 127.0 MB (127040553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1e8bfc72f79aaecc8c16669712400f2dcd30cd0eb102d53a2ac410d440ad91`  
		Last Modified: Tue, 30 Nov 2021 02:05:28 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d67776f010a857b6e06385539c82f4026a667cd113a26fd360ece160f846e0`  
		Last Modified: Tue, 30 Nov 2021 02:05:28 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7.16`

```console
$ docker pull arangodb@sha256:698d6e77da3e489b90b90e248015971fcbbc8d03b026ecf3f0777b4810d42ff6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.7.16` - linux; amd64

```console
$ docker pull arangodb@sha256:5f3d7baa1ac1bb1619a0edaf299ab3fe5f6b374822353727a9091d270a4fdc48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129852374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab06ec13d370dc7d8a3bd427355464266ba070c73c43ceeb57cf898b16292a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 23:39:44 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Tue, 30 Nov 2021 02:04:38 GMT
ENV ARANGO_VERSION=3.7.16
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.16-1_amd64.deb
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.16-1_amd64.deb
# Tue, 30 Nov 2021 02:04:39 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.16-1_amd64.deb.asc
# Tue, 30 Nov 2021 02:05:08 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Tue, 30 Nov 2021 02:05:09 GMT
ENV GLIBCXX_FORCE_NEW=1
# Tue, 30 Nov 2021 02:05:09 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Tue, 30 Nov 2021 02:05:10 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Tue, 30 Nov 2021 02:05:10 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Tue, 30 Nov 2021 02:05:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 30 Nov 2021 02:05:10 GMT
EXPOSE 8529
# Tue, 30 Nov 2021 02:05:10 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326555101505cf4c0cbca4a485745d6347b07afab2743a6613c92206ea93e86a`  
		Last Modified: Tue, 30 Nov 2021 02:05:49 GMT  
		Size: 127.0 MB (127040553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1e8bfc72f79aaecc8c16669712400f2dcd30cd0eb102d53a2ac410d440ad91`  
		Last Modified: Tue, 30 Nov 2021 02:05:28 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d67776f010a857b6e06385539c82f4026a667cd113a26fd360ece160f846e0`  
		Last Modified: Tue, 30 Nov 2021 02:05:28 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8`

```console
$ docker pull arangodb@sha256:19b63c015a039fafd5e1705d83786377931afdf1adea7c33b6ba3df385a417c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8` - linux; amd64

```console
$ docker pull arangodb@sha256:4b41477b95f65d47d93b48c230d22b9f7f00a85769d3c80d3d33a0871d05c1fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187775382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:110b5bf1d7158166adf4edd1da2d682498251b1b93768f937c78a78b54b1d36d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 23:39:44 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_VERSION=3.8.4
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.4-1_amd64.deb
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.4-1_amd64.deb
# Fri, 03 Dec 2021 23:27:34 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.4-1_amd64.deb.asc
# Fri, 03 Dec 2021 23:28:03 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 03 Dec 2021 23:28:05 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 03 Dec 2021 23:28:05 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 03 Dec 2021 23:28:05 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 03 Dec 2021 23:28:05 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 03 Dec 2021 23:28:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 23:28:06 GMT
EXPOSE 8529
# Fri, 03 Dec 2021 23:28:06 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f317d973024fc02e027e207bbf3d56dd9b4b8deb0194b195aac23b49979dfee`  
		Last Modified: Fri, 03 Dec 2021 23:28:43 GMT  
		Size: 185.0 MB (184963562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7e77ac0f227233e7db80881842d2e52ee61aedbb77f6c540a166fe145c6c7e`  
		Last Modified: Fri, 03 Dec 2021 23:28:22 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66773346014d4517452ffb01285bf2c30ffa80b893c7fd6c1a3756a58351b74b`  
		Last Modified: Fri, 03 Dec 2021 23:28:22 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8.4`

```console
$ docker pull arangodb@sha256:19b63c015a039fafd5e1705d83786377931afdf1adea7c33b6ba3df385a417c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8.4` - linux; amd64

```console
$ docker pull arangodb@sha256:4b41477b95f65d47d93b48c230d22b9f7f00a85769d3c80d3d33a0871d05c1fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187775382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:110b5bf1d7158166adf4edd1da2d682498251b1b93768f937c78a78b54b1d36d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 23:39:44 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_VERSION=3.8.4
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.4-1_amd64.deb
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.4-1_amd64.deb
# Fri, 03 Dec 2021 23:27:34 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.4-1_amd64.deb.asc
# Fri, 03 Dec 2021 23:28:03 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 03 Dec 2021 23:28:05 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 03 Dec 2021 23:28:05 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 03 Dec 2021 23:28:05 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 03 Dec 2021 23:28:05 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 03 Dec 2021 23:28:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 23:28:06 GMT
EXPOSE 8529
# Fri, 03 Dec 2021 23:28:06 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f317d973024fc02e027e207bbf3d56dd9b4b8deb0194b195aac23b49979dfee`  
		Last Modified: Fri, 03 Dec 2021 23:28:43 GMT  
		Size: 185.0 MB (184963562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7e77ac0f227233e7db80881842d2e52ee61aedbb77f6c540a166fe145c6c7e`  
		Last Modified: Fri, 03 Dec 2021 23:28:22 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66773346014d4517452ffb01285bf2c30ffa80b893c7fd6c1a3756a58351b74b`  
		Last Modified: Fri, 03 Dec 2021 23:28:22 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:19b63c015a039fafd5e1705d83786377931afdf1adea7c33b6ba3df385a417c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:4b41477b95f65d47d93b48c230d22b9f7f00a85769d3c80d3d33a0871d05c1fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187775382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:110b5bf1d7158166adf4edd1da2d682498251b1b93768f937c78a78b54b1d36d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 23:39:44 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_VERSION=3.8.4
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.4-1_amd64.deb
# Fri, 03 Dec 2021 23:27:33 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.4-1_amd64.deb
# Fri, 03 Dec 2021 23:27:34 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.4-1_amd64.deb.asc
# Fri, 03 Dec 2021 23:28:03 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 03 Dec 2021 23:28:05 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 03 Dec 2021 23:28:05 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 03 Dec 2021 23:28:05 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 03 Dec 2021 23:28:05 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 03 Dec 2021 23:28:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 23:28:06 GMT
EXPOSE 8529
# Fri, 03 Dec 2021 23:28:06 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f317d973024fc02e027e207bbf3d56dd9b4b8deb0194b195aac23b49979dfee`  
		Last Modified: Fri, 03 Dec 2021 23:28:43 GMT  
		Size: 185.0 MB (184963562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7e77ac0f227233e7db80881842d2e52ee61aedbb77f6c540a166fe145c6c7e`  
		Last Modified: Fri, 03 Dec 2021 23:28:22 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66773346014d4517452ffb01285bf2c30ffa80b893c7fd6c1a3756a58351b74b`  
		Last Modified: Fri, 03 Dec 2021 23:28:22 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
