## `maven:3-amazoncorretto-8-al2023`

```console
$ docker pull maven@sha256:26ee86b9792a2bce8cdeabecbe42b95e4cf8e246ab37c78410ba386afe535e2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8-al2023` - linux; amd64

```console
$ docker pull maven@sha256:86fc8735d15a438d934399997b4380fc30a78aa58561514ec86e6b7b70e985ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.5 MB (385483796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:474d54fd036d84255b8cc1e954bd62f88a6f6224e72dc6b56405d169d3b8a0be`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 25 Oct 2023 01:19:32 GMT
COPY dir:9af41cf6ce642147a5bc5b6f2e8b2df0656b169c3bf33f1a1298ad1ff250d756 in / 
# Wed, 25 Oct 2023 01:19:33 GMT
CMD ["/bin/bash"]
# Wed, 25 Oct 2023 01:37:03 GMT
ARG version=1.8.0_392.b08-1
# Wed, 25 Oct 2023 01:37:35 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 25 Oct 2023 01:37:37 GMT
ENV LANG=C.UTF-8
# Wed, 25 Oct 2023 01:37:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
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
	-	`sha256:0a6c593c8e04001d8931ffb2ceb4e908d842ee1006df9a0264f87fc42a32debf`  
		Last Modified: Wed, 25 Oct 2023 01:53:10 GMT  
		Size: 278.5 MB (278478955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f32b450b6f9098bf70b5277beb371ed3b3ee56f5f4aa0bc49c1ca6f30a9a62`  
		Last Modified: Wed, 25 Oct 2023 02:59:10 GMT  
		Size: 45.2 MB (45171981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8160d156bf7edc65e872dfbcbaa8c7f89665a308034e31b30dd0866321b26e89`  
		Last Modified: Wed, 25 Oct 2023 02:59:08 GMT  
		Size: 9.4 MB (9429514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9747543a11bb0e8811df24fdc458e7d91c94c0991cf5ca22a82a568434a3cbee`  
		Last Modified: Wed, 25 Oct 2023 02:59:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0bf2a0752cdaca1f55022eef489daf9cc1304736ba2d48e05c6f5f7cd2837b3`  
		Last Modified: Wed, 25 Oct 2023 02:59:07 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d65a04f7ff2011579112e5bfe12a5ef0dc6422ac3d37b8520d0b07a0fcd243e`  
		Last Modified: Wed, 25 Oct 2023 02:59:07 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:7ebc9d42340256a45f62d6fccaa04d85807f9fc2a509fb2f7cc943b89bf7f775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.8 MB (222790857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad0edf33c7403937553620f8d16e3ff8be991d8b3c67ce129a7a15ebf88da52`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 25 Oct 2023 00:39:28 GMT
COPY dir:479ee478c40efe0225a7bfb57784564c52845a04479c6b1813627da25975830a in / 
# Wed, 25 Oct 2023 00:39:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Oct 2023 01:18:00 GMT
ARG version=1.8.0_392.b08-1
# Wed, 25 Oct 2023 01:18:15 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 25 Oct 2023 01:18:16 GMT
ENV LANG=C.UTF-8
# Wed, 25 Oct 2023 01:18:16 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
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
	-	`sha256:dd081b68f5aa2c87b7a0b34ee007f79777fcd2ad4973be50499adcdedef4643d`  
		Last Modified: Wed, 25 Oct 2023 01:28:15 GMT  
		Size: 118.6 MB (118585270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19be8799efbab7e4dc11e0f90bf95b589579c9be2a51545ba4445bbc63d08712`  
		Last Modified: Wed, 25 Oct 2023 01:56:37 GMT  
		Size: 43.3 MB (43295543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf06c678ace4a177b141b7c466bbebbc18a5fd8d371b51beaae81d0e58b2bafe`  
		Last Modified: Wed, 25 Oct 2023 01:56:35 GMT  
		Size: 9.4 MB (9429504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0a25a618f8af809a44ad054fb9126b03c2e40c1ce499aa9120070011444638`  
		Last Modified: Wed, 25 Oct 2023 01:56:34 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b44593d9a7f397d09395b48bb0ebb1f4b85baa713d4cbab0e72a0662c55a47`  
		Last Modified: Wed, 25 Oct 2023 01:56:34 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a4f04056bf19ad88eff851660953fc9d384316689f6d5b98888ce92e266c4`  
		Last Modified: Wed, 25 Oct 2023 01:56:34 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
