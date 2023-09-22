## `amazoncorretto:21-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:8c6cee17dd3ebdd5b9c1b2f217b243f97e03a1c025f0834920ea1b0645ab80cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:21-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:9028037d406342c9bf6b305ee750d048c30c363bf9253d84202ec4473e9d47e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141701543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf219cf81c365b1d04d8d8b42b7b333fb5a410e9a90acc966589197d49f32019`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 29 Aug 2023 18:29:04 GMT
COPY dir:5aeab1edfeaa7561058aadd3dc752f2959c8cd0e5442b979406e3948fdedb852 in / 
# Tue, 29 Aug 2023 18:29:05 GMT
CMD ["/bin/bash"]
# Fri, 22 Sep 2023 00:22:04 GMT
ARG version=21.0.0.35-1
# Fri, 22 Sep 2023 00:22:04 GMT
ARG package_version=1
# Fri, 22 Sep 2023 00:22:48 GMT
# ARGS: package_version=1 version=21.0.0.35-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 22 Sep 2023 00:22:48 GMT
ENV LANG=C.UTF-8
# Fri, 22 Sep 2023 00:22:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:8c169abda7fcf89d4baeaacf8e5d709a6112b4a6babe0c195a42404bca597f55`  
		Last Modified: Sat, 26 Aug 2023 03:05:59 GMT  
		Size: 52.3 MB (52287844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934533cb859b1dc1889d373e8089e14d35dd0c9843ae14451a214f91fa8116cb`  
		Last Modified: Fri, 22 Sep 2023 00:27:49 GMT  
		Size: 89.4 MB (89413699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:21-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1f26f76842b2e03dca7e6e7d8893d16f5a0011cd41ee2a163f53122ce429e8e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139810197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:119ce81d7cc64fe4713cd4852b776980fed1be36ad35b82e64345439f560e1d4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 29 Aug 2023 18:40:45 GMT
COPY dir:0004a2667b3e5dc5080ba46954457d05835caf07f7030d94b953f1c3cede9b0c in / 
# Tue, 29 Aug 2023 18:40:47 GMT
CMD ["/bin/bash"]
# Fri, 22 Sep 2023 00:42:29 GMT
ARG version=21.0.0.35-1
# Fri, 22 Sep 2023 00:42:29 GMT
ARG package_version=1
# Fri, 22 Sep 2023 00:43:05 GMT
# ARGS: package_version=1 version=21.0.0.35-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 22 Sep 2023 00:43:06 GMT
ENV LANG=C.UTF-8
# Fri, 22 Sep 2023 00:43:06 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:8e2acd49419010bc77a61e38a85963f09e403f004635f24c436d177a08df1040`  
		Last Modified: Sat, 26 Aug 2023 03:06:10 GMT  
		Size: 51.3 MB (51324150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cfd220e724d09e81314e869eb7a22a4e0b7bf94774a1e7260227594f8cbf11`  
		Last Modified: Fri, 22 Sep 2023 00:47:26 GMT  
		Size: 88.5 MB (88486047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
