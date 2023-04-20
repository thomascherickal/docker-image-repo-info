## `amazoncorretto:17-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:fa2b864fa3bc9016cb9a2fed5e65ed6459fa81bdb4f73a3c9dc87f3e444825ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:470b63ec6480e0f3d1e8a590dea18e975704a75bb820a9e6f6f5f008c7b74d65
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135198868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc01732f154d194963100297899e09b6125be34a559dc3025f61f80c8e8a5131`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Mar 2023 18:20:25 GMT
COPY dir:c497d3c24209ef7d81f9c5abb7b10467dadda6adcaf860be5c03baaf83b5e43b in / 
# Tue, 28 Mar 2023 18:20:26 GMT
CMD ["/bin/bash"]
# Tue, 28 Mar 2023 19:12:16 GMT
ARG version=17.0.6.10-1
# Tue, 28 Mar 2023 19:12:17 GMT
ARG package_version=1
# Tue, 28 Mar 2023 19:13:07 GMT
# ARGS: package_version=1 version=17.0.6.10-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 28 Mar 2023 19:13:08 GMT
ENV LANG=C.UTF-8
# Tue, 28 Mar 2023 19:13:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:ee5c3b4d09bc9dd7590b7480cb385347f445a9fa73056b912cc9ed67ce54d0ce`  
		Last Modified: Fri, 24 Mar 2023 03:10:39 GMT  
		Size: 52.3 MB (52255843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0197d80c0950c4eca6625f5df4d329b517787571a6022cf41f53cdc0507a3ed0`  
		Last Modified: Tue, 28 Mar 2023 19:19:01 GMT  
		Size: 82.9 MB (82943025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e6716fac1cbf66ae92180bcc094c16c7f095557515597cf5cf7064c1346779f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133603403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7675c1082a95c29e3aafdb867011d8a9130141f9a0290bf5e7f054f6af191c01`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Mar 2023 18:39:52 GMT
COPY dir:0b162ee66bcb569c55f662aaca3ee7fff9bf5a498748208a280de7797569e5dc in / 
# Tue, 28 Mar 2023 18:39:53 GMT
CMD ["/bin/bash"]
# Thu, 20 Apr 2023 17:43:09 GMT
ARG version=17.0.7.7-1
# Thu, 20 Apr 2023 17:43:09 GMT
ARG package_version=1
# Thu, 20 Apr 2023 17:44:01 GMT
# ARGS: package_version=1 version=17.0.7.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Thu, 20 Apr 2023 17:44:02 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:44:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:3a410071be52fec7335cb666804896319a1ac81ef15af4c0f1302ffe8834b63f`  
		Last Modified: Fri, 24 Mar 2023 03:10:43 GMT  
		Size: 51.3 MB (51297211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92371ff3ab7f2316940e2a3c16644ab2e3640e1389f37419a761bf4fd05e5385`  
		Last Modified: Thu, 20 Apr 2023 17:54:13 GMT  
		Size: 82.3 MB (82306192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
