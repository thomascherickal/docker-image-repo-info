## `maven:3-amazoncorretto-8-al2023`

```console
$ docker pull maven@sha256:ad2509bd20bf98ffc9e199a9ac1fed9e7e568daeab4d288e779eac3aeb76b3c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8-al2023` - linux; amd64

```console
$ docker pull maven@sha256:cc132c13744caf585dafc4508221444f639a41be590b0a66bd154f189a87ab59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.8 MB (386845441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4559abf0284d8b74dbdb68ff36e2ac44f4bc8a5b2383689a81e1387cc86905fa`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:34 GMT
COPY dir:a736dc55b3f736cb7e8fc1978dac2536c3df3a8e3e684d650ab946ec3bfffd4d in / 
# Tue, 21 Nov 2023 03:21:35 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:13:30 GMT
ARG version=1.8.0_392.b08-1
# Tue, 21 Nov 2023 04:14:03 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 04:14:05 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:14:05 GMT
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
	-	`sha256:bad342ce986c7387f9e03cc2deafa306717aed86685ac6e1705ccc016b283eca`  
		Last Modified: Tue, 14 Nov 2023 20:44:05 GMT  
		Size: 52.2 MB (52218672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386370d1c1f74d85b091767d5b1bb292da0d3185de7301c183258981a681ef03`  
		Last Modified: Tue, 21 Nov 2023 04:26:36 GMT  
		Size: 278.5 MB (278478072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec182d6d4188b48220d711d504b1636266b05cfbf83493089a415ed04a8aedee`  
		Last Modified: Tue, 21 Nov 2023 05:20:29 GMT  
		Size: 46.7 MB (46717815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e495f88bdb0722edb8af5f7f2265009e35eb63c7e390ca439884fcb04cc39ac`  
		Last Modified: Tue, 21 Nov 2023 05:20:27 GMT  
		Size: 9.4 MB (9429502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d135769ce6c57021113f5f838d7645f63d0d17e4c2474b4762d4c713e4bda76`  
		Last Modified: Tue, 21 Nov 2023 05:20:26 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22a46a3fbbf4c08c4cfdebf3c524529b735832fb6489b83cac259076985bf4a`  
		Last Modified: Tue, 21 Nov 2023 05:20:26 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e2f67bb8f7bfc2a4708a0879dc8d56c8c1d4518f196a52f05592a44064c369`  
		Last Modified: Tue, 21 Nov 2023 05:20:26 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:60cb755cc0c5fab62a1c5fc265a58618b3b0155b9ec89048bc329db29e5eeb7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.1 MB (224130621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba15c4e404b1207610c2496080a5f9754b30c9f098e789c2d2cc05470d554cb`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Nov 2023 03:39:34 GMT
COPY dir:fac986ebd66714776e9e2c25ed83431bd5e6692d32fdb5c2c74b9c2916168b3e in / 
# Tue, 21 Nov 2023 03:39:34 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 05:07:36 GMT
ARG version=1.8.0_392.b08-1
# Tue, 21 Nov 2023 05:07:51 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 05:07:52 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:07:52 GMT
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
	-	`sha256:f8ec7f6a4acb7febbe0e77fe9bba1064900d89cbf939e87733102926ad5870fd`  
		Last Modified: Tue, 14 Nov 2023 20:44:04 GMT  
		Size: 51.3 MB (51307015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6a0e1531190dd4d81b29d5fd110db7efb04b7f313b1fec9d8a86bd5e705420`  
		Last Modified: Tue, 21 Nov 2023 05:17:22 GMT  
		Size: 118.6 MB (118586919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf5af4c62e587d4b44115b3a1880ab23fb6cb17a9c845e008f0ffd0a4d25478`  
		Last Modified: Tue, 21 Nov 2023 06:02:35 GMT  
		Size: 44.8 MB (44805803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb3c08ac445d09069ec3a1e85d4cd06da5b6f467b43353e9c87d52ddf357cea`  
		Last Modified: Tue, 21 Nov 2023 06:02:33 GMT  
		Size: 9.4 MB (9429507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c7f38b729ce47e672245f59cbac3e5835188cb299687b825f8ad79329f7fd2`  
		Last Modified: Tue, 21 Nov 2023 06:02:32 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6734413cdf9c6a4576c1d8bc337917e380c7ad940d8016a184db64bc9223171`  
		Last Modified: Tue, 21 Nov 2023 06:02:32 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598ac401fa67f7d2110046f5aead740a2ce5ef87ab65807e0b23ae772f3c70f0`  
		Last Modified: Tue, 21 Nov 2023 06:02:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
