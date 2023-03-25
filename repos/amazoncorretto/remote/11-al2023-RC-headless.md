## `amazoncorretto:11-al2023-RC-headless`

```console
$ docker pull amazoncorretto@sha256:1bef9732894572761368c39971ba51783a293f9126344ccc5b5cc4ebc8e88de3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-RC-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:38d1fb9032414b871f9a3038f58eac1a2c2a373dfe8ed91bb4470dea889c7edf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128089636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b080a3937bba25c05e593cda1f98460deeb34c21d6607d1540aa612fc32768cc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Mar 2023 23:27:36 GMT
COPY dir:42fc532f6972d7f1219ad34006b64c07b3ddb71b58ff263ab8c6aa98dab00541 in / 
# Wed, 15 Mar 2023 23:27:37 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 23:20:20 GMT
ARG version=11.0.18.10-1
# Fri, 24 Mar 2023 23:20:50 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 24 Mar 2023 23:20:50 GMT
ENV LANG=C.UTF-8
# Fri, 24 Mar 2023 23:20:51 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:b76f3b09316a1df6bfea69401870e8b9b4b467d535795e2ba0908c4d3bd438b9`  
		Last Modified: Wed, 15 Mar 2023 23:27:59 GMT  
		Size: 52.3 MB (52268492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100639de6e09357a669f5246e64d5832b929ffcccdebebb9fb5bf47acd0ab05a`  
		Last Modified: Fri, 24 Mar 2023 23:24:50 GMT  
		Size: 75.8 MB (75821144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-RC-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:5ca6803c441721268681013e283756411c3cdea4478416a9b6080255682c8603
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126277782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f623be3048e47bcb78772975549dfedc292752bb255b1bd71eb5c7fedc234da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Mar 2023 23:39:28 GMT
COPY dir:6216321324f425942c20403c2b329b848d15da8e81fc7ff80ef8243170c71d61 in / 
# Wed, 15 Mar 2023 23:39:29 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 22:45:00 GMT
ARG version=11.0.18.10-1
# Fri, 24 Mar 2023 22:45:28 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 24 Mar 2023 22:45:29 GMT
ENV LANG=C.UTF-8
# Fri, 24 Mar 2023 22:45:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:7ec7ca6df11f626205137bf1acf9efe68492ded671bc9f023577533727044ff6`  
		Last Modified: Wed, 15 Mar 2023 23:39:46 GMT  
		Size: 51.3 MB (51302659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3dcb16c191c645983ff9544ebd736d1047bbdcf6a0da047574976dbbefd481`  
		Last Modified: Fri, 24 Mar 2023 22:47:52 GMT  
		Size: 75.0 MB (74975123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
