## `amazoncorretto:11-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:3e5582aab88288d8ed1a7bc2eccf9c85ffafa72b97f870befc1b69c1a895432f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:9337c864e396745ada7f6faa78ff9b0f0a489a431560ec9a70f5f076ad169ddf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (129015589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf5acbbd1690ab1eb0627812203400fec20d00ed94492d8145b2164479cfbda`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 20:19:35 GMT
COPY dir:c2400bc0d1a5c32eb725de8e35d10b308c821586fa71a0a3f5ba3aa5cf9bb127 in / 
# Tue, 22 Aug 2023 20:19:35 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:28:43 GMT
ARG version=11.0.20.8-1
# Tue, 22 Aug 2023 21:29:39 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 22 Aug 2023 21:29:39 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:29:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:1e6dafe971b21b19c13aac9adec0ca5084ccd36d780a9b704ea649071d8e7bb9`  
		Last Modified: Thu, 10 Aug 2023 03:05:52 GMT  
		Size: 52.3 MB (52305790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9106e03b64bdb3e4509bf071fb1b4f3b7b7178f0c72fad09d905c545df6e7b50`  
		Last Modified: Tue, 22 Aug 2023 21:40:46 GMT  
		Size: 76.7 MB (76709799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:148095d3b2ec34d1bcfb9f457d1bccfd8ee686a310ccaa34bed2f93c821b3335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127223148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907e13226b970ba9f5d86cc0332016ce921048966922ba8569d3560b6a09595c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 19:39:35 GMT
COPY dir:92c63817c19adbcfee66efbdf593beff7587a951a074d0392645d3c4900d19b4 in / 
# Tue, 22 Aug 2023 19:39:36 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:08:34 GMT
ARG version=11.0.20.8-1
# Tue, 22 Aug 2023 21:09:26 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 22 Aug 2023 21:09:27 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:09:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:9fbecb9d3a17a188c49f0cab3521b4c760f46722f3e0e83726ccf3f972d8acbf`  
		Last Modified: Thu, 10 Aug 2023 03:04:18 GMT  
		Size: 51.3 MB (51348140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f81c8d8a5414f6b09107b9a96ada5009c405f39993d2d5c491aab16ec739240`  
		Last Modified: Tue, 22 Aug 2023 21:18:16 GMT  
		Size: 75.9 MB (75875008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
