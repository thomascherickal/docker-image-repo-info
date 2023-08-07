## `amazoncorretto:11-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:c21afb4f7b60e2371d0e202cb451a9b10d5bffb7635f1b64395d6b7778ed9bed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3473b3fdf787a380d9d02d01915aee50af85a88759f4c3922942d991bfb0cb33
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128320744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e78edad59f3ec8f9f92f1f3c8091a0d5464fa7d3856be33bdf1b6776c45da64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:58:54 GMT
COPY dir:1f2861cb5cb66982b608640300c5c9fa18eb5f3b855ebdd670700b8f8998b047 in / 
# Mon, 07 Aug 2023 19:58:55 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:52:57 GMT
ARG version=11.0.20.8-1
# Mon, 07 Aug 2023 20:53:35 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Mon, 07 Aug 2023 20:53:35 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:53:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:f87c7e5d5d0812576f02b4bd88ec48dfecf7a6fa89ac4925de3439f1546d8bda`  
		Last Modified: Thu, 27 Jul 2023 17:50:07 GMT  
		Size: 52.3 MB (52309413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff10f70eb51e37584503e78ecc2676b0109e1cbeee9e05f3d43a6f3a6d2256dc`  
		Last Modified: Mon, 07 Aug 2023 21:05:21 GMT  
		Size: 76.0 MB (76011331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:4b273ec431ca0795f025c6e5dbf2cb08aaf26f137f5d42184754cc140de4413e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126507173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95346d22b8ffcee2128cfcb98197a78d98afc419e1104a0bdb7e80f0abee151d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:40:41 GMT
COPY dir:d866155bb3759779912648033754c105594f55cc5e898364d07a4900eb79c222 in / 
# Mon, 07 Aug 2023 19:40:41 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:24:05 GMT
ARG version=11.0.20.8-1
# Mon, 07 Aug 2023 20:24:51 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Mon, 07 Aug 2023 20:24:52 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:24:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:28978a1daafcb3277e8070ffe6b95fb9b5a83e6ffe571c09bd0354db9d3da1cd`  
		Last Modified: Thu, 27 Jul 2023 17:49:44 GMT  
		Size: 51.3 MB (51348282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7133f82a67b7e39adb5165e118a1e2a027239d82f951cf5976e358cbe38a29d`  
		Last Modified: Mon, 07 Aug 2023 20:38:03 GMT  
		Size: 75.2 MB (75158891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
