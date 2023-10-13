## `maven:3-amazoncorretto-8-al2023`

```console
$ docker pull maven@sha256:9bd1a793ddab6f156f0b387039ea99ac7240c18c61c4a087129cb218bff1b44e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8-al2023` - linux; amd64

```console
$ docker pull maven@sha256:9083b68bff6a0400917c84bf69abc8a7b6d3aac87f54c05bcf7002e2a90b6dd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.0 MB (384032471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ed68f116a30e9b806a0a3d860643e3ecbfd0e3a057a2dc12c259329e54badf`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 12 Oct 2023 22:37:51 GMT
COPY dir:73a08d9acd2707b5f429ab7e4f26f6f5880d94265654591f74d7102f20954c66 in / 
# Thu, 12 Oct 2023 22:37:52 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 23:02:41 GMT
ARG version=1.8.0_382.b05-1
# Thu, 12 Oct 2023 23:03:13 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Thu, 12 Oct 2023 23:03:15 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 23:03:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
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
	-	`sha256:faff55e961c0125b67db4ecec7330c924c17f2e9ac9e2ea5c6af1af054992c20`  
		Last Modified: Thu, 12 Oct 2023 23:20:33 GMT  
		Size: 278.5 MB (278456617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6d5f309132047b0b6c6c71ed87a464aba3779b4548d6528c5ba9b1fa9f107c`  
		Last Modified: Fri, 13 Oct 2023 01:21:46 GMT  
		Size: 43.8 MB (43772301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef281397781ebabca59826e5ced358968bfec8a7f657fc5f4c014de4fd9d1543`  
		Last Modified: Fri, 13 Oct 2023 01:21:43 GMT  
		Size: 9.4 MB (9406425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb99dd905e0ff9a2babe4e9275644fbe4c378806201dd4219fbbe2f4a919206`  
		Last Modified: Fri, 13 Oct 2023 01:21:42 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d822bf5060711b598ccaa37dd5299bc37f8af1f73ca457ac04d19014614e0895`  
		Last Modified: Fri, 13 Oct 2023 01:21:42 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7737d4fe6a2f0b2dca4bb2f786da6555acd3802a24821344d96f4f833ab9beea`  
		Last Modified: Fri, 13 Oct 2023 01:21:42 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:fae350495c94560212acbd4c4cfdc1445c926bca803d6298ce3e805c276079b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221350331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca82dd4b4d273e3de03d8ce2db4ec112118d3dea62ebbbeb8d0a480e9a00db94`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 12 Oct 2023 22:23:51 GMT
COPY dir:23c4f526fba599c79c471bcc9a859c715cfebcd3d79aabf95868c2189962dde3 in / 
# Thu, 12 Oct 2023 22:23:51 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 23:12:08 GMT
ARG version=1.8.0_382.b05-1
# Thu, 12 Oct 2023 23:12:22 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Thu, 12 Oct 2023 23:12:24 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 23:12:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
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
	-	`sha256:dd68161e86242cc39523eb2c12865b2ea986c57b8cae99c71aa202b4f2adf209`  
		Last Modified: Thu, 12 Oct 2023 23:25:25 GMT  
		Size: 118.6 MB (118563259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0588c4f8142c195dd9aee730b8d9ee205ff42ce81720edb14844e968649faf`  
		Last Modified: Fri, 13 Oct 2023 00:11:33 GMT  
		Size: 41.9 MB (41904905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abd271da2c3034bbeb4adcc06339cfd6fb98aac5feac93fa3551aa54b0992c`  
		Last Modified: Fri, 13 Oct 2023 00:11:31 GMT  
		Size: 9.4 MB (9406426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00748bc78d362d8603e46c456f3d1db06d09f1b36c463cf489ec9aec7dfa6473`  
		Last Modified: Fri, 13 Oct 2023 00:11:30 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8150eb64443f5e24fbc2561b7c448b9f11673a81c49164f5b5abddbd7a6a009a`  
		Last Modified: Fri, 13 Oct 2023 00:11:30 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7f1e9d64f09339eb773b73c6dacc02101210205aba64e061394311172395a7`  
		Last Modified: Fri, 13 Oct 2023 00:11:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
