## `amazoncorretto:11-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:d2f83f43b700ed6dc470789498011667364fd609d2bf76038c422b7a386d2103
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:aa931dc85fb2ddf5b00ef10b471169828d73053dd2291cce2535591b154d12a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128761946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:844830e4c312d52f5ebb52de8a7e75ea45b5b884be1e4d916472feeaf91166e4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Mar 2023 18:20:25 GMT
COPY dir:c497d3c24209ef7d81f9c5abb7b10467dadda6adcaf860be5c03baaf83b5e43b in / 
# Tue, 28 Mar 2023 18:20:26 GMT
CMD ["/bin/bash"]
# Tue, 28 Mar 2023 19:10:48 GMT
ARG version=11.0.18.10-1
# Tue, 28 Mar 2023 19:11:38 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 28 Mar 2023 19:11:39 GMT
ENV LANG=C.UTF-8
# Tue, 28 Mar 2023 19:11:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:ee5c3b4d09bc9dd7590b7480cb385347f445a9fa73056b912cc9ed67ce54d0ce`  
		Last Modified: Fri, 24 Mar 2023 03:10:39 GMT  
		Size: 52.3 MB (52255843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a951a00cd00162f7c11fade0cf157f3e0617c69180ef916ea0585bdc1c575e5`  
		Last Modified: Tue, 28 Mar 2023 19:17:34 GMT  
		Size: 76.5 MB (76506103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:cc06becbb4a4546983e95400a362c961f84921b5848cceb8b741a0193fdce8e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127009793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ba74b99ea9928ef4713439bb59702b7b3d4a2fb18df24b018fae2f081f3703d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Mar 2023 18:39:52 GMT
COPY dir:0b162ee66bcb569c55f662aaca3ee7fff9bf5a498748208a280de7797569e5dc in / 
# Tue, 28 Mar 2023 18:39:53 GMT
CMD ["/bin/bash"]
# Thu, 20 Apr 2023 17:41:13 GMT
ARG version=11.0.19.7-1
# Thu, 20 Apr 2023 17:42:04 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Thu, 20 Apr 2023 17:42:05 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:42:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:3a410071be52fec7335cb666804896319a1ac81ef15af4c0f1302ffe8834b63f`  
		Last Modified: Fri, 24 Mar 2023 03:10:43 GMT  
		Size: 51.3 MB (51297211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01465a9b19324a05840e8616e3abd86f97a8b68ee39da17e86c970a57c5866be`  
		Last Modified: Thu, 20 Apr 2023 17:51:09 GMT  
		Size: 75.7 MB (75712582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
