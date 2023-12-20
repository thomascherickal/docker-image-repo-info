## `amazoncorretto:8u392-al2-native-jdk`

```console
$ docker pull amazoncorretto@sha256:e1512e3067163eee8d2d19af4d034c230ee982a9a61d36456d421d3bb2b5511d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u392-al2-native-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:50b836464a042e267e591c82a8489fbf2e72e98b78dbf2cdc1f1404312a02e60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187945241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a298c0a8ce616ccfdde3be1e75e8877ce8b5e858158a58fd43855a68111865f7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:49 GMT
COPY dir:fd6bc3e61b31127123e1a8c57613d9baa7f5605d29d858f885c6a105709aa8fd in / 
# Fri, 15 Dec 2023 20:22:50 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:39:44 GMT
ARG version=1.8.0_392.b08-1
# Fri, 15 Dec 2023 20:42:16 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -v log4j-cve | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m) -name "*src.zip" -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Fri, 15 Dec 2023 20:42:17 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:42:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:497f6fc6e5d7835e37c10dd6462da0d293dc146b7ead757dc61e580b47fd2578`  
		Last Modified: Tue, 12 Dec 2023 02:10:17 GMT  
		Size: 62.6 MB (62645650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4429c0323facd5b6389acab258670d8a4d2e11c040454ea94fe133cf8918a10`  
		Last Modified: Fri, 15 Dec 2023 20:54:16 GMT  
		Size: 125.3 MB (125299591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u392-al2-native-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:47d6346a3bbf4322f18f69c88fdd24fd194dbcd425ff4441331c89dc2ffb1281
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131925609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e074e4de3f6170d0660352fcad9e37b5935ff0945d50c94a1898651c7fde08`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 20 Dec 2023 01:32:23 GMT
COPY dir:380956fd469c5bff2cfd19545c66184d8301b431f1a3cd9c8338b2680a7f7a2b in / 
# Wed, 20 Dec 2023 01:32:24 GMT
CMD ["/bin/bash"]
# Wed, 20 Dec 2023 01:56:00 GMT
ARG version=1.8.0_392.b08-1
# Wed, 20 Dec 2023 01:57:19 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -v log4j-cve | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m) -name "*src.zip" -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Wed, 20 Dec 2023 01:57:20 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 01:57:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:1cdee3d784afc8dc3a31863ea6b75bfb24c3394d454dd5ca221d29fbd4c3f130`  
		Last Modified: Wed, 20 Dec 2023 01:32:56 GMT  
		Size: 64.4 MB (64445029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dd12e0a2b09b31cdf234ef578038fcbb0a88b0d5e741dc59b35e4f09087ec6`  
		Last Modified: Wed, 20 Dec 2023 02:07:00 GMT  
		Size: 67.5 MB (67480580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
