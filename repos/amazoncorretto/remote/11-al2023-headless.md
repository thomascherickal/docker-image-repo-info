## `amazoncorretto:11-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:4eb14d6776cdbb8d83ca48408bef07c10cf778e99be6d4f6c8bb89c5817fe192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:199833a5da96751cd1062b1128a2fa6f279a4f577538989c84e0be52509b0611
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128312551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:017efcc38bd4ce5eab34e22afc9723629636c219a84a81d0766d6f221335083a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 20:19:35 GMT
COPY dir:c2400bc0d1a5c32eb725de8e35d10b308c821586fa71a0a3f5ba3aa5cf9bb127 in / 
# Tue, 22 Aug 2023 20:19:35 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:28:43 GMT
ARG version=11.0.20.8-1
# Tue, 22 Aug 2023 21:29:21 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 22 Aug 2023 21:29:21 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:29:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:1e6dafe971b21b19c13aac9adec0ca5084ccd36d780a9b704ea649071d8e7bb9`  
		Last Modified: Thu, 10 Aug 2023 03:05:52 GMT  
		Size: 52.3 MB (52305790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b8f51909f99e8c53c434a53c2a0d91ea5fdc8a736673d2d61ffc9df64a1d12`  
		Last Modified: Tue, 22 Aug 2023 21:40:29 GMT  
		Size: 76.0 MB (76006761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:a7fb051f4919d36b532c7477479a45c2913b15998790f4981f889d8dcba8390f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126509671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a816dac62806a5fa098c9b8a7260922189da07cca00fdcb6aac76532bfd6269`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 19:39:35 GMT
COPY dir:92c63817c19adbcfee66efbdf593beff7587a951a074d0392645d3c4900d19b4 in / 
# Tue, 22 Aug 2023 19:39:36 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:08:34 GMT
ARG version=11.0.20.8-1
# Tue, 22 Aug 2023 21:09:09 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 22 Aug 2023 21:09:10 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:09:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:9fbecb9d3a17a188c49f0cab3521b4c760f46722f3e0e83726ccf3f972d8acbf`  
		Last Modified: Thu, 10 Aug 2023 03:04:18 GMT  
		Size: 51.3 MB (51348140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648931725753cf441dc08cc73bf9c9b29d9e1c323ccd3ed6b06bed17503c6249`  
		Last Modified: Tue, 22 Aug 2023 21:18:00 GMT  
		Size: 75.2 MB (75161531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
