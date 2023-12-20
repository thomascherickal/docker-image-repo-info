## `amazoncorretto:11-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:c0da2ef3ecb69950445b781c4955ea5d0fe25ac087b383770f24e980cdcd4368
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b38e775c6bc440d19a212cefa497142a5edee9673f81dd7665ae2db4baf539e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128980796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acd710346cddea14ab34f105d5d0c69fbfa29617ce8d95a112b11fbb13906057`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:29 GMT
COPY dir:6a0327957e10cfc5aab398cafdbbdbefb52a510a0fb73d8bf1952a36ff5452a4 in / 
# Fri, 15 Dec 2023 20:22:30 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:43:10 GMT
ARG version=11.0.21.9-1
# Fri, 15 Dec 2023 20:44:10 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 15 Dec 2023 20:44:11 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:44:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:97668dd20d4358bee95dea91ba9ca63bae56f3a5759ca22763c5940071e14884`  
		Last Modified: Fri, 15 Dec 2023 01:53:15 GMT  
		Size: 52.2 MB (52221241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed240a9278d8860778f68ea3e555d5c43c077fcfd696c577b4e310d3300ac015`  
		Last Modified: Fri, 15 Dec 2023 20:55:52 GMT  
		Size: 76.8 MB (76759555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:a3d1cdcc81cc502b8c8bb6611198c996ec8ae98872eeab98a97af16c465f518e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127236503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bb9569ea1abcaa25ff134ae4293a46bad78d3bd7121536a82c4d31df5a134e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 20 Dec 2023 01:32:07 GMT
COPY dir:d006faf7e50cd8429d93f8cf8ea807b50b60a3c38783c4d247b3e56de7d9a3dc in / 
# Wed, 20 Dec 2023 01:32:07 GMT
CMD ["/bin/bash"]
# Wed, 20 Dec 2023 01:57:58 GMT
ARG version=11.0.21.9-1
# Wed, 20 Dec 2023 01:58:51 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 20 Dec 2023 01:58:52 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 01:58:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:62dac1e13f9aa133cbec88aa21ded5df9ecd8a8ff67fc7ac9887cc25f3c387fb`  
		Last Modified: Mon, 18 Dec 2023 19:12:13 GMT  
		Size: 51.3 MB (51307984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1716ec223694bd51fe6eb69cf0d91292172e96405e6961ffa20cb66db9672417`  
		Last Modified: Wed, 20 Dec 2023 02:08:30 GMT  
		Size: 75.9 MB (75928519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
