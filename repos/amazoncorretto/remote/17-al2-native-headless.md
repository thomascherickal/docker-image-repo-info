## `amazoncorretto:17-al2-native-headless`

```console
$ docker pull amazoncorretto@sha256:6ab337f1a1ec5ea542650317b0a80715080a545c7ca7ed9898d420fd2d310616
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2-native-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:213eb97f1691507b962892fed0c9ccb7416f54ce1385878fd998fa73c80b18b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.3 MB (150332771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:876c9c8601003072cc0ccfcc1a63fd50bc8c96ac1469f66c742159e4658de072`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:49 GMT
COPY dir:fd6bc3e61b31127123e1a8c57613d9baa7f5605d29d858f885c6a105709aa8fd in / 
# Fri, 15 Dec 2023 20:22:50 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:45:52 GMT
ARG version=17.0.9.8-1
# Fri, 15 Dec 2023 20:47:59 GMT
# ARGS: version=17.0.9.8-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2.1.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -vE "log4j-cve|corretto" | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-17-amazon-corretto.$(uname -m) -name src.zip -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Fri, 15 Dec 2023 20:48:00 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:48:00 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:497f6fc6e5d7835e37c10dd6462da0d293dc146b7ead757dc61e580b47fd2578`  
		Last Modified: Tue, 12 Dec 2023 02:10:17 GMT  
		Size: 62.6 MB (62645650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56c26db4b14fd6673e52817e2f4373b3c760c3c4c3dfa4cf32e9581aab55ad2`  
		Last Modified: Fri, 15 Dec 2023 20:58:31 GMT  
		Size: 87.7 MB (87687121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2-native-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:9e613dce4ac79809151e10af02b4cb0217513f74210a3126b7366424fff69c78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.2 MB (144187137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34444ad20be94866b6ea2d14f4750e3f5a62d3ef54cb6320b7932fb183062d3c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 20 Dec 2023 01:32:23 GMT
COPY dir:380956fd469c5bff2cfd19545c66184d8301b431f1a3cd9c8338b2680a7f7a2b in / 
# Wed, 20 Dec 2023 01:32:24 GMT
CMD ["/bin/bash"]
# Wed, 20 Dec 2023 02:00:07 GMT
ARG version=17.0.9.8-1
# Wed, 20 Dec 2023 02:01:52 GMT
# ARGS: version=17.0.9.8-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2.1.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -vE "log4j-cve|corretto" | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-17-amazon-corretto.$(uname -m) -name src.zip -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Wed, 20 Dec 2023 02:01:54 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 02:01:54 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:1cdee3d784afc8dc3a31863ea6b75bfb24c3394d454dd5ca221d29fbd4c3f130`  
		Last Modified: Wed, 20 Dec 2023 01:32:56 GMT  
		Size: 64.4 MB (64445029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536ba57c2f85c75d3fd9bd9056fac5b0feda5a2e01899099ee28689344ffbef9`  
		Last Modified: Wed, 20 Dec 2023 02:10:53 GMT  
		Size: 79.7 MB (79742108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
