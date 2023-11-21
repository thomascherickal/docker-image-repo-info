## `amazoncorretto:17-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:c6142174f8d1daacf30e28c79775efe70de2267a68e38bea3d2ec0ac2b664a24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:aa8ec9d479f57dfcaf10799d6cf1623adc844bb8f3c8a9c61650601e8bc8f1d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135225648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a36f80c85c17fdbe03d286f28483606393c3939848ba8f9bcb4595eaa9a5691`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:34 GMT
COPY dir:a736dc55b3f736cb7e8fc1978dac2536c3df3a8e3e684d650ab946ec3bfffd4d in / 
# Tue, 21 Nov 2023 03:21:35 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:19:35 GMT
ARG version=17.0.9.8-1
# Tue, 21 Nov 2023 04:19:35 GMT
ARG package_version=1
# Tue, 21 Nov 2023 04:20:35 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 04:20:35 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:20:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:bad342ce986c7387f9e03cc2deafa306717aed86685ac6e1705ccc016b283eca`  
		Last Modified: Tue, 14 Nov 2023 20:44:05 GMT  
		Size: 52.2 MB (52218672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fbe8207286aa0d854df386913d34192815bcc1000855451209df9a707eb02b`  
		Last Modified: Tue, 21 Nov 2023 04:31:18 GMT  
		Size: 83.0 MB (83006976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:ef5a53a794b831a547d6ad163e5ec215099de20d0009e5589d0608f5a07a108a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133834668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4c39eed57b6d1ab1feb3f28710672d5fb04a56a9d5d0b994bc40099a5c6ed4a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 03 Nov 2023 22:39:55 GMT
COPY dir:c10f7b11e978070d5aeb6ea4db7b31b48bfb2cb9b0062451e8bf9592fb61a2e4 in / 
# Fri, 03 Nov 2023 22:39:56 GMT
CMD ["/bin/bash"]
# Fri, 03 Nov 2023 23:00:54 GMT
ARG version=17.0.9.8-1
# Fri, 03 Nov 2023 23:00:54 GMT
ARG package_version=1
# Fri, 03 Nov 2023 23:01:47 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 03 Nov 2023 23:01:48 GMT
ENV LANG=C.UTF-8
# Fri, 03 Nov 2023 23:01:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:85509e5088985a7b5d6c9025cce59b920ce6ac3e2035241e3b24d9d86bfe0904`  
		Last Modified: Tue, 31 Oct 2023 01:59:43 GMT  
		Size: 51.5 MB (51484639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907791dc31e398b00427a37bb482f6f6bb7de54ae3c5cf52e74fcb177c8c4ea4`  
		Last Modified: Fri, 03 Nov 2023 23:11:46 GMT  
		Size: 82.4 MB (82350029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
