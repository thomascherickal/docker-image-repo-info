## `amazoncorretto:17-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:b3ba523fc4d88be932e85b27d78bacd762a526424ecb57c0fdb4caa3a42c8112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ae84633b09ecc7c80f873ba744b2aa7498d6aabadc9ae494c1b846049e7a0690
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135229537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a551bb92f22c9c1558fcc2eaf9df9042156be4b66c3c7a52a67d21f06081cf12`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:29 GMT
COPY dir:6a0327957e10cfc5aab398cafdbbdbefb52a510a0fb73d8bf1952a36ff5452a4 in / 
# Fri, 15 Dec 2023 20:22:30 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:46:21 GMT
ARG version=17.0.9.8-1
# Fri, 15 Dec 2023 20:46:21 GMT
ARG package_version=1
# Fri, 15 Dec 2023 20:47:26 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 15 Dec 2023 20:47:27 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:47:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:97668dd20d4358bee95dea91ba9ca63bae56f3a5759ca22763c5940071e14884`  
		Last Modified: Fri, 15 Dec 2023 01:53:15 GMT  
		Size: 52.2 MB (52221241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311db123cfc207be2bb8ef8398915b1336dc64ec74e379edaab0965dd55c29e6`  
		Last Modified: Fri, 15 Dec 2023 20:58:12 GMT  
		Size: 83.0 MB (83008296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0b04f61ffc2b890bfccc39d0af2a5c5cc557831d51ec66bea200a627d186b51e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133653368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba730b0030c45193009deab92505594c68e5800b0b16921642ab932bd94bf1a5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 20 Dec 2023 01:32:07 GMT
COPY dir:d006faf7e50cd8429d93f8cf8ea807b50b60a3c38783c4d247b3e56de7d9a3dc in / 
# Wed, 20 Dec 2023 01:32:07 GMT
CMD ["/bin/bash"]
# Wed, 20 Dec 2023 02:00:30 GMT
ARG version=17.0.9.8-1
# Wed, 20 Dec 2023 02:00:30 GMT
ARG package_version=1
# Wed, 20 Dec 2023 02:01:28 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 20 Dec 2023 02:01:29 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 02:01:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:62dac1e13f9aa133cbec88aa21ded5df9ecd8a8ff67fc7ac9887cc25f3c387fb`  
		Last Modified: Mon, 18 Dec 2023 19:12:13 GMT  
		Size: 51.3 MB (51307984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93ddeb31306dc3f03b0d8e4ec08f75bd35c5430527f9bbfcf1d183b26af9a17`  
		Last Modified: Wed, 20 Dec 2023 02:10:37 GMT  
		Size: 82.3 MB (82345384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
