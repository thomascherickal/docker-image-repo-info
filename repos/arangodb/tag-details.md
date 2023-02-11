<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `arangodb`

-	[`arangodb:3.10`](#arangodb310)
-	[`arangodb:3.10.3`](#arangodb3103)
-	[`arangodb:3.8`](#arangodb38)
-	[`arangodb:3.8.8`](#arangodb388)
-	[`arangodb:3.9`](#arangodb39)
-	[`arangodb:3.9.8`](#arangodb398)
-	[`arangodb:latest`](#arangodblatest)

## `arangodb:3.10`

```console
$ docker pull arangodb@sha256:2477f18ef19f7b4f9423bc5dd36efdad4abd261005794dc87821d09140f6c520
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10` - linux; amd64

```console
$ docker pull arangodb@sha256:6d636e4c35f07d60f94a200c4aeb415e899881951037a7f1e8f8f2ff1bdfc108
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219637048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b406ed867db8704973416c7f9abbad168166efe7a43147c2764c5deffd79177a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:14:04 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 11 Feb 2023 07:14:04 GMT
ENV ARANGO_VERSION=3.10.3
# Sat, 11 Feb 2023 07:14:29 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 11 Feb 2023 07:14:31 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 11 Feb 2023 07:14:31 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 11 Feb 2023 07:14:31 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 11 Feb 2023 07:14:31 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 11 Feb 2023 07:14:32 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 11 Feb 2023 07:14:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 07:14:32 GMT
EXPOSE 8529
# Sat, 11 Feb 2023 07:14:32 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f91516352792b0a83c3a19c8533ee3a80884dc0c3e10763bd114526245cfab`  
		Last Modified: Sat, 11 Feb 2023 07:16:12 GMT  
		Size: 216.8 MB (216826800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8067412b9ca332602e838f51cf865ee2cbec707bef662de31077bc77d8a96a7`  
		Last Modified: Sat, 11 Feb 2023 07:15:48 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76221af3d175c5aeb608cdef6ebaf9863948bbe113d4cbc1f70363b8566181f8`  
		Last Modified: Sat, 11 Feb 2023 07:15:48 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382b7163ed35efa634c24f98989d54f42e5da8d61a7fdaba18a9850bd96a8b31`  
		Last Modified: Sat, 11 Feb 2023 07:15:48 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:6b5783485564f6ba62949982632c67f23142174ae4f681f5c557187291fae414
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.4 MB (214389785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be30a56e2da10ebc19123787e7ae49791dd08b349913b57e1ebb328f5f913b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:40:53 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 10 Feb 2023 21:40:53 GMT
ENV ARANGO_VERSION=3.10.3
# Fri, 10 Feb 2023 21:41:16 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 10 Feb 2023 21:41:19 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 10 Feb 2023 21:41:20 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 10 Feb 2023 21:41:20 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 10 Feb 2023 21:41:20 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 10 Feb 2023 21:41:20 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 10 Feb 2023 21:41:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Feb 2023 21:41:20 GMT
EXPOSE 8529
# Fri, 10 Feb 2023 21:41:20 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ec61f8cffad1681adf6e5c6f8c51070d75f2161d772c59b296317679747e2f`  
		Last Modified: Fri, 10 Feb 2023 21:41:51 GMT  
		Size: 211.7 MB (211677800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59977b4ada21a00341a32868d332d8f335ab14093feaf3ca711cd31e4b7db319`  
		Last Modified: Fri, 10 Feb 2023 21:41:34 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559d59e6dde21cd70d89260297a1afe7537fb882d4641546a09913a928fbedd2`  
		Last Modified: Fri, 10 Feb 2023 21:41:34 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1184bb17d814dbb866bf75053957e1cc46e7834fb732cf27a548264a4646ce9`  
		Last Modified: Fri, 10 Feb 2023 21:41:34 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.10.3`

```console
$ docker pull arangodb@sha256:2477f18ef19f7b4f9423bc5dd36efdad4abd261005794dc87821d09140f6c520
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10.3` - linux; amd64

```console
$ docker pull arangodb@sha256:6d636e4c35f07d60f94a200c4aeb415e899881951037a7f1e8f8f2ff1bdfc108
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219637048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b406ed867db8704973416c7f9abbad168166efe7a43147c2764c5deffd79177a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:14:04 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 11 Feb 2023 07:14:04 GMT
ENV ARANGO_VERSION=3.10.3
# Sat, 11 Feb 2023 07:14:29 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 11 Feb 2023 07:14:31 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 11 Feb 2023 07:14:31 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 11 Feb 2023 07:14:31 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 11 Feb 2023 07:14:31 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 11 Feb 2023 07:14:32 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 11 Feb 2023 07:14:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 07:14:32 GMT
EXPOSE 8529
# Sat, 11 Feb 2023 07:14:32 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f91516352792b0a83c3a19c8533ee3a80884dc0c3e10763bd114526245cfab`  
		Last Modified: Sat, 11 Feb 2023 07:16:12 GMT  
		Size: 216.8 MB (216826800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8067412b9ca332602e838f51cf865ee2cbec707bef662de31077bc77d8a96a7`  
		Last Modified: Sat, 11 Feb 2023 07:15:48 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76221af3d175c5aeb608cdef6ebaf9863948bbe113d4cbc1f70363b8566181f8`  
		Last Modified: Sat, 11 Feb 2023 07:15:48 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382b7163ed35efa634c24f98989d54f42e5da8d61a7fdaba18a9850bd96a8b31`  
		Last Modified: Sat, 11 Feb 2023 07:15:48 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:3.10.3` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:6b5783485564f6ba62949982632c67f23142174ae4f681f5c557187291fae414
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.4 MB (214389785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be30a56e2da10ebc19123787e7ae49791dd08b349913b57e1ebb328f5f913b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:40:53 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 10 Feb 2023 21:40:53 GMT
ENV ARANGO_VERSION=3.10.3
# Fri, 10 Feb 2023 21:41:16 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 10 Feb 2023 21:41:19 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 10 Feb 2023 21:41:20 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 10 Feb 2023 21:41:20 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 10 Feb 2023 21:41:20 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 10 Feb 2023 21:41:20 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 10 Feb 2023 21:41:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Feb 2023 21:41:20 GMT
EXPOSE 8529
# Fri, 10 Feb 2023 21:41:20 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ec61f8cffad1681adf6e5c6f8c51070d75f2161d772c59b296317679747e2f`  
		Last Modified: Fri, 10 Feb 2023 21:41:51 GMT  
		Size: 211.7 MB (211677800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59977b4ada21a00341a32868d332d8f335ab14093feaf3ca711cd31e4b7db319`  
		Last Modified: Fri, 10 Feb 2023 21:41:34 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559d59e6dde21cd70d89260297a1afe7537fb882d4641546a09913a928fbedd2`  
		Last Modified: Fri, 10 Feb 2023 21:41:34 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1184bb17d814dbb866bf75053957e1cc46e7834fb732cf27a548264a4646ce9`  
		Last Modified: Fri, 10 Feb 2023 21:41:34 GMT  
		Size: 262.0 B  
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
$ docker pull arangodb@sha256:865274e2f56149c9d1255aeb3c3a1dcb92c90d62294d4c7799e7013b0a23b644
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9` - linux; amd64

```console
$ docker pull arangodb@sha256:dc2a37589c0704de770ab1fed0a74f7c5c5f61d3d6f6c0b89444757af613d29c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202368296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8302c7dc2bde65898edefb87ead92c5521aa190ad212c71f2f397a31429cf9c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:12:56 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 11 Feb 2023 07:13:30 GMT
ENV ARANGO_VERSION=3.9.8
# Sat, 11 Feb 2023 07:13:30 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Sat, 11 Feb 2023 07:13:30 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.8-1_amd64.deb
# Sat, 11 Feb 2023 07:13:30 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.8-1_amd64.deb
# Sat, 11 Feb 2023 07:13:31 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.8-1_amd64.deb.asc
# Sat, 11 Feb 2023 07:13:56 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 11 Feb 2023 07:13:57 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 11 Feb 2023 07:13:58 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 11 Feb 2023 07:13:58 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 11 Feb 2023 07:13:58 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 11 Feb 2023 07:13:58 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 11 Feb 2023 07:13:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 07:13:59 GMT
EXPOSE 8529
# Sat, 11 Feb 2023 07:13:59 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd343ac9659d4dd1ed03832a272a663927c5e8a183591fb96ed92bc77affa1fc`  
		Last Modified: Sat, 11 Feb 2023 07:15:39 GMT  
		Size: 199.5 MB (199536180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b4e47a5c7f17353582fa74e0a89d8c3c2abc6cd2a3dd482e3bd02f12f399db`  
		Last Modified: Sat, 11 Feb 2023 07:15:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cf04c218bafe0ed4f7ac288174a74c32f2846305ede5411784b1b6a5f58aae`  
		Last Modified: Sat, 11 Feb 2023 07:15:17 GMT  
		Size: 2.1 KB (2083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a529910748aca4c2e3d8234f4264565ca2a26de774ecf3955244fd61e927226`  
		Last Modified: Sat, 11 Feb 2023 07:15:17 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9.8`

```console
$ docker pull arangodb@sha256:865274e2f56149c9d1255aeb3c3a1dcb92c90d62294d4c7799e7013b0a23b644
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9.8` - linux; amd64

```console
$ docker pull arangodb@sha256:dc2a37589c0704de770ab1fed0a74f7c5c5f61d3d6f6c0b89444757af613d29c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202368296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8302c7dc2bde65898edefb87ead92c5521aa190ad212c71f2f397a31429cf9c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:12:56 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 11 Feb 2023 07:13:30 GMT
ENV ARANGO_VERSION=3.9.8
# Sat, 11 Feb 2023 07:13:30 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Sat, 11 Feb 2023 07:13:30 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.8-1_amd64.deb
# Sat, 11 Feb 2023 07:13:30 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.8-1_amd64.deb
# Sat, 11 Feb 2023 07:13:31 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.8-1_amd64.deb.asc
# Sat, 11 Feb 2023 07:13:56 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 11 Feb 2023 07:13:57 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 11 Feb 2023 07:13:58 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 11 Feb 2023 07:13:58 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 11 Feb 2023 07:13:58 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 11 Feb 2023 07:13:58 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 11 Feb 2023 07:13:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 07:13:59 GMT
EXPOSE 8529
# Sat, 11 Feb 2023 07:13:59 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd343ac9659d4dd1ed03832a272a663927c5e8a183591fb96ed92bc77affa1fc`  
		Last Modified: Sat, 11 Feb 2023 07:15:39 GMT  
		Size: 199.5 MB (199536180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b4e47a5c7f17353582fa74e0a89d8c3c2abc6cd2a3dd482e3bd02f12f399db`  
		Last Modified: Sat, 11 Feb 2023 07:15:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cf04c218bafe0ed4f7ac288174a74c32f2846305ede5411784b1b6a5f58aae`  
		Last Modified: Sat, 11 Feb 2023 07:15:17 GMT  
		Size: 2.1 KB (2083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a529910748aca4c2e3d8234f4264565ca2a26de774ecf3955244fd61e927226`  
		Last Modified: Sat, 11 Feb 2023 07:15:17 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:2477f18ef19f7b4f9423bc5dd36efdad4abd261005794dc87821d09140f6c520
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:6d636e4c35f07d60f94a200c4aeb415e899881951037a7f1e8f8f2ff1bdfc108
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219637048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b406ed867db8704973416c7f9abbad168166efe7a43147c2764c5deffd79177a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:14:04 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Sat, 11 Feb 2023 07:14:04 GMT
ENV ARANGO_VERSION=3.10.3
# Sat, 11 Feb 2023 07:14:29 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Sat, 11 Feb 2023 07:14:31 GMT
ENV GLIBCXX_FORCE_NEW=1
# Sat, 11 Feb 2023 07:14:31 GMT
RUN echo "UTC" > /etc/timezone
# Sat, 11 Feb 2023 07:14:31 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Sat, 11 Feb 2023 07:14:31 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Sat, 11 Feb 2023 07:14:32 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Sat, 11 Feb 2023 07:14:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 07:14:32 GMT
EXPOSE 8529
# Sat, 11 Feb 2023 07:14:32 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f91516352792b0a83c3a19c8533ee3a80884dc0c3e10763bd114526245cfab`  
		Last Modified: Sat, 11 Feb 2023 07:16:12 GMT  
		Size: 216.8 MB (216826800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8067412b9ca332602e838f51cf865ee2cbec707bef662de31077bc77d8a96a7`  
		Last Modified: Sat, 11 Feb 2023 07:15:48 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76221af3d175c5aeb608cdef6ebaf9863948bbe113d4cbc1f70363b8566181f8`  
		Last Modified: Sat, 11 Feb 2023 07:15:48 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382b7163ed35efa634c24f98989d54f42e5da8d61a7fdaba18a9850bd96a8b31`  
		Last Modified: Sat, 11 Feb 2023 07:15:48 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `arangodb:latest` - linux; arm64 variant v8

```console
$ docker pull arangodb@sha256:6b5783485564f6ba62949982632c67f23142174ae4f681f5c557187291fae414
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.4 MB (214389785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be30a56e2da10ebc19123787e7ae49791dd08b349913b57e1ebb328f5f913b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:40:53 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 10 Feb 2023 21:40:53 GMT
ENV ARANGO_VERSION=3.10.3
# Fri, 10 Feb 2023 21:41:16 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 10 Feb 2023 21:41:19 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 10 Feb 2023 21:41:20 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 10 Feb 2023 21:41:20 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 10 Feb 2023 21:41:20 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 10 Feb 2023 21:41:20 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 10 Feb 2023 21:41:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Feb 2023 21:41:20 GMT
EXPOSE 8529
# Fri, 10 Feb 2023 21:41:20 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ec61f8cffad1681adf6e5c6f8c51070d75f2161d772c59b296317679747e2f`  
		Last Modified: Fri, 10 Feb 2023 21:41:51 GMT  
		Size: 211.7 MB (211677800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59977b4ada21a00341a32868d332d8f335ab14093feaf3ca711cd31e4b7db319`  
		Last Modified: Fri, 10 Feb 2023 21:41:34 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559d59e6dde21cd70d89260297a1afe7537fb882d4641546a09913a928fbedd2`  
		Last Modified: Fri, 10 Feb 2023 21:41:34 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1184bb17d814dbb866bf75053957e1cc46e7834fb732cf27a548264a4646ce9`  
		Last Modified: Fri, 10 Feb 2023 21:41:34 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
