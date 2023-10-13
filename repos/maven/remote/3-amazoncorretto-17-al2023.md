## `maven:3-amazoncorretto-17-al2023`

```console
$ docker pull maven@sha256:946005f4640228794cc7ea6b4f033207a83cc535cd69b4112a6fd60a3989fa98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17-al2023` - linux; amd64

```console
$ docker pull maven@sha256:84e37219a961b0388bb1e64eb2b32d05963a267e843eb224997adeb4cf8aa30c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261011625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ec2a9372643cc51d5cc75a0d5893c460b156fd7bd72752ecc79ea8c9c0b2c8`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 12 Oct 2023 22:37:51 GMT
COPY dir:73a08d9acd2707b5f429ab7e4f26f6f5880d94265654591f74d7102f20954c66 in / 
# Thu, 12 Oct 2023 22:37:52 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 23:10:33 GMT
ARG version=17.0.8.8-1
# Thu, 12 Oct 2023 23:10:33 GMT
ARG package_version=1
# Thu, 12 Oct 2023 23:10:54 GMT
# ARGS: package_version=1 version=17.0.8.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Thu, 12 Oct 2023 23:10:54 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 23:10:54 GMT
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
	-	`sha256:860bcbd64bf9485a06bc1858b0de975763ffab4b4fb53fb19b66b42536e48fe7`  
		Last Modified: Wed, 11 Oct 2023 21:33:29 GMT  
		Size: 52.4 MB (52395746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776a29338268a9c82f2ee68cd77d1d7b4c1aa81c31c22bc5bdab6a5aa5622e3a`  
		Last Modified: Thu, 12 Oct 2023 23:24:48 GMT  
		Size: 156.9 MB (156947401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fe94b8dc281f4a4791bb758cb0521b333cf30fd7046e2db65c4bbce1951aa0`  
		Last Modified: Fri, 13 Oct 2023 01:19:26 GMT  
		Size: 42.3 MB (42260666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8c38c7a00929d969eafaad583a4f80f7c04c23e04709a1745832ccf204de5f`  
		Last Modified: Fri, 13 Oct 2023 01:19:23 GMT  
		Size: 9.4 MB (9406428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910cbae9265338e627a74a0b5bef6114e27dd59a5585185ca1fdc6e16a69aeea`  
		Last Modified: Fri, 13 Oct 2023 01:19:23 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3155ecf05bd9fd495dcd5c925fbc86d3f295a85c9301e252199097acad03b3`  
		Last Modified: Fri, 13 Oct 2023 01:19:23 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37452430899ce335e426136e7005fdd7f6a4af6b2a9665694535146c4789bc76`  
		Last Modified: Fri, 13 Oct 2023 01:19:23 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:5de615f1d80cc2a1c77f9623225e70dd3c38e4fab6ea2da3e93cac455f722223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.5 MB (258451459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e330772c50780227530274485fe71dba5d2fb3de2649554713491eaa3bf05c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 12 Oct 2023 22:23:51 GMT
COPY dir:23c4f526fba599c79c471bcc9a859c715cfebcd3d79aabf95868c2189962dde3 in / 
# Thu, 12 Oct 2023 22:23:51 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 23:17:17 GMT
ARG version=17.0.8.8-1
# Thu, 12 Oct 2023 23:17:17 GMT
ARG package_version=1
# Thu, 12 Oct 2023 23:17:35 GMT
# ARGS: package_version=1 version=17.0.8.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Thu, 12 Oct 2023 23:17:37 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 23:17:37 GMT
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
	-	`sha256:d726870119c530d3b141cccd8b55693be0fc259a674ed2bc3bcf5999ff1434d3`  
		Last Modified: Thu, 12 Oct 2023 01:34:33 GMT  
		Size: 51.5 MB (51474358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa44ab746eeef2b94f8b1dee667d1e4111cb27180fb60094220d1796ccf591d1`  
		Last Modified: Thu, 12 Oct 2023 23:29:09 GMT  
		Size: 155.7 MB (155656543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddc50e9c71203806d27e6c4bfe885d67686bf3223bccaa0a6f84684fb50e9a1`  
		Last Modified: Fri, 13 Oct 2023 00:09:32 GMT  
		Size: 41.9 MB (41912756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4095c1b8313f7671654e8b06ac93775b48f5c054a596b1e78cd4f09fb2e23a3c`  
		Last Modified: Fri, 13 Oct 2023 00:09:30 GMT  
		Size: 9.4 MB (9406421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fe5dc46dd16342eb1193921f0ca57b3f90642d6dd1d648eb08690d97fd4f5d`  
		Last Modified: Fri, 13 Oct 2023 00:09:29 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b597b49213e61e45220890c7ce32eb20052febc5534623862d95988a8e7aaf`  
		Last Modified: Fri, 13 Oct 2023 00:09:29 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792a8103f8ec92e01f5fe6d9a2d4416d2946e20a1419d0dccb112876b66622d3`  
		Last Modified: Fri, 13 Oct 2023 00:09:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
