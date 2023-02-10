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
