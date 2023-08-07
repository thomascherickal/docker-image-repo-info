## `amazoncorretto:17-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:458be45615e499d3e4c3a4a4e6b0b8e4a3b8ff5039bb9fe294e909ae74f7bcf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e914e94f61e2179346388c5bf713817784e198972c25eb00bfbd9c5c7a8dded9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134812889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3ef0554999a96730620ed663288d2dd0f46f817500eb341649e79d432e65326`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:58:54 GMT
COPY dir:1f2861cb5cb66982b608640300c5c9fa18eb5f3b855ebdd670700b8f8998b047 in / 
# Mon, 07 Aug 2023 19:58:55 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:56:04 GMT
ARG version=17.0.8.7-1
# Mon, 07 Aug 2023 20:56:04 GMT
ARG package_version=1
# Mon, 07 Aug 2023 20:56:47 GMT
# ARGS: package_version=1 version=17.0.8.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Mon, 07 Aug 2023 20:56:47 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:56:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:f87c7e5d5d0812576f02b4bd88ec48dfecf7a6fa89ac4925de3439f1546d8bda`  
		Last Modified: Thu, 27 Jul 2023 17:50:07 GMT  
		Size: 52.3 MB (52309413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f786d0891d564be49d565f06ef055ed61c7a13388a98e759b33fe82d6a1188`  
		Last Modified: Mon, 07 Aug 2023 21:07:54 GMT  
		Size: 82.5 MB (82503476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:386538dcd12d21242787d965b297fb71fa1c2053a62eb49a59a9d2f9098b9c10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133172081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91d90a6da9b6d29351ffb2cdc99385b456ccd0300c8680ce13be81d5c3aa6a95`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:40:41 GMT
COPY dir:d866155bb3759779912648033754c105594f55cc5e898364d07a4900eb79c222 in / 
# Mon, 07 Aug 2023 19:40:41 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:27:09 GMT
ARG version=17.0.8.7-1
# Mon, 07 Aug 2023 20:27:09 GMT
ARG package_version=1
# Mon, 07 Aug 2023 20:27:45 GMT
# ARGS: package_version=1 version=17.0.8.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Mon, 07 Aug 2023 20:27:46 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:27:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:28978a1daafcb3277e8070ffe6b95fb9b5a83e6ffe571c09bd0354db9d3da1cd`  
		Last Modified: Thu, 27 Jul 2023 17:49:44 GMT  
		Size: 51.3 MB (51348282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ad54b055e22555606cc9962ffd6172c850a71e267c91045be6c1c785026804`  
		Last Modified: Mon, 07 Aug 2023 20:42:03 GMT  
		Size: 81.8 MB (81823799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
