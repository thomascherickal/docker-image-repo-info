## `maven:3-amazoncorretto-17-al2023`

```console
$ docker pull maven@sha256:c668a2ee8a376c82977408f57970a996f5d6d3d5f017149d02d396eed2c850b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17-al2023` - linux; amd64

```console
$ docker pull maven@sha256:5ec6a61e3f3eb477716e4f2a070bfee87ce5e0a03dd47983a6eeb2599bf43081
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.4 MB (255361463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1488f690ab78adb8ca1fd2fa2183734bd9fc2369727a9b76c651f374090584ab`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 29 Aug 2023 18:29:04 GMT
COPY dir:5aeab1edfeaa7561058aadd3dc752f2959c8cd0e5442b979406e3948fdedb852 in / 
# Tue, 29 Aug 2023 18:29:05 GMT
CMD ["/bin/bash"]
# Tue, 29 Aug 2023 19:45:57 GMT
ARG version=17.0.8.7-1
# Tue, 29 Aug 2023 19:45:57 GMT
ARG package_version=1
# Tue, 29 Aug 2023 19:46:21 GMT
# ARGS: package_version=1 version=17.0.8.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 29 Aug 2023 19:46:22 GMT
ENV LANG=C.UTF-8
# Tue, 29 Aug 2023 19:46:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Mon, 28 Aug 2023 11:26:15 GMT
RUN yum install -y tar which gzip findutils # TODO remove # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
ARG MAVEN_VERSION=3.9.4
# Mon, 28 Aug 2023 11:26:15 GMT
ARG USER_HOME_DIR=/root
# Mon, 28 Aug 2023 11:26:15 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 28 Aug 2023 11:26:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 28 Aug 2023 11:26:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8c169abda7fcf89d4baeaacf8e5d709a6112b4a6babe0c195a42404bca597f55`  
		Last Modified: Sat, 26 Aug 2023 03:05:59 GMT  
		Size: 52.3 MB (52287844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf795763d5dcca11336815cbb05f4c5b4b0b5d8d4a15c0b06167569bb97469a`  
		Last Modified: Tue, 29 Aug 2023 19:56:55 GMT  
		Size: 157.0 MB (156966024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c031ae516b3d6fb0430d2ad6a82f60a13760633da230272f5ec4ea6654532f19`  
		Last Modified: Tue, 29 Aug 2023 20:20:12 GMT  
		Size: 36.7 MB (36699789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db9c94644c6db81597b9de2a5513d57f61439fa1505478339c681960c4b3e42`  
		Last Modified: Tue, 29 Aug 2023 20:20:10 GMT  
		Size: 9.4 MB (9406424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8809ccbb14baf6afea47a3e9af02681b50978d4966f1353ac97211a04cd1a9`  
		Last Modified: Tue, 29 Aug 2023 20:20:09 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c61d1fa07e0dba1fbeb8c163e25592334de0d2cff5fbb2bea082f535090ca`  
		Last Modified: Tue, 29 Aug 2023 20:20:09 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698c1fa08bfeed6f9b9591fccc233012fabca04a77ac6ee5365804f814f72762`  
		Last Modified: Tue, 29 Aug 2023 20:20:09 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:dee887680bf8c9ed551486fc5d728b46ba79d5f883d15ef3f8982b7b96176533
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.8 MB (252791842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0466da27a7aa0c808c76ad260fbf85dc6daf0fb4bf287dffb32143beb91ae06`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 29 Aug 2023 18:40:45 GMT
COPY dir:0004a2667b3e5dc5080ba46954457d05835caf07f7030d94b953f1c3cede9b0c in / 
# Tue, 29 Aug 2023 18:40:47 GMT
CMD ["/bin/bash"]
# Tue, 29 Aug 2023 19:11:26 GMT
ARG version=17.0.8.7-1
# Tue, 29 Aug 2023 19:11:26 GMT
ARG package_version=1
# Tue, 29 Aug 2023 19:11:47 GMT
# ARGS: package_version=1 version=17.0.8.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 29 Aug 2023 19:11:49 GMT
ENV LANG=C.UTF-8
# Tue, 29 Aug 2023 19:11:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Mon, 28 Aug 2023 11:26:15 GMT
RUN yum install -y tar which gzip findutils # TODO remove # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
ARG MAVEN_VERSION=3.9.4
# Mon, 28 Aug 2023 11:26:15 GMT
ARG USER_HOME_DIR=/root
# Mon, 28 Aug 2023 11:26:15 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 28 Aug 2023 11:26:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 28 Aug 2023 11:26:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8e2acd49419010bc77a61e38a85963f09e403f004635f24c436d177a08df1040`  
		Last Modified: Sat, 26 Aug 2023 03:06:10 GMT  
		Size: 51.3 MB (51324150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c572ef532f8d609e7e1e438eb1feb317f961b65516d07622aec217faca2982`  
		Last Modified: Tue, 29 Aug 2023 19:20:29 GMT  
		Size: 155.7 MB (155670060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf36cd2b2b1eebb2cb83900dfcb84e9998375fea87400dfc1e954ddf8cdbf535`  
		Last Modified: Tue, 29 Aug 2023 19:51:49 GMT  
		Size: 36.4 MB (36389836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70ac416847207fd574ba00b48fa9ed0e9694f6459e9a4c2d7dd1cd5079e0c47`  
		Last Modified: Tue, 29 Aug 2023 19:51:48 GMT  
		Size: 9.4 MB (9406417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4dc40ddfde7a02b11965d7bc11960b98e00b76f21219cc05fec0534e584e06`  
		Last Modified: Tue, 29 Aug 2023 19:51:47 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b2f46bf0015ca1ed83f88395c0836b0ec1c84039578189143b2cb30a03cbf5`  
		Last Modified: Tue, 29 Aug 2023 19:51:47 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1dbbb5adb0b23c643b76361b3bedf6da54ca303e32d36b8694d4c1f139bd3e`  
		Last Modified: Tue, 29 Aug 2023 19:51:47 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
