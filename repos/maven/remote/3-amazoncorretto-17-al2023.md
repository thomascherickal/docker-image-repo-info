## `maven:3-amazoncorretto-17-al2023`

```console
$ docker pull maven@sha256:0833a880c950a9418cd51e51100635c6e003eb879a9664793bd7b46b0a57b4dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17-al2023` - linux; amd64

```console
$ docker pull maven@sha256:8180a87aa4a44037ab22b2fc5e5ca3ef7b7d4ddc084f8289f99640f3cf64fe27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.7 MB (263686748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f44715d0d5c3887d928b62353d2ad07dd1616c5f1deb80aee90bc0b6addc4a4c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:34 GMT
COPY dir:a736dc55b3f736cb7e8fc1978dac2536c3df3a8e3e684d650ab946ec3bfffd4d in / 
# Tue, 21 Nov 2023 03:21:35 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:19:35 GMT
ARG version=17.0.9.8-1
# Tue, 21 Nov 2023 04:19:35 GMT
ARG package_version=1
# Tue, 21 Nov 2023 04:19:55 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 04:19:56 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:19:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Thu, 19 Oct 2023 09:04:18 GMT
RUN yum install -y tar which gzip findutils # TODO remove # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ARG MAVEN_VERSION=3.9.5
# Thu, 19 Oct 2023 09:04:18 GMT
ARG USER_HOME_DIR=/root
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 19 Oct 2023 09:04:18 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 19 Oct 2023 09:04:18 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:bad342ce986c7387f9e03cc2deafa306717aed86685ac6e1705ccc016b283eca`  
		Last Modified: Tue, 14 Nov 2023 20:44:05 GMT  
		Size: 52.2 MB (52218672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ba5dbcb655330751e78e278980c20255bb9abb58f59dfeab04bc12b5d9b5e1`  
		Last Modified: Tue, 21 Nov 2023 04:30:38 GMT  
		Size: 156.8 MB (156833453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03dedbdb9a4785dd01058c39a9c1dbc311a7755a5f92d8371d5e18f6cde9604d`  
		Last Modified: Tue, 21 Nov 2023 05:19:13 GMT  
		Size: 45.2 MB (45203740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07f07d5a593bd962a4e878af4f4982846f1c0c007d184c037041e46fc5cb9f9`  
		Last Modified: Tue, 21 Nov 2023 05:19:11 GMT  
		Size: 9.4 MB (9429502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e949820aa447ae4c73135e2fd1b2f60cbac8dd337a2595b08d9ce18f18365a8`  
		Last Modified: Tue, 21 Nov 2023 05:19:10 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5277ee9d0d0e9e1e62313b59fd517cfbc6bd119c002fa143a6d207ef737fa2f1`  
		Last Modified: Tue, 21 Nov 2023 05:19:10 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3842017cd6357c7f9a838cb1bebb68355298fb9faac88b10a72b001ecdef2dc0`  
		Last Modified: Tue, 21 Nov 2023 05:19:10 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:3b0b9df2ff6c5820ab92ca4dc71c7be83ab583eec678fecd430625ccb0a690a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261117008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70601bd12c10f58b9ff42d2ca68ecda4c3916283ddc07903b697023a0a086f60`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 03:39:34 GMT
COPY dir:fac986ebd66714776e9e2c25ed83431bd5e6692d32fdb5c2c74b9c2916168b3e in / 
# Tue, 21 Nov 2023 03:39:34 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 05:11:40 GMT
ARG version=17.0.9.8-1
# Tue, 21 Nov 2023 05:11:40 GMT
ARG package_version=1
# Tue, 21 Nov 2023 05:11:57 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 05:11:59 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:11:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Thu, 19 Oct 2023 09:04:18 GMT
RUN yum install -y tar which gzip findutils # TODO remove # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 19 Oct 2023 09:04:18 GMT
ARG MAVEN_VERSION=3.9.5
# Thu, 19 Oct 2023 09:04:18 GMT
ARG USER_HOME_DIR=/root
# Thu, 19 Oct 2023 09:04:18 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 19 Oct 2023 09:04:18 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 19 Oct 2023 09:04:18 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:f8ec7f6a4acb7febbe0e77fe9bba1064900d89cbf939e87733102926ad5870fd`  
		Last Modified: Tue, 14 Nov 2023 20:44:04 GMT  
		Size: 51.3 MB (51307015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b881191a874a94a8bee7ec7318e4e6babc896d67535930d346b16625be7d202`  
		Last Modified: Tue, 21 Nov 2023 05:21:10 GMT  
		Size: 155.6 MB (155566221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f841c5ba51b20fb1620584762c95965ae1b5969efe29ef8a6544f21c54d44566`  
		Last Modified: Tue, 21 Nov 2023 06:01:20 GMT  
		Size: 44.8 MB (44812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b62b8cff82ba1a9cab77bbbc3c0f1d7f547ae56b13ec4870d274494c9b7a59`  
		Last Modified: Tue, 21 Nov 2023 06:01:18 GMT  
		Size: 9.4 MB (9429508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63483d048597f07aa8a1ba919c1e0e65b29208abf887eba6c86f04fc2373ad7b`  
		Last Modified: Tue, 21 Nov 2023 06:01:17 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3138fcb225e6977256caf337b95a2e610409ea8aab2818515714a2a15bf6440f`  
		Last Modified: Tue, 21 Nov 2023 06:01:17 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60152e9675384a0936ca35257e52f803bebda0912d7718e80ac040e1db13df54`  
		Last Modified: Tue, 21 Nov 2023 06:01:17 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
