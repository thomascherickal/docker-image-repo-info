## `amazoncorretto:11-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:1702ffd63f56fb6ad033265e78b1ec38b4cebd942c0f9be538a607b0c94aa782
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3164df0a9c70fdf6c509563d157187d9a26d89613a60d08088bed4cab8881f44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (129025719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb8e0eb77b68e15aa67be4d01b3ae30f48c72ede5d6bd857e488112b2cde080`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:58:54 GMT
COPY dir:1f2861cb5cb66982b608640300c5c9fa18eb5f3b855ebdd670700b8f8998b047 in / 
# Mon, 07 Aug 2023 19:58:55 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:52:57 GMT
ARG version=11.0.20.8-1
# Mon, 07 Aug 2023 20:53:52 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Mon, 07 Aug 2023 20:53:52 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:53:53 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:f87c7e5d5d0812576f02b4bd88ec48dfecf7a6fa89ac4925de3439f1546d8bda`  
		Last Modified: Thu, 27 Jul 2023 17:50:07 GMT  
		Size: 52.3 MB (52309413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b35615da7a3df67f0cf91e9a0beade91d8cb6abf8b7216aab6a06ff718da72`  
		Last Modified: Mon, 07 Aug 2023 21:05:41 GMT  
		Size: 76.7 MB (76716306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:53439a586b3c417ac6a7fdd37ffc894ba6d5125a660c737c301d092a0c50e682
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127216354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30690299b7ae16a318d8b49c99a236d6ca3854c2e91aa30c3238e026e6d5feed`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:40:41 GMT
COPY dir:d866155bb3759779912648033754c105594f55cc5e898364d07a4900eb79c222 in / 
# Mon, 07 Aug 2023 19:40:41 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:24:05 GMT
ARG version=11.0.20.8-1
# Mon, 07 Aug 2023 20:25:07 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Mon, 07 Aug 2023 20:25:08 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:25:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:28978a1daafcb3277e8070ffe6b95fb9b5a83e6ffe571c09bd0354db9d3da1cd`  
		Last Modified: Thu, 27 Jul 2023 17:49:44 GMT  
		Size: 51.3 MB (51348282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd313f3b44042cc6acb9fb76ffd821d8056b0d1f2c56a445b8eec902eba26c12`  
		Last Modified: Mon, 07 Aug 2023 20:38:20 GMT  
		Size: 75.9 MB (75868072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
