<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.6`](#arangodb36)
-	[`arangodb:3.6.12`](#arangodb3612)
-	[`arangodb:3.7`](#arangodb37)
-	[`arangodb:3.7.10`](#arangodb3710)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.6`

```console
$ docker pull arangodb@sha256:051e6dfdc72a0b724522bd15f20949dc631b6c3179d7e4da07bb7985f9928b62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6` - linux; amd64

```console
$ docker pull arangodb@sha256:601557f98c2992e22035f5d4fc3e6ba89699d6583f445af7a3a133a7d418dd5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119520118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f754fa5128e287451829f7be0633813b9ff37695cb7973d06f2ecd017e8a174`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:25:14 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 06 Mar 2021 07:25:15 GMT
ENV ARANGO_VERSION=3.6.12
# Sat, 06 Mar 2021 07:25:15 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Sat, 06 Mar 2021 07:25:15 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.12-1_amd64.deb
# Sat, 06 Mar 2021 07:25:15 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.12-1_amd64.deb
# Sat, 06 Mar 2021 07:25:15 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.12-1_amd64.deb.asc
# Sat, 06 Mar 2021 07:25:43 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 06 Mar 2021 07:25:44 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 06 Mar 2021 07:25:44 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 06 Mar 2021 07:25:44 GMT
COPY file:0906ed6b024317ae8adc7caf5905c27c8ed6d7c227bbbfd131411e3fb9a6beaa in /entrypoint.sh 
# Sat, 06 Mar 2021 07:25:45 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 06 Mar 2021 07:25:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 06 Mar 2021 07:25:45 GMT
EXPOSE 8529
# Sat, 06 Mar 2021 07:25:45 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a857b9674091016699b78acd58a65032fbbaecbfc8185ed89f91c18d5568987`  
		Last Modified: Sat, 06 Mar 2021 07:26:52 GMT  
		Size: 116.7 MB (116702368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac595b7462206b32b9f568e43d96425c5ae8062f8efa60e4c2004892182f9f4`  
		Last Modified: Sat, 06 Mar 2021 07:26:31 GMT  
		Size: 2.2 KB (2176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dd85654caa75413c2045c5c6c19ce5ade5f16d087263c230ce4d033b75deeb`  
		Last Modified: Sat, 06 Mar 2021 07:26:31 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.6.12`

```console
$ docker pull arangodb@sha256:051e6dfdc72a0b724522bd15f20949dc631b6c3179d7e4da07bb7985f9928b62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.6.12` - linux; amd64

```console
$ docker pull arangodb@sha256:601557f98c2992e22035f5d4fc3e6ba89699d6583f445af7a3a133a7d418dd5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119520118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f754fa5128e287451829f7be0633813b9ff37695cb7973d06f2ecd017e8a174`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:25:14 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 06 Mar 2021 07:25:15 GMT
ENV ARANGO_VERSION=3.6.12
# Sat, 06 Mar 2021 07:25:15 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64
# Sat, 06 Mar 2021 07:25:15 GMT
ENV ARANGO_PACKAGE=arangodb3_3.6.12-1_amd64.deb
# Sat, 06 Mar 2021 07:25:15 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.12-1_amd64.deb
# Sat, 06 Mar 2021 07:25:15 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb36/DEBIAN/amd64/arangodb3_3.6.12-1_amd64.deb.asc
# Sat, 06 Mar 2021 07:25:43 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 06 Mar 2021 07:25:44 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 06 Mar 2021 07:25:44 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 06 Mar 2021 07:25:44 GMT
COPY file:0906ed6b024317ae8adc7caf5905c27c8ed6d7c227bbbfd131411e3fb9a6beaa in /entrypoint.sh 
# Sat, 06 Mar 2021 07:25:45 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 06 Mar 2021 07:25:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 06 Mar 2021 07:25:45 GMT
EXPOSE 8529
# Sat, 06 Mar 2021 07:25:45 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a857b9674091016699b78acd58a65032fbbaecbfc8185ed89f91c18d5568987`  
		Last Modified: Sat, 06 Mar 2021 07:26:52 GMT  
		Size: 116.7 MB (116702368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac595b7462206b32b9f568e43d96425c5ae8062f8efa60e4c2004892182f9f4`  
		Last Modified: Sat, 06 Mar 2021 07:26:31 GMT  
		Size: 2.2 KB (2176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dd85654caa75413c2045c5c6c19ce5ade5f16d087263c230ce4d033b75deeb`  
		Last Modified: Sat, 06 Mar 2021 07:26:31 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7`

```console
$ docker pull arangodb@sha256:80c75afcb850644e919cbf3c015ba6d8c423392ca0b7e9f16a3f137e2430c90f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.7` - linux; amd64

```console
$ docker pull arangodb@sha256:4bf9c5ea0863ba2017b5d70410681af4af48a3f3bce37e27337299d717e4ea3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128354529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bd980968ca12197099ef28cc17cf9c2138af6cf8d122ff3ba06fc554bff84d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:25:14 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_VERSION=3.7.10
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.10-1_amd64.deb
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb.asc
# Fri, 19 Mar 2021 19:39:33 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 19 Mar 2021 19:39:34 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 19 Mar 2021 19:39:34 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 19 Mar 2021 19:39:34 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 19 Mar 2021 19:39:35 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 19 Mar 2021 19:39:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Mar 2021 19:39:35 GMT
EXPOSE 8529
# Fri, 19 Mar 2021 19:39:35 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29327df5bc0434de2d4737e35de6196654c0af3669370072b730a441c38cbbb0`  
		Last Modified: Fri, 19 Mar 2021 19:40:09 GMT  
		Size: 125.5 MB (125536870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ede15edd077c4173d8ffd4c78321f2f759be9797fd5c262fa19b3cf1db55f5e`  
		Last Modified: Fri, 19 Mar 2021 19:39:50 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5183ee4e47deba794201ebd5252ff288419880c28cf8c8060440a46aee5f339a`  
		Last Modified: Fri, 19 Mar 2021 19:39:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.7.10`

```console
$ docker pull arangodb@sha256:80c75afcb850644e919cbf3c015ba6d8c423392ca0b7e9f16a3f137e2430c90f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:3.7.10` - linux; amd64

```console
$ docker pull arangodb@sha256:4bf9c5ea0863ba2017b5d70410681af4af48a3f3bce37e27337299d717e4ea3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128354529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bd980968ca12197099ef28cc17cf9c2138af6cf8d122ff3ba06fc554bff84d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:25:14 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_VERSION=3.7.10
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.10-1_amd64.deb
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb.asc
# Fri, 19 Mar 2021 19:39:33 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 19 Mar 2021 19:39:34 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 19 Mar 2021 19:39:34 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 19 Mar 2021 19:39:34 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 19 Mar 2021 19:39:35 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 19 Mar 2021 19:39:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Mar 2021 19:39:35 GMT
EXPOSE 8529
# Fri, 19 Mar 2021 19:39:35 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29327df5bc0434de2d4737e35de6196654c0af3669370072b730a441c38cbbb0`  
		Last Modified: Fri, 19 Mar 2021 19:40:09 GMT  
		Size: 125.5 MB (125536870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ede15edd077c4173d8ffd4c78321f2f759be9797fd5c262fa19b3cf1db55f5e`  
		Last Modified: Fri, 19 Mar 2021 19:39:50 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5183ee4e47deba794201ebd5252ff288419880c28cf8c8060440a46aee5f339a`  
		Last Modified: Fri, 19 Mar 2021 19:39:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:80c75afcb850644e919cbf3c015ba6d8c423392ca0b7e9f16a3f137e2430c90f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:4bf9c5ea0863ba2017b5d70410681af4af48a3f3bce37e27337299d717e4ea3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128354529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bd980968ca12197099ef28cc17cf9c2138af6cf8d122ff3ba06fc554bff84d2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:25:14 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_VERSION=3.7.10
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_PACKAGE=arangodb3_3.7.10-1_amd64.deb
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb
# Fri, 19 Mar 2021 19:39:09 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb37/DEBIAN/amd64/arangodb3_3.7.10-1_amd64.deb.asc
# Fri, 19 Mar 2021 19:39:33 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli &&     apk del yarn &&     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     echo chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     echo chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 19 Mar 2021 19:39:34 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 19 Mar 2021 19:39:34 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 19 Mar 2021 19:39:34 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 19 Mar 2021 19:39:35 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 19 Mar 2021 19:39:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 19 Mar 2021 19:39:35 GMT
EXPOSE 8529
# Fri, 19 Mar 2021 19:39:35 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29327df5bc0434de2d4737e35de6196654c0af3669370072b730a441c38cbbb0`  
		Last Modified: Fri, 19 Mar 2021 19:40:09 GMT  
		Size: 125.5 MB (125536870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ede15edd077c4173d8ffd4c78321f2f759be9797fd5c262fa19b3cf1db55f5e`  
		Last Modified: Fri, 19 Mar 2021 19:39:50 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5183ee4e47deba794201ebd5252ff288419880c28cf8c8060440a46aee5f339a`  
		Last Modified: Fri, 19 Mar 2021 19:39:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
