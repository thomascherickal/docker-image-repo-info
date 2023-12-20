## `amazoncorretto:11-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:e54291dac867bafd8259791b41170a2599bbf255d5d1685fb802feee91216f73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6a2de9e7eeffab5d458b6ee4e447375b8d81fc5100e13d836bcee03954c2ea40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128279092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd23b748e01f5935b98f5b266265a9574da684397386113145a987a7ab7994b6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:29 GMT
COPY dir:6a0327957e10cfc5aab398cafdbbdbefb52a510a0fb73d8bf1952a36ff5452a4 in / 
# Fri, 15 Dec 2023 20:22:30 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:43:10 GMT
ARG version=11.0.21.9-1
# Fri, 15 Dec 2023 20:43:49 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 15 Dec 2023 20:43:49 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:43:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:97668dd20d4358bee95dea91ba9ca63bae56f3a5759ca22763c5940071e14884`  
		Last Modified: Fri, 15 Dec 2023 01:53:15 GMT  
		Size: 52.2 MB (52221241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc343c63f8e14763bd355afde899d512a98c4291a258dc3f33b222f53a35f75`  
		Last Modified: Fri, 15 Dec 2023 20:55:35 GMT  
		Size: 76.1 MB (76057851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:6781498822319cb93ba5a1cc0f0d72fa641b8be00244b4312ee1adbc29447ccd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126536474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6f4b2c2747b95d2fca676930c6103d537e54ff7ff61bf43ec4cb113d57ca0d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 20 Dec 2023 01:32:07 GMT
COPY dir:d006faf7e50cd8429d93f8cf8ea807b50b60a3c38783c4d247b3e56de7d9a3dc in / 
# Wed, 20 Dec 2023 01:32:07 GMT
CMD ["/bin/bash"]
# Wed, 20 Dec 2023 01:57:58 GMT
ARG version=11.0.21.9-1
# Wed, 20 Dec 2023 01:58:35 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 20 Dec 2023 01:58:36 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 01:58:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:62dac1e13f9aa133cbec88aa21ded5df9ecd8a8ff67fc7ac9887cc25f3c387fb`  
		Last Modified: Mon, 18 Dec 2023 19:12:13 GMT  
		Size: 51.3 MB (51307984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa44ba3375c478dfbcc8ebd8b82262e406df2cfba33d0a33b5a198dfef20f9f`  
		Last Modified: Wed, 20 Dec 2023 02:08:15 GMT  
		Size: 75.2 MB (75228490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
