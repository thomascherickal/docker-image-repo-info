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
$ docker pull arangodb@sha256:51f26a384a4e8f77c2a7c746f3020e92aae4578efd503be1e2726543a3b93120
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10` - linux; amd64

```console
$ docker pull arangodb@sha256:e677bb691675c638935620d22cd959a7d1db49a5830b08bcacde41b239a55a37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219614135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:810966db200d53658daba71395e2604a3b5e59d0690e436c157623b460410d26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:42:19 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 27 Jan 2023 23:19:50 GMT
ENV ARANGO_VERSION=3.10.3
# Fri, 27 Jan 2023 23:20:16 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 27 Jan 2023 23:20:18 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 27 Jan 2023 23:20:18 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 27 Jan 2023 23:20:18 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 27 Jan 2023 23:20:18 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 27 Jan 2023 23:20:19 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 27 Jan 2023 23:20:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 Jan 2023 23:20:19 GMT
EXPOSE 8529
# Fri, 27 Jan 2023 23:20:19 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbf6d2efb32dea28c31e4b3397d0f8332e94d36d32397abd5ad25a21b121c1a`  
		Last Modified: Fri, 27 Jan 2023 23:21:32 GMT  
		Size: 216.8 MB (216805378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c38805d02782797aaabb8d86bb73596cb5e0615f994e73283a2e2e524e8ff68`  
		Last Modified: Fri, 27 Jan 2023 23:21:08 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac23a5fe0b52fc41f6945a0abbce1b011d37223e6d0469f15f29853cd0759bd`  
		Last Modified: Fri, 27 Jan 2023 23:21:08 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8191ee5c177d6d68c2e51bd4a69002088905e4a570b8d25320f8b6c42c26804`  
		Last Modified: Fri, 27 Jan 2023 23:21:08 GMT  
		Size: 261.0 B  
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
$ docker pull arangodb@sha256:51f26a384a4e8f77c2a7c746f3020e92aae4578efd503be1e2726543a3b93120
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:3.10.3` - linux; amd64

```console
$ docker pull arangodb@sha256:e677bb691675c638935620d22cd959a7d1db49a5830b08bcacde41b239a55a37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219614135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:810966db200d53658daba71395e2604a3b5e59d0690e436c157623b460410d26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:42:19 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 27 Jan 2023 23:19:50 GMT
ENV ARANGO_VERSION=3.10.3
# Fri, 27 Jan 2023 23:20:16 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 27 Jan 2023 23:20:18 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 27 Jan 2023 23:20:18 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 27 Jan 2023 23:20:18 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 27 Jan 2023 23:20:18 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 27 Jan 2023 23:20:19 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 27 Jan 2023 23:20:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 Jan 2023 23:20:19 GMT
EXPOSE 8529
# Fri, 27 Jan 2023 23:20:19 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbf6d2efb32dea28c31e4b3397d0f8332e94d36d32397abd5ad25a21b121c1a`  
		Last Modified: Fri, 27 Jan 2023 23:21:32 GMT  
		Size: 216.8 MB (216805378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c38805d02782797aaabb8d86bb73596cb5e0615f994e73283a2e2e524e8ff68`  
		Last Modified: Fri, 27 Jan 2023 23:21:08 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac23a5fe0b52fc41f6945a0abbce1b011d37223e6d0469f15f29853cd0759bd`  
		Last Modified: Fri, 27 Jan 2023 23:21:08 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8191ee5c177d6d68c2e51bd4a69002088905e4a570b8d25320f8b6c42c26804`  
		Last Modified: Fri, 27 Jan 2023 23:21:08 GMT  
		Size: 261.0 B  
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
$ docker pull arangodb@sha256:2a87ce7fd3bfb80fb57d802d533b960ed91c69df92ede6f3834550c9311a93d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8` - linux; amd64

```console
$ docker pull arangodb@sha256:82ccaafd5b9c219349bdafd666ee800bc00908d700af2962cc08d163e11de7fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195268712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e80ef161d591ff18c52eca3538ec44e42819183e354f709278962b14025a118`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:51:41 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 27 Oct 2022 00:44:25 GMT
ENV ARANGO_VERSION=3.8.8
# Thu, 27 Oct 2022 00:44:25 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Thu, 27 Oct 2022 00:44:25 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.8-1_amd64.deb
# Thu, 27 Oct 2022 00:44:25 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.8-1_amd64.deb
# Thu, 27 Oct 2022 00:44:25 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.8-1_amd64.deb.asc
# Thu, 27 Oct 2022 00:44:51 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 27 Oct 2022 00:44:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 27 Oct 2022 00:44:54 GMT
RUN echo "UTC" > /etc/timezone
# Thu, 27 Oct 2022 00:44:54 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 27 Oct 2022 00:44:54 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 27 Oct 2022 00:44:54 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 27 Oct 2022 00:44:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Oct 2022 00:44:54 GMT
EXPOSE 8529
# Thu, 27 Oct 2022 00:44:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487a9ea0d1ee31646f1db6eed2b72422eec6050cabde55ea9242e08219565270`  
		Last Modified: Thu, 27 Oct 2022 00:46:08 GMT  
		Size: 192.4 MB (192438735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7f0c4d39107a370e74ba90537142345ca825ce6adeb7b6b8cbf0935cbad919`  
		Last Modified: Thu, 27 Oct 2022 00:45:45 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f2bc8d483668b3099208c86d5ebab704d1a990a2d6f9a657f5e9b520c20d92`  
		Last Modified: Thu, 27 Oct 2022 00:45:45 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1975f6734b8a781ef62fe7666ce113b642303738fc119f1c99887943511c03`  
		Last Modified: Thu, 27 Oct 2022 00:45:45 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.8.8`

```console
$ docker pull arangodb@sha256:2a87ce7fd3bfb80fb57d802d533b960ed91c69df92ede6f3834550c9311a93d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.8.8` - linux; amd64

```console
$ docker pull arangodb@sha256:82ccaafd5b9c219349bdafd666ee800bc00908d700af2962cc08d163e11de7fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195268712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e80ef161d591ff18c52eca3538ec44e42819183e354f709278962b14025a118`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:51:41 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Thu, 27 Oct 2022 00:44:25 GMT
ENV ARANGO_VERSION=3.8.8
# Thu, 27 Oct 2022 00:44:25 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64
# Thu, 27 Oct 2022 00:44:25 GMT
ENV ARANGO_PACKAGE=arangodb3_3.8.8-1_amd64.deb
# Thu, 27 Oct 2022 00:44:25 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.8-1_amd64.deb
# Thu, 27 Oct 2022 00:44:25 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb38/DEBIAN/amd64/arangodb3_3.8.8-1_amd64.deb.asc
# Thu, 27 Oct 2022 00:44:51 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.0.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Thu, 27 Oct 2022 00:44:53 GMT
ENV GLIBCXX_FORCE_NEW=1
# Thu, 27 Oct 2022 00:44:54 GMT
RUN echo "UTC" > /etc/timezone
# Thu, 27 Oct 2022 00:44:54 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Thu, 27 Oct 2022 00:44:54 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Thu, 27 Oct 2022 00:44:54 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Thu, 27 Oct 2022 00:44:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 27 Oct 2022 00:44:54 GMT
EXPOSE 8529
# Thu, 27 Oct 2022 00:44:54 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487a9ea0d1ee31646f1db6eed2b72422eec6050cabde55ea9242e08219565270`  
		Last Modified: Thu, 27 Oct 2022 00:46:08 GMT  
		Size: 192.4 MB (192438735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7f0c4d39107a370e74ba90537142345ca825ce6adeb7b6b8cbf0935cbad919`  
		Last Modified: Thu, 27 Oct 2022 00:45:45 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f2bc8d483668b3099208c86d5ebab704d1a990a2d6f9a657f5e9b520c20d92`  
		Last Modified: Thu, 27 Oct 2022 00:45:45 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1975f6734b8a781ef62fe7666ce113b642303738fc119f1c99887943511c03`  
		Last Modified: Thu, 27 Oct 2022 00:45:45 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9`

```console
$ docker pull arangodb@sha256:6958db927de75e28a1e779c08145b3583d5ba16eda02bdc576edef6bab9aee4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9` - linux; amd64

```console
$ docker pull arangodb@sha256:fe7ef7c60f3c59505295233b3f7e8efba97f08b814b47fe58c194cfb749b45bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.3 MB (202342603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13208e0502f21a841fd66b19d94cae5d5590f43d742a56f42bd66ab5a7f848af`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:51:41 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 27 Jan 2023 23:19:17 GMT
ENV ARANGO_VERSION=3.9.8
# Fri, 27 Jan 2023 23:19:17 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Fri, 27 Jan 2023 23:19:17 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.8-1_amd64.deb
# Fri, 27 Jan 2023 23:19:17 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.8-1_amd64.deb
# Fri, 27 Jan 2023 23:19:17 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.8-1_amd64.deb.asc
# Fri, 27 Jan 2023 23:19:44 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 27 Jan 2023 23:19:46 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 27 Jan 2023 23:19:47 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 27 Jan 2023 23:19:47 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 27 Jan 2023 23:19:47 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 27 Jan 2023 23:19:47 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 27 Jan 2023 23:19:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 Jan 2023 23:19:47 GMT
EXPOSE 8529
# Fri, 27 Jan 2023 23:19:47 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c7c748d7ac2ecc994b86b8116e60ba4d542b0615d4da05c62e229e76e00347`  
		Last Modified: Fri, 27 Jan 2023 23:20:58 GMT  
		Size: 199.5 MB (199512624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d874a5f9673643b8aa03b0a2586a1b4ae446d5fc1f95db8f7d4dfbf637250623`  
		Last Modified: Fri, 27 Jan 2023 23:20:35 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2d8c6983a31affc3eba41ca2bbc5c2cac0fbaca49d96b102faad654772cd30`  
		Last Modified: Fri, 27 Jan 2023 23:20:35 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea7a24f6e438570ccd9ca7d94bb7784645e08ddc6276d92cbe69349bfcbab00`  
		Last Modified: Fri, 27 Jan 2023 23:20:35 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:3.9.8`

```console
$ docker pull arangodb@sha256:6958db927de75e28a1e779c08145b3583d5ba16eda02bdc576edef6bab9aee4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `arangodb:3.9.8` - linux; amd64

```console
$ docker pull arangodb@sha256:fe7ef7c60f3c59505295233b3f7e8efba97f08b814b47fe58c194cfb749b45bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.3 MB (202342603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13208e0502f21a841fd66b19d94cae5d5590f43d742a56f42bd66ab5a7f848af`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:51:41 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 27 Jan 2023 23:19:17 GMT
ENV ARANGO_VERSION=3.9.8
# Fri, 27 Jan 2023 23:19:17 GMT
ENV ARANGO_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64
# Fri, 27 Jan 2023 23:19:17 GMT
ENV ARANGO_PACKAGE=arangodb3_3.9.8-1_amd64.deb
# Fri, 27 Jan 2023 23:19:17 GMT
ENV ARANGO_PACKAGE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.8-1_amd64.deb
# Fri, 27 Jan 2023 23:19:17 GMT
ENV ARANGO_SIGNATURE_URL=https://download.arangodb.com/arangodb39/DEBIAN/amd64/arangodb3_3.9.8-1_amd64.deb.asc
# Fri, 27 Jan 2023 23:19:44 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 27 Jan 2023 23:19:46 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 27 Jan 2023 23:19:47 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 27 Jan 2023 23:19:47 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 27 Jan 2023 23:19:47 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 27 Jan 2023 23:19:47 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 27 Jan 2023 23:19:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 Jan 2023 23:19:47 GMT
EXPOSE 8529
# Fri, 27 Jan 2023 23:19:47 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c7c748d7ac2ecc994b86b8116e60ba4d542b0615d4da05c62e229e76e00347`  
		Last Modified: Fri, 27 Jan 2023 23:20:58 GMT  
		Size: 199.5 MB (199512624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d874a5f9673643b8aa03b0a2586a1b4ae446d5fc1f95db8f7d4dfbf637250623`  
		Last Modified: Fri, 27 Jan 2023 23:20:35 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2d8c6983a31affc3eba41ca2bbc5c2cac0fbaca49d96b102faad654772cd30`  
		Last Modified: Fri, 27 Jan 2023 23:20:35 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea7a24f6e438570ccd9ca7d94bb7784645e08ddc6276d92cbe69349bfcbab00`  
		Last Modified: Fri, 27 Jan 2023 23:20:35 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `arangodb:latest`

```console
$ docker pull arangodb@sha256:51f26a384a4e8f77c2a7c746f3020e92aae4578efd503be1e2726543a3b93120
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `arangodb:latest` - linux; amd64

```console
$ docker pull arangodb@sha256:e677bb691675c638935620d22cd959a7d1db49a5830b08bcacde41b239a55a37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219614135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:810966db200d53658daba71395e2604a3b5e59d0690e436c157623b460410d26`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:42:19 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 27 Jan 2023 23:19:50 GMT
ENV ARANGO_VERSION=3.10.3
# Fri, 27 Jan 2023 23:20:16 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 27 Jan 2023 23:20:18 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 27 Jan 2023 23:20:18 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 27 Jan 2023 23:20:18 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 27 Jan 2023 23:20:18 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 27 Jan 2023 23:20:19 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 27 Jan 2023 23:20:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 Jan 2023 23:20:19 GMT
EXPOSE 8529
# Fri, 27 Jan 2023 23:20:19 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbf6d2efb32dea28c31e4b3397d0f8332e94d36d32397abd5ad25a21b121c1a`  
		Last Modified: Fri, 27 Jan 2023 23:21:32 GMT  
		Size: 216.8 MB (216805378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c38805d02782797aaabb8d86bb73596cb5e0615f994e73283a2e2e524e8ff68`  
		Last Modified: Fri, 27 Jan 2023 23:21:08 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac23a5fe0b52fc41f6945a0abbce1b011d37223e6d0469f15f29853cd0759bd`  
		Last Modified: Fri, 27 Jan 2023 23:21:08 GMT  
		Size: 2.1 KB (2085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8191ee5c177d6d68c2e51bd4a69002088905e4a570b8d25320f8b6c42c26804`  
		Last Modified: Fri, 27 Jan 2023 23:21:08 GMT  
		Size: 261.0 B  
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
