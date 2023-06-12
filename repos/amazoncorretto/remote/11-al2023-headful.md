## `amazoncorretto:11-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:63252de921f8f61130e2128b233d9ab06726496049f2a6355792aa89a1eaed20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d0753651ef5faea6e5837b95ca03a9e0f3c40dcbffb7dbbd49432b32578b6510
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128811494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3931f51f1ccce44acba1e2ee8841c007d6853e0ef18e548eb73a769721a2748f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 19:19:51 GMT
COPY dir:1553450ba97bd4c18de1700ea705f96cfd1bbce308dbe1d199eeabb8ba521c1f in / 
# Mon, 12 Jun 2023 19:19:51 GMT
CMD ["/bin/bash"]
# Mon, 12 Jun 2023 19:39:10 GMT
ARG version=11.0.19.7-1
# Mon, 12 Jun 2023 19:40:05 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Mon, 12 Jun 2023 19:40:05 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jun 2023 19:40:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:91bcc9cfee804c575f99a19254c21e0ba20dd5e4d5999423d8b7d646fee7ee83`  
		Last Modified: Thu, 08 Jun 2023 03:04:23 GMT  
		Size: 52.3 MB (52259866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cede2294156d3d64a62ce38e4b343e25e25d844521e43828904f0b449fed6b2`  
		Last Modified: Mon, 12 Jun 2023 19:45:39 GMT  
		Size: 76.6 MB (76551628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:bc00c7f3a74c3fbdd3303150722921a565e84b4eadf128dbab469a5b275374b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127022870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83640d181d41e2ae87b7d1507d38c498ab2af5c388d1491a309a61150ee8963`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 19:39:24 GMT
COPY dir:b120bacefa2a5fa3406277711f62c4883d7d0d799a5b2b67f75ac06b20d48583 in / 
# Mon, 12 Jun 2023 19:39:25 GMT
CMD ["/bin/bash"]
# Mon, 12 Jun 2023 19:56:49 GMT
ARG version=11.0.19.7-1
# Mon, 12 Jun 2023 19:57:40 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Mon, 12 Jun 2023 19:57:41 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jun 2023 19:57:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:3f7a91766b698ad4c2f6498113be92c8e4ff8009f265117cfc4ce3507cdbb6c3`  
		Last Modified: Thu, 08 Jun 2023 03:06:47 GMT  
		Size: 51.3 MB (51304663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c978f0f5a112c6414a9039c1a5efbb218441bdbe3fa66535f4b8b0f76b0c87`  
		Last Modified: Mon, 12 Jun 2023 20:02:25 GMT  
		Size: 75.7 MB (75718207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
