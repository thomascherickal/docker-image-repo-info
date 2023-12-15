## `maven:3-amazoncorretto-21-al2023`

```console
$ docker pull maven@sha256:a8230e2ba5f30a7515fd1fb5e8c07de590fad6396952fa91f8dcfc98d7e9abf0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-21-al2023` - linux; amd64

```console
$ docker pull maven@sha256:9e18773b936ea7fbd8d7bf2e8c7fa3a7e2546ed568c116ec687e1b2d82759c78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.5 MB (278518093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5622043852d6347bd7853d35ea4655daf66cd9889089802fae9f1fb662e37f1e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:29 GMT
COPY dir:6a0327957e10cfc5aab398cafdbbdbefb52a510a0fb73d8bf1952a36ff5452a4 in / 
# Fri, 15 Dec 2023 20:22:30 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:50:11 GMT
ARG version=21.0.1.12-1
# Fri, 15 Dec 2023 20:50:11 GMT
ARG package_version=2
# Fri, 15 Dec 2023 20:50:32 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 15 Dec 2023 20:50:33 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:50:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
# Mon, 11 Dec 2023 11:12:11 GMT
RUN yum install -y tar which gzip findutils # TODO remove # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
ARG MAVEN_VERSION=3.9.6
# Mon, 11 Dec 2023 11:12:11 GMT
ARG USER_HOME_DIR=/root
# Mon, 11 Dec 2023 11:12:11 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 11 Dec 2023 11:12:11 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 11 Dec 2023 11:12:11 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:97668dd20d4358bee95dea91ba9ca63bae56f3a5759ca22763c5940071e14884`  
		Last Modified: Fri, 15 Dec 2023 01:53:15 GMT  
		Size: 52.2 MB (52221241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f32ed42f12e8b37de4f2ca3922a01c743ff1b5f773b440514a68d431ad7d79a`  
		Last Modified: Fri, 15 Dec 2023 21:00:21 GMT  
		Size: 170.4 MB (170373789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a2728532829598cdd98d86e762784f930e98d3b5b8ffb8e5ec1e08b5ededc1`  
		Last Modified: Fri, 15 Dec 2023 21:54:15 GMT  
		Size: 46.4 MB (46441736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfc365a5cc65ca59d9d30dd3845ec5bf38cb02f67501a35ab7d78cb52b5b4`  
		Last Modified: Fri, 15 Dec 2023 21:54:13 GMT  
		Size: 9.5 MB (9479948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab13d44e1034af41be6a49a5fbb37fd6a6df271a9f06626f3f007f3621ad93d`  
		Last Modified: Fri, 15 Dec 2023 21:54:13 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372ff1f56dfe717ce3ed5db69feb00f6557946a464aa8fd3f5072309b38ac0c6`  
		Last Modified: Fri, 15 Dec 2023 21:54:13 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8023f8230af312d584e98de65bdb93e370813b9ff53a65bc465a1e3b05d87911`  
		Last Modified: Fri, 15 Dec 2023 21:54:12 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-21-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:3a60465ea3a97e8508f9a4c1942b12883cd517dac4f9e119af9c637fbbf3405c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.4 MB (275417749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d31052cc9c882406e83a1842a6541d77b652e04a20863a2b3db6641c47d722d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 15 Dec 2023 20:44:19 GMT
COPY dir:02d504631605340a0b119cb2fbfb77790d9edc1c5c4eae4b1c4c4761f2d76905 in / 
# Fri, 15 Dec 2023 20:44:20 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 21:16:26 GMT
ARG version=21.0.1.12-1
# Fri, 15 Dec 2023 21:16:26 GMT
ARG package_version=2
# Fri, 15 Dec 2023 21:16:45 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 15 Dec 2023 21:16:47 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 21:16:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
# Mon, 11 Dec 2023 11:12:11 GMT
RUN yum install -y tar which gzip findutils # TODO remove # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
ARG MAVEN_VERSION=3.9.6
# Mon, 11 Dec 2023 11:12:11 GMT
ARG USER_HOME_DIR=/root
# Mon, 11 Dec 2023 11:12:11 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 11 Dec 2023 11:12:11 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 11 Dec 2023 11:12:11 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:ce0da89e7bfb7e6039e531a7f8bb3d39522916880c6425022b0ab8562dea66c3`  
		Last Modified: Fri, 15 Dec 2023 01:53:13 GMT  
		Size: 51.3 MB (51304607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5283e2863fa7bb9cee391c8e37177b860ba64e7b7b268f4eb1295949566d5364`  
		Last Modified: Fri, 15 Dec 2023 21:24:42 GMT  
		Size: 168.6 MB (168588446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b81177efd9cf31090753e3ecf9481d12f8c06b76c354a476a68abdcd641d5f8`  
		Last Modified: Fri, 15 Dec 2023 21:47:03 GMT  
		Size: 46.0 MB (46043375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05acda911573960c19a686991da7aaddc7568f54839cc932b4d98219fa84bce`  
		Last Modified: Fri, 15 Dec 2023 21:47:02 GMT  
		Size: 9.5 MB (9479934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b815a876c3994e1a307a2d9137ee9e16a88e33cf0116593c9280397afcf1b`  
		Last Modified: Fri, 15 Dec 2023 21:47:00 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e9febf6dc5b8eca1854840c7b0df9ca73a0a85aa1cbf1ba77a5769c514e5d9`  
		Last Modified: Fri, 15 Dec 2023 21:47:00 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b2ad94f2b580edbce3118bbb6d9a09a94a3dcbd8065d99a2b4b48a2df3b482`  
		Last Modified: Fri, 15 Dec 2023 21:47:00 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
