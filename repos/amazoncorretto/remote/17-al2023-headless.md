## `amazoncorretto:17-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:6801368cacd2b918accacaf8ed7ffb8432706e45668fcc84c06732e88037dff1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1b51039a8ab47c65985c53ab72d3dba6a2c5c23c2e6f8811ced11b57beefda36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134546741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:292629e8ebc50f07ec96313e4c07bb457e1d01cb742e323e789340923dfaf133`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 19:19:51 GMT
COPY dir:1553450ba97bd4c18de1700ea705f96cfd1bbce308dbe1d199eeabb8ba521c1f in / 
# Mon, 12 Jun 2023 19:19:51 GMT
CMD ["/bin/bash"]
# Mon, 12 Jun 2023 19:40:45 GMT
ARG version=17.0.7.7-1
# Mon, 12 Jun 2023 19:40:46 GMT
ARG package_version=1
# Mon, 12 Jun 2023 19:41:22 GMT
# ARGS: package_version=1 version=17.0.7.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Mon, 12 Jun 2023 19:41:23 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jun 2023 19:41:23 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:91bcc9cfee804c575f99a19254c21e0ba20dd5e4d5999423d8b7d646fee7ee83`  
		Last Modified: Thu, 08 Jun 2023 03:04:23 GMT  
		Size: 52.3 MB (52259866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f3159c02cd27652f6c8251c4fcc63ba833385699a1514de14e76a98c98ed24`  
		Last Modified: Mon, 12 Jun 2023 19:46:48 GMT  
		Size: 82.3 MB (82286875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:6be51f0de59f68f79da7a275327b8e5d568ee37fa17096af355fe9b9437c12a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132910703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d37f9abaee498fc9610c73048c4b6eb9a62cc142e2dc141408f2b9fb4a3f9e06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 19:39:24 GMT
COPY dir:b120bacefa2a5fa3406277711f62c4883d7d0d799a5b2b67f75ac06b20d48583 in / 
# Mon, 12 Jun 2023 19:39:25 GMT
CMD ["/bin/bash"]
# Mon, 12 Jun 2023 19:58:14 GMT
ARG version=17.0.7.7-1
# Mon, 12 Jun 2023 19:58:14 GMT
ARG package_version=1
# Mon, 12 Jun 2023 19:58:45 GMT
# ARGS: package_version=1 version=17.0.7.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Mon, 12 Jun 2023 19:58:46 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jun 2023 19:58:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:3f7a91766b698ad4c2f6498113be92c8e4ff8009f265117cfc4ce3507cdbb6c3`  
		Last Modified: Thu, 08 Jun 2023 03:06:47 GMT  
		Size: 51.3 MB (51304663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70d79ddee041e226b4ad2317bd8fe1a72882ff66f38a5f3c53d7cac6e94dea6`  
		Last Modified: Mon, 12 Jun 2023 20:03:29 GMT  
		Size: 81.6 MB (81606040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
