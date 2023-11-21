## `amazoncorretto:8u392-al2-native-jdk`

```console
$ docker pull amazoncorretto@sha256:7b3448cd078fbffb8555b7fb08fd556a813ceb6a3028df7f388a267e5581dae5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u392-al2-native-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4abc35c53f2b5c8645f441e9c798014882ea5c920915a9c15aeec5ffd25036b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187936991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b16bc4adcc956d8a2a3803c0565a350216cd47f7c1de6da25a4da9c49ae3a0ec`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:54 GMT
COPY dir:ddf8ce4c235ebf92718d40c0041035b283a61cbd94b49610e57999ebc78d3ec6 in / 
# Tue, 21 Nov 2023 03:21:55 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:13:06 GMT
ARG version=1.8.0_392.b08-1
# Tue, 21 Nov 2023 04:15:32 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -v log4j-cve | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m) -name "*src.zip" -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Tue, 21 Nov 2023 04:15:33 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:15:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:0b4a6f011995244a95bff79a1298e83d230bc0aa22871a9c510745cafebec227`  
		Last Modified: Sun, 19 Nov 2023 03:18:53 GMT  
		Size: 62.6 MB (62641917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1632d26e20ec3d5e4ae422ed8fcd5565dec41a2b7f8705ffd9b3a0bb3ac8c7e3`  
		Last Modified: Tue, 21 Nov 2023 04:27:25 GMT  
		Size: 125.3 MB (125295074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u392-al2-native-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:a33ea10d849d8ad4e789ff352d4c90a66635e4c351f32484f6dd1c9b8eab9dbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131908457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:534dbef7d8b0ebc47bd7809ce02ef96d6e97dc0b5112d8a21460f7a5ec855856`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:39:49 GMT
COPY dir:21fc61c0ea1d6a14f556bdbd5029389644807e82a8de54f60438fc773e3e2465 in / 
# Tue, 21 Nov 2023 03:39:51 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 05:07:17 GMT
ARG version=1.8.0_392.b08-1
# Tue, 21 Nov 2023 05:08:36 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -v log4j-cve | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m) -name "*src.zip" -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Tue, 21 Nov 2023 05:08:37 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:08:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:ae50e077554aa1fe734206cc35e32dc0b0389a0ff7aa8d08626157b225100b42`  
		Last Modified: Mon, 20 Nov 2023 21:52:59 GMT  
		Size: 64.4 MB (64424056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70752e7a51dea370b663a9178922b64431745adc151139da35e9d9cac7c9bf83`  
		Last Modified: Tue, 21 Nov 2023 05:17:58 GMT  
		Size: 67.5 MB (67484401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
