<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.10`](#arangodb310)
-	[`arangodb:3.10.5`](#arangodb3105)
-	[`arangodb:3.8`](#arangodb38)
-	[`arangodb:3.8.9`](#arangodb389)
-	[`arangodb:3.9`](#arangodb39)
-	[`arangodb:3.9.10`](#arangodb3910)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.10`

```console
$ docker pull arangodb@sha256:5c4712780d5b8734ea6cce294bb97d94415b72c39273c6b65d5499a8e19246ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10` - linux; amd64

```console
$ docker pull arangodb@sha256:eeaa1a333a1a5ecd100af72f9fe786294673668c63a6f98f25e37ddb00db2de8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.0 MB (220040318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cca4640f3fa0e30579ce690c6794cb990bce502fb094419671b1979dae9d820`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:35:19 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 29 Mar 2023 19:35:19 GMT
ENV ARANGO_VERSION=3.10.5
# Wed, 29 Mar 2023 19:35:44 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 29 Mar 2023 19:35:45 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 29 Mar 2023 19:35:46 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 29 Mar 2023 19:35:46 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 29 Mar 2023 19:35:46 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:35:46 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 29 Mar 2023 19:35:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:35:46 GMT
EXPOSE 8529
# Wed, 29 Mar 2023 19:35:46 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954c1d7a38461f43b4f0cdf953de4e6373945fb95e7488bad928df5c73c90023`  
		Last Modified: Wed, 29 Mar 2023 19:37:20 GMT  
		Size: 217.2 MB (217230037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553d4935f63dc7018c0ef04ec189ec375ae76d237b8edd142dd587f75c744865`  
		Last Modified: Wed, 29 Mar 2023 19:36:58 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5db0bf8ded33550aeb17ec7bf15b5fabacea28dacd10ccfedc8eec2b5dbc67`  
		Last Modified: Wed, 29 Mar 2023 19:36:58 GMT  
		Size: 2.1 KB (2082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356707677e241cda360bae2efde877b799777a5a61e6421336bce22fa30be504`  
		Last Modified: Wed, 29 Mar 2023 19:36:58 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:9d8e69619c9b2e1b62c4e5c5f9db963128ad9f440e8faf65f74c8a95f8341899
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.8 MB (214758504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cab9121030fe4c2fbb0cf461ca9d85fb96d604ca8d1aa14cf106a8c35b34ee0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:53:47 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 30 Mar 2023 03:53:47 GMT
ENV ARANGO_VERSION=3.10.5
# Thu, 30 Mar 2023 03:54:12 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 30 Mar 2023 03:54:16 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 30 Mar 2023 03:54:16 GMT
RUN echo "UTC" > /etc/timezone
# Thu, 30 Mar 2023 03:54:16 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 30 Mar 2023 03:54:17 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 30 Mar 2023 03:54:17 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 30 Mar 2023 03:54:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:54:17 GMT
EXPOSE 8529
# Thu, 30 Mar 2023 03:54:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2603c55c8ee808f1142ac63c3eca3735cffecad487d363ccf31157ed433937f0`  
		Last Modified: Thu, 30 Mar 2023 03:54:41 GMT  
		Size: 212.0 MB (212046675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c3ee4a624fdef84b5f020d3b733296ce036f1c9421b9dcb2945335560d04f2`  
		Last Modified: Thu, 30 Mar 2023 03:54:25 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248fd4321833cef12930b649a046af7e8cde95f1c770365cd764cf92baec7f28`  
		Last Modified: Thu, 30 Mar 2023 03:54:26 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2290cf2b56a837dea5a39f0bd24468afbfbb74a00186dba67f85c45a839fbe`  
		Last Modified: Thu, 30 Mar 2023 03:54:25 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.10.5`

```console
$ docker pull arangodb@sha256:5c4712780d5b8734ea6cce294bb97d94415b72c39273c6b65d5499a8e19246ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10.5` - linux; amd64

```console
$ docker pull arangodb@sha256:eeaa1a333a1a5ecd100af72f9fe786294673668c63a6f98f25e37ddb00db2de8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.0 MB (220040318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cca4640f3fa0e30579ce690c6794cb990bce502fb094419671b1979dae9d820`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:35:19 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 29 Mar 2023 19:35:19 GMT
ENV ARANGO_VERSION=3.10.5
# Wed, 29 Mar 2023 19:35:44 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 29 Mar 2023 19:35:45 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 29 Mar 2023 19:35:46 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 29 Mar 2023 19:35:46 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 29 Mar 2023 19:35:46 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:35:46 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 29 Mar 2023 19:35:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:35:46 GMT
EXPOSE 8529
# Wed, 29 Mar 2023 19:35:46 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954c1d7a38461f43b4f0cdf953de4e6373945fb95e7488bad928df5c73c90023`  
		Last Modified: Wed, 29 Mar 2023 19:37:20 GMT  
		Size: 217.2 MB (217230037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553d4935f63dc7018c0ef04ec189ec375ae76d237b8edd142dd587f75c744865`  
		Last Modified: Wed, 29 Mar 2023 19:36:58 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5db0bf8ded33550aeb17ec7bf15b5fabacea28dacd10ccfedc8eec2b5dbc67`  
		Last Modified: Wed, 29 Mar 2023 19:36:58 GMT  
		Size: 2.1 KB (2082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356707677e241cda360bae2efde877b799777a5a61e6421336bce22fa30be504`  
		Last Modified: Wed, 29 Mar 2023 19:36:58 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10.5` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:9d8e69619c9b2e1b62c4e5c5f9db963128ad9f440e8faf65f74c8a95f8341899
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.8 MB (214758504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cab9121030fe4c2fbb0cf461ca9d85fb96d604ca8d1aa14cf106a8c35b34ee0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:53:47 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 30 Mar 2023 03:53:47 GMT
ENV ARANGO_VERSION=3.10.5
# Thu, 30 Mar 2023 03:54:12 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 30 Mar 2023 03:54:16 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 30 Mar 2023 03:54:16 GMT
RUN echo "UTC" > /etc/timezone
# Thu, 30 Mar 2023 03:54:16 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 30 Mar 2023 03:54:17 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 30 Mar 2023 03:54:17 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 30 Mar 2023 03:54:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:54:17 GMT
EXPOSE 8529
# Thu, 30 Mar 2023 03:54:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2603c55c8ee808f1142ac63c3eca3735cffecad487d363ccf31157ed433937f0`  
		Last Modified: Thu, 30 Mar 2023 03:54:41 GMT  
		Size: 212.0 MB (212046675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c3ee4a624fdef84b5f020d3b733296ce036f1c9421b9dcb2945335560d04f2`  
		Last Modified: Thu, 30 Mar 2023 03:54:25 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248fd4321833cef12930b649a046af7e8cde95f1c770365cd764cf92baec7f28`  
		Last Modified: Thu, 30 Mar 2023 03:54:26 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2290cf2b56a837dea5a39f0bd24468afbfbb74a00186dba67f85c45a839fbe`  
		Last Modified: Thu, 30 Mar 2023 03:54:25 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8`

```console
$ docker pull arangodb@sha256:0284eeac59d57f7342936e346a00bb8be6f2bb1613fec55e430212bcfd3c1b8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8` - linux; amd64

```console
$ docker pull arangodb@sha256:2223d885c9b7a1adae7ac9ae7d74e7e7d56eaf08ea2926fc418d4ac11441122e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196757580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c423d420f46475e0e328b78c5990120c7cb4066eb308906db384223de77486`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:34:12 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 30 Mar 2023 19:19:22 GMT
ENV ARANGO_VERSION=3.8.9
# Thu, 30 Mar 2023 19:19:22 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Thu, 30 Mar 2023 19:19:22 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.9-1_amd64.deb
# Thu, 30 Mar 2023 19:19:22 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.9-1_amd64.deb
# Thu, 30 Mar 2023 19:19:22 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.9-1_amd64.deb.asc
# Thu, 30 Mar 2023 19:19:48 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 30 Mar 2023 19:19:49 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 30 Mar 2023 19:19:50 GMT
RUN echo "UTC" > /etc/timezone
# Thu, 30 Mar 2023 19:19:50 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 30 Mar 2023 19:19:50 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 30 Mar 2023 19:19:50 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 30 Mar 2023 19:19:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 19:19:50 GMT
EXPOSE 8529
# Thu, 30 Mar 2023 19:19:50 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621d97c079e44d4504070e4b37418ba255e9fd146da3d72cd28219f614749b2`  
		Last Modified: Thu, 30 Mar 2023 19:20:27 GMT  
		Size: 193.9 MB (193925447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a17af87a7f15255bd35a5df2ebdf8d5088ca6473c90494da9ec22f186ae7129`  
		Last Modified: Thu, 30 Mar 2023 19:20:06 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e70c75facea75f5a08ae8a8075555df8fc7eba68bf0255ed54740cce4a66574`  
		Last Modified: Thu, 30 Mar 2023 19:20:06 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844ed65c77ba47b3b9d7ead2331aefd221ed22a75fc1dad7b601000f1f8d1e8e`  
		Last Modified: Thu, 30 Mar 2023 19:20:06 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8.9`

```console
$ docker pull arangodb@sha256:0284eeac59d57f7342936e346a00bb8be6f2bb1613fec55e430212bcfd3c1b8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8.9` - linux; amd64

```console
$ docker pull arangodb@sha256:2223d885c9b7a1adae7ac9ae7d74e7e7d56eaf08ea2926fc418d4ac11441122e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.8 MB (196757580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5c423d420f46475e0e328b78c5990120c7cb4066eb308906db384223de77486`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:34:12 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 30 Mar 2023 19:19:22 GMT
ENV ARANGO_VERSION=3.8.9
# Thu, 30 Mar 2023 19:19:22 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Thu, 30 Mar 2023 19:19:22 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.9-1_amd64.deb
# Thu, 30 Mar 2023 19:19:22 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.9-1_amd64.deb
# Thu, 30 Mar 2023 19:19:22 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.9-1_amd64.deb.asc
# Thu, 30 Mar 2023 19:19:48 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 30 Mar 2023 19:19:49 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 30 Mar 2023 19:19:50 GMT
RUN echo "UTC" > /etc/timezone
# Thu, 30 Mar 2023 19:19:50 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 30 Mar 2023 19:19:50 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 30 Mar 2023 19:19:50 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 30 Mar 2023 19:19:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 19:19:50 GMT
EXPOSE 8529
# Thu, 30 Mar 2023 19:19:50 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d621d97c079e44d4504070e4b37418ba255e9fd146da3d72cd28219f614749b2`  
		Last Modified: Thu, 30 Mar 2023 19:20:27 GMT  
		Size: 193.9 MB (193925447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a17af87a7f15255bd35a5df2ebdf8d5088ca6473c90494da9ec22f186ae7129`  
		Last Modified: Thu, 30 Mar 2023 19:20:06 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e70c75facea75f5a08ae8a8075555df8fc7eba68bf0255ed54740cce4a66574`  
		Last Modified: Thu, 30 Mar 2023 19:20:06 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844ed65c77ba47b3b9d7ead2331aefd221ed22a75fc1dad7b601000f1f8d1e8e`  
		Last Modified: Thu, 30 Mar 2023 19:20:06 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9`

```console
$ docker pull arangodb@sha256:873c36d65bc0649dd3406e13ff9c7b08c5feb1dfe2887b39f2d267792794ce6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9` - linux; amd64

```console
$ docker pull arangodb@sha256:8f575ea63ae1e3fb4776162f6d74782af3274e7208f8db8b6ebf426dde9c61b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.7 MB (202742656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51aae7c4d3a0c7a35e1afc2266db04dbe562079963fbfec0de84fcd2df20beb5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:34:12 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 29 Mar 2023 19:34:45 GMT
ENV ARANGO_VERSION=3.9.10
# Wed, 29 Mar 2023 19:34:46 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Wed, 29 Mar 2023 19:34:46 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.10-1_amd64.deb
# Wed, 29 Mar 2023 19:34:46 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.10-1_amd64.deb
# Wed, 29 Mar 2023 19:34:46 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.10-1_amd64.deb.asc
# Wed, 29 Mar 2023 19:35:11 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 29 Mar 2023 19:35:12 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 29 Mar 2023 19:35:13 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 29 Mar 2023 19:35:13 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 29 Mar 2023 19:35:13 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:35:13 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 29 Mar 2023 19:35:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:35:13 GMT
EXPOSE 8529
# Wed, 29 Mar 2023 19:35:13 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b36f9d97a4baa241ecafbe5c33d4653dd1a116351a3a4747647bcb89a67e12a`  
		Last Modified: Wed, 29 Mar 2023 19:36:50 GMT  
		Size: 199.9 MB (199910531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d68b0ce6647bbee6e6271fe26f0313457ff3333f1106b4a6e332d33b8e2316`  
		Last Modified: Wed, 29 Mar 2023 19:36:29 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9bde01a8ebdadeac677a8cd2aa72cb4b9fdbb527d76da698419d2e25e68907`  
		Last Modified: Wed, 29 Mar 2023 19:36:29 GMT  
		Size: 2.1 KB (2083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bfba5b887e5077a2fd7401163ac55ccdb763e213e24238e750edc679d2ee13`  
		Last Modified: Wed, 29 Mar 2023 19:36:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9.10`

```console
$ docker pull arangodb@sha256:873c36d65bc0649dd3406e13ff9c7b08c5feb1dfe2887b39f2d267792794ce6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9.10` - linux; amd64

```console
$ docker pull arangodb@sha256:8f575ea63ae1e3fb4776162f6d74782af3274e7208f8db8b6ebf426dde9c61b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.7 MB (202742656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51aae7c4d3a0c7a35e1afc2266db04dbe562079963fbfec0de84fcd2df20beb5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:34:12 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 29 Mar 2023 19:34:45 GMT
ENV ARANGO_VERSION=3.9.10
# Wed, 29 Mar 2023 19:34:46 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Wed, 29 Mar 2023 19:34:46 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.10-1_amd64.deb
# Wed, 29 Mar 2023 19:34:46 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.10-1_amd64.deb
# Wed, 29 Mar 2023 19:34:46 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.10-1_amd64.deb.asc
# Wed, 29 Mar 2023 19:35:11 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 29 Mar 2023 19:35:12 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 29 Mar 2023 19:35:13 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 29 Mar 2023 19:35:13 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 29 Mar 2023 19:35:13 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:35:13 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 29 Mar 2023 19:35:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:35:13 GMT
EXPOSE 8529
# Wed, 29 Mar 2023 19:35:13 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b36f9d97a4baa241ecafbe5c33d4653dd1a116351a3a4747647bcb89a67e12a`  
		Last Modified: Wed, 29 Mar 2023 19:36:50 GMT  
		Size: 199.9 MB (199910531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d68b0ce6647bbee6e6271fe26f0313457ff3333f1106b4a6e332d33b8e2316`  
		Last Modified: Wed, 29 Mar 2023 19:36:29 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9bde01a8ebdadeac677a8cd2aa72cb4b9fdbb527d76da698419d2e25e68907`  
		Last Modified: Wed, 29 Mar 2023 19:36:29 GMT  
		Size: 2.1 KB (2083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bfba5b887e5077a2fd7401163ac55ccdb763e213e24238e750edc679d2ee13`  
		Last Modified: Wed, 29 Mar 2023 19:36:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:5c4712780d5b8734ea6cce294bb97d94415b72c39273c6b65d5499a8e19246ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:eeaa1a333a1a5ecd100af72f9fe786294673668c63a6f98f25e37ddb00db2de8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.0 MB (220040318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cca4640f3fa0e30579ce690c6794cb990bce502fb094419671b1979dae9d820`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:35:19 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Wed, 29 Mar 2023 19:35:19 GMT
ENV ARANGO_VERSION=3.10.5
# Wed, 29 Mar 2023 19:35:44 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Wed, 29 Mar 2023 19:35:45 GMT
ENV GLIBCXX_FORCE_NEW=1
# Wed, 29 Mar 2023 19:35:46 GMT
RUN echo "UTC" > /etc/timezone
# Wed, 29 Mar 2023 19:35:46 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Wed, 29 Mar 2023 19:35:46 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Wed, 29 Mar 2023 19:35:46 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Wed, 29 Mar 2023 19:35:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Mar 2023 19:35:46 GMT
EXPOSE 8529
# Wed, 29 Mar 2023 19:35:46 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954c1d7a38461f43b4f0cdf953de4e6373945fb95e7488bad928df5c73c90023`  
		Last Modified: Wed, 29 Mar 2023 19:37:20 GMT  
		Size: 217.2 MB (217230037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553d4935f63dc7018c0ef04ec189ec375ae76d237b8edd142dd587f75c744865`  
		Last Modified: Wed, 29 Mar 2023 19:36:58 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5db0bf8ded33550aeb17ec7bf15b5fabacea28dacd10ccfedc8eec2b5dbc67`  
		Last Modified: Wed, 29 Mar 2023 19:36:58 GMT  
		Size: 2.1 KB (2082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356707677e241cda360bae2efde877b799777a5a61e6421336bce22fa30be504`  
		Last Modified: Wed, 29 Mar 2023 19:36:58 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:latest` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:9d8e69619c9b2e1b62c4e5c5f9db963128ad9f440e8faf65f74c8a95f8341899
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.8 MB (214758504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cab9121030fe4c2fbb0cf461ca9d85fb96d604ca8d1aa14cf106a8c35b34ee0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:53:47 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 30 Mar 2023 03:53:47 GMT
ENV ARANGO_VERSION=3.10.5
# Thu, 30 Mar 2023 03:54:12 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 30 Mar 2023 03:54:16 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 30 Mar 2023 03:54:16 GMT
RUN echo "UTC" > /etc/timezone
# Thu, 30 Mar 2023 03:54:16 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 30 Mar 2023 03:54:17 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 30 Mar 2023 03:54:17 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 30 Mar 2023 03:54:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 03:54:17 GMT
EXPOSE 8529
# Thu, 30 Mar 2023 03:54:17 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2603c55c8ee808f1142ac63c3eca3735cffecad487d363ccf31157ed433937f0`  
		Last Modified: Thu, 30 Mar 2023 03:54:41 GMT  
		Size: 212.0 MB (212046675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c3ee4a624fdef84b5f020d3b733296ce036f1c9421b9dcb2945335560d04f2`  
		Last Modified: Thu, 30 Mar 2023 03:54:25 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248fd4321833cef12930b649a046af7e8cde95f1c770365cd764cf92baec7f28`  
		Last Modified: Thu, 30 Mar 2023 03:54:26 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2290cf2b56a837dea5a39f0bd24468afbfbb74a00186dba67f85c45a839fbe`  
		Last Modified: Thu, 30 Mar 2023 03:54:25 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
