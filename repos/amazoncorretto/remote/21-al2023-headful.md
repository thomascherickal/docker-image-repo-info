## `amazoncorretto:21-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:f6808227f555a55b05c639c0c2b36142145917ba4524635f20bf74048c8646c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:21-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:0561d425729a33f97754eca15524333849afbda466e6b04ed502806fd8167701
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142342892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ddf8b144656a476cf1e539efc5b7efa5ab99762d2e350f035358cc4fb3da7ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:29 GMT
COPY dir:6a0327957e10cfc5aab398cafdbbdbefb52a510a0fb73d8bf1952a36ff5452a4 in / 
# Fri, 15 Dec 2023 20:22:30 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:50:11 GMT
ARG version=21.0.1.12-1
# Fri, 15 Dec 2023 20:50:11 GMT
ARG package_version=2
# Fri, 15 Dec 2023 20:51:16 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 15 Dec 2023 20:51:17 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:51:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:97668dd20d4358bee95dea91ba9ca63bae56f3a5759ca22763c5940071e14884`  
		Last Modified: Fri, 15 Dec 2023 01:53:15 GMT  
		Size: 52.2 MB (52221241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdc4b950382c4d2be79c06e13296e7b99693bf635cbe3b87e6d82865a623828`  
		Last Modified: Fri, 15 Dec 2023 21:01:04 GMT  
		Size: 90.1 MB (90121651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:21-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:94432851c60273170ec2b5fe38206283b587c1e9751b6ab09b6492925ebc5c91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140518856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fc15e43ec1adae0471c6f499c09d9f3dc389c11df6cd75699403545999b9082`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 20 Dec 2023 01:32:07 GMT
COPY dir:d006faf7e50cd8429d93f8cf8ea807b50b60a3c38783c4d247b3e56de7d9a3dc in / 
# Wed, 20 Dec 2023 01:32:07 GMT
CMD ["/bin/bash"]
# Wed, 20 Dec 2023 02:03:41 GMT
ARG version=21.0.1.12-1
# Wed, 20 Dec 2023 02:03:41 GMT
ARG package_version=2
# Wed, 20 Dec 2023 02:04:37 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 20 Dec 2023 02:04:39 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 02:04:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:62dac1e13f9aa133cbec88aa21ded5df9ecd8a8ff67fc7ac9887cc25f3c387fb`  
		Last Modified: Mon, 18 Dec 2023 19:12:13 GMT  
		Size: 51.3 MB (51307984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc79f4d86313a6608ed5f6a5435287746c7ae94c67f12c963c591743f2a1459f`  
		Last Modified: Wed, 20 Dec 2023 02:13:00 GMT  
		Size: 89.2 MB (89210872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
