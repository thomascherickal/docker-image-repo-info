<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.10`](#arangodb310)
-	[`arangodb:3.10.4`](#arangodb3104)
-	[`arangodb:3.8`](#arangodb38)
-	[`arangodb:3.8.8`](#arangodb388)
-	[`arangodb:3.9`](#arangodb39)
-	[`arangodb:3.9.9`](#arangodb399)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.10`

```console
$ docker pull arangodb@sha256:a803a019b599ee44a6450b9c999cf7496e0f7539f03a7f7e8cea17117c19bc92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10` - linux; amd64

```console
$ docker pull arangodb@sha256:c45344554d1fb30c465d4e6d11aa89c126663bdd0bc11f64b350dcfefaa211b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.1 MB (220135630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af7cfb02b2a50cfdb4aa8109aac4087d29c986c27c72b55179630952e7a44e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:14:04 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Feb 2023 20:20:03 GMT
ENV ARANGO_VERSION=3.10.4
# Fri, 24 Feb 2023 20:20:28 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Feb 2023 20:20:30 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 24 Feb 2023 20:20:31 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 24 Feb 2023 20:20:31 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Feb 2023 20:20:31 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 24 Feb 2023 20:20:31 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 24 Feb 2023 20:20:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:20:31 GMT
EXPOSE 8529
# Fri, 24 Feb 2023 20:20:31 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02de890c89804f3c91d247171359c79d80d8234c96395e8bf53ac7669ca84bf4`  
		Last Modified: Fri, 24 Feb 2023 20:21:41 GMT  
		Size: 217.3 MB (217325380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab06140fef655fab9f1b98fd18f0ad2d57411c9f1de3bf20a24b46edcfa55960`  
		Last Modified: Fri, 24 Feb 2023 20:21:19 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019e5ab3f453cb5c95f2110839b80997740150d699d7931e1fc1c2645225e8f0`  
		Last Modified: Fri, 24 Feb 2023 20:21:19 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daad25b957b5fe87a87686f37c7ca40de420f6bc4dd2aea74e24ae26d96e3b8`  
		Last Modified: Fri, 24 Feb 2023 20:21:19 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:78130449c892b57daa06c5f5f473e19c865eb72fd00471f668b302e8c801ffc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.9 MB (214851831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f4058d4b45268f7fbe6cbcdd2b087fcc7dd9e01df2c0baa1e68bd22b2ba4dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:40:53 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Feb 2023 20:39:16 GMT
ENV ARANGO_VERSION=3.10.4
# Fri, 24 Feb 2023 20:39:38 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Feb 2023 20:39:41 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 24 Feb 2023 20:39:42 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 24 Feb 2023 20:39:42 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Feb 2023 20:39:42 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 24 Feb 2023 20:39:42 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 24 Feb 2023 20:39:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:39:42 GMT
EXPOSE 8529
# Fri, 24 Feb 2023 20:39:42 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafb352ff91973c28cd7f1047ee4df5d379f9d8fb02eb62e520f0d17e9033f7e`  
		Last Modified: Fri, 24 Feb 2023 20:40:12 GMT  
		Size: 212.1 MB (212139841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cebc70d6090c700f2aabdb4b9b11b3964a4e70a782d9e2516a0f74727ab13ae`  
		Last Modified: Fri, 24 Feb 2023 20:39:56 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0fad549334b131e887c7052e0f35934a481740f814523834d9d951f10e87e9`  
		Last Modified: Fri, 24 Feb 2023 20:39:56 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26da16676128bc72b2ef5006b1d7502740071b0608c285e24c793ba37f898aac`  
		Last Modified: Fri, 24 Feb 2023 20:39:56 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.10.4`

```console
$ docker pull arangodb@sha256:a803a019b599ee44a6450b9c999cf7496e0f7539f03a7f7e8cea17117c19bc92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10.4` - linux; amd64

```console
$ docker pull arangodb@sha256:c45344554d1fb30c465d4e6d11aa89c126663bdd0bc11f64b350dcfefaa211b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.1 MB (220135630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af7cfb02b2a50cfdb4aa8109aac4087d29c986c27c72b55179630952e7a44e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:14:04 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Feb 2023 20:20:03 GMT
ENV ARANGO_VERSION=3.10.4
# Fri, 24 Feb 2023 20:20:28 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Feb 2023 20:20:30 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 24 Feb 2023 20:20:31 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 24 Feb 2023 20:20:31 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Feb 2023 20:20:31 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 24 Feb 2023 20:20:31 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 24 Feb 2023 20:20:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:20:31 GMT
EXPOSE 8529
# Fri, 24 Feb 2023 20:20:31 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02de890c89804f3c91d247171359c79d80d8234c96395e8bf53ac7669ca84bf4`  
		Last Modified: Fri, 24 Feb 2023 20:21:41 GMT  
		Size: 217.3 MB (217325380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab06140fef655fab9f1b98fd18f0ad2d57411c9f1de3bf20a24b46edcfa55960`  
		Last Modified: Fri, 24 Feb 2023 20:21:19 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019e5ab3f453cb5c95f2110839b80997740150d699d7931e1fc1c2645225e8f0`  
		Last Modified: Fri, 24 Feb 2023 20:21:19 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daad25b957b5fe87a87686f37c7ca40de420f6bc4dd2aea74e24ae26d96e3b8`  
		Last Modified: Fri, 24 Feb 2023 20:21:19 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10.4` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:78130449c892b57daa06c5f5f473e19c865eb72fd00471f668b302e8c801ffc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.9 MB (214851831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f4058d4b45268f7fbe6cbcdd2b087fcc7dd9e01df2c0baa1e68bd22b2ba4dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:40:53 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Feb 2023 20:39:16 GMT
ENV ARANGO_VERSION=3.10.4
# Fri, 24 Feb 2023 20:39:38 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Feb 2023 20:39:41 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 24 Feb 2023 20:39:42 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 24 Feb 2023 20:39:42 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Feb 2023 20:39:42 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 24 Feb 2023 20:39:42 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 24 Feb 2023 20:39:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:39:42 GMT
EXPOSE 8529
# Fri, 24 Feb 2023 20:39:42 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafb352ff91973c28cd7f1047ee4df5d379f9d8fb02eb62e520f0d17e9033f7e`  
		Last Modified: Fri, 24 Feb 2023 20:40:12 GMT  
		Size: 212.1 MB (212139841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cebc70d6090c700f2aabdb4b9b11b3964a4e70a782d9e2516a0f74727ab13ae`  
		Last Modified: Fri, 24 Feb 2023 20:39:56 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0fad549334b131e887c7052e0f35934a481740f814523834d9d951f10e87e9`  
		Last Modified: Fri, 24 Feb 2023 20:39:56 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26da16676128bc72b2ef5006b1d7502740071b0608c285e24c793ba37f898aac`  
		Last Modified: Fri, 24 Feb 2023 20:39:56 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8`

```console
$ docker pull arangodb@sha256:8875dd096a2bf77e0b4e09ccb22eecc62194ff97e3676d76a119072381d8232a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8` - linux; amd64

```console
$ docker pull arangodb@sha256:5e9491426371da85a3f76964df73af2bee2b2fd1f2afc2bb37ec6d27399e1321
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.6 MB (195563968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a69ee5f4a17e15afb32ca08346a1d3735b40dd04a0e1114815c95ce7d3df229f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:12:56 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 11 Feb 2023 07:12:56 GMT
ENV ARANGO_VERSION=3.8.8
# Sat, 11 Feb 2023 07:12:56 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Sat, 11 Feb 2023 07:12:56 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.8-1_amd64.deb
# Sat, 11 Feb 2023 07:12:56 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.8-1_amd64.deb
# Sat, 11 Feb 2023 07:12:57 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.8-1_amd64.deb.asc
# Sat, 11 Feb 2023 07:13:22 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 11 Feb 2023 07:13:24 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 11 Feb 2023 07:13:24 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 11 Feb 2023 07:13:24 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 11 Feb 2023 07:13:24 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 11 Feb 2023 07:13:25 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 11 Feb 2023 07:13:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 07:13:25 GMT
EXPOSE 8529
# Sat, 11 Feb 2023 07:13:25 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52f97a875524282e52658d0cebb1aea3d76cdb9d92896c0af291ccc4c5fd45a`  
		Last Modified: Sat, 11 Feb 2023 07:15:09 GMT  
		Size: 192.7 MB (192731851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbca32a09d4b2233aaf87eb68dd9d99ff43903a1bedf0db1209bf01ba0a01e51`  
		Last Modified: Sat, 11 Feb 2023 07:14:47 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f77081e4f0927ab4c1d0968996a8c52e9d6c6582f16dd9034623b62f7242d7`  
		Last Modified: Sat, 11 Feb 2023 07:14:47 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a35dade599ba08dfe1b3eff1eed291c8e245457e46f26ca672739180e40f16`  
		Last Modified: Sat, 11 Feb 2023 07:14:47 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8.8`

```console
$ docker pull arangodb@sha256:8875dd096a2bf77e0b4e09ccb22eecc62194ff97e3676d76a119072381d8232a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8.8` - linux; amd64

```console
$ docker pull arangodb@sha256:5e9491426371da85a3f76964df73af2bee2b2fd1f2afc2bb37ec6d27399e1321
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.6 MB (195563968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a69ee5f4a17e15afb32ca08346a1d3735b40dd04a0e1114815c95ce7d3df229f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:12:56 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 11 Feb 2023 07:12:56 GMT
ENV ARANGO_VERSION=3.8.8
# Sat, 11 Feb 2023 07:12:56 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Sat, 11 Feb 2023 07:12:56 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.8-1_amd64.deb
# Sat, 11 Feb 2023 07:12:56 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.8-1_amd64.deb
# Sat, 11 Feb 2023 07:12:57 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.8-1_amd64.deb.asc
# Sat, 11 Feb 2023 07:13:22 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 11 Feb 2023 07:13:24 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 11 Feb 2023 07:13:24 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 11 Feb 2023 07:13:24 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 11 Feb 2023 07:13:24 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 11 Feb 2023 07:13:25 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 11 Feb 2023 07:13:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 07:13:25 GMT
EXPOSE 8529
# Sat, 11 Feb 2023 07:13:25 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52f97a875524282e52658d0cebb1aea3d76cdb9d92896c0af291ccc4c5fd45a`  
		Last Modified: Sat, 11 Feb 2023 07:15:09 GMT  
		Size: 192.7 MB (192731851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbca32a09d4b2233aaf87eb68dd9d99ff43903a1bedf0db1209bf01ba0a01e51`  
		Last Modified: Sat, 11 Feb 2023 07:14:47 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f77081e4f0927ab4c1d0968996a8c52e9d6c6582f16dd9034623b62f7242d7`  
		Last Modified: Sat, 11 Feb 2023 07:14:47 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a35dade599ba08dfe1b3eff1eed291c8e245457e46f26ca672739180e40f16`  
		Last Modified: Sat, 11 Feb 2023 07:14:47 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9`

```console
$ docker pull arangodb@sha256:058b5cd0d179e28c2f6e73c3a0727ded6f9a6bd86d678df7cfa0842935843f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9` - linux; amd64

```console
$ docker pull arangodb@sha256:1271e3a0617de4c915fda5037a3a4c31cc2706446b5df47b0c162c9f0c5773a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.7 MB (202731833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf5cc242c78b64345d1fc349e43fa30f054956ef97d1351e15adb91ea17c922`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:12:56 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Feb 2023 20:19:29 GMT
ENV ARANGO_VERSION=3.9.9
# Fri, 24 Feb 2023 20:19:29 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Fri, 24 Feb 2023 20:19:29 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.9-1_amd64.deb
# Fri, 24 Feb 2023 20:19:29 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.9-1_amd64.deb
# Fri, 24 Feb 2023 20:19:29 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.9-1_amd64.deb.asc
# Fri, 24 Feb 2023 20:19:54 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Feb 2023 20:19:56 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 24 Feb 2023 20:19:56 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 24 Feb 2023 20:19:56 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Feb 2023 20:19:57 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 24 Feb 2023 20:19:57 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 24 Feb 2023 20:19:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:19:57 GMT
EXPOSE 8529
# Fri, 24 Feb 2023 20:19:57 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc67d8063d0c9718fbf2e971e08a9783861294a54c7d39f503acdef9527856`  
		Last Modified: Fri, 24 Feb 2023 20:21:10 GMT  
		Size: 199.9 MB (199899715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6787059ed08419f2b154006d9231f902bc8c692074013f82a71bbb1098398ced`  
		Last Modified: Fri, 24 Feb 2023 20:20:49 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3439fef56d7a5a91c8d80b34c415be288466f1802ef7cb87bb76431069c88846`  
		Last Modified: Fri, 24 Feb 2023 20:20:49 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dda6f9f9dd59f5c797ffbcbb7eb760f7fc3a45416ef573ceb79978a528833d7`  
		Last Modified: Fri, 24 Feb 2023 20:20:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9.9`

```console
$ docker pull arangodb@sha256:058b5cd0d179e28c2f6e73c3a0727ded6f9a6bd86d678df7cfa0842935843f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9.9` - linux; amd64

```console
$ docker pull arangodb@sha256:1271e3a0617de4c915fda5037a3a4c31cc2706446b5df47b0c162c9f0c5773a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.7 MB (202731833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf5cc242c78b64345d1fc349e43fa30f054956ef97d1351e15adb91ea17c922`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:12:56 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Feb 2023 20:19:29 GMT
ENV ARANGO_VERSION=3.9.9
# Fri, 24 Feb 2023 20:19:29 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Fri, 24 Feb 2023 20:19:29 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.9-1_amd64.deb
# Fri, 24 Feb 2023 20:19:29 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.9-1_amd64.deb
# Fri, 24 Feb 2023 20:19:29 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.9-1_amd64.deb.asc
# Fri, 24 Feb 2023 20:19:54 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Feb 2023 20:19:56 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 24 Feb 2023 20:19:56 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 24 Feb 2023 20:19:56 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Feb 2023 20:19:57 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 24 Feb 2023 20:19:57 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 24 Feb 2023 20:19:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:19:57 GMT
EXPOSE 8529
# Fri, 24 Feb 2023 20:19:57 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc67d8063d0c9718fbf2e971e08a9783861294a54c7d39f503acdef9527856`  
		Last Modified: Fri, 24 Feb 2023 20:21:10 GMT  
		Size: 199.9 MB (199899715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6787059ed08419f2b154006d9231f902bc8c692074013f82a71bbb1098398ced`  
		Last Modified: Fri, 24 Feb 2023 20:20:49 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3439fef56d7a5a91c8d80b34c415be288466f1802ef7cb87bb76431069c88846`  
		Last Modified: Fri, 24 Feb 2023 20:20:49 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dda6f9f9dd59f5c797ffbcbb7eb760f7fc3a45416ef573ceb79978a528833d7`  
		Last Modified: Fri, 24 Feb 2023 20:20:49 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:a803a019b599ee44a6450b9c999cf7496e0f7539f03a7f7e8cea17117c19bc92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:c45344554d1fb30c465d4e6d11aa89c126663bdd0bc11f64b350dcfefaa211b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.1 MB (220135630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af7cfb02b2a50cfdb4aa8109aac4087d29c986c27c72b55179630952e7a44e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:14:04 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Feb 2023 20:20:03 GMT
ENV ARANGO_VERSION=3.10.4
# Fri, 24 Feb 2023 20:20:28 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Feb 2023 20:20:30 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 24 Feb 2023 20:20:31 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 24 Feb 2023 20:20:31 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Feb 2023 20:20:31 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 24 Feb 2023 20:20:31 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 24 Feb 2023 20:20:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:20:31 GMT
EXPOSE 8529
# Fri, 24 Feb 2023 20:20:31 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02de890c89804f3c91d247171359c79d80d8234c96395e8bf53ac7669ca84bf4`  
		Last Modified: Fri, 24 Feb 2023 20:21:41 GMT  
		Size: 217.3 MB (217325380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab06140fef655fab9f1b98fd18f0ad2d57411c9f1de3bf20a24b46edcfa55960`  
		Last Modified: Fri, 24 Feb 2023 20:21:19 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019e5ab3f453cb5c95f2110839b80997740150d699d7931e1fc1c2645225e8f0`  
		Last Modified: Fri, 24 Feb 2023 20:21:19 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daad25b957b5fe87a87686f37c7ca40de420f6bc4dd2aea74e24ae26d96e3b8`  
		Last Modified: Fri, 24 Feb 2023 20:21:19 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:latest` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:78130449c892b57daa06c5f5f473e19c865eb72fd00471f668b302e8c801ffc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.9 MB (214851831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f4058d4b45268f7fbe6cbcdd2b087fcc7dd9e01df2c0baa1e68bd22b2ba4dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:40:53 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 24 Feb 2023 20:39:16 GMT
ENV ARANGO_VERSION=3.10.4
# Fri, 24 Feb 2023 20:39:38 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 24 Feb 2023 20:39:41 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 24 Feb 2023 20:39:42 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 24 Feb 2023 20:39:42 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 24 Feb 2023 20:39:42 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 24 Feb 2023 20:39:42 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 24 Feb 2023 20:39:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Feb 2023 20:39:42 GMT
EXPOSE 8529
# Fri, 24 Feb 2023 20:39:42 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafb352ff91973c28cd7f1047ee4df5d379f9d8fb02eb62e520f0d17e9033f7e`  
		Last Modified: Fri, 24 Feb 2023 20:40:12 GMT  
		Size: 212.1 MB (212139841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cebc70d6090c700f2aabdb4b9b11b3964a4e70a782d9e2516a0f74727ab13ae`  
		Last Modified: Fri, 24 Feb 2023 20:39:56 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0fad549334b131e887c7052e0f35934a481740f814523834d9d951f10e87e9`  
		Last Modified: Fri, 24 Feb 2023 20:39:56 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26da16676128bc72b2ef5006b1d7502740071b0608c285e24c793ba37f898aac`  
		Last Modified: Fri, 24 Feb 2023 20:39:56 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
