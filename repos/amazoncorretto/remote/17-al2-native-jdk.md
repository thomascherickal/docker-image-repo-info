## `amazoncorretto:17-al2-native-jdk`

```console
$ docker pull amazoncorretto@sha256:87dcd8707ac2c2c85e58568758cb397db6e67e4141fe3d53023a3d1157b960ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2-native-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7daa6a28ea27257ae47efbf435f36c8b98dd948efbb4e0732d2b20242a71d957
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.4 MB (228378673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b520aa8c8487fdddf9fd3ab56998655ddf4e91853355e5c4c62d03e21d9f248`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:54 GMT
COPY dir:ddf8ce4c235ebf92718d40c0041035b283a61cbd94b49610e57999ebc78d3ec6 in / 
# Tue, 21 Nov 2023 03:21:55 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:19:06 GMT
ARG version=17.0.9.8-1
# Tue, 21 Nov 2023 04:22:38 GMT
# ARGS: version=17.0.9.8-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2.1.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2.1.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2.1.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2.1.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && if [[ ${rpm} != *jmods* ]]; then       yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -vE "log4j-cve|corretto" | tr -s ' ' |cut -d ' ' -f 3 );       fi;       done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-17-amazon-corretto.$(uname -m) -name src.zip -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Tue, 21 Nov 2023 04:22:39 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:22:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:0b4a6f011995244a95bff79a1298e83d230bc0aa22871a9c510745cafebec227`  
		Last Modified: Sun, 19 Nov 2023 03:18:53 GMT  
		Size: 62.6 MB (62641917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922a8ce26a5060b362f16038f1d4ce0522139d8086da8aac74b699fe29c2abf4`  
		Last Modified: Tue, 21 Nov 2023 04:32:19 GMT  
		Size: 165.7 MB (165736756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2-native-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:c119fa20584d8af8456eef565ab9d7bdd9b308a8cf230e957f037beaf2737fea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220524843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0b46b6695d75c2bc5871a8a2be02b6d636ecd261e8e88d358590e4a235c206`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:39:49 GMT
COPY dir:21fc61c0ea1d6a14f556bdbd5029389644807e82a8de54f60438fc773e3e2465 in / 
# Tue, 21 Nov 2023 03:39:51 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 05:11:17 GMT
ARG version=17.0.9.8-1
# Tue, 21 Nov 2023 05:14:04 GMT
# ARGS: version=17.0.9.8-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2.1.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2.1.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2.1.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2.1.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && if [[ ${rpm} != *jmods* ]]; then       yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -vE "log4j-cve|corretto" | tr -s ' ' |cut -d ' ' -f 3 );       fi;       done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-17-amazon-corretto.$(uname -m) -name src.zip -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Tue, 21 Nov 2023 05:14:05 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:14:06 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:ae50e077554aa1fe734206cc35e32dc0b0389a0ff7aa8d08626157b225100b42`  
		Last Modified: Mon, 20 Nov 2023 21:52:59 GMT  
		Size: 64.4 MB (64424056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56ca7a58ecf5b9294dfe6f027eb5e9b7bd0ed52e3329fd8a6d15f83e95620b8`  
		Last Modified: Tue, 21 Nov 2023 05:22:38 GMT  
		Size: 156.1 MB (156100787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
