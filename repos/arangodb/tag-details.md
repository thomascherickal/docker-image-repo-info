<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.10`](#arangodb310)
-	[`arangodb:3.10.10`](#arangodb31010)
-	[`arangodb:3.11`](#arangodb311)
-	[`arangodb:3.11.4`](#arangodb3114)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.10`

```console
$ docker pull arangodb@sha256:812e21cb74024707cc809da69464299d67d65aa52b5aa9ba5befc03b91e43ede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10` - linux; amd64

```console
$ docker pull arangodb@sha256:bb4ae260253ed2dadefc508bb159c18a3bc99dc98aaaa4411957728be96c3881
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227207426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8db97376ac62f2550ee44972e787df9ad01599a614b0bb657f07687d6f730f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:58 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 21 Oct 2023 00:05:58 GMT
ENV ARANGO_VERSION=3.10.10
# Sat, 21 Oct 2023 00:06:28 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 21 Oct 2023 00:06:29 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 21 Oct 2023 00:06:30 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 21 Oct 2023 00:06:30 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 21 Oct 2023 00:06:30 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:06:30 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 21 Oct 2023 00:06:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:06:30 GMT
EXPOSE 8529
# Sat, 21 Oct 2023 00:06:31 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cff3ef6b601bd937b9f2938a372380a8d874466e863bff42f5208253ca42f0`  
		Last Modified: Sat, 21 Oct 2023 00:07:50 GMT  
		Size: 224.4 MB (224397256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29312478c7b365c526381f57be7f926c2652266e2e7f68cf301e8499f55ab4`  
		Last Modified: Sat, 21 Oct 2023 00:07:27 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa9dc8905bb5ab939ec42d9fb0717809642bae19ab3a0b4065f34e0400dcc7d`  
		Last Modified: Sat, 21 Oct 2023 00:07:27 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765a1a00a1a38a32de587dcc74a00f9f23e92f8cee92bf53f955303fa8a515f`  
		Last Modified: Sat, 21 Oct 2023 00:07:27 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:91781b8fde647b68d174c9312f55900f848d4cf0cf2b603516f5a59b1946cc11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.2 MB (222178198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7401ab8c4e0f526a55bcdc40d4f007521b14f1564e76da1563aaa12bf87cc99`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:18:50 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 21 Oct 2023 00:18:50 GMT
ENV ARANGO_VERSION=3.10.10
# Sat, 21 Oct 2023 00:19:15 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 21 Oct 2023 00:19:19 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 21 Oct 2023 00:19:20 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 21 Oct 2023 00:19:20 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 21 Oct 2023 00:19:20 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:19:20 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 21 Oct 2023 00:19:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:19:20 GMT
EXPOSE 8529
# Sat, 21 Oct 2023 00:19:20 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78365d339f291e5e650be08ad3b409e80dbdcb980c6343c3c17f861711f0ea60`  
		Last Modified: Sat, 21 Oct 2023 00:20:22 GMT  
		Size: 219.5 MB (219467688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f821420c1a38c188bf8c7b61f45fdc29fc60fdcad7af1877f9f9f047251994a5`  
		Last Modified: Sat, 21 Oct 2023 00:20:05 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3d68ce3734c05ba9e8b53f191aa163dac25c10be9c3feb9dfe5a3862461d45`  
		Last Modified: Sat, 21 Oct 2023 00:20:05 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07696d937f3ca3ebd7cb9240074c092cf566273e873d10346bbcd2d2cbb037e`  
		Last Modified: Sat, 21 Oct 2023 00:20:05 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.10.10`

```console
$ docker pull arangodb@sha256:812e21cb74024707cc809da69464299d67d65aa52b5aa9ba5befc03b91e43ede
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10.10` - linux; amd64

```console
$ docker pull arangodb@sha256:bb4ae260253ed2dadefc508bb159c18a3bc99dc98aaaa4411957728be96c3881
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227207426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8db97376ac62f2550ee44972e787df9ad01599a614b0bb657f07687d6f730f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:58 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 21 Oct 2023 00:05:58 GMT
ENV ARANGO_VERSION=3.10.10
# Sat, 21 Oct 2023 00:06:28 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 21 Oct 2023 00:06:29 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 21 Oct 2023 00:06:30 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 21 Oct 2023 00:06:30 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 21 Oct 2023 00:06:30 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:06:30 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 21 Oct 2023 00:06:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:06:30 GMT
EXPOSE 8529
# Sat, 21 Oct 2023 00:06:31 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cff3ef6b601bd937b9f2938a372380a8d874466e863bff42f5208253ca42f0`  
		Last Modified: Sat, 21 Oct 2023 00:07:50 GMT  
		Size: 224.4 MB (224397256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29312478c7b365c526381f57be7f926c2652266e2e7f68cf301e8499f55ab4`  
		Last Modified: Sat, 21 Oct 2023 00:07:27 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa9dc8905bb5ab939ec42d9fb0717809642bae19ab3a0b4065f34e0400dcc7d`  
		Last Modified: Sat, 21 Oct 2023 00:07:27 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a765a1a00a1a38a32de587dcc74a00f9f23e92f8cee92bf53f955303fa8a515f`  
		Last Modified: Sat, 21 Oct 2023 00:07:27 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10.10` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:91781b8fde647b68d174c9312f55900f848d4cf0cf2b603516f5a59b1946cc11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.2 MB (222178198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7401ab8c4e0f526a55bcdc40d4f007521b14f1564e76da1563aaa12bf87cc99`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:18:50 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 21 Oct 2023 00:18:50 GMT
ENV ARANGO_VERSION=3.10.10
# Sat, 21 Oct 2023 00:19:15 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 21 Oct 2023 00:19:19 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 21 Oct 2023 00:19:20 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 21 Oct 2023 00:19:20 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 21 Oct 2023 00:19:20 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:19:20 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 21 Oct 2023 00:19:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:19:20 GMT
EXPOSE 8529
# Sat, 21 Oct 2023 00:19:20 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78365d339f291e5e650be08ad3b409e80dbdcb980c6343c3c17f861711f0ea60`  
		Last Modified: Sat, 21 Oct 2023 00:20:22 GMT  
		Size: 219.5 MB (219467688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f821420c1a38c188bf8c7b61f45fdc29fc60fdcad7af1877f9f9f047251994a5`  
		Last Modified: Sat, 21 Oct 2023 00:20:05 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3d68ce3734c05ba9e8b53f191aa163dac25c10be9c3feb9dfe5a3862461d45`  
		Last Modified: Sat, 21 Oct 2023 00:20:05 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07696d937f3ca3ebd7cb9240074c092cf566273e873d10346bbcd2d2cbb037e`  
		Last Modified: Sat, 21 Oct 2023 00:20:05 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.11`

```console
$ docker pull arangodb@sha256:36df678f9c031f610a0945892f7ca4a85622e01225a5eb7ec84a297285993fd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.11` - linux; amd64

```console
$ docker pull arangodb@sha256:6914a16efd1cc4f09e9131dfa39973c33942c6d6ec61e598a5f7a78b3a133920
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.0 MB (245961189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d9b01076ffd3d11cf5e371bf88370c4f76a566c2e94595b314b20c81f9a52f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:58 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 21 Oct 2023 00:06:39 GMT
ENV ARANGO_VERSION=3.11.4
# Sat, 21 Oct 2023 00:07:11 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 21 Oct 2023 00:07:13 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 21 Oct 2023 00:07:14 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 21 Oct 2023 00:07:14 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 21 Oct 2023 00:07:14 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:07:14 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 21 Oct 2023 00:07:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:07:14 GMT
EXPOSE 8529
# Sat, 21 Oct 2023 00:07:14 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eac11788e442e21395e642b216c13eced6eeb3e5b3ca3f5acb1fcfd68d0f57e`  
		Last Modified: Sat, 21 Oct 2023 00:08:22 GMT  
		Size: 243.2 MB (243151020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b0f6de89089f6c9ea53ba958bfde3a917a5705ecc2f9473deefa806123c7a5`  
		Last Modified: Sat, 21 Oct 2023 00:07:59 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdee9cc52af0e35b1793710e468f4eb220e6623c4a6cd0b18fde9cee8001a5c4`  
		Last Modified: Sat, 21 Oct 2023 00:07:59 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99936916e75caa02724ef34dbf43b34f0bd68dc679d08112cc83e1363ae3e4cb`  
		Last Modified: Sat, 21 Oct 2023 00:07:59 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.11` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:25782976ae0cd79c739a406499253e436abbe6767c4eaae07eff94901974f2b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240200370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9056940840017fc22d157b4e9989634e3da3d3389b7dc8c03ea71f0a1806d07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:18:50 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 21 Oct 2023 00:19:23 GMT
ENV ARANGO_VERSION=3.11.4
# Sat, 21 Oct 2023 00:19:50 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 21 Oct 2023 00:19:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 21 Oct 2023 00:19:53 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 21 Oct 2023 00:19:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 21 Oct 2023 00:19:53 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:19:53 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 21 Oct 2023 00:19:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:19:53 GMT
EXPOSE 8529
# Sat, 21 Oct 2023 00:19:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6787ad5016b38fde32138aa1d164399c80b9ddb82c1865e2a4334baf1811164`  
		Last Modified: Sat, 21 Oct 2023 00:20:50 GMT  
		Size: 237.5 MB (237489861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ee76e317819f04b15af41ab5014fd5d21e295a4396d7781b04e6b5afd16419`  
		Last Modified: Sat, 21 Oct 2023 00:20:33 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ba5c5073f63fccbdd55172847a7ae6d67927572c1f4e8c7c1eb8f016586955`  
		Last Modified: Sat, 21 Oct 2023 00:20:33 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7367fac5c5aedd40e3406d75d549d874faaf9bd339514cc5a41dcbec6843e42`  
		Last Modified: Sat, 21 Oct 2023 00:20:33 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.11.4`

```console
$ docker pull arangodb@sha256:36df678f9c031f610a0945892f7ca4a85622e01225a5eb7ec84a297285993fd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.11.4` - linux; amd64

```console
$ docker pull arangodb@sha256:6914a16efd1cc4f09e9131dfa39973c33942c6d6ec61e598a5f7a78b3a133920
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.0 MB (245961189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d9b01076ffd3d11cf5e371bf88370c4f76a566c2e94595b314b20c81f9a52f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:58 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 21 Oct 2023 00:06:39 GMT
ENV ARANGO_VERSION=3.11.4
# Sat, 21 Oct 2023 00:07:11 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 21 Oct 2023 00:07:13 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 21 Oct 2023 00:07:14 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 21 Oct 2023 00:07:14 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 21 Oct 2023 00:07:14 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:07:14 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 21 Oct 2023 00:07:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:07:14 GMT
EXPOSE 8529
# Sat, 21 Oct 2023 00:07:14 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eac11788e442e21395e642b216c13eced6eeb3e5b3ca3f5acb1fcfd68d0f57e`  
		Last Modified: Sat, 21 Oct 2023 00:08:22 GMT  
		Size: 243.2 MB (243151020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b0f6de89089f6c9ea53ba958bfde3a917a5705ecc2f9473deefa806123c7a5`  
		Last Modified: Sat, 21 Oct 2023 00:07:59 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdee9cc52af0e35b1793710e468f4eb220e6623c4a6cd0b18fde9cee8001a5c4`  
		Last Modified: Sat, 21 Oct 2023 00:07:59 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99936916e75caa02724ef34dbf43b34f0bd68dc679d08112cc83e1363ae3e4cb`  
		Last Modified: Sat, 21 Oct 2023 00:07:59 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.11.4` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:25782976ae0cd79c739a406499253e436abbe6767c4eaae07eff94901974f2b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240200370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9056940840017fc22d157b4e9989634e3da3d3389b7dc8c03ea71f0a1806d07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:18:50 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 21 Oct 2023 00:19:23 GMT
ENV ARANGO_VERSION=3.11.4
# Sat, 21 Oct 2023 00:19:50 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 21 Oct 2023 00:19:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 21 Oct 2023 00:19:53 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 21 Oct 2023 00:19:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 21 Oct 2023 00:19:53 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:19:53 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 21 Oct 2023 00:19:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:19:53 GMT
EXPOSE 8529
# Sat, 21 Oct 2023 00:19:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6787ad5016b38fde32138aa1d164399c80b9ddb82c1865e2a4334baf1811164`  
		Last Modified: Sat, 21 Oct 2023 00:20:50 GMT  
		Size: 237.5 MB (237489861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ee76e317819f04b15af41ab5014fd5d21e295a4396d7781b04e6b5afd16419`  
		Last Modified: Sat, 21 Oct 2023 00:20:33 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ba5c5073f63fccbdd55172847a7ae6d67927572c1f4e8c7c1eb8f016586955`  
		Last Modified: Sat, 21 Oct 2023 00:20:33 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7367fac5c5aedd40e3406d75d549d874faaf9bd339514cc5a41dcbec6843e42`  
		Last Modified: Sat, 21 Oct 2023 00:20:33 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:36df678f9c031f610a0945892f7ca4a85622e01225a5eb7ec84a297285993fd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:6914a16efd1cc4f09e9131dfa39973c33942c6d6ec61e598a5f7a78b3a133920
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.0 MB (245961189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d9b01076ffd3d11cf5e371bf88370c4f76a566c2e94595b314b20c81f9a52f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:05:58 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 21 Oct 2023 00:06:39 GMT
ENV ARANGO_VERSION=3.11.4
# Sat, 21 Oct 2023 00:07:11 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 21 Oct 2023 00:07:13 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 21 Oct 2023 00:07:14 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 21 Oct 2023 00:07:14 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 21 Oct 2023 00:07:14 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:07:14 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 21 Oct 2023 00:07:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:07:14 GMT
EXPOSE 8529
# Sat, 21 Oct 2023 00:07:14 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eac11788e442e21395e642b216c13eced6eeb3e5b3ca3f5acb1fcfd68d0f57e`  
		Last Modified: Sat, 21 Oct 2023 00:08:22 GMT  
		Size: 243.2 MB (243151020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b0f6de89089f6c9ea53ba958bfde3a917a5705ecc2f9473deefa806123c7a5`  
		Last Modified: Sat, 21 Oct 2023 00:07:59 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdee9cc52af0e35b1793710e468f4eb220e6623c4a6cd0b18fde9cee8001a5c4`  
		Last Modified: Sat, 21 Oct 2023 00:07:59 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99936916e75caa02724ef34dbf43b34f0bd68dc679d08112cc83e1363ae3e4cb`  
		Last Modified: Sat, 21 Oct 2023 00:07:59 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:latest` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:25782976ae0cd79c739a406499253e436abbe6767c4eaae07eff94901974f2b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240200370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9056940840017fc22d157b4e9989634e3da3d3389b7dc8c03ea71f0a1806d07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:18:50 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 21 Oct 2023 00:19:23 GMT
ENV ARANGO_VERSION=3.11.4
# Sat, 21 Oct 2023 00:19:50 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb311/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 21 Oct 2023 00:19:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 21 Oct 2023 00:19:53 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 21 Oct 2023 00:19:53 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 21 Oct 2023 00:19:53 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 21 Oct 2023 00:19:53 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 21 Oct 2023 00:19:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 21 Oct 2023 00:19:53 GMT
EXPOSE 8529
# Sat, 21 Oct 2023 00:19:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6787ad5016b38fde32138aa1d164399c80b9ddb82c1865e2a4334baf1811164`  
		Last Modified: Sat, 21 Oct 2023 00:20:50 GMT  
		Size: 237.5 MB (237489861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ee76e317819f04b15af41ab5014fd5d21e295a4396d7781b04e6b5afd16419`  
		Last Modified: Sat, 21 Oct 2023 00:20:33 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ba5c5073f63fccbdd55172847a7ae6d67927572c1f4e8c7c1eb8f016586955`  
		Last Modified: Sat, 21 Oct 2023 00:20:33 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7367fac5c5aedd40e3406d75d549d874faaf9bd339514cc5a41dcbec6843e42`  
		Last Modified: Sat, 21 Oct 2023 00:20:33 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
