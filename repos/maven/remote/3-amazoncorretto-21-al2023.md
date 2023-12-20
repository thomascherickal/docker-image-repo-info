## `maven:3-amazoncorretto-21-al2023`

```console
$ docker pull maven@sha256:bf0a2946e328e6816f1fca3f3b825e2e0d4e0949e9d9fd3283498965b6279208
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-21-al2023` - linux; amd64

```console
$ docker pull maven@sha256:804191391f20e273c10a68b848f24a5f2ef4b25e267e812839c0c13f30e3a956
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.5 MB (278527649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb82644c1094d47b4a2c59a7fc9118f8916fc68c50e661b79b5fb842811edb21`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 20 Dec 2023 08:49:17 GMT
COPY dir:53a31edf8963d6fd2d947e72f41a518efb3266cde6711aa27f12fbd3bb05b5cc in / 
# Wed, 20 Dec 2023 08:49:17 GMT
CMD ["/bin/bash"]
# Wed, 20 Dec 2023 09:34:50 GMT
ARG version=21.0.1.12-1
# Wed, 20 Dec 2023 09:34:50 GMT
ARG package_version=2
# Wed, 20 Dec 2023 09:35:16 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 20 Dec 2023 09:35:17 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 09:35:17 GMT
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
	-	`sha256:1db371c0a72a30b037eddab3bf3f6091c0226e7b6e3a122c8e0e27d2ea7e5432`  
		Last Modified: Mon, 18 Dec 2023 19:12:16 GMT  
		Size: 52.2 MB (52217769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301aec3c6ad6c0700a9d5b955347a845b129d13e82927a8eb221145808309f6b`  
		Last Modified: Wed, 20 Dec 2023 09:44:55 GMT  
		Size: 170.4 MB (170371264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cb2b5452b36b5366d202e99d1593ef12a3f11482a985a90cacd97d56c26257`  
		Last Modified: Wed, 20 Dec 2023 11:30:32 GMT  
		Size: 46.5 MB (46457299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045c3aa1710a168499c2c3698e0a9a457360582285df2f2de04cab24faa5ff92`  
		Last Modified: Wed, 20 Dec 2023 11:30:30 GMT  
		Size: 9.5 MB (9479934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509def108700c1af7cfe896f9470834c998228b790907ea5b2523a90bd7539e5`  
		Last Modified: Wed, 20 Dec 2023 11:30:29 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d37929bb78c6fc5b85f72531e9c2254bf321c6c8753ccbe9e212c07cc82130`  
		Last Modified: Wed, 20 Dec 2023 11:30:29 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081d5cb7a449ff866e1a457d5b7dc329f7bfb7499aa16876293171a91c3fc015`  
		Last Modified: Wed, 20 Dec 2023 11:30:29 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-21-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:f4769be23d58a33b52b59aa3c7b7408cf8db2e13be6cf732f19efce4a8e8f337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275457816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f701f1a933a9d799ce4fe6b1d415f336172cc2eb36e7f6da339a22c24e205105`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 20 Dec 2023 01:32:07 GMT
COPY dir:d006faf7e50cd8429d93f8cf8ea807b50b60a3c38783c4d247b3e56de7d9a3dc in / 
# Wed, 20 Dec 2023 01:32:07 GMT
CMD ["/bin/bash"]
# Wed, 20 Dec 2023 02:03:41 GMT
ARG version=21.0.1.12-1
# Wed, 20 Dec 2023 02:03:41 GMT
ARG package_version=2
# Wed, 20 Dec 2023 02:03:59 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 20 Dec 2023 02:04:01 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 02:04:01 GMT
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
	-	`sha256:62dac1e13f9aa133cbec88aa21ded5df9ecd8a8ff67fc7ac9887cc25f3c387fb`  
		Last Modified: Mon, 18 Dec 2023 19:12:13 GMT  
		Size: 51.3 MB (51307984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa239869aab6b6c9165afc6f3580e0469aafd770597f91c6b7f52b9ab5ad3573`  
		Last Modified: Wed, 20 Dec 2023 02:12:24 GMT  
		Size: 168.6 MB (168588400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f49e892b8a23194cedad697784365e0a9111f21e6764fa1a0b719dd41cec3c`  
		Last Modified: Wed, 20 Dec 2023 03:23:22 GMT  
		Size: 46.1 MB (46080105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1388f26f4db2690e479385a9034979eaacd0c7a0916b781b5ef08187bd87d2`  
		Last Modified: Wed, 20 Dec 2023 03:23:20 GMT  
		Size: 9.5 MB (9479943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc736e0971bc8e21cd13764ab0779b918a89fb0dfe7a7f002169369c33f28fc`  
		Last Modified: Wed, 20 Dec 2023 03:23:19 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358552aa734c3e247529d73b9ab3ff592edc704b408bd05498655d04aa9fddb4`  
		Last Modified: Wed, 20 Dec 2023 03:23:19 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11dc70b8bce89d2440778ce9c38cfab808fb4eb416b8cfbc029aee1a5b2baec3`  
		Last Modified: Wed, 20 Dec 2023 03:23:20 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
