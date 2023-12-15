## `maven:3-amazoncorretto-17-al2023`

```console
$ docker pull maven@sha256:185b08191f639f01ef9edccb694305c4d1d4218d291fbb7fafb5b2493e108891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17-al2023` - linux; amd64

```console
$ docker pull maven@sha256:71b6177073b377dd7cf6388c682996982fe854de62af6922105f1f8412485a57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.0 MB (264990068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b1999938a31085bcda2b54a20a49ca5cceed318d1f93c31c96ae25d4ac064e2`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:29 GMT
COPY dir:6a0327957e10cfc5aab398cafdbbdbefb52a510a0fb73d8bf1952a36ff5452a4 in / 
# Fri, 15 Dec 2023 20:22:30 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:46:21 GMT
ARG version=17.0.9.8-1
# Fri, 15 Dec 2023 20:46:21 GMT
ARG package_version=1
# Fri, 15 Dec 2023 20:46:42 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 15 Dec 2023 20:46:43 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:46:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
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
	-	`sha256:51434d40bc8e653496d9fe19d2eae590bfa9fd806f4b7d3a5e08fb147050d259`  
		Last Modified: Fri, 15 Dec 2023 20:57:33 GMT  
		Size: 156.8 MB (156837076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9204b7e084cced47efc4e7025dde0fe1bb80d5f618c6aff84996fd0c48acf50f`  
		Last Modified: Fri, 15 Dec 2023 21:53:38 GMT  
		Size: 46.5 MB (46450425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c25bff3f9ccf7cb703b61ec89865eaba39cc392693a764988d3733dbbe5d56`  
		Last Modified: Fri, 15 Dec 2023 21:53:35 GMT  
		Size: 9.5 MB (9479947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957e4fcb21c102711ff53e3102f490b2af6d216184758b31ccabf31afff28ff2`  
		Last Modified: Fri, 15 Dec 2023 21:53:35 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7569303ded18615b476d88c730023ce582b177269e47c97a3bb635cf295592af`  
		Last Modified: Fri, 15 Dec 2023 21:53:35 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78341fbd3f02ea9d676b990dc2f43a02b22c87cbc0136dcbf57db3dd6ef7bfb`  
		Last Modified: Fri, 15 Dec 2023 21:53:35 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:dd2ed086037244244588766b64c6640f9aab18ca03ea9d93d83a2645daec3e9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.4 MB (262400943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:906b9086d52cda1f23a74861ab0b5fee2137304a03f94d4294995b9e93ebdf4e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 15 Dec 2023 20:44:19 GMT
COPY dir:02d504631605340a0b119cb2fbfb77790d9edc1c5c4eae4b1c4c4761f2d76905 in / 
# Fri, 15 Dec 2023 20:44:20 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 21:13:20 GMT
ARG version=17.0.9.8-1
# Fri, 15 Dec 2023 21:13:20 GMT
ARG package_version=1
# Fri, 15 Dec 2023 21:13:38 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-devel-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-jmods-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 15 Dec 2023 21:13:40 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 21:13:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
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
	-	`sha256:cc77ee89e2640a36477073ffe029859927e10c8561fd7080e45f0c65a0f03aab`  
		Last Modified: Fri, 15 Dec 2023 21:22:21 GMT  
		Size: 155.6 MB (155562360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77968373184b4c012875b7df6714b3ce0e9cdf98df477052385a3a92a067da4`  
		Last Modified: Fri, 15 Dec 2023 21:46:29 GMT  
		Size: 46.1 MB (46052659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f90f4e0c5e0e2e1b71608bb4df4fc26b68fbeb60205bed416be0d91ab248d27`  
		Last Modified: Fri, 15 Dec 2023 21:46:27 GMT  
		Size: 9.5 MB (9479933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa02338f70a5e7f6faa5df184a30fdb9868d69e33886095baa65bdf5dbc86e`  
		Last Modified: Fri, 15 Dec 2023 21:46:26 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab266db08937af98a2fddee95f8fac00c2eb58afea4d0ea6b745af07c29bb0f`  
		Last Modified: Fri, 15 Dec 2023 21:46:26 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f27719eccd40d546d88327f44a27618b8aa5e370793f5539eccdd1aa7247f3d`  
		Last Modified: Fri, 15 Dec 2023 21:46:26 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
