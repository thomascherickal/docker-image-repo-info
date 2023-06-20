## `amazoncorretto:11-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:28a362dcd1377ec99464d9c39ef47ccc21d7178414362c36e3ed19e75744bad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:a9a4e262d8fa8d4ff5e1382ea76da3f6ab2ed156131960205e3f4fadb64ca4aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128099865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5adfaf6d071bb96fab3e2ee3dc9900f29029c06da2b589814704c509be918c5c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 20 Jun 2023 22:19:53 GMT
COPY dir:63b753315cbc8a46d071e63503518488c1171a5492a355d5915f823055385aa8 in / 
# Tue, 20 Jun 2023 22:19:53 GMT
CMD ["/bin/bash"]
# Tue, 20 Jun 2023 22:54:31 GMT
ARG version=11.0.19.7-1
# Tue, 20 Jun 2023 22:55:09 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 20 Jun 2023 22:55:09 GMT
ENV LANG=C.UTF-8
# Tue, 20 Jun 2023 22:55:09 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:a802d1401e244b250dd1bf27864d0c9b6b46b98aa0b6061bce13e9dc82bc082e`  
		Last Modified: Tue, 13 Jun 2023 21:23:05 GMT  
		Size: 52.3 MB (52256179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46321f8b74056641ecf3617c0417f3510c340472f317421e351cc3ccee95ef2`  
		Last Modified: Tue, 20 Jun 2023 23:01:07 GMT  
		Size: 75.8 MB (75843686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:ebbd69bd325e35adb46e222c57642fa980770bf48427689ba3adbf1d42040c3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126316155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a4fd93d2001517f84900d9915beea34f2f96a4d78072d9124d7c9923506c9a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 12 Jun 2023 19:39:24 GMT
COPY dir:b120bacefa2a5fa3406277711f62c4883d7d0d799a5b2b67f75ac06b20d48583 in / 
# Mon, 12 Jun 2023 19:39:25 GMT
CMD ["/bin/bash"]
# Mon, 12 Jun 2023 19:56:49 GMT
ARG version=11.0.19.7-1
# Mon, 12 Jun 2023 19:57:24 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Mon, 12 Jun 2023 19:57:25 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jun 2023 19:57:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:3f7a91766b698ad4c2f6498113be92c8e4ff8009f265117cfc4ce3507cdbb6c3`  
		Last Modified: Thu, 08 Jun 2023 03:06:47 GMT  
		Size: 51.3 MB (51304663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e722c973850e83e875890fe2f1632e0ee343ae6aa913bd5f0000d6cb93cce74`  
		Last Modified: Mon, 12 Jun 2023 20:02:11 GMT  
		Size: 75.0 MB (75011492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
