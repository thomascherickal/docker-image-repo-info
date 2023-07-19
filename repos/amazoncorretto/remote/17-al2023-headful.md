## `amazoncorretto:17-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:4dfd119979c498f8fc8d537f6eb042b8fe6e7e7d43cc57879624453ee8f2aae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1522a8f3807f2ca94d3ce9d05558a5c2f3eedeeca37e763f31923f8ec410de4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135507681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cec00c5fc40692e334759ca2979e5f88809ea1220a657466d3f7ddbb4f2c2477`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Jul 2023 01:19:51 GMT
COPY dir:6bcf60f30d73b947ca07a9033109632c5faea18ed42743e2d6374e73b77d7d3a in / 
# Thu, 13 Jul 2023 01:19:51 GMT
CMD ["/bin/bash"]
# Wed, 19 Jul 2023 00:27:10 GMT
ARG version=17.0.8.7-1
# Wed, 19 Jul 2023 00:27:10 GMT
ARG package_version=1
# Wed, 19 Jul 2023 00:28:06 GMT
# ARGS: package_version=1 version=17.0.8.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 19 Jul 2023 00:28:06 GMT
ENV LANG=C.UTF-8
# Wed, 19 Jul 2023 00:28:06 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:3b8efe8e8a66806c25259c3f18e066eaef344018f8fb28a90db73bb2c2379601`  
		Last Modified: Fri, 07 Jul 2023 03:04:17 GMT  
		Size: 52.3 MB (52314023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb8b8514b12ec095f16393fd8bc4db9be56b55d1feb2365cd056da960d7b17a`  
		Last Modified: Wed, 19 Jul 2023 00:43:22 GMT  
		Size: 83.2 MB (83193658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e1fa405037df38d2204a0ff2709ca48fd5460baab5f17cc6edbdde01c0b1ee04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133888023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f614c1588049eb22bb2e5e454b85f4e97878fa79cf11b62ddf361abcfd253ab`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 13 Jul 2023 00:39:43 GMT
COPY dir:c971849a42f287ec4e3f54148631542a63e55183107bf0088e1c6913d556d33d in / 
# Thu, 13 Jul 2023 00:39:43 GMT
CMD ["/bin/bash"]
# Wed, 19 Jul 2023 00:44:38 GMT
ARG version=17.0.8.7-1
# Wed, 19 Jul 2023 00:44:38 GMT
ARG package_version=1
# Wed, 19 Jul 2023 00:45:30 GMT
# ARGS: package_version=1 version=17.0.8.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 19 Jul 2023 00:45:31 GMT
ENV LANG=C.UTF-8
# Wed, 19 Jul 2023 00:45:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:8df4f3b6d932cf6e3c467c8f32011fb41de2120bd82bf33f3469b54bbc38d5c5`  
		Last Modified: Fri, 07 Jul 2023 03:06:46 GMT  
		Size: 51.4 MB (51360865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60621970ab7e1771a429198ca6c6af5fcb5abbc7b59b2079eb5eee313d4e5af4`  
		Last Modified: Wed, 19 Jul 2023 00:59:05 GMT  
		Size: 82.5 MB (82527158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
