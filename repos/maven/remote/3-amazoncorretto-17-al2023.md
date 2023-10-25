## `maven:3-amazoncorretto-17-al2023`

```console
$ docker pull maven@sha256:a7862c641ae580f29e0fe9e39d129d71e811c3f9b2d95412507fd132220cf900
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17-al2023` - linux; amd64

```console
$ docker pull maven@sha256:72210bff60e3e0e46a6e30c84477644c9073a0ff83954fd4a6f8b46aa737fb87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.3 MB (262333708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ee1b3465cb6e741cf030848c01c0c333ffe39746ff579b5e0c96e3d896f4836`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 25 Oct 2023 01:19:32 GMT
COPY dir:9af41cf6ce642147a5bc5b6f2e8b2df0656b169c3bf33f1a1298ad1ff250d756 in / 
# Wed, 25 Oct 2023 01:19:33 GMT
CMD ["/bin/bash"]
# Wed, 25 Oct 2023 01:45:33 GMT
ARG version=17.0.9.8-1
# Wed, 25 Oct 2023 01:45:33 GMT
ARG package_version=1
# Wed, 25 Oct 2023 01:45:53 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 25 Oct 2023 01:45:54 GMT
ENV LANG=C.UTF-8
# Wed, 25 Oct 2023 01:45:54 GMT
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
	-	`sha256:e3e7439f4f2df32dd5fd7f5b3d13a3b40e7d4a7e355827d2a2e794717b58e1a0`  
		Last Modified: Tue, 24 Oct 2023 18:05:52 GMT  
		Size: 52.4 MB (52401965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c798e647361eeb6d8e009404a4196845a2bc868de6b5d3df85a4426aeca7dabf`  
		Last Modified: Wed, 25 Oct 2023 01:57:27 GMT  
		Size: 156.8 MB (156836312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8c4ccd4e0297821081b428a39b3b582bbe742a4c96e731ecb7b16f0639d2fe`  
		Last Modified: Wed, 25 Oct 2023 02:57:49 GMT  
		Size: 43.7 MB (43664538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e37a01dd20cc7602efc67a7eb169ae1ea3741d973eccb9c410a696e80d66d7`  
		Last Modified: Wed, 25 Oct 2023 02:57:46 GMT  
		Size: 9.4 MB (9429511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c29ce849eed9834fb856c06e09d349a7cf213a1798d5d33072dc87af2c065`  
		Last Modified: Wed, 25 Oct 2023 02:57:45 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9881f009b284c1a36c9476a65763f6a6ab7af1bb6ce906a45b89113b59a6a8a`  
		Last Modified: Wed, 25 Oct 2023 02:57:45 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e89c37e2faeaf6458078011ac6a0f8b9e2fc1fc45e7b98a865bd5ed960c029c`  
		Last Modified: Wed, 25 Oct 2023 02:57:45 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:6caad41a51f6cd7bf2ca42ad3ba41c3b1b4b8061a45ed86dd424c4afd878406c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.8 MB (259773296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7443a2d0f6616d7a021a9c11acb2aa40acaac6b6153943630e2f99d9fcaeb38a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 25 Oct 2023 00:39:28 GMT
COPY dir:479ee478c40efe0225a7bfb57784564c52845a04479c6b1813627da25975830a in / 
# Wed, 25 Oct 2023 00:39:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Oct 2023 01:22:09 GMT
ARG version=17.0.9.8-1
# Wed, 25 Oct 2023 01:22:09 GMT
ARG package_version=1
# Wed, 25 Oct 2023 01:22:26 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 25 Oct 2023 01:22:28 GMT
ENV LANG=C.UTF-8
# Wed, 25 Oct 2023 01:22:28 GMT
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
	-	`sha256:5d5c8b11ebace3512444acd4525be845e8ec3d2fd0e5999e358a7c7c74805db5`  
		Last Modified: Wed, 25 Oct 2023 00:40:02 GMT  
		Size: 51.5 MB (51479162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759744d3bdf03f3329cedc0f779ad73c0ce10ad5d9f6d62a47f7794bae5c0d3b`  
		Last Modified: Wed, 25 Oct 2023 01:31:56 GMT  
		Size: 155.6 MB (155563552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b1b50065ec835259fd794b0846d3d3f245b89cad951ef8889048c2a66a22e`  
		Last Modified: Wed, 25 Oct 2023 01:55:18 GMT  
		Size: 43.3 MB (43299699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6633cce75018d1b0cfcb9fc81320ed1d8de099a4258797639a5d9f497cea5919`  
		Last Modified: Wed, 25 Oct 2023 01:55:15 GMT  
		Size: 9.4 MB (9429504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845bf49c5225dcb07de75b696944b999c7ff3f01b984bcc14933695925f0032c`  
		Last Modified: Wed, 25 Oct 2023 01:55:14 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81141b1080194b36c310b7c5336be559caa714be2ee7c3be5da5216743ef9a34`  
		Last Modified: Wed, 25 Oct 2023 01:55:14 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23aadecdae5069a980733c998cf1f9665ecc6fa1a2677051de246f8438c94d51`  
		Last Modified: Wed, 25 Oct 2023 01:55:14 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
