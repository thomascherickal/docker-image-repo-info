## `amazoncorretto:21-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:5fb312b146df76571bc48abe6fc5a1279b7ce88f32a27102f732f1a386775224
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:21-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6862726c409a88dd177cfcb7b872e119b2a446944c149b5d4b0a5124db8def85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142420701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48a1d876ab28adf939b231c62c1f6e08ef7597bf42af5fa560c8d8bf96474300`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 29 Aug 2023 18:29:04 GMT
COPY dir:5aeab1edfeaa7561058aadd3dc752f2959c8cd0e5442b979406e3948fdedb852 in / 
# Tue, 29 Aug 2023 18:29:05 GMT
CMD ["/bin/bash"]
# Fri, 22 Sep 2023 00:22:04 GMT
ARG version=21.0.0.35-1
# Fri, 22 Sep 2023 00:22:04 GMT
ARG package_version=1
# Fri, 22 Sep 2023 00:23:08 GMT
# ARGS: package_version=1 version=21.0.0.35-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 22 Sep 2023 00:23:08 GMT
ENV LANG=C.UTF-8
# Fri, 22 Sep 2023 00:23:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:8c169abda7fcf89d4baeaacf8e5d709a6112b4a6babe0c195a42404bca597f55`  
		Last Modified: Sat, 26 Aug 2023 03:05:59 GMT  
		Size: 52.3 MB (52287844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5613eed546856b0c5f44f02b5b4de9a5264bfaac7c1d8a077e625fc5ddc67c`  
		Last Modified: Fri, 22 Sep 2023 00:28:08 GMT  
		Size: 90.1 MB (90132857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:21-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:179beca7166398fbd26ef8503b04b02c8605c87e39e9d3d5a3ddc205995cc8ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140533855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:786ad07333411fbe5030f31acd7afdd25a98398c0c4c5b8f2a41d8e6f7d63327`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 29 Aug 2023 18:40:45 GMT
COPY dir:0004a2667b3e5dc5080ba46954457d05835caf07f7030d94b953f1c3cede9b0c in / 
# Tue, 29 Aug 2023 18:40:47 GMT
CMD ["/bin/bash"]
# Fri, 22 Sep 2023 00:42:29 GMT
ARG version=21.0.0.35-1
# Fri, 22 Sep 2023 00:42:29 GMT
ARG package_version=1
# Fri, 22 Sep 2023 00:43:22 GMT
# ARGS: package_version=1 version=21.0.0.35-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 22 Sep 2023 00:43:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Sep 2023 00:43:23 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:8e2acd49419010bc77a61e38a85963f09e403f004635f24c436d177a08df1040`  
		Last Modified: Sat, 26 Aug 2023 03:06:10 GMT  
		Size: 51.3 MB (51324150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ceac8e14f5315545234988f4cb72b67062cfa833340ace09f50706944b9895`  
		Last Modified: Fri, 22 Sep 2023 00:47:43 GMT  
		Size: 89.2 MB (89209705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
