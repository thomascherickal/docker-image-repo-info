## `maven:3-amazoncorretto-11-al2023`

```console
$ docker pull maven@sha256:03fe9e86e256081a1583a79f28e296f1be483b681a96ba728f69c7820f20579b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-11-al2023` - linux; amd64

```console
$ docker pull maven@sha256:a7e01d5f244980bf2eb980c5c5fb344e86af76ab40cb3ba648f01e4b608648cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.4 MB (260425186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccb6045824a41ba064ba27e8d5a23162b1d2df6bc0f2a3bba9f78d149b272080`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:34 GMT
COPY dir:a736dc55b3f736cb7e8fc1978dac2536c3df3a8e3e684d650ab946ec3bfffd4d in / 
# Tue, 21 Nov 2023 03:21:35 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:16:24 GMT
ARG version=11.0.21.9-1
# Tue, 21 Nov 2023 04:16:44 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-jmods-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 04:16:45 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:16:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
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
	-	`sha256:e56b9e651e139f587693c83304d78cb368c3865e5b484befe5789c73bac4aff6`  
		Last Modified: Tue, 21 Nov 2023 04:28:24 GMT  
		Size: 153.6 MB (153573606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3e62476e0808591a76b419f1a08b4670198763872e5034102372a5c3720258`  
		Last Modified: Tue, 21 Nov 2023 05:18:33 GMT  
		Size: 45.2 MB (45202029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22b5e9f0d90683af057e82dd71b09949a8d5afd839f0d7da84e38f6ec4c9262`  
		Last Modified: Tue, 21 Nov 2023 05:18:31 GMT  
		Size: 9.4 MB (9429502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4977005d7523e0b0e6e59c7027d1bd7961e85d36ab7c44c97bd7b06843bb3c41`  
		Last Modified: Tue, 21 Nov 2023 05:18:30 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8243929a8382f30315cca43bdaf24df1bf76ab60730c0e646b41b0eac2719230`  
		Last Modified: Tue, 21 Nov 2023 05:18:30 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e67b2624902379f54495370583029f2fc4a78c93a72e178fe9ea5f63adf226`  
		Last Modified: Tue, 21 Nov 2023 05:18:30 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-11-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:12cba1b902056ede0b4664b204f02f60e0ec00071f4ba82a92b17546602a9cba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.6 MB (257602642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cad0fb2874192d937055ef419b8982378c7c8274cf0022739e60c3ec843589e5`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 03:39:34 GMT
COPY dir:fac986ebd66714776e9e2c25ed83431bd5e6692d32fdb5c2c74b9c2916168b3e in / 
# Tue, 21 Nov 2023 03:39:34 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 05:09:15 GMT
ARG version=11.0.21.9-1
# Tue, 21 Nov 2023 05:09:33 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-jmods-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 05:09:34 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:09:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
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
	-	`sha256:a3e63d6fa51f54e501e1a12b1f213e77434e44b11905ebe18b6a320b6ccbc568`  
		Last Modified: Tue, 21 Nov 2023 05:18:55 GMT  
		Size: 152.1 MB (152052063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35e12ae4a82a2546a68ddb4cdf65d2bfdd156c12f9f71c739a6aa2a386ad0ce`  
		Last Modified: Tue, 21 Nov 2023 06:00:43 GMT  
		Size: 44.8 MB (44812679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d05347bfa804c1f2f5d50bfa93d23c6fc46ab5eb8d9920d809da45f9e6c8ede`  
		Last Modified: Tue, 21 Nov 2023 06:00:40 GMT  
		Size: 9.4 MB (9429509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ab791d9abe7f83f4eaa552872690e523647e184575be862125b105efb2e95e`  
		Last Modified: Tue, 21 Nov 2023 06:00:39 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc8ab5d4b7570e6de9ac78ac66fec6f3d350e477cc2470aa6c67bc48aaa00ea`  
		Last Modified: Tue, 21 Nov 2023 06:00:39 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebebf0b40b3139b2a88be9accbaf450053d48bac4139e2bfa98da330fe2151b`  
		Last Modified: Tue, 21 Nov 2023 06:00:39 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
