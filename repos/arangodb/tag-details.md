<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.10`](#arangodb310)
-	[`arangodb:3.10.10`](#arangodb31010)
-	[`arangodb:3.11`](#arangodb311)
-	[`arangodb:3.11.3`](#arangodb3113)
-	[`arangodb:3.9`](#arangodb39)
-	[`arangodb:3.9.12`](#arangodb3912)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.10`

```console
$ docker pull arangodb@sha256:6f7711e4288a92254817e77736afaa9d45be4efa371e8517e61e3c67d6cfa25c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10` - linux; amd64

```console
$ docker pull arangodb@sha256:424ef6a85329477a444b54967ea9746416261a84027eb92fc9907b8109b14c0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.7 MB (226744266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600c0e566e9251ebca9d9c4699977968f38e48f02071a27f6151d22850681021`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:01:27 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 21 Aug 2023 19:19:31 GMT
ENV ARANGO_VERSION=3.10.10
# Mon, 21 Aug 2023 19:19:56 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 21 Aug 2023 19:19:58 GMT
ENV GLIBCXX_FORCE_NEW=1
# Mon, 21 Aug 2023 19:19:58 GMT
RUN echo "UTC" > /etc/timezone
# Mon, 21 Aug 2023 19:19:58 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 21 Aug 2023 19:19:58 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Mon, 21 Aug 2023 19:19:59 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Mon, 21 Aug 2023 19:19:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 21 Aug 2023 19:19:59 GMT
EXPOSE 8529
# Mon, 21 Aug 2023 19:19:59 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae398ef6901e4172e9d8bfd4d62f0d7b112f439a63f4301a411f0f1efacde88`  
		Last Modified: Mon, 21 Aug 2023 19:20:41 GMT  
		Size: 223.9 MB (223934098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8b3246fcccaaa1b3d29d73261a94a892d7cd4f333effa106766bc0e977fa82`  
		Last Modified: Mon, 21 Aug 2023 19:20:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9704714408ea2be75f35013744819901bf86066a417647cb46366d23fab875`  
		Last Modified: Mon, 21 Aug 2023 19:20:17 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3137eb4955e4dba15333ece4d3d56b3b53728a495949b0479f4b76fe68d70911`  
		Last Modified: Mon, 21 Aug 2023 19:20:17 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:b607323009dd9978b531a0cdbc35a042d28f0006bd7d15f4b2530b1679d0b312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221711843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600684ab3da573d28a906134e6a6c1220bd97aff7994e4fb375ceea79924fb7b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:49:17 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 21 Aug 2023 19:40:31 GMT
ENV ARANGO_VERSION=3.10.10
# Mon, 21 Aug 2023 19:41:02 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 21 Aug 2023 19:41:06 GMT
ENV GLIBCXX_FORCE_NEW=1
# Mon, 21 Aug 2023 19:41:06 GMT
RUN echo "UTC" > /etc/timezone
# Mon, 21 Aug 2023 19:41:06 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 21 Aug 2023 19:41:06 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Mon, 21 Aug 2023 19:41:06 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Mon, 21 Aug 2023 19:41:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 21 Aug 2023 19:41:07 GMT
EXPOSE 8529
# Mon, 21 Aug 2023 19:41:07 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89002c5ef1b82dbaac8f16649adebbad02e242fcadacb44b2c62822d0c5f5836`  
		Last Modified: Mon, 21 Aug 2023 19:41:36 GMT  
		Size: 219.0 MB (219001332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f82c2aac4963a58b5832844f8618ca3b0019d5ab1281177bd3566c40e9c28c2`  
		Last Modified: Mon, 21 Aug 2023 19:41:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3134033bba2cf7fd148ad96f8f574330c747d9530b41de735eaee526b49ef27c`  
		Last Modified: Mon, 21 Aug 2023 19:41:18 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be72d85d599f281a01080cb6093fab0995d2f677e49aa5162e6d568b656552d`  
		Last Modified: Mon, 21 Aug 2023 19:41:18 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.10.10`

```console
$ docker pull arangodb@sha256:6f7711e4288a92254817e77736afaa9d45be4efa371e8517e61e3c67d6cfa25c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10.10` - linux; amd64

```console
$ docker pull arangodb@sha256:424ef6a85329477a444b54967ea9746416261a84027eb92fc9907b8109b14c0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.7 MB (226744266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600c0e566e9251ebca9d9c4699977968f38e48f02071a27f6151d22850681021`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:01:27 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 21 Aug 2023 19:19:31 GMT
ENV ARANGO_VERSION=3.10.10
# Mon, 21 Aug 2023 19:19:56 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 21 Aug 2023 19:19:58 GMT
ENV GLIBCXX_FORCE_NEW=1
# Mon, 21 Aug 2023 19:19:58 GMT
RUN echo "UTC" > /etc/timezone
# Mon, 21 Aug 2023 19:19:58 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 21 Aug 2023 19:19:58 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Mon, 21 Aug 2023 19:19:59 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Mon, 21 Aug 2023 19:19:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 21 Aug 2023 19:19:59 GMT
EXPOSE 8529
# Mon, 21 Aug 2023 19:19:59 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae398ef6901e4172e9d8bfd4d62f0d7b112f439a63f4301a411f0f1efacde88`  
		Last Modified: Mon, 21 Aug 2023 19:20:41 GMT  
		Size: 223.9 MB (223934098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8b3246fcccaaa1b3d29d73261a94a892d7cd4f333effa106766bc0e977fa82`  
		Last Modified: Mon, 21 Aug 2023 19:20:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9704714408ea2be75f35013744819901bf86066a417647cb46366d23fab875`  
		Last Modified: Mon, 21 Aug 2023 19:20:17 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3137eb4955e4dba15333ece4d3d56b3b53728a495949b0479f4b76fe68d70911`  
		Last Modified: Mon, 21 Aug 2023 19:20:17 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10.10` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:b607323009dd9978b531a0cdbc35a042d28f0006bd7d15f4b2530b1679d0b312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221711843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600684ab3da573d28a906134e6a6c1220bd97aff7994e4fb375ceea79924fb7b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:49:17 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 21 Aug 2023 19:40:31 GMT
ENV ARANGO_VERSION=3.10.10
# Mon, 21 Aug 2023 19:41:02 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 21 Aug 2023 19:41:06 GMT
ENV GLIBCXX_FORCE_NEW=1
# Mon, 21 Aug 2023 19:41:06 GMT
RUN echo "UTC" > /etc/timezone
# Mon, 21 Aug 2023 19:41:06 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 21 Aug 2023 19:41:06 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Mon, 21 Aug 2023 19:41:06 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Mon, 21 Aug 2023 19:41:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 21 Aug 2023 19:41:07 GMT
EXPOSE 8529
# Mon, 21 Aug 2023 19:41:07 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89002c5ef1b82dbaac8f16649adebbad02e242fcadacb44b2c62822d0c5f5836`  
		Last Modified: Mon, 21 Aug 2023 19:41:36 GMT  
		Size: 219.0 MB (219001332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f82c2aac4963a58b5832844f8618ca3b0019d5ab1281177bd3566c40e9c28c2`  
		Last Modified: Mon, 21 Aug 2023 19:41:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3134033bba2cf7fd148ad96f8f574330c747d9530b41de735eaee526b49ef27c`  
		Last Modified: Mon, 21 Aug 2023 19:41:18 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be72d85d599f281a01080cb6093fab0995d2f677e49aa5162e6d568b656552d`  
		Last Modified: Mon, 21 Aug 2023 19:41:18 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.11`

```console
$ docker pull arangodb@sha256:cc7c3240ef734aae4dacb39d033b2a5b2314537538d433b632a2fe401639c6e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.11` - linux; amd64

```console
$ docker pull arangodb@sha256:085b45e8c56d5d4114e409482694d40fc8d1678c6b5d98d774bab31193034d6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246850504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183452951676a6d90d93eb3f66cd5e7402cf498c0b2d246efc8b4aae2d4ddc41`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:01:27 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 23 Aug 2023 20:19:28 GMT
ENV ARANGO_VERSION=3.11.3
# Wed, 23 Aug 2023 20:19:57 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 23 Aug 2023 20:19:58 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 23 Aug 2023 20:19:59 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 23 Aug 2023 20:19:59 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 23 Aug 2023 20:19:59 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 23 Aug 2023 20:19:59 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 23 Aug 2023 20:19:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Aug 2023 20:19:59 GMT
EXPOSE 8529
# Wed, 23 Aug 2023 20:19:59 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645ad15a725a0c9072260aec5247a42252584953ce2aafaa60190f4355eb9f6a`  
		Last Modified: Wed, 23 Aug 2023 20:20:37 GMT  
		Size: 244.0 MB (244040336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a686aa678f013782e34d27e4103937fe35253ba1b18b7a5793d0ae2e73321fa`  
		Last Modified: Wed, 23 Aug 2023 20:20:11 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4089e6ea3be15277246a38813a053532502eafe3be28df06a94131a4e57452d8`  
		Last Modified: Wed, 23 Aug 2023 20:20:11 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da43f6b1468d05814316eadb10cb5d9b204ee05a0d1e1914fa7c29f9620cc898`  
		Last Modified: Wed, 23 Aug 2023 20:20:11 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.11` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:49803e8e3b052c61e85e34a44a2b2a52ee3c44df22e04d4c74fee8a4d9b83a4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.1 MB (241128530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5271b65694ee7c8eadf25096340e567c4060291d17f5f9c3a5c94a6f458eb23f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:49:17 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 23 Aug 2023 19:39:17 GMT
ENV ARANGO_VERSION=3.11.3
# Wed, 23 Aug 2023 19:39:45 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 23 Aug 2023 19:39:49 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 23 Aug 2023 19:39:49 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 23 Aug 2023 19:39:49 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 23 Aug 2023 19:39:50 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 23 Aug 2023 19:39:50 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 23 Aug 2023 19:39:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Aug 2023 19:39:50 GMT
EXPOSE 8529
# Wed, 23 Aug 2023 19:39:50 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e634dac6be770d49f166f9a458788f8b4200e647b495b41fe32882c9ba9ca798`  
		Last Modified: Wed, 23 Aug 2023 19:40:23 GMT  
		Size: 238.4 MB (238418021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf1015a9de00cd94a01c03bee21a804c6512192a95d0edddfd6641f9696ef91`  
		Last Modified: Wed, 23 Aug 2023 19:40:04 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4d060b501907de308ea18ca0b473b33f5074b258d5e1789d54ab7b60af3cbc`  
		Last Modified: Wed, 23 Aug 2023 19:40:04 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e01148f6b31155b0556f41e483075d733542d6585b907b024a16ed53bfa5f4`  
		Last Modified: Wed, 23 Aug 2023 19:40:05 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.11.3`

```console
$ docker pull arangodb@sha256:cc7c3240ef734aae4dacb39d033b2a5b2314537538d433b632a2fe401639c6e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.11.3` - linux; amd64

```console
$ docker pull arangodb@sha256:085b45e8c56d5d4114e409482694d40fc8d1678c6b5d98d774bab31193034d6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246850504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183452951676a6d90d93eb3f66cd5e7402cf498c0b2d246efc8b4aae2d4ddc41`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:01:27 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 23 Aug 2023 20:19:28 GMT
ENV ARANGO_VERSION=3.11.3
# Wed, 23 Aug 2023 20:19:57 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 23 Aug 2023 20:19:58 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 23 Aug 2023 20:19:59 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 23 Aug 2023 20:19:59 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 23 Aug 2023 20:19:59 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 23 Aug 2023 20:19:59 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 23 Aug 2023 20:19:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Aug 2023 20:19:59 GMT
EXPOSE 8529
# Wed, 23 Aug 2023 20:19:59 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645ad15a725a0c9072260aec5247a42252584953ce2aafaa60190f4355eb9f6a`  
		Last Modified: Wed, 23 Aug 2023 20:20:37 GMT  
		Size: 244.0 MB (244040336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a686aa678f013782e34d27e4103937fe35253ba1b18b7a5793d0ae2e73321fa`  
		Last Modified: Wed, 23 Aug 2023 20:20:11 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4089e6ea3be15277246a38813a053532502eafe3be28df06a94131a4e57452d8`  
		Last Modified: Wed, 23 Aug 2023 20:20:11 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da43f6b1468d05814316eadb10cb5d9b204ee05a0d1e1914fa7c29f9620cc898`  
		Last Modified: Wed, 23 Aug 2023 20:20:11 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.11.3` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:49803e8e3b052c61e85e34a44a2b2a52ee3c44df22e04d4c74fee8a4d9b83a4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.1 MB (241128530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5271b65694ee7c8eadf25096340e567c4060291d17f5f9c3a5c94a6f458eb23f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:49:17 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 23 Aug 2023 19:39:17 GMT
ENV ARANGO_VERSION=3.11.3
# Wed, 23 Aug 2023 19:39:45 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 23 Aug 2023 19:39:49 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 23 Aug 2023 19:39:49 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 23 Aug 2023 19:39:49 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 23 Aug 2023 19:39:50 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 23 Aug 2023 19:39:50 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 23 Aug 2023 19:39:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Aug 2023 19:39:50 GMT
EXPOSE 8529
# Wed, 23 Aug 2023 19:39:50 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e634dac6be770d49f166f9a458788f8b4200e647b495b41fe32882c9ba9ca798`  
		Last Modified: Wed, 23 Aug 2023 19:40:23 GMT  
		Size: 238.4 MB (238418021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf1015a9de00cd94a01c03bee21a804c6512192a95d0edddfd6641f9696ef91`  
		Last Modified: Wed, 23 Aug 2023 19:40:04 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4d060b501907de308ea18ca0b473b33f5074b258d5e1789d54ab7b60af3cbc`  
		Last Modified: Wed, 23 Aug 2023 19:40:04 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e01148f6b31155b0556f41e483075d733542d6585b907b024a16ed53bfa5f4`  
		Last Modified: Wed, 23 Aug 2023 19:40:05 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9`

```console
$ docker pull arangodb@sha256:48444fecfbd47c46b39273e285eabfd0d4bc38c0e663cf290f9859fb1258dd7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9` - linux; amd64

```console
$ docker pull arangodb@sha256:b684ee4696aaa277213b729dbfc97523c069b30adb27d6f3c083f3362715ff13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.3 MB (205259056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a828c1780a3534212e7e84822bda377579c8c05f4aaaebf925a95074089f5809`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:00:53 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Mon, 07 Aug 2023 20:00:53 GMT
ENV ARANGO_VERSION=3.9.11
# Mon, 07 Aug 2023 20:00:53 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Mon, 07 Aug 2023 20:00:53 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.11-1_amd64.deb
# Mon, 07 Aug 2023 20:00:53 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.11-1_amd64.deb
# Mon, 07 Aug 2023 20:00:53 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.11-1_amd64.deb.asc
# Mon, 07 Aug 2023 20:01:21 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Mon, 07 Aug 2023 20:01:22 GMT
ENV GLIBCXX_FORCE_NEW=1
# Mon, 07 Aug 2023 20:01:23 GMT
RUN echo "UTC" > /etc/timezone
# Mon, 07 Aug 2023 20:01:23 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Mon, 07 Aug 2023 20:01:23 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Mon, 07 Aug 2023 20:01:23 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Mon, 07 Aug 2023 20:01:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 07 Aug 2023 20:01:23 GMT
EXPOSE 8529
# Mon, 07 Aug 2023 20:01:23 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c566ea949470dfa5a39d8cbab7a2eeaac8bcea317ac08e61baab3ab187f0d7`  
		Last Modified: Mon, 07 Aug 2023 20:03:11 GMT  
		Size: 202.4 MB (202430564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d76fe7b5c0012d15f8beb4f1bb4e1f8e8e6b84c6b380586a6692649ce4f84b`  
		Last Modified: Mon, 07 Aug 2023 20:02:45 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e2ece5d15da38fd51256f56856f25ff1fd57932f14ee1ab28d79fbab87fdd`  
		Last Modified: Mon, 07 Aug 2023 20:02:45 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04056651227117636854c720f1abe7d7b7a1e360324af9e192bed188a33cbc40`  
		Last Modified: Mon, 07 Aug 2023 20:02:45 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9.12`

**does not exist** (yet?)

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:cc7c3240ef734aae4dacb39d033b2a5b2314537538d433b632a2fe401639c6e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:085b45e8c56d5d4114e409482694d40fc8d1678c6b5d98d774bab31193034d6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246850504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183452951676a6d90d93eb3f66cd5e7402cf498c0b2d246efc8b4aae2d4ddc41`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:01:27 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 23 Aug 2023 20:19:28 GMT
ENV ARANGO_VERSION=3.11.3
# Wed, 23 Aug 2023 20:19:57 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 23 Aug 2023 20:19:58 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 23 Aug 2023 20:19:59 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 23 Aug 2023 20:19:59 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 23 Aug 2023 20:19:59 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 23 Aug 2023 20:19:59 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 23 Aug 2023 20:19:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Aug 2023 20:19:59 GMT
EXPOSE 8529
# Wed, 23 Aug 2023 20:19:59 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645ad15a725a0c9072260aec5247a42252584953ce2aafaa60190f4355eb9f6a`  
		Last Modified: Wed, 23 Aug 2023 20:20:37 GMT  
		Size: 244.0 MB (244040336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a686aa678f013782e34d27e4103937fe35253ba1b18b7a5793d0ae2e73321fa`  
		Last Modified: Wed, 23 Aug 2023 20:20:11 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4089e6ea3be15277246a38813a053532502eafe3be28df06a94131a4e57452d8`  
		Last Modified: Wed, 23 Aug 2023 20:20:11 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da43f6b1468d05814316eadb10cb5d9b204ee05a0d1e1914fa7c29f9620cc898`  
		Last Modified: Wed, 23 Aug 2023 20:20:11 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:latest` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:49803e8e3b052c61e85e34a44a2b2a52ee3c44df22e04d4c74fee8a4d9b83a4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.1 MB (241128530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5271b65694ee7c8eadf25096340e567c4060291d17f5f9c3a5c94a6f458eb23f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:49:17 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 23 Aug 2023 19:39:17 GMT
ENV ARANGO_VERSION=3.11.3
# Wed, 23 Aug 2023 19:39:45 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 23 Aug 2023 19:39:49 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 23 Aug 2023 19:39:49 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 23 Aug 2023 19:39:49 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 23 Aug 2023 19:39:50 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 23 Aug 2023 19:39:50 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 23 Aug 2023 19:39:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 23 Aug 2023 19:39:50 GMT
EXPOSE 8529
# Wed, 23 Aug 2023 19:39:50 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e634dac6be770d49f166f9a458788f8b4200e647b495b41fe32882c9ba9ca798`  
		Last Modified: Wed, 23 Aug 2023 19:40:23 GMT  
		Size: 238.4 MB (238418021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf1015a9de00cd94a01c03bee21a804c6512192a95d0edddfd6641f9696ef91`  
		Last Modified: Wed, 23 Aug 2023 19:40:04 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4d060b501907de308ea18ca0b473b33f5074b258d5e1789d54ab7b60af3cbc`  
		Last Modified: Wed, 23 Aug 2023 19:40:04 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e01148f6b31155b0556f41e483075d733542d6585b907b024a16ed53bfa5f4`  
		Last Modified: Wed, 23 Aug 2023 19:40:05 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
