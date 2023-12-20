## `amazoncorretto:21-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:933e25501dc9ccca22765aea775b1fba0ccb97a7a92c38aab251bfa0bd11cebb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:21-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:cee620103875c2756ceba47212b9f3723aaed882443243a7e37e8dcfc2168b00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141636119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc0f13245ebc229b45a0f9acf5815fdfe124df28427a27e5793ec3dc33ac5ce`
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
# Fri, 15 Dec 2023 20:50:55 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 15 Dec 2023 20:50:55 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:50:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:97668dd20d4358bee95dea91ba9ca63bae56f3a5759ca22763c5940071e14884`  
		Last Modified: Fri, 15 Dec 2023 01:53:15 GMT  
		Size: 52.2 MB (52221241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8649e6ddff6ddaf625d416b636708ceb508ee50df27d1e422e8bd18fb5db81e5`  
		Last Modified: Fri, 15 Dec 2023 21:00:44 GMT  
		Size: 89.4 MB (89414878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:21-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:74a2c876fbd1e43fff5be797e1deb028f91502ce037d697ad574b7cebb24008e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139802413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:827b7af94bce0a63943399c04a5d6bd725cc7f0f1d5e8e0252a841a4f41c1ff9`
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
# Wed, 20 Dec 2023 02:04:18 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 20 Dec 2023 02:04:19 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 02:04:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:62dac1e13f9aa133cbec88aa21ded5df9ecd8a8ff67fc7ac9887cc25f3c387fb`  
		Last Modified: Mon, 18 Dec 2023 19:12:13 GMT  
		Size: 51.3 MB (51307984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613d48017ea08b79e2ca27662a98b1b267818273d18c12d5ab8e10d5c53becaa`  
		Last Modified: Wed, 20 Dec 2023 02:12:43 GMT  
		Size: 88.5 MB (88494429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
