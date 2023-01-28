## `arangodb:latest`

```console
$ docker pull arangodb@sha256:e7f871b3e1b49efcbec91f92fb2911f4dc49575bbfeec7e5010597107c7420c0
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
$ docker pull arangodb@sha256:17f65c9975aad44a7f92b3fa389b38dd09dbfb2ebf27462be8edd8cfbd0e579c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.4 MB (214360728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ad59bc40b956a5049a42835f95fce7e7a190079f52bb125857ade4a1e415e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["arangod"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 06:03:28 GMT
MAINTAINER Frank Celler <info@arangodb.com>
# Fri, 27 Jan 2023 22:39:13 GMT
ENV ARANGO_VERSION=3.10.3
# Fri, 27 Jan 2023 22:39:35 GMT
RUN apk add --no-cache gnupg pwgen binutils numactl numactl-tools nodejs yarn &&     yarn global add foxx-cli@2.1.1 &&     apk del yarn &&     gpg --batch --keyserver keys.openpgp.org --recv-keys CD8CB0F1E0AD5B52E93F41E7EA93F5E56E751E9B &&     mkdir /docker-entrypoint-initdb.d &&     cd /tmp                                &&     arch="$(apk --print-arch)"             &&     case "$arch" in                                   x86_64)  dpkgArch='amd64'          ;;         aarch64) dpkgArch='arm64'          ;;         *) echo >&2 "unsupported: $arch" && exit 1 ;;     esac                                   &&     ARANGO_URL="https://download.arangodb.com/arangodb310/DEBIAN/$dpkgArch" &&     ARANGO_PACKAGE="arangodb3_${ARANGO_VERSION}-1_${dpkgArch}.deb" &&     ARANGO_PACKAGE_URL="${ARANGO_URL}/${ARANGO_PACKAGE}" &&     ARANGO_SIGNATURE_URL="${ARANGO_PACKAGE_URL}.asc" &&     wget ${ARANGO_SIGNATURE_URL}           &&     wget ${ARANGO_PACKAGE_URL}             &&     gpg --verify ${ARANGO_PACKAGE}.asc     &&     ar x ${ARANGO_PACKAGE} data.tar.gz     &&     tar -C / -x -z -f data.tar.gz          &&     sed -ri         -e 's!127\.0\.0\.1!0.0.0.0!g'         -e 's!^(file\s*=\s*).*!\1 -!'         -e 's!^\s*uid\s*=.*!!'         /etc/arangodb3/arangod.conf        &&     chgrp -R 0 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     chmod -R 775 /var/lib/arangodb3 /var/lib/arangodb3-apps &&     rm -f /usr/bin/foxx &&     rm -f ${ARANGO_PACKAGE}* data.tar.gz &&     apk del gnupg
# Fri, 27 Jan 2023 22:39:39 GMT
ENV GLIBCXX_FORCE_NEW=1
# Fri, 27 Jan 2023 22:39:39 GMT
RUN echo "UTC" > /etc/timezone
# Fri, 27 Jan 2023 22:39:39 GMT
VOLUME [/var/lib/arangodb3 /var/lib/arangodb3-apps]
# Fri, 27 Jan 2023 22:39:39 GMT
COPY file:5186b735a7f691f0963e16d7add12851632ad73eceed0dc74092096025935cb4 in /entrypoint.sh 
# Fri, 27 Jan 2023 22:39:39 GMT
COPY file:e891c9dc63d937e22dc27abb45afa31518cd659993e0c54dab0f6cde8d994063 in /usr/bin/foxx 
# Fri, 27 Jan 2023 22:39:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 27 Jan 2023 22:39:40 GMT
EXPOSE 8529
# Fri, 27 Jan 2023 22:39:40 GMT
CMD ["arangod"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3d89e4a791fde9f5f79176012765e91a24ee6d7e5ee7fc52caae3b093e8f6f`  
		Last Modified: Fri, 27 Jan 2023 22:40:11 GMT  
		Size: 211.7 MB (211650486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7554fce1fc5639835ff71530ec139ccc248b1e90e7aa23c72ce98534a8f5bf9`  
		Last Modified: Fri, 27 Jan 2023 22:39:53 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540d052851b52e5a4f2bd409c75e19f89193993c0831bc8a22be8da41c69d42b`  
		Last Modified: Fri, 27 Jan 2023 22:39:53 GMT  
		Size: 2.1 KB (2086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275da84480f52cc656ab4d5cf1a73beee02bc2ddccd2f64d3f5af50d44412d33`  
		Last Modified: Fri, 27 Jan 2023 22:39:53 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
